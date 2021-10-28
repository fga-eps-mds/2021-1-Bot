# Como instalar e configurar o rasa
Este e um tutorial de instalação do rasa para poder utilizado


## Começando
Certifique-se de que você tem o python 3 instalado com o pip3 verificando suas versões
siga os este passo e va para o terminal digitar:

    python3 --version
    pip3 --version
    
Instale as dependencias e o rasa:

    

    pip3 install -U pip
    pip3 install rasa
    

### Rasa
Atualize o local aonde esta o rasa e baixe a dependencia do python:

    sudo apt update
    sudo apt install python3-dev python3-pip

Configure o ambiente virtual disponivel da linguagem python:

    python3 -m venv ./venv
    source ./venv/bin/activate

### Teste o bot inicial fornecido pelo framwork rasa
Inicie o rasa:

    rasa init
    
    
### Depois de iniciar o rasa vai pedir para cria o direito
    
    
    Exemplo casa ,toda vez que for testar o bot tera que ir na pasta /casa e inciar os comandos

Voltando para testar novamente:
        
        
    
    rasa train
    rasa shell


## Referências Use as para mais explicações
- [Rasa installation](https://rasa.com/docs/rasa/installation)

