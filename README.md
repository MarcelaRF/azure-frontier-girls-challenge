## azure-frontier-girls-challenge

## **Challenge AFG**
### Criação de um agente, tipo o Copilot, através da plataforma Azure.

No Challenge meu foco inicial era criar um agente que pudesse me ajudar na rotina de criação. Tenho uma marca de acessórios e sou a responsável pelo desenvolvimento de novas peças e coleções.  Gostaria de criar um agente que me ajudesse na pesquisa de tendências e inovações na moda para que eu consiga agilizar meu processo criativo.  
A princípio estava planejando criar um agente integrando o gpt-4o e o dall-e 3 para gerar moodboards. No entanto devido a limitações de cotas na conta de estudante no Azure acabei modificando um pouco o projeto, já que não foi possível a implantação do DALL-E(teria que fazer uma solicitação de aumento de cota, que poderia levar tempo para sair e talvez não saísse até o prazo final para envio do projeto). Com o auxílio do Copilot e do Gemini cheguei ao prompt que utilizei na criação do agente no Foundry, utilizando o gpt-4o, que gera um prompt para ser usado com o DALL-E.

## Criação de um Grupo de Recurso no Azure
<img width="1917" height="913" alt="Screenshot 2025-11-20 184731" src="https://github.com/user-attachments/assets/4772495c-5561-43e8-a038-62c41e902e56" />

## Implementação do projeto no Foundry

<img width="1920" height="1080" alt="Screenshot 2025-11-20 184408" src="https://github.com/user-attachments/assets/1eec9aee-f54d-4cad-bb65-8f95fce8b40e" />

Foram diversas tentativas até conseguir implementar o GPT-4o, pois muitos dos modelos que estava tentando selecionar, não tinham cota disponível para conta de estudante ou não estavam disponíveis na região selecionada. Cheguei a tentar algumas vezes o GPT-4o-mini sem sucesso.



<img width="1920" height="1080" alt="Screenshot 2025-11-20 161345" src="https://github.com/user-attachments/assets/45fb933b-229b-4541-81d7-57a5a2ee3bbe" />
<img width="1882" height="913" alt="Screenshot 2025-11-20 161119" src="https://github.com/user-attachments/assets/bc362d9c-c5bc-442d-bf97-e405a5ee3e9b" />
<img width="827" height="933" alt="Screenshot 2025-11-20 161147" src="https://github.com/user-attachments/assets/0f640a6c-696d-4514-839f-a0a24ef8ef93" />


<img width="1920" height="1080" alt="Screenshot 2025-11-20 161806" src="https://github.com/user-attachments/assets/712edcca-690a-4571-8f8f-9cffd35227f0" />
<img width="788" height="889" alt="Screenshot 2025-11-20 161905" src="https://github.com/user-attachments/assets/00b3f2c6-668e-45c5-8136-d67d8efc8313" />
<img width="809" height="838" alt="Screenshot 2025-11-20 161926" src="https://github.com/user-attachments/assets/ad00e076-21d5-47dc-9c20-dc9e75556139" />

tentei outros modelos de text to image, mas tambem sem sucesso.
<img width="1247" height="891" alt="Screenshot 2025-11-20 163128" src="https://github.com/user-attachments/assets/0081d6b1-df40-4244-8b63-0ab7d3c8876e" />
<img width="1597" height="832" alt="Screenshot 2025-11-20 163151" src="https://github.com/user-attachments/assets/926c7df3-a508-4473-9afb-78bf92d9fbba" />
<img width="1245" height="895" alt="Screenshot 2025-11-20 163250" src="https://github.com/user-attachments/assets/0a7f8479-a33a-4954-b160-728835963667" />
<img width="1623" height="417" alt="Screenshot 2025-11-20 163305" src="https://github.com/user-attachments/assets/7232bbfe-069d-4321-a160-aa04465b34a6" />

Então fui fazer as definições do que o meu agente deveria fazer.
<img width="1895" height="903" alt="Screenshot 2025-11-20 164918" src="https://github.com/user-attachments/assets/0e429b79-a8bc-4767-ae4c-23538841a704" />
<img width="953" height="385" alt="Screenshot 2025-11-20 165357" src="https://github.com/user-attachments/assets/b01d7ad3-3b2c-481d-b3aa-315199cfc1e0" />
<img width="924" height="375" alt="Screenshot 2025-11-20 165418" src="https://github.com/user-attachments/assets/910a4fe5-f776-404a-b57d-001b50fca060" />
<img width="810" height="189" alt="Screenshot 2025-11-20 165455" src="https://github.com/user-attachments/assets/f05c2279-b82c-4328-afed-ac37a74f204c" />
<img width="858" height="495" alt="Screenshot 2025-11-20 165524" src="https://github.com/user-attachments/assets/794297a9-0356-44bb-97dd-6ced9de1e746" />
<img width="848" height="270" alt="Screenshot 2025-11-20 165550" src="https://github.com/user-attachments/assets/47d3ad40-0f23-43de-8b41-5582d8915425" />

Feito isso segui para o Playground para testar o modelo
<img width="1920" height="1080" alt="Screenshot 2025-11-20 165651" src="https://github.com/user-attachments/assets/94755971-3d83-49a1-b044-7f4be38b3f37" />



