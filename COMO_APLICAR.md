# Correções para ocatarinav2

Arquivos incluídos:

- `package.json`
- `api/index.js`
- `vercel.json`
- `.gitignore`
- `src/auth/auth-service.js`
- `src/auth/cookies/.gitkeep`

## O que foi feito

1. Adaptação para Vercel via `api/index.js`.
2. Criação de `vercel.json`.
3. Correção da função `authorize` em `auth-service.js`.
4. Inclusão de `.gitignore`.
5. Inclusão explícita de `lodash` e `bluebird` no `package.json`.
6. Mantido `engines.node` como `24.x`.
7. Não foi alterado o arquivo `src/config.js`.

## Como aplicar

Copie os arquivos deste ZIP para a raiz do projeto, substituindo os existentes quando solicitado.

Depois rode:

```bash
git add .
git commit -m "fix: prepare API for Vercel deploy"
git push
```

Depois, na Vercel, faça novo deploy.
