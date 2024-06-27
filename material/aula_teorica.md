# Semana 14: Análise de Dados do Mundo Real 

### Objetivo
- Introduzir as alunas aos conceitos de análise de dados com o uso da linguagem Python, explorando todas as etapas desse processo: coleta, limpeza, análise e visualização de dados. 


### Agenda Parte I (Manhã)
- 09:00 - Boas Vindas: Objetivo da semana + Apresentação Professora - 15’
- 09:15 - Apresentação dos conteúdos: Contextualização - 30’
- 09:45 - Apresentação dos conteúdos: Introdução a análise de dados - 40’
- 10:20 - Dinâmica: Explorando os dados da Netflix - 20’
- 10:40 - Apresentação dos conteúdos: coleta e limpeza com os dados da Netflix - 30’
- 11:10 - Intervalo - 15’
- 11:25 - Apresentação dos conteúdos: Analisando os dados da Netflix - 50’
- 12:05 - Apresentação dos conteúdos: Visualização dos dados - 25’
- 10:20 - Exercícios Práticos: dados da Netflix - 30’
- 13:00 - Pausa para o almoço

### Agenda Parte II (Tarde)
- 14:00 - Apresentação dos dados da Olist - 15’
- 14:15 - Prática: Coletando dados da Olist - 10’
- 14:25 - Prática: Limpando os dados da Olist - 30’
- 14:55 - Prática: Analisando os dados da Olist - 30’
- 15:25 - Dinâmica: Explorando os dados da Olist - 30’
- 15:55 - Intervalo - 15’
- 16:10 - Dinâmica: Visualizações dos dados da Olist - 40’
- 16:50 - Encerramento do dia com avisos e desafio da semana. - 10’


##  Contextualização
Nas aulas anteriores, vocês aprenderam sobre banco de dados, como funcionam, e tiveram uma breve apresentação sobre pensamento analítico e o uso da biblioteca Pandas para manipular dados. Nesta aula, iremos aprofundar nossos conhecimentos em dados. Porém, antes de tudo é importante entender um conceito importante sobre dados: o que difere um dado do banco de dados para um dado em um gráfico? O processamento dessa informação. Vamos entender melhor? 

Existem 3 conceitos que precisamos entender, o conceito de dados, informação e conhecimento.

- *Dados*: são a unidade base da informação. São registros soltos sem contexto ou análise prévia.
    - Exemplo: Ontem João tinha batatas.


- *Informação*: É a estruturação e organização dos dados. É a matéria base para o conhecimento.
    - Exemplo: Ontem João tinha batatas, hoje João tem 40 batatas.


- *Conhecimento*: É a informação processada, que nos permite tirar insights.
    - Exemplo: Como João tinha 50 batatas ontem e hoje ele tem apenas 40, em um dia ele perdeu 20% das suas batatas.


Agora que entendemos esses conceitos entre um dado e o conhecimento. Por que dados são tão importantes? E por que especialmente no século 21, dados viraram protagonistas? 

![image](noticias_dados.png)

"Os dados são o novo petróleo. É valioso, mas se não for refinado não pode realmente ser usado (...) então os dados devem ser decompostos, analisados ​​para que tenham valor." - Clive Humby (Tradução livre)

Essa frase foi criada por Clive Humby, um matemático londrino especializado em ciência de dados.Basicamente, ele defende que, assim como o petróleo precisa ser refinado, dados precisam ser analisados. A maior riqueza se encontra não nos dados em si, mas sim na capacidade de usá-los de forma analítica. A inteligência por trás deles é quem determina seu maior valor pois, a partir dela, serão extraídas as descobertas que irão influenciar na tomada de decisões, sejam elas grandes ou pequenas, das empresas. 

E com esse fenômeno, as empresas estão cada vez mais com uma cultura data-driven. Mas o que é a cultura data-driven?

Empresas data driven são aquelas que planejam, executam e gerenciam estratégias com base em **dados**, com o objetivo de se manterem relevantes no mercado utilizando a análise de dados em suas tomadas de decisão. Empresas que seguem essa cultura, quando bem aplicadas, possuem vários benefícios, como: 

- **Assertividade nas previsões**: Empresas de sucesso não vivem apenas o momento presente. Elas pautam suas decisões em previsões de mercado e se preparam para possíveis mudanças. Nesse momento, nada melhor do que contar com dados e informações seguras e confiáveis. A cultura data driven promove maior assertividade para o futuro das empresas por permitir que elas se preparem para os anos seguintes com base em noções sólidas do que está por vir em suas áreas.

- **Decisões mais ágeis**: A velocidade de tomada de decisões em uma empresa também diz muito sobre sua resiliência em meio às dificuldades do mercado. Com o auxílio de dados consistentes e business intelligence, as resoluções de problemas e a montagem de novas estratégias se tornam mais ágeis e pontuais.

- **Serviços e produtos superiores**: É inegável que produtos e serviços direcionados, por exemplo, para personas com características embasadas em dados advindos de pesquisas de mercado e online são muito mais propensos a gerar bons resultados e autoridade do que os divulgados arbitrariamente.

E no Brasil, quais empresas possuem essa cultura data-driven? 
- Itaú
- Nubank
- iFood
- PicPay
- Stone

## Introdução à Análise de Dados

A análise de dados é o processo de buscar informações relevantes a partir de dados quantitativos e qualitativos de um determinado tema. Através da análise de dados, é possível confirmar e refutar hipóteses, identificar soluções para um problema e ser mais assertivo na tomada de decisões. 

### Quais os tipos de análise de dados?
#### Análise preditiva
Neste tipo de análise, os dados são utilizados para fazer projeções e identificar tendências futuras a partir de determinados padrões previamente definidos.


#### Análise prescritiva
A análise prescritiva busca avaliar as consequências que certas decisões podem trazer, esse tipo de análise é geralmente utilizado para definir qual o melhor caminho para alcançar um objetivo definido. 

Se a análise preditiva atua na previsão de comportamentos futuros, a análise prescritiva auxilia nas tomadas de decisão com o objetivo de melhorar o alcance de resultados e reduzir cenários negativos.

#### Análise descritiva
A análise descritiva é feita em cima de dados reais e passados, é descrever certos eventos que já ocorreram. Esse tipo de análise é normalmente é utilizada como um passo anterior às análises mais robustas, a etapa de descrição é o pontapé inicial para um estudo mais aprofundado. 


#### Análise diagnóstica
Esse tipo de análise busca investigar as causas e efeitos dos eventos e objetos analisados. 

Então, em resumo:
![img](tipos-de-analise.png)


E quais são as etapas da análise de dados? 

1. Definição do problema;
2. Coleta dos dados;
3. Limpeza dos dados;
4. Análise dos dados;
5. Interpretação e visualização dos dados.

Etapa 1 – Definição do problema
Nesse primeiro momento, você precisa definir qual será o problema que você irá resolver. Estabeleça quais perguntas deverão ser respondidas.

Para que tenham o efeito desejado, os objetivos devem ser claros e mensuráveis, assim, as decisões serão tomadas com maior embasamento, você evitará desperdícios e as ações serão mais eficazes.


Etapa 2 – Coleta dos dados 
Entenda de onde você precisará buscar informação para responder suas perguntas. Alguns lugares para buscar esses dados:
- Web scraping para coletar dados online;
- APIs;
- Dados públicos;
- Kaggle;

Etapa 3 - Limpeza dos dados
A limpeza de dados é um processo de eliminar inconsistências, ou seja, registros de baixa integridade, informações duplicadas, informações nulas, erradas ou de baixa relevância. 

Etapa 4 - Análise dos dados
Nessa etapa, com as tabelas prontas, começamos a manipular os dados, agrupando, ordenando, buscando por padrões e o mais importante, buscando responder as perguntas que nós fizemos no início.

Etapa 5 - Interpretação e visualização dos dados.
Nessa etapa, os questionamentos iniciais devem ser respondidos e as conclusões precisam ser tomadas. Para melhorar a forma de comunicar os resultados, desenvolvemos gráficos, tabelas agregadas que possam melhorar o entendimento dos resultados obtidos. 

Para explorarmos todas as etapas da análise de dados, iremos trabalhar em cima de uma base de dados que vocês tiveram a oportunidade de mexer anteriormente, a base de dados do Titanic. Nesta primeira parte da aula, realizar a análise completa dos dados do Titanic.

## Dinâmica: Explorando os dados da Netflix
Em grupo, vocês irão abrir os dados da Netflix e definir um problema para responder com os dados. Entenda o tipo de dado que estamos trabalhando, qual o tipo de dados de cada coluna (inteiros, decimais, booleanos, strings), temos dados nulos? Quais colunas precisaremos manipular? 

## Etapas: Coleta, Limpeza e Análise dos Dados

A partir daqui, iremos continuar no arquivo `s14_parte1.ipynb`

Para a segunda parte da aula (período da tarde), continuar no arquivo `s14_parte2.ipynb`


**Nota para a professora**: Todas as bases utilizadas e criadas em aula estão disponibilizadas nesse Drive: https://drive.google.com/drive/folders/1RuibSOdMp-cR6niAdbH8bRIj3PO4EOlh?usp=sharing

As bases são enormes e não consigo subir pelo Git :/ 
