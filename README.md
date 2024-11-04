Foi utilizado HTML e CSS para estruturar e estilizar de forma básica a página. Também foi utilizado o HTML para fazer as funcionalidades.

Foi utilizado o NODE.JS para criar o servidor e o Express para criar a rota API. O banco de dados foi utilizado para armazenar os dados após o cadastro do usuário.



# DEPLOY:
- 



1. Banco de dados:

- Certifique-se de ter instalado o MySQL Workbench em seu computador.

- Abra o MySQL e selecione o workbench, use a senha "root" para acessá-la.

- Copie o código do arquivo SQL presente no arquivo do VScode, cole no workbench do MySQL e certifique-se de salvar para testar o código, utilizando "ctrl + enter" em todo ele, ou selecionando todo código e clicando no ícone do raio.

- ATENÇÃO: Lembre-se de sempre que for utilizar o código salve o "use Bilu_StoreOFC", para confirmar o uso do banco de dados.

- Para conferir se algo está salvo no banco de dados use "SELECT * FROM usuarios".


2. Node

- Certifique-se de possuir instalado na máquina o Git Bash e execute-o.

- Utilize os comandos em ordem: "cd trabalho_deploy"/"cd Back-end"/, para poder acessar a pasta do arquivo.

- Certifique-se de possuir o Node instalado no dispositivo.

- Utilize o comando "npm i" para baixar os arquivos JSON.

- Utilize o comando "npm start" para rodar o sistema do NODE.

- O node também pode ser usado no terminal do VScode, no qual você deve usar o comando "cd Back-end" e o npm start.


3. Testando a API

- Para testar a API, certifique-se de que esteja instalado no computador o thunder client (Caso não tenha instalado, clique na opção extensões, no VScode, e pesquise por thunder client, então é só instalar).

- Abra o Thunder client no Visual code.

- Clique na opção New request.

- Selecione o método a ser utilizado (POST, GET, USE, etc).

- Adicione a URL aonde se pede.

- Clique na opção "Body", abaixo de onde é inserido a URL, e teste de acordo com os exemplos mostrados abaixo.

- Após isso, clique na opção "Send" (certifique-se de que o npm esteja rodando e o banco de dados esteja sendo usado. Caso não esteja, utilize o "npm start" no git bash e salve o "use deployCadastro" no banco de dados).



<!-- Cadastrar o usuário! -->

- É necessário utilizar o método POST

# URL: http://localhost:3001/usuario/cadastrar

# POST(/usuario/cadastrar)

- BODY:
{
    "cpf": "cpf do usuário",
    "nome": "nome do usuário",
    "email": "email do usuário",
    "senha": "senha do usuário"
}

Retorna as mensagens de sucesso ao funcionar e sem sucesso quando não funcionar.

# Essa API serve para criar um novo usuário no sistema.
