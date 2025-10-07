# Microsoft Copilot Studio

- O Copilot Studio é uma ferramenta gráfica low-code para compilar agentes e fluxos de agentes.
- Se conecta com diferentes fontes de dados usando plug-ins predefinidos ou personalizados.
- É uma ferramenta que torna acessível o poder da IA e todos os seus benefícios.

## Agente/Copiloto
- É um companheiro/ajudante, no qual por meio de um sistema de software em conjunto com a inteligência artificial age de forma autônoma, realizando tarefas desde que são mais simples até as que tem um nível maior de complexibilidade.Os agentes coordenam uma coleção de modelos de linguagem, com instruções, contexto, fontes de conhecimento, tópicos, ações, entradas e gatilhos para atingir as metas desejadas.
Exemplo:
````
- Ajuda e problemas de suporte de Vendas.
- Horário de funcionamento e informações da loja.
- Benefícios de férias e saúde para funcionários.
- Informações de rastreamento de saúde pública.
- Perguntas comuns dos funcionários para empresas.
````

## Ambiente
- Um ambiente é um espaço para armazenar, gerenciar e compartilhar dados corporativos da sua organização. Os agentes criados são armazenados em um ambiente (aplicativos e fluxos também são armazenados em ambientes). Os ambientes também podem ter diferentes funções, requisitos de segurança e públicos-alvo, e cada ambiente é criado em um local diferente. 
- Tipos de ambientes:
    - Desenvolvedor
    - Produção
    - Avaliação
    - Área Restrita

## Soluções
- São os mecanismos para gerenciar o ciclo de vidas do aplicativos, atuando como contêineres organizacionais que agrupam e transportam aplicativos, componentes e personalizações de um ambiente para outro.
- Elas permitem a distribuição de objetos como fluxos, tabelas e recursos da web, facilitando a implantação, manutenção e compartilhamento de projetos entre diferentes ambientes de desenvolvimento
- **Versões Gerenciadas e Não Gerenciadas:**
    - Gerenciavel - passando de um ambiente de desenvolvimento para um ambiente de produção, e para que não haja alteração no ambiente em produção. Força a não edição do ambiente em produção
    - Não gerenciavel-  as pessoas poderam editar diretamente no ambiente em produção

## Criando agentes
- Criar um Copilot baseado em modelo

<img src="https://github.com/Fredericobarbosa/microsoft_copilot_dio/blob/main/img/Copilot_modelo.png" alt="Exemplo de agentes já existentes"><br/>

<img src="https://github.com/Fredericobarbosa/microsoft_copilot_dio/blob/main/img/Copilot_modelo_1.png" alt="Tela de criação"><br/>

- Criar um Copilot baseado em descrição com IA

<img src="https://github.com/Fredericobarbosa/microsoft_copilot_dio/blob/main/img/Copilot_descri%C3%A7%C3%A3o.png" alt= "Criando por meio de prompt"><br/>

- Criar um Copilot em branco

<img src="https://github.com/Fredericobarbosa/microsoft_copilot_dio/blob/main/img/Copilot_branco.png" alt="Como criar"><br/>

<img src="https://github.com/Fredericobarbosa/microsoft_copilot_dio/blob/main/img/Copilot_branco_1.png" alt="Tela de criação"><br/>


## Tópicos
- São conversas dentro de um copiloto (ramificações)
- Elas são fixas 
- Sistema (tópico que a Microsoft cria) ou Customização 
- Sempre tem:
    - 1 gatilho com frases
    - 1 ou mais ações

## Melhores práticas do tópico
- Ter de 5-10 frases dentro de um gatilho
- Ter nomes claros e não repetitivos
- Ter frases de gatilho que não conflitem entre outros tópicos
- Ter em mente quando dividir os tópicos ou copilotos diferentes

## Observações:
- 1.11.24.1 - fase_projeto.mês_desenvolvimento.ano.versão_trabalhada
- Para a criação de agentes é melhor de ser feito o prompt em inglês
