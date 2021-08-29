# Configurar o rasa para portugues
Este e um tutorial de edição do rasa

# Para utilizar este Tutorial primeiro faças os passos de instalação do rasa.

Primeiro va para o link do rasa inicial [Rasa instalação](https://github.com/fga-eps-mds/2021-1-Bot/blob/dev_plusultra-from-docs_plusultra/docs/tutoriais/Tutorial_edicao_Rasa.md) 

## Começando
Certifique-se de ir na config.yml e mudar linguagem para pt.

    config.yml

    
Depois va para a pasta com nome /data.
    Nesta caminho configure a os arquivos nos arquivos troque os greet por otimo neste 3 arquivos

    nlu.yml
    rules.yml
    stories.yml


No arquivo  nlu.yml:

    - intent: otimo

    examples: |
        - Oi
        - Bom dia
        - Boa Tarde
        - prevenção    

No arquivo rules.yml


    - rule: Despedida do bot
        steps:
        - intent: goodbye
        - action: utter_goodbye

No arquivo stories.yml


    - story: happy path
        steps:
        - intent: otimo
        - action: utter_greet
        - intent: mood_great
        - action: utter_happy


Agora vamos para o arquivo fora da pasta data chamado:

    domain.yml

e fazer a mesma coisa feito nos 3 arquivos de /data:


    intents:
        - otimo
        - goodbye
        - affirm
        - deny
        - mood_great
        - mood_unhappy
        - bot_challenge



    


    

### Rasa
Agora va para o terminal e execute o comando

    rasa train


E

    rasa shell

E teste as modificações do seu bot
        
        
    


## Referências
- [Rasa installation](https://rasa.com/docs/rasa/installation)

