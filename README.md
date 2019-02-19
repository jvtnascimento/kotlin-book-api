# Instruções de como rodar projeto

## Requisitos

- Necessário ter Node.js instalado.
- Necessário ter MongoDB instalado.
- Necessário ter Insomnia instalado.
- NoSQLBooster for MongoDB, caso queira ver os resgistros no banco de dados.

## Iniciar API ## 

- Passo 1: Faça o download do projeto e descompacte, caso tenha baixado como .zip.
- Passo 2: Abra o Prompt de Comando e entre na pasta do projeto.
- Passo 3: Execute o comando 'npm install' para instalar os pacotes necessários.
- Passo 4: Após o download dos pacotes, basta apenas executar o comando _'npm start'_.
- Passo 5: Quando aparecer a mensagem 'Express server listening on port 3001 in development mode', está pronto pra ser utilizado.

_Obs.: O projeto está configurado pra rodar na porta **3001** do **localhost**_

### Testes ###

- Passo 1: Abra o Insomia e clique na seta para abrir o menu. (fica no header de fundo roxo, ao lado do nome do programa)
- Passo 2: Escolha a opção _Import/Export_.
- Passo 3: Na view que irá aparecer, Clique em _Import Data > From File_.
- Passo 4: Vá até a pasta do projeto, entre na pasta **insomia/** e selecione o arquivo **insomnia_workspace** e clique no botão _Import_.
- Passo 5: Após isso você terá em mãos as 3 requests: **Find (GET)**, **FindById (GET)** e **Create (POST)**.

#### POST /book (Create) - Refere-se ao primeiro item do desafio ####

- Você pode passar os dados que desejar através do JSON que já está montado no formato necessário.
- Para executar basta apenas clicar em _'Send'_ que fica no canto superior direito, ao lado da url.
- Caso os dados estejam de acordo com o que o projeto precisa, será retornado o registro salvo no banco de dados.
- Copie o valor do campo "_id_" retornado, pois será necessário para o próximo teste.

#### GET /books/{id} (FindById) - Refere-se ao segundo item do desafio ####

- Com o id do item desejado em mãos, insira ou substitua o valor na url do request após 'books/'. (ex: /books/*_ID AQUI*)
- Para executar basta apenas clicar em _'Send'_ que fica no canto superior direito, ao lado da url.
- Caso o id seja válido, será retornado o registro salvo no banco de dados.

#### GET /books (Find) - Refere-se ao terceiro item do desafio #### 

- Para executar basta apenas clicar em _'Send'_ que fica no canto superior direito, ao lado da url.
- O resultado será retornado com a mesma estrutura especificada no desafio.
