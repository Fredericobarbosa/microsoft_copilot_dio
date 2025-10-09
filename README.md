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

## Entidades
- Um modelo pré-definido ou personalizado usado para capturar e estruturar informações específicas fornecidas pelo usuário.
- Uma parte significativa das conversas do copiloto no Copilot Studio é o reconhecimento de linguagem natural, que é a capacidade da IA de compreender a intenção do usuário.
- **Uma entidade** pode ser considerada uma unidade de informação que representa um certo **tipo de assunto**.
- **Tipos de entidades:**
    - Entidades predefinidas:
        - Idade
        - Verdadeiro e Falso
        - Cidade
        - Cor
        - etc...
    - Entidades personalizadas:
        - Closed list (Lista fechada)
        - Regular expression (Regex)
- **Resumo:** As entidades podem facilitar as **entradas do usuário** sem a necessidade de usar a parte de Resposta Generativa ou AI Builder dentro do Copilot Studio para **reconhecer informações já mapeadas**.

## Melhores práticas de uma entidade
- Definir um nome claro
- Descrever a sua entidade para outros darem a manutenção no futuro
- Definir sinônimos para garantir o mapeamento
- Usar Regex sempre que possível para identificar padrões

## Preenchimento de slot
- O preenchimento de slot é um **conceito de reconhecimento de linguagem natural** que significa salvar uma entidade extraída para um objeto.
- No entanto, no Copilot Studio, o preenchimento do slot significa colocar o **valor da entidade** extraída em uma **variável**.

## Variáveis
- Elementos usados para armazenar e reutilizar informações obtidas durante a conversa.
- As variáveis servem para **salvar respostas** do usuário e **reutilizar seu conteúdo** posteriormente na conversa.
- Também pode usar variáveis para **criar expressões lógicas** que direcionam dinamicamente o usuário por diferentes caminhos de conversa.
- **Tipos de variáveis:**
    - Tópico: conversas das quais não se tem uma necessidade alta de salvamento de dados relacionados, salvamento relacionado a um tópico em específico.
    - Variáveis globais: salvamento de dados durante uma sessão
    - Variáveis de sistema:  salvamento de dados criados e controlados pela Microsoft
    - Variáveis de ambiente: reutilização de variaveis por meio de mudança de ambientes
- **Tipos de base de variáveis:**
    - Cadeia de caracteres
    - Booleano
    - Número
    - Tabela
    - Registro
    - DateTime
    - Opção
    - Em branco

## Fórmulas
-**Exemplos de casos reais:**
    - Comparar duas datas para férias
    - Customizar o nome do usuário
    - Verificar se uma data está dentro do período
    - Calcular preço com imposto
    - Verificar se tem um produto no estoque
    - Calcular a média de preço

- Para se encontrar uma variável para utilizar na fórmula se utiliza:
    - Topic. - se for uma variável de tópico
    - Global. - se for uma variável global
    - Env. - se for uma variável de sistema

## Knowledge Sources
- São os dados e documentos que o agente usa para responder às perguntas dos usuários, permitindo que ele acesse e utilize informações de forma inteligente.

## Observações:
- 1.11.24.1 - fase_projeto.mês_desenvolvimento.ano.versão_trabalhada
- Para a criação de agentes é melhor de ser feito o prompt em inglês
- Ramificação ocorre dentro do mesmo tópico, enquanto a transição conecta tópicos diferentes.
- **Fallback:** Esse tópico do sistema é disparado quando o enunciado do usuário não corresponde aos tópicos existentes.
- **Smart matching/ Correspondência inteligente:** o agente pode corrigir automaticamente os erros ortográficos e expandir sua lógica de correspondência semanticamente.