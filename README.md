# RECEBA BI

Dashboard operacional e financeiro da Receba Logistica.

## Rodar local

```bash
npm install
npm start
```

Acesse:

```text
http://localhost:3000
```

## Publicar na Railway

1. Crie um novo projeto na Railway a partir do repositório GitHub.
2. A Railway detecta Node.js automaticamente.
3. O comando de start já está configurado:

```bash
npm start
```

4. O app usa a porta automática da Railway através de `process.env.PORT`.

## Pasta BI

Por padrão, o sistema lê os arquivos Excel em:

```text
BI/
```

O financeiro deve ficar em:

```text
BI/FINANCEIRO/
```

Na Railway, se você criar um Volume, pode montar o volume e configurar a variável:

```text
BI_DIR=/caminho/do/volume/BI
```

Se `BI_DIR` ou o volume estiverem vazios, o sistema usa a pasta `BI` versionada no repositório.

## Login

Os logins autorizados estão configurados no frontend. A senha inicial é:

```text
RECEBA99
```

No primeiro acesso, o usuário deve criar uma nova senha.
