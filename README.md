# Azure

> #  Criando uma função no Azure com o Python usando o Visual Studio Code 



✅ Configurando o ambiente:
> * [x]  Azure Functions Core Tools, versão 3.x.
> * [x] Python 3.9.7
> * [x] Visual Studio Code
> * [x] Extensão Azure Functions para Visual Studio Code.

## 1. Criando o projeto local : 
  ❗ Usará o Visual Studio Code para criar um projeto local do Azure Functions em Python
1. Escolha o ícone do Azure na Barra de atividade e, em seguida, na área Azure: Functions e selecione o ícone Criar projeto
2. Escolha um local de diretório
3. Forneça as seguintes informações nos prompts:
- Selecione uma linguagem para o projeto de função: Python
- Selecione um modelo para a primeira função: HTTP trigger.
- Forneça um nome de função: HttpExample.
- Nível de autorização: Anonymous

4. O Visual Studio Code gera um projeto do Azure Functions com um gatilho HTTP

## 2.Executar a função localmente
❗ O Visual Studio Code integra-se ao Azure Functions Core Tools para permitir que execute no computador de desenvolvimento local antes da publicação no Azure.
1. Para chamar a função, pressione F5. A saída do Core Tools é exibida no painel Terminal. 
2. Com o Core Tools em execução, acesse a área Azure: Funções. Clique em : "Executar função agora".
3. Em "Insira o corpo da solicitação", pressione ENTER para enviar essa mensagem de solicitação à função.
4. Quando a função é executada localmente e retorna uma resposta, uma notificação é gerada no Visual Studio Code. 
5. Pressione Ctrl + C para parar o Core Tools e desconectar o depurador.

## 3.Entrar no Azure
❗ Antes de poder publicar, precisa entrar no Azure.
1. Se ainda não estiver conectado, escolha o ícone do Azure na barra Atividade e, em seguida, na área Azure: Functions, escolha Entrar no Azure
2. Após entrar com êxito, poderá fechar a nova janela do navegador.

## 4. Publicar o projeto no Azure
❗ Criará um aplicativo de funções e os recursos relacionados à assinatura do Azure 
1. Escolha o ícone do Azure na Barra de atividade e, em seguida, na área Azure: Functions, escolha o botão Implantar no aplicativo de funções.
2. Forneça as seguintes informações nos prompts:
- Selecione a pasta: escolha uma pasta
- Selecione a assinatura
- Insira um nome para o aplicativo de funções
- Selecione um runtime: Escolha a versão do Python em que você está executando localmente. É possível usar o comando python --version para verificar a versão.
3. Escolha "Exibir Saída" para exibir a criação e os resultados da implantação

## 5. Executar a função no Azure

1. De volta na área Azure. Clique na função HttpExample e escolha Função "Executar Agora"
2. Em Insira o corpo da solicitação, clique em ENTER para enviar essa mensagem de solicitação à função.
3. Pressione F1 para abrir a paleta de comandos. Pesquise e selecione Azure Functions: Open in portal.
4. Escolha o aplicativo de funções e pressione Enter. A página do aplicativo de funções é aberta no portal do Azure.



