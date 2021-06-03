# BoilerPlate NodeJS TS

- Message Linter /_Garante que os commits serão dentro do padrão [conventional](https://www.conventionalcommits.org/en/v1.0.0/#specification) _/

  - <code> npm i -D git-commit-msg-linter</code>

- TypeScript /_Usar o tsconfig.json como base_/

  - <code>npm i -D typescript @types/node</code>

- Linter /_Usar o .eslintrc.json, .eslintignore, .prettierrc e .editorconfig como base_/
  - <code>npm i -D eslint eslint-config-standard-with-typescript eslint-plugin-import eslint-plugin-promise eslint-plugin-node @typescript-eslint/eslint-plugin </code>
  - <code>npm i -D --exact prettier</code>
  - <code>npm i -D eslint-plugin-prettier eslint-config-prettier</code>
  - Adicionar ao arquivo .vscode/settings.json
    - <code>{ "editor.formatOnSave": false, "editor.codeActionsOnSave": { "source.fixAll.eslint": true } }</code>

### Git Hooks

- Garantir que o código esteja formatado corretamente antes do commit/_Usar .lintstagedrc.json e .huskyrc.json como base_/
  - <code>npm i -D lint-staged husky</code>

### Jest

- Biblioteca de testes /_usar o jest.config.js como base e scripts estão package.json_/
  - <code>npm i -D jest @types/jest ts-jest faker</code>

### Sucrase

- <code>npm i -D sucrase</code>
- Adicionar o comando no package.json para executar o servidor de desenvolvimento para TS
  - <code>"start": "sucrase-node src/main/server.ts"</code>
