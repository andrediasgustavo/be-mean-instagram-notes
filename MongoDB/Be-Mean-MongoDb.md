# Anotações do modulo de MongoDb

NOSQL = NOT ONLY SQL

Tipos de NoSqls

* Documento (MongoDb, CouchDb)
* Grafo (Neo4j)
* Chave-Valor (Redis)
* Coluna (Cassandra("não vamos usar"))
* Misto (OrientDb(Documento e Grafo))

MongoDb é escrito em C++

Aceita JS

Schemaless ("Não tem estrutura de dados difinida")

Trabalha com JSON && BSON ("Forma Binaria do JSON")

Pré-Aloca 80mb de espaço quando cria o Db por isso que na primeira vez que é inserido dados demora muito mais do que nas próximas vezes.

Uma tabela do SQL = Collection E as linhas da tabela = Documento JSON

Comandos MongoDb

Para criar um database e ja dar um checkout para ele 

* use NomedoDb

Para mostrar os Dbs 

* show dbs

E para mostrar as coleções

* show collections

Como exportar uma collection para um arquivo JSON

* mongoexport --db <nomeDB> --collection <nomedacollection> --out <nomedoarquivo.JSON>

E para importar dados de um arquivo para uma collection

* mongoimport --db <nomeDb> --collection <nomedacollection> --drop --file --host=127.0.0.1 <nomedoarquivo.JSON>

Comando para criar uma coleção

* db.createCollection("Nome da Collection")


