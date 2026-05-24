# Plano do contexto tools

## Objetivo

Manter o contexto `C:\codes\tools` como area global de artefatos operacionais reutilizaveis para skills.

## Escopo

1. Regras do contexto `C:\codes\tools`.
2. Planos de tools especificas.
3. Contratos entre skills e tools.

## Fora de escopo

1. Criar tools especificas sem pedido aprovado.
2. Mover artefatos de skills, projetos ou controles sem plano de migracao.
3. Substituir responsabilidades de skills.

## Regras aplicaveis

1. Tools apoiam skills e nao substituem skills.
2. Skills decidem quando consultar tools.
3. Tools devem ter artefatos uteis e validaveis.
4. Tools devem ser consultadas sob demanda.

## Atividades planejadas

### TOOLS-001 - Criar contexto tools

- Status: feito
- Data de implementacao: 2026-05-11
- Escopo: `C:\codes\tools`.
- Dependencias: `C:\codes\plan\contexto-autonomia-tools.md`.
- Skills recomendadas atuais: `maintain-planner`, `maintain-filesystem`, `maintain-activities`.
- Skills futuras relacionadas: nenhuma.
- Acao: criar a pasta `C:\codes\tools` com regras e plano minimo.
- Criterio de aceite: `C:\codes\tools\AGENTS.md` e `C:\codes\tools\plan` existem.
- Observacoes: implementado nesta sessao.

### TOOLS-002 - Avaliar primeira tool especifica

- Status: feito
- Data de implementacao: 2026-05-12
- Escopo: `C:\codes\tools\git`, `C:\codes\tools\chamados`, `C:\codes\tools\planejador` e `C:\codes\tools\file-system`.
- Dependencias: TOOLS-001.
- Skills recomendadas atuais: `maintain-planner`, `maintain-skills`, `maintain-automations`.
- Skills futuras relacionadas: nenhuma.
- Acao: avaliar e formalizar o conjunto inicial de tools especificas com artefatos compartilhados.
- Criterio de aceite: decisao documentada com objetivo, limites, artefatos e validacao.
- Observacoes: decisao implementada com as subpastas e regras proprias das tools `git`, `chamados`, `planejador` e `file-system`.

#### Decisao documentada (TOOLS-002)

- Objetivo: separar artefatos operacionais globais por dominio, mantendo skills como orquestradoras.
- Limites: tools nao executam fluxos por conta propria, nao substituem skills e nao movem artefatos sem plano especifico.
- Artefatos:
  - `C:\codes\tools\git`: regras Git e inventario de apoio.
  - `C:\codes\tools\chamados`: regras e dados oficiais de chamados/sessoes.
  - `C:\codes\tools\planejador`: apoio de planejamento e atividades por contexto.
  - `C:\codes\tools\file-system`: apoio reutilizavel de padroes e validacoes de estrutura.
- Validacao: existencia de `AGENTS.md` e `plan/` por tool, com roteamento no `root` e nas skills aderentes.

## Checklist

1. [x] Contexto tools criado.
2. [x] Regras locais criadas.
3. [x] Plano local criado.
4. [x] Primeira tool especifica avaliada.

