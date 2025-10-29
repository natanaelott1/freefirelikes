# BanCheck via GitHub Actions

This repo provides a GitHub Actions workflow to check Free Fire ban status using `https://bancheck.tsunstudio.pw/bancheck`.

## Como usar

1. Faça commit/push deste repositório no GitHub.
2. Vá em **Actions → BanCheck** no repositório.
3. Clique em **Run workflow**.
4. Insira o `uid` e (opcional) `key` (padrão: `saeed`) e execute.
5. Aguarde o run concluir. Na página do run:
   - Veja os logs (o JSON da resposta é impresso).
   - Faça download do artifact `bancheck-result-{run_id}` que contém `result.json`.

## Observações de segurança e privacidade

- O workflow roda no servidor do GitHub Actions (Ubuntu runner). A chamada API é feita por lá.
- Não partilhe UIDs sensíveis sem consentimento.
- Se quiseres tornar isto automático (ex.: um bot que roda periodicamente), podemos adaptar o workflow — mas verifica limits e termos do serviço antes.
