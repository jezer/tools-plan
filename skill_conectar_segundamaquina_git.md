# Skill Plan - connect-secondary-machine-git

## Objetivo

Padronizar configuracao Git/SSH em segunda maquina (`jz`/`jf`) usando scripts parametrizaveis.

## Skill alvo

- `C:\codes\skills\connect-secondary-machine-git`

## Quando usar

1. Segunda maquina nao autentica em GitHub/GitLab.
2. Troca de maquina com necessidade de reaproveitar chave SSH.
3. Falha apos bootstrap de repositorios por indice.

## Scripts oficiais

1. `scripts/copiar-chave-segundamaquina.ps1`
2. `scripts/configurar-ssh-segundamaquina.ps1`
3. `scripts/validar-segundamaquina.ps1`

## Resultado esperado

1. Chave instalada em `~/.ssh` com configuracao valida.
2. `ssh-agent` ativo e chave carregada.
3. Teste de conectividade positivo para `github.com` e/ou `gitlab.com`.

