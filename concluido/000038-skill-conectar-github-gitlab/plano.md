# Skill Plan - connect-github-gitlab

## Objetivo

Estabelecer padrao de recuperacao de conectividade Git com GitHub/GitLab por scripts parametrizaveis.

## Skill alvo

- `C:\codes\skills\connect-github-gitlab`

## Quando usar

1. `Permission denied (publickey)`.
2. `Could not read from remote repository`.
3. `ssh-agent` parado ou sem chave carregada.
4. Falha de autenticacao em `fetch/pull/push`.

## Scripts oficiais

1. `scripts/diagnosticar-conexao-git.ps1`
2. `scripts/configurar-ssh-windows.ps1`
3. `scripts/gerar-chave-ssh.ps1`
4. `scripts/testar-conexao-remota.ps1`

## Resultado esperado

1. Conexao validada para `github.com` e/ou `gitlab.com`.
2. Ambiente com OpenSSH do Windows padronizado.
3. Evidencia registrada em chamado.

