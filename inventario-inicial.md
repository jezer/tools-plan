# Inventario inicial de tools

## Objetivo

Registrar os artefatos candidatos identificados antes de qualquer migracao para tools especificas.

## Escopo

1. Skills relacionadas a Git, chamados, planejamento e file system.
2. Contextos PV apoiados pelas tools iniciais.
3. Decisao inicial de manter, copiar ou migrar artefatos.

## Fora de escopo

1. Mover artefatos.
2. Copiar scripts para tools.
3. Alterar contextos PV.

## Regras aplicaveis

1. Skills continuam donas de seus scripts atuais.
2. Contextos PV continuam donos de suas regras.
3. Tools so recebem artefatos depois de plano especifico aprovado.

## Atividades planejadas

### INV-001 - Registrar inventario inicial

- Status: feito
- Data de implementacao: 2026-05-11
- Escopo: `C:\codes\tools`.
- Dependencias: `C:\codes\plan\tools-globais.md`.
- Skills recomendadas atuais: `maintain-planner`, `maintain-filesystem`, `maintain-skills`, `maintain-automations`.
- Skills futuras relacionadas: nenhuma.
- Acao: registrar matriz inicial de artefatos candidatos.
- Criterio de aceite: matriz contem origem, destino sugerido, contexto dono, skill usuaria, risco e decisao inicial.
- Observacoes: nenhum arquivo foi movido.

## Matriz inicial

| Origem | Destino sugerido | Contexto dono | Skill usuaria | Risco | Decisao inicial |
| --- | --- | --- | --- | --- | --- |
| `C:\codes\skills\maintain-git\scripts\*.ps1` | `C:\codes\tools\git` | `C:\codes\skills\maintain-git` | `maintain-git` | Quebrar skill existente | Manter na skill; avaliar copia futura |
| `C:\codes\pv\ct_git\AGENTS.md` | `C:\codes\tools\git` | `C:\codes\tools\git` | `maintain-git` | Duplicar regra Git | Centralizado em `tools/git`; `ct_git` fica como ponte |
| `C:\codes\skills\maintain-tickets\scripts\novo-chamado.ps1` | `C:\codes\tools\chamados` | `C:\codes\skills\maintain-tickets` | `maintain-tickets` | Quebrar criacao de chamados | Manter na skill; avaliar referencia futura |
| `C:\codes\skills\register-ticket-session\scripts\registrar-sessao.ps1` | `C:\codes\tools\chamados` | `C:\codes\skills\register-ticket-session` | `register-ticket-session` | Quebrar registro de sessoes | Manter na skill; avaliar referencia futura |
| `C:\codes\pv\ctrl_chamados\AGENTS.md` | `C:\codes\tools\chamados` | `C:\codes\tools\chamados` | `maintain-tickets` | Duplicar regra de chamados | Centralizado em `tools/chamados`; `pv/ctrl_chamados` fica como ponte |
| `C:\codes\skills\core\planner\maintain-planner\scripts\validar-plano.ps1` | `C:\codes\tools\planejador` | `C:\codes\skills\core\planner\maintain-planner` | `maintain-planner` | Quebrar validacao de planos | Manter na skill; avaliar validador compartilhado futuro |
| `C:\codes\skills\core\planner\maintain-activities\scripts\atualizar-atividade.ps1` | `C:\codes\tools\planejador` | `C:\codes\skills\core\planner\maintain-activities` | `maintain-activities` | Quebrar atualizacao de atividades | Manter na skill; avaliar referencia futura |
| `C:\codes\pv\ct_planejador\AGENTS.md` | `C:\codes\tools\planejador` | `C:\codes\pv\ct_planejador` | `maintain-planner` | Duplicar regra de planejamento | Nao migrar; tool apenas apoia |
| `C:\codes\pv\regras_file_system\AGENTS.md` | `C:\codes\tools\file-system` | `C:\codes\pv\regras_file_system` | `maintain-filesystem` | Duplicar regra de file system | Nao migrar; tool apenas apoia |

## Checklist

1. [x] Inventario inicial registrado.
2. [x] Nenhum artefato movido.
3. [x] Contextos donos preservados.


