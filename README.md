- Foi utilizado HTML e CSS para estruturar e estilizar de forma básica a página. Também foi utilizado o HTML para fazer as funcionalidades.

- Foi utilizado o NODE.JS para criar o servidor e o Express para criar a rota API. O banco de dados foi utilizado para armazenar os dados após o cadastro do usuário.



# DEPLOY:
* Front e Back-end:
Para realizar o deploy do front-end e back-end, foi utilizada a plataforma de hospedagem, GitHub Pages.
- Como utilizar?
É necessário que você acesse o site "Github.com", faça seu login (caso não tenha um, cadastre-se).
- Assim que você acessar a página inicial, clique no botão verde "new".
- Adicione o nome da pasta e marque a opção "ADD README".
- AVISO: Lembre-se de deixar o repositório na opção "público".
- Após isso clique no botão verde "Create repository".
- Após clicar no botão, você irá para outra página com alguns códigos, e caso você queira selecionar um arquivo existente, clique na opção "uploading an existing file".
- Clique em "choose your files" e arraste os arquivos do projeto para o repositório, adicione uma descrição no commit e clique no botão "Commit changes".
- Escreva no README a documentação do projeto.
- Após isso, clique em "Settings" ou "Configurações", na parte superior do site.
- Na seção "Code and Automation", clique em "Pages" (última opção).
- Mude o Branch de "None" para "Main", após isso irá aparecer "/ (root)". Isso não é para alterar. Após isso é só clicar em salvar, esperar um pouco, atualizar a página e copiar o link que irá aparecer depois de pouco tempo de espera.
- O link será mais ou menos assim "https://nomeusuario.github.io/nomeProjeto/", com seu nome de usuário antes de ".github.io/" e o nome do projeto após a barra.


* Banco de dados:
Para realizar o deploy do banco de dados, foi utilizada a plataforma de hospedagem, Clever Clouds.
- Como utilizar?
É necessário que você acesse o site "https://www.clever-cloud.com", após isso clique em "Free Trial", no caso, um teste grátis. Você possui a opção de se cadastrar com a conta do GitHub ou com sua conta do google e criando uma senha.
- Clique em "Personal space", no canto superior esquerdo da tela.
- Clique na opção "Create" e selecione "an add-on".
- Selecione o banco de dados utilizado, nesse caso, o MySQL.
- Selecione a versão gratuita "Dev", após isso, arraste até o final da página e clique em "Next".
- Escolha o nome do banco de dados e a localização dele.
- Depois de criar o banco de dados, acesse ele no canto superior esquerdo da tela.
- Após clicar no banco criado, clique em "Addon dashboard".
- Clique em "PHPMyAdmin", ao lado de "Admin", no canto superior da tela.
- Após clicar em "PHPMyAdmin", clique em "SQL" e escreva o código do banco de dados do projeto.

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
