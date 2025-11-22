## azure-frontier-girls-challenge

# **Challenge AFG**
## Conceito inicial de agente

No Challenge meu foco inicial era criar um agente para me ajudar na rotina de criação. Tenho uma marca de acessórios nada básicos e sou a responsável pelo desenvolvimento de novas peças e coleções.  Gostaria de criar um agente que pudesse me ajudar na pesquisa de tendências e inovações na moda e que fosse capaz de gerar um moodboard com sugestões para que eu consiga agilizar meu processo criativo

## Fluxo 

<img width="928" height="681" alt="Generated Image2" src="https://github.com/user-attachments/assets/74e91323-6606-4043-b5c6-a110c315d6d4" />


Conversando com o Copilot sobre o projeto ele chegou a sugerir esse outro fluxo:

<img width="512" height="768" alt="Flowchart diagram of" src="https://github.com/user-attachments/assets/aea004a4-58bf-42f5-850e-186127eb3be5" />



## Criação de um agente, tipo o Copilot, através da plataforma Azure.

No Challenge meu foco inicial era criar um agente que pudesse me ajudar na rotina de criação. Tenho uma marca de acessórios e sou a responsável pelo desenvolvimento de novas peças e coleções.  Gostaria de criar um agente que me ajudesse na pesquisa de tendências e inovações na moda para que eu consiga agilizar meu processo criativo.  
A princípio estava planejando criar um agente integrando o gpt-4o e o dall-e 3 para gerar moodboards. No entanto devido a limitações de cotas na conta de estudante no Azure acabei modificando um pouco o projeto, já que não foi possível a implantação do DALL-E(teria que fazer uma solicitação de aumento de cota, que poderia levar tempo para sair e talvez não saísse até o prazo final para envio do projeto). Com o auxílio do Copilot e do Gemini cheguei ao prompt que utilizei na criação do agente no Foundry, utilizando o gpt-4o, que gera um prompt para ser usado com o DALL-E.


## Criação de um Grupo de Recurso no Azure

Foi criado o resource group e nele foi criado o projeto no Foundry

<img width="1917" height="913" alt="Screenshot 2025-11-20 184731" src="https://github.com/user-attachments/assets/4772495c-5561-43e8-a038-62c41e902e56" />


## Implementação do projeto no Foundry
Foram diversas tentativas até conseguir implementar o GPT-4o, pois muitos dos modelos que estava tentando selecionar, não tinham cota disponível para conta de estudante ou não estavam disponíveis na região selecionada. Cheguei a tentar algumas vezes o GPT-4o-mini sem sucesso. Em seguida fui tentar implementar um agente de text to image para usar em conjunto com o gpt-4o no agente.

Acabei esquecendo de tirar prints desse inicio da implementação do agente de chat

<img width="1407" height="893" alt="image" src="https://github.com/user-attachments/assets/771db1bc-82b2-48f5-81cb-37710542059c" />


## Tentativas de implementacao de um agente Text to Image
Com o auxilio do Copilot que havia sugerido o uso do Dall-e 3 para a geração de imagens e moodboard, fui tentar fazer a implementação, mas devido as restrições da conta de estudante, não foi possível.
<img width="1920" height="1080" alt="Screenshot 2025-11-20 161345" src="https://github.com/user-attachments/assets/45fb933b-229b-4541-81d7-57a5a2ee3bbe" />


<img width="1882" height="913" alt="Screenshot 2025-11-20 161119" src="https://github.com/user-attachments/assets/bc362d9c-c5bc-442d-bf97-e405a5ee3e9b" />
</br></br>

<img width="414" height="466" alt="Screenshot 2025-11-20 161147" src="https://github.com/user-attachments/assets/0f640a6c-696d-4514-839f-a0a24ef8ef93" />
</br></br>

<img width="1920" height="1080" alt="Screenshot 2025-11-20 161806" src="https://github.com/user-attachments/assets/712edcca-690a-4571-8f8f-9cffd35227f0" />
</br></br>

<img width="394" height="444" alt="Screenshot 2025-11-20 161905" src="https://github.com/user-attachments/assets/00b3f2c6-668e-45c5-8136-d67d8efc8313" />
</br></br>

<img width="404" height="419" alt="Screenshot 2025-11-20 161926" src="https://github.com/user-attachments/assets/ad00e076-21d5-47dc-9c20-dc9e75556139" />
</br></br>


### Fiz a gravação da tentativa de implementação do DALL-e  https://youtu.be/Kv_E_L9gI5c


Tentei outros modelos de text to image além do Dall-e, mas também, sem sucesso.


<img width="1247" height="891" alt="Screenshot 2025-11-20 163128" src="https://github.com/user-attachments/assets/0081d6b1-df40-4244-8b63-0ab7d3c8876e" /></br>
<img width="1597" height="832" alt="Screenshot 2025-11-20 163151" src="https://github.com/user-attachments/assets/926c7df3-a508-4473-9afb-78bf92d9fbba" /></br>
<img width="1245" height="895" alt="Screenshot 2025-11-20 163250" src="https://github.com/user-attachments/assets/0a7f8479-a33a-4954-b160-728835963667" /></br>
<img width="1623" height="417" alt="Screenshot 2025-11-20 163305" src="https://github.com/user-attachments/assets/7232bbfe-069d-4321-a160-aa04465b34a6" /></br>



## Definindo as funções do agente 

Então fui fazer as definições do que o meu agente consultor deveria fazer. Para verificar se o projeto que tinha em mente seria possível de criar com a conta de estudante e o orçamento de dela, fui conversar com o Copilot e o Gemini. O Copilot estava gerando um passo a passo da criação do agente, porém o Gemini foi mais específico em relação a questão de custos e viabilidade do projeto com o orçamento de $100, acabei concordando com a sugestão que o Gemini me apresentou de inserir no prompt do agente a orientação de que o agente gerasse o prompt para o Dall-e para que esse depois fosse usado na criação de um moodboard ou de imagens de referência. Inicialmente queria ter integrado essa funcionalidade ao meu agente, mas por conta das limitações da conta de estudante, fiz essa adaptação.

<img width="1895" height="903" alt="Screenshot 2025-11-20 164918" src="https://github.com/user-attachments/assets/0e429b79-a8bc-4767-ae4c-23538841a704" />
<img width="953" height="385" alt="Screenshot 2025-11-20 165357" src="https://github.com/user-attachments/assets/b01d7ad3-3b2c-481d-b3aa-315199cfc1e0" />
<img width="924" height="375" alt="Screenshot 2025-11-20 165418" src="https://github.com/user-attachments/assets/910a4fe5-f776-404a-b57d-001b50fca060" />
<img width="810" height="189" alt="Screenshot 2025-11-20 165455" src="https://github.com/user-attachments/assets/f05c2279-b82c-4328-afed-ac37a74f204c" />
<img width="858" height="495" alt="Screenshot 2025-11-20 165524" src="https://github.com/user-attachments/assets/794297a9-0356-44bb-97dd-6ced9de1e746" />
<img width="848" height="270" alt="Screenshot 2025-11-20 165550" src="https://github.com/user-attachments/assets/47d3ad40-0f23-43de-8b41-5582d8915425" />



## Configuração do agente

### Fiz a gravação da configuracao do agente: https://youtube.com/shorts/WTwwAB-bKdU



## Teste no Playground

Feito isso segui para o Playground para testar o modelo
### Vídeo do chat no Playground com o agente https://youtu.be/fY42QT3kOIw

<img width="1920" height="1080" alt="Screenshot 2025-11-20 165651" src="https://github.com/user-attachments/assets/94755971-3d83-49a1-b044-7f4be38b3f37" />

<img width="1649" height="845" alt="Screenshot 2025-11-20 165717" src="https://github.com/user-attachments/assets/9ae91c87-f6a3-449e-a142-e421c2fabfa7" />

<img width="1674" height="838" alt="Screenshot 2025-11-20 170217" src="https://github.com/user-attachments/assets/f9ec7909-d9a7-46c3-acf4-e6f6a84871e7" />

<img width="1427" height="712" alt="Screenshot 2025-11-20 170248" src="https://github.com/user-attachments/assets/bed6dd6c-19f7-4946-af04-2d841e69a15d" />

<img width="1474" height="831" alt="Screenshot 2025-11-20 170818" src="https://github.com/user-attachments/assets/df4a86c8-ac8f-4672-a75f-b11f7a5996fa" />

<img width="1453" height="854" alt="Screenshot 2025-11-20 170846" src="https://github.com/user-attachments/assets/869eef62-19b0-4725-b171-de21083d6f3c" />

<img width="1464" height="858" alt="Screenshot 2025-11-20 170907" src="https://github.com/user-attachments/assets/5dff8a2f-5c35-4e7a-be0b-5f008c6832fb" />

### Código do agente

```python

from azure.ai.projects import AIProjectClient
from azure.identity import DefaultAzureCredential
from azure.ai.agents.models import ListSortOrder

project = AIProjectClient(
    credential=DefaultAzureCredential(),
    endpoint="https://aif-afg-challenge.services.ai.azure.com/api/projects/proj-afg-challenge")

agent = project.agents.get_agent("asst_lA7NfSOkeaVeaf6fL6T8f3S1")

thread = project.agents.threads.create()
print(f"Created thread, ID: {thread.id}")

message = project.agents.messages.create(
    thread_id=thread.id,
    role="user",
    content="Hi Agent Consultor"
)

run = project.agents.runs.create_and_process(
    thread_id=thread.id,
    agent_id=agent.id)

if run.status == "failed":
    print(f"Run failed: {run.last_error}")
else:
    messages = project.agents.messages.list(thread_id=thread.id, order=ListSortOrder.ASCENDING)

    for message in messages:
        if message.text_messages:
            print(f"{message.role}: {message.text_messages[-1].text.value}")
```
            

<img width="1124" height="909" alt="Screenshot 2025-11-20 170601" src="https://github.com/user-attachments/assets/540b768e-4a01-4e00-9902-2492bc902cbd" />

## Referências
- ### Aulas do curso sobre a criação do agente https://github.com/Miyake-Diogo/AzureFrontierGirls-AI-Challenge
      - https://www.youtube.com/watch?v=drXfes7p9sg
      - https://www.youtube.com/watch?v=LnPL1ftGbN4
      - https://www.youtube.com/watch?v=0RE8sqlzvdo
      - https://www.youtube.com/watch?v=blQRiAglNsw
  
- ### https://learn.microsoft.com/en-us/azure/ai-foundry/?view=foundry-classic
