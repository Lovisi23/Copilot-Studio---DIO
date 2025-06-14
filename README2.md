#  Copiloto com Fluxo de Conversa Personalizado no Microsoft Copilot Studio
## O que aprendi
### Criando um Copilot em Branco
Nessa aula revi os conceitos de como criar um copilot em branco, para isso basta ir na aba "Agents" do Copliot Studio e clicar 
no botão "Create new Agent", nessa aula foi criado um agente no idioma inglês, com o seguinte nome "Agente da DIO"
#### foi adicionada a seguinte descrição: 
Agente responsavel por buscar conteudos de Copilot Studios dentro da documentação oficial da
Microsoft, sendo que toda resposta dele será como o "Agente da DIO".
#### Foram-lhe dada as seguintes instruções:
Você é o agente chamado "Agente da DIO", e vai agir em tom formal com o idioma em português, para retornar informações relevantes 
da documentação oficial da Microsoft, o Microsoft Learn.
Ao retornar uma resposta para a pergunta do usúario você deve considerar:
- Buscar a melhor resposta na documentação
- Retornar a resposta apropriada e amigável de tom formal
- Retornar uma ou mais citações da documentação
#### Knowledge
eu adicionei o site do Microsoft Learn em sua aba de conhecimentos
### Costumizar um tópico
Nessa aula foi criado um novo tópico em branco com o nome de "AI Builder Topics", onde foi possivel configurar suas frases de "trigger", ou seja, de gatilho e depois
foi criado um node de IA generativa com um input do próprio texto do usúario conectado ao trigger, além de um outro node sequencial ao anterior que manda uma mensagem de encerramento do tópico.
#### Triggers
- buscar informações de ai builder
- o que é ai builder
- onde encontro informações da ferramenta de AI da Power Plataform
### Personalizar uma mensagem de erro
O copilot studio já tem tópicos padrões para mensagem de erro que podem ser achados na aba sistema, como o Fallback e Conversational Boosting,
que são ativados quando o agente não reconhce uma mensagem do usuario, nesse caso foi adicionada uma condição no tópico Conversational Boosting,
em que a IA retorna uma mensagem contendo a variavel "user.Personalname" e uma mensagem com um telefone ou email para o usuario entrar em contato
### Aumentar ou diminuir a qualidade da resposta GenAI
nas propriedades do node de AI, se pode botar outro prompt para deixar ainda mais detahada a pesquisa da IA, além de se poder mudar a content moderation do Agente,
podendo seta-la para High ou Low, em que High ele pega so documentos com prompr igual e Low ele pega todos documentos que contenham algum pedaço do prompt(menos especifico)

