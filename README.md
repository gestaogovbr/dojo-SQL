# dojo-SQL
Este repositório contém o material para realização do **DOJO sobre SQL**. O objetivo deste Dojo é treinar o uso da linguagem de SQL. Ou seja, pretendemos exercitar a compreensão e escrita de *Queries SQL*.

Para o exercício foi escolhido um banco de dados contendo registros de locadora de DVD. As tabelas estão organizadas como dispostas no diagrama a seguir:

![Diagrama da base dados](dvd-rental-sample-database-diagram.png)

# Como rodar

Estão incluídos um Script `docker-compose` que inicializa 2 containers, um para rodar o servidor de banco de dados PostgreSQL e outro para rodar a aplicação PgAdmin, utilizada para acessar o BD e onde executaremos as consultas SQL.

1. Clone o código deste repositório `$ git clone https://github.com/economiagovbr/dojo-SQL.git`
2. Acesse o diretório do material `$ cd dojo-SQL`
3. Execute o Docker-Compose para rodar os 2 containers `$ sudo docker-compose up`
4. Acesse o **PgAdmin** no navegador através do enderço local [http://localhost:5555/](http://localhost:5555/) e utilize o email `pgadmin4@pgadmin.org` e a senha `admin` para logar na aplicação
5. Crie uma nova conexão com o PostgreSQL utilizando o host: `postgres`, na porta padrão `5432`, nome de usuário `postgres` e senha `postgres`. Insira um nome qualquer para salvar esta nova conexão
6. Através da interface gráfica (utilizando o menu ou o botão direito do mouse na árvore), crie um novo banco de dados (*Database*) com o nome `dvdrental`
7. Através da interface gráfica (utilizando o menu ou o botão direito do mouse na árvore), restaure o dump **dentro do banco de dados recém criado**. Para isso utilize a opção de realizar *Upload* do arquivo `dvdrental.tar` que está disponível na raiz deste diretório.
8. MÃOS À MASSA!
9. Para iniciar, listamos no arquivo [desafios.md](desafios.md) algumas questões introdutórias sobre a base de dados de aluguel de DVDs.