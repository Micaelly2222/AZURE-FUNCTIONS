
# Azure

> #  Criando uma função no Azure com o Python usando o Visual Studio Code 



✅ Tecnologias Utilizadas:
> * [x]  Azure Functions Core Tools, versão 3.x.
> * [x] Python 3.9.7
> * [x] Visual Studio Code
> * [x] Extensão Azure Functions para Visual Studio Code.

## 1. Criando o projeto local : 
  ❗ Usar o Visual Studio Code para criar um projeto local do Azure Functions em Python
  
  Escolher o ícone do Azure no Visual Studio Code e ir em : Functions> Criar Projeto> Escolher um diretório > Fornecer as informações solicitadas :
  Uma linguagem para o projeto: Python
  Um modelo para a primeira função: HTTP trigger
  Um nome de função: HttpExample
  Nível de autorização: Anonymous
  
  O Visual Studio Code vai gerar um projeto do Azure Functions com um gatilho HTTP

## 2.Executar a função localmente

❗ O Visual Studio Code vai se integrar ao Azure Functions Core Tools para permitir que execute na maquina antes da publicação no Azure.

Para chamar a função, pressionar F5. Com o Core Tools em execução, acessar a área do Azure> "Executar função agora" > "Insira o corpo da solicitação", pressionar ENTER para enviar essa mensagem de solicitação à função.


## 3.Entrar no Azure
❗ Antes de poder publicar, precisa entrar no Azure.

Se ainda não estiver conectado, escolher o ícone do Azure> Functions> entrar no Azure


## 4. Publicar o projeto no Azure
❗ Criará um aplicativo de funções 

Escolha o ícone do Azure> Functions> " Implantar no aplicativo de funções". Forneçer as informações:
 Selecione a pasta
 Selecione a assinatura
-Inserir um nome para o aplicativo de funções
"Exibir Saída" para exibir os resultados da implantação

## 5. Executar a função no Azure

  De volta na área Azure> função HttpExample >  "Executar Agora" > "Insira o corpo da solicitação"> clicar em ENTER para enviar essa mensagem de solicitação à função.
  Pressionar F1 para abrir a paleta de comandos> Azure Functions: Open in portal> escolher o aplicativo de funções e pressione Enter> a página do aplicativo de funções   é aberta no portal do Azure.

## 6. Testar a função

A função pode ser testada no próprio Visual Studio Code 

Selecionar o depurador no menu à esquerda> selecionar "Attach to Python Functios"> copiar a URL da função no terminal> testar abrindo http://localhost:7071/api/HttpExample em seu navegador> acrescentar o valor de consulta ?name=functions> http://localhost:7071/api/HttpExample?name=functions

Ou na function publicada no Azure
APP functions> copiar URL>https://funcaoazure123.azurewebsites.net/api/HttpExample? > testar no Postman

