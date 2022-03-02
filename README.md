# COLETANDO DADOS DO TWITTER

## OBJETIVO
- A ideia deste script é coletar dados do twitter utilizando a API disponibilizada pela própria empresa e, armazenar em um banco de dados.

## OBSERVAÇÕES
- É necessário criar um cadastro para ter acesso a API do twitter, feito isto, será disponibilizado 4 keys importantes:
- * BEARER_TOKEN, CONSUMER_KEY, 
- * CONSUMER_SECRET, 
- * ACCESS_TOKEN, 
- * ACCESS_TOKEN_SECRET
- Salve estes valores e adicione no código.

## COMO USAR?
* Após gerar esses tokens e inseri-los no código, é bem simples continuar:
* Chame a função connect_twitter com os argumentos necessários.
* Crie um BD, lembre-se que a função retorna dois objetos, o con e o cur.
* Crie um objeto do tipo datetime inserindo o ano/mes/dia/hora/minuto/segundo, da forma que está no código.
* insira quanto tempo será feito a coleta na variável end_minutes_time.
* Insira a query para busca dos tweets, no exemplo foi utilizado a palavra sentimento.
* chame a função extracting_data, passando estes argumentos. Lembre-se que será retornado uma lista. Aqui você já pode percorrer e manusear da forma que quiser.
* Após, chame a funão insert_db, passando o cur, con e o nome da variável que esta armazenada os dados da função anterior.
* Agora, chame a função read_data, informando o nome do bd. Dessa forma, será retornado um DataFrame pronto para ser utilizado.
