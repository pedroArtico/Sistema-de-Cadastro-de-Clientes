O sistema consiste em um cadastro de clientes em uma loja, utilizando `HTML`, `CSS`, `PHP` ou `JavaScript`. O sistema deverá utilizar o **SGBD MySQL e permitir o cadastramento e a consulta de dados de clientes apenas para usuários que estiverem autenticados.

A primeira tela a ser exibida para qualquer usuário que acessar o sistema deve conter dois campos de um formulário para autenticação: um para o **usuário** e o outro para a **senha** (e um botão para enviar os dados fornecidos). 

Caso o usuário autenticado seja o/a **gerente** da loja (usuário: *admin* – senha: *admin*), ele terá duas opções de uso do sistema. Na primeira deverá ser exibido o **formulário de cadastro de um cliente** (com todos os campos descritos a seguir). 

Caso o gerente forneça os dados de um cliente ainda não cadastrado, este cliente será **inserido no sistema**. Caso o cliente já exista (identificado pela **chave** CPF), os valores fornecidos nos campos deverão ser utilizados para **atualizar o cadastro** deste cliente. Na segunda opção de uso, o gerente deverá poder **visualizar os dados de todos os clientes** cadastrados no sistema.

Caso o usuário autenticado seja um **cliente** comum, ele terá acesso apenas à **tela de consulta** e **atualização de seus dados cadastrais**.

Além disso, todos os usuários autenticados devem ter a opção de **sair** do sistema. Quando isto ocorrer, o sistema deverá retornar para a tela inicial de *login*.

O sistema deverá manter os seguintes dados referentes a um **cliente**: 

* Nome completo
* Data de aniversário 
* CPF (chave) 
* Telefone 
* E-mail
* Endereço:
	* Rua 
	* Número
	* Bairro
	* Complemento
	* Cidade
	* CEP
	* País

### Observações:

* Tanto os dados dos clientes como os dados de usuários do sistema devem ser mantidos em tabelas do MySQL/MariaDB. Cabe ao grupo definir a organização destas tabelas e **indicar** (em um arquivo-texto na pasta do sistema) **qual SGBD foi usado nos testes**.

* Deverá ser entregue um *script* PHP (separado do projeto principal) para criar as tabelas necessárias para o correto funcionamento do sistema, além de um arquivo-texto com instruções para sua utilização.

* Os dados do usuário *gerente* (usuário e senha) devem ser **pré-cadastrados no Banco de Dados** pelo *script* responsável pela criação das tabelas no SGBD.

* Utilize **sessões** para fazer o controle de acesso ao sistema.

* Todos os documentos gerados **devem seguir o padrão HTML5**.

* O grupo deve incluir **pelo menos** uma folha de estilo externa.

* **Não é permitido o uso de frameworks PHP.**

### Regras Gerais:

* Este trabalho terá peso igual ao do primeiro trabalho (*site*).

* Este trabalho deve ser desenvolvido pelo mesmo grupo definido no início da disciplina.

* Deverá ser entregue um arquivo .ZIP contendo **todos** os arquivos necessários para execução e exibição correta dos *scripts* (`.html`, `.js`, `.css`, `.php`, imagens etc.). Favor manter, no arquivo .ZIP, a estrutura de diretórios necessária para execução do sistema.
