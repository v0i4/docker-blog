para startar a aplicacao:
- configurar p dev.exs com o seu banco de dados postgres

para startar a aplicacao com o docker-compose:
- precisa configurar o dev.exs > hostname para 'db'

para startar a aplicacao em ambiente de docker de producao
-necessario passar como variaveis de ambiente: SECRET_KEY_BASE, DATABASE_URL

-docker build -t nomerepo/nomeapp:versao .
-docker run --env-file .env -p 8080:4000 nomerepo/nomeapp:versao

