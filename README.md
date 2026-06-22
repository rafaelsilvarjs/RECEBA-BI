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

## Publicar no Render

1. Crie um novo **Web Service** no Render usando este repositorio GitHub.
2. O Render detecta Node.js automaticamente.
3. Use:

```bash
Build Command: npm install
Start Command: npm start
```

4. O app usa a porta automatica do Render por `process.env.PORT`.
5. O arquivo `render.yaml` ja inclui um disco persistente montado em:

```text
/var/data
```

6. Para usar arquivos Excel fora do repositorio, coloque a pasta BI dentro do disco:

```text
/var/data/BI
```

Estrutura esperada:

```text
/var/data/BI/
  CURITIBA/
  GOIANIA/
  RIO DE JANEIRO/
  SAO PAULO/
  FINANCEIRO/
```

Se `/var/data/BI` estiver vazio, o sistema usa a pasta `BI` versionada no repositorio.

## Pasta BI local

Por padrao, em ambiente local, o sistema le os arquivos Excel em:

```text
BI/
```

O financeiro deve ficar em:

```text
BI/FINANCEIRO/
```

## Variaveis opcionais

Voce pode forcar outro caminho para os arquivos BI com:

```text
BI_DIR=/caminho/para/BI
```

## Login

Os logins autorizados estao configurados no frontend. A senha inicial e:

```text
RECEBA99
```

No primeiro acesso, o usuario deve criar uma nova senha.
