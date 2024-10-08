![image](https://github.com/user-attachments/assets/96b697a4-0de7-47bd-8afa-d695761b5694)<h1 align="center">
  <img src="assets/reprograma-fundos-claros.png" alt="logo reprograma" width="500">
</h1>

# Estatística com python - probabilidade e amostragem

Turma Online On34 | Python | Semana 09 | 2024 | <a href="https://www.linkedin.com/in/roberta-cristina-ruedas-martins-96369696/" target="_blank" rel="noopener noreferrer">Professora Roberta Martins</a>

### Instruções
Antes de começar, vamos organizar nosso setup.
* Fork esse repositório 
* Clone o fork na sua máquina (Para isso basta abrir o seu terminal e digitar `git clone url-do-seu-repositorio-forkado`)
* Entre na pasta do seu repositório (Para isso basta abrir o seu terminal e digitar `cd nome-do-seu-repositorio-forkado`)
* [Add outras intrucoes caso necessario]

### Resumo
O que veremos na aula de hoje?
* [1 Introdução à Estatística](#tema1)
* [2 Probabilidade](#tema2)
* [3 Amostragem](#tema3)

## Conteúdo
### 1 Introdução à Estatística
1. [Definição e Objetivos da Estatística](#topico1)
2. [Classificação de Dados e Variáveis](#topico2)
3. [Medidas Descritivas: Média, Mediana, Moda, Variância e Desvio Padrão](#topico3)
### 2 Probabilidade
1. [Conceitos Fundamentais de Probabilidade](#topico4)
2. [Regras de Probabilidade](#topico5)
### 3 Amostragem

### 1 Introdução à Estatística

A Estatística é uma disciplina essencial para analisar e interpretar dados, fornecendo as ferramentas necessárias para tomar decisões informadas em diversas áreas.

#### 1.1 Definição e Objetivos da Estatística

Estatística é uma disciplina da matemática que lida com a coleta, organização, análise, interpretação e apresentação de dados. Ela é fundamental para a compreensão e descrição de padrões, tendências e características relevantes para a tomada de decisões.

A importância da estatística é evidente em diversas áreas:
- Tomada de Decisão: A estatística fornece métodos para analisar dados e tirar conclusões objetivas, ajudando na tomada de decisões informadas em negócios, governo, saúde, entre outros.
- Pesquisa Científica: Na ciência, a estatística é essencial para planejar experimentos, analisar resultados e validar hipóteses de forma rigorosa.
- Economia e Finanças: Em economia, estatísticas são usadas para medir indicadores como inflação, desemprego e produção econômica, enquanto em finanças ajudam a modelar riscos e prever tendências de mercado.
- Medicina e Saúde: Na área da saúde, a estatística é vital para entender a eficácia de tratamentos, estudar padrões epidemiológicos e planejar intervenções de saúde pública.
- Engenharia e Tecnologia: Em engenharia, a estatística auxilia no controle de qualidade e na melhoria de processos, enquanto na tecnologia é fundamental para análise de dados em áreas como inteligência artificial e aprendizado de máquina.
- Ciências Sociais: Em disciplinas como sociologia e psicologia, a estatística é utilizada para estudar comportamentos, atitudes e padrões sociais.

Vantagens de Estudar Estatística:
- Aprimora o pensamento crítico, auxilia na compreensão da incerteza, favorece decisões racionais e amplia oportunidades profissionais.

Desvantagens de Estudar Estatística:
- Complexidade, necessidade de softwares/ferramentas, a importância da interpretação correta e suas limitações.

Em resumo, a estatística permite transformar dados brutos em informações úteis e compreensíveis, fornecendo uma base sólida para a compreensão do mundo ao nosso redor e para a formulação de políticas, estratégias e descobertas científicas.

Exemplo: 
Imagine uma empresa que deseja entender o desempenho de vendas ao longo dos meses. A estatística permite analisar esses dados para identificar padrões sazonais, picos de vendas e áreas de melhoria.

#### 1.2 Classificação de Dados e Variáveis

Os dados podem ser classificados de diversas maneiras, sendo essencial compreender essa classificação para realizar análises estatísticas apropriadas. 
Existem variáveis qualitativas (categóricas) e quantitativas (numéricas).

As VARIÁVEIS QUALITATIVAS descrevem características que não podem ser medidas numericamente de forma direta. 
Elas são divididas em dois tipos:
- Variáveis Nominais
- Variáveis Ordinais

1. Variáveis Nominais: São variáveis que representam categorias sem uma ordem específica. 
Exemplos:
- Cor dos olhos: Azul, verde, castanho, preto.
- Tipo de carro: SUV, Sedan, Hatch, Pick-up.
- Estado civil: Solteira, casada, divorciada, viúva.
- Profissão: Médica, professora, advogada, engenheira, bióloga, arquiteta.

2. Variáveis Ordinais: São variáveis que possuem uma ordem ou hierarquia natural entre as categorias. 
Exemplos:
- Nível de Educação: Ensino Fundamental, Ensino Médio, Graduação, Pós-graduação e assim por diante.
- Nível Socioeconômico: Baixo, Médio e Alto.
- Classificação de Dor: Sem dor, Dor leve, Dor moderada, Dor intensa.
- Classificação de Satisfação: Muito insatisfeito, Insatisfeito, Neutro, Satisfeito, Muito satisfeito.
- Classificação de Desempenho: Abaixo das expectativas, Atende às expectativas, Excede as expectativas.

As VARIÁVEIS QUANTITATIVAS representam quantidades numéricas que podem ser medidas ou contadas. 
Elas são divididas em dois tipos:
- Variáveis Contínuas
- Variáveis Discretas

1. Variáveis Contínuas: São variáveis que podem assumir qualquer valor dentro de um intervalo (ou seja, podem ser medidas dentro de um intervalo contínuo). 
Exemplos:
- Altura: A altura de uma pessoa pode ser medida com precisão variável (por exemplo, 165,2 cm, 170,5 cm, etc.). É uma variável contínua porque pode assumir um número infinito de valores dentro de um intervalo.
- Temperatura: A temperatura em graus Celsius ou Fahrenheit pode ser medida com qualquer grau de precisão (por exemplo, 25,3°C, 30,1°C, etc.). É uma variável contínua porque pode assumir valores em uma escala contínua
- Peso: O peso de uma pessoa pode ser medido com qualquer precisão (por exemplo, 65,4 kg, 70,2 kg, etc.). É uma variável contínua porque pode assumir valores em uma escala contínua.
- Tempo: O tempo decorrido em horas, minutos e segundos. É uma variável contínua, pois pode ser medido com qualquer grau de precisão.

2. Variáveis Discretas: São variáveis que assumem valores específicos e geralmente são contáveis (ou seja, podem ser contadas, números inteiros).
Exemplos:
- Número de Filhos: O número de filhos em uma família é uma variável discreta porque só pode assumir valores inteiros (por exemplo, 0, 1, 2, 3, etc.).
- Número de Carros em um Estacionamento: O número de carros em um estacionamento em um determinado momento é uma variável discreta, pois só pode assumir valores inteiros, (por exemplo: 10, 50,170, etc.).
- Pontuação em um Teste: A pontuação obtida por um aluno em um teste (por exemplo, 7, 8, 9, 10), geralmente expressa em números inteiros, é uma variável discreta.
- Quantidade de Produtos Vendidos: O número de produtos vendidos em uma loja em um determinado dia é uma variável discreta (por exemplo: 200, 1000, 5000, etc.), pois só pode assumir valores inteiros.
- Número de Pacientes em um Hospital: O número de pacientes internados em um hospital em um determinado momento é uma variável discreta (por exemplo: 1000, 200, 369, etc.), pois só pode ser um número inteiro.

#### 1.3 Medidas Descritivas: Média, Mediana, Moda, Variância e Desvio Padrão

Medidas descritivas em estatística são técnicas utilizadas para resumir e descrever as características principais de um conjunto de dados. Elas ajudam a compreender melhor a distribuição, a centralidade e a variabilidade dos dados. 
As medidas descritivas mais comuns incluem:
1. Medidas de Tendência Central
2. Medidas de Dispersão

1. Medidas de Tendência Central
As medidas de tendência central são estatísticas que resumem um conjunto de dados em um único valor que representa o centro ou a posição central dos dados. Elas são úteis para descrever a localização típica dos dados e são amplamente utilizadas na análise estatística. 
- Média
- Mediana
- Moda

2. Medidas de Dispersão
As medidas de dispersão são estatísticas que indicam o quanto os dados estão espalhados ou dispersos em torno da medida de tendência central. Elas fornecem insights sobre a variabilidade dos dados, o que é crucial para entender a consistência ou a dispersão dos valores dentro de um conjunto de dados. 
As principais medidas de dispersão incluem:
- Variância
- Desvio Padrão

#### Medidas de Tendência Central - Média
A média é a medida de tendência central mais comum.
É calculada somando todos os valores dos dados e dividindo pelo número total de valores.

Fórmula para Calcular:
Média = Soma dos valores / Número de valores

Exemplo:
Se as idades de cinco amigos são 20, 25, 30, 35 e 40, a média das idades é?
Média = (20 + 25 + 30 + 35 + 40) / 5 = 30 anos.
Então em média, os amigos têm 30 anos.







#### Topico2
  - Lorem ipsum dolor sit amet, consectetur adipiscing elit.
  - Donec erat mauris, laoreet in tortor vel
  - Nunc ante massa, dictum eget justo eget, feugiat tincidunt.

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam leo nibh, tempus sed rhoncus et, ultrices vitae orci. Donec erat mauris, laoreet in tortor vel, eleifend suscipit nibh. Mauris pharetra dui quis turpis rutrum blandit.

### Tema2
#### Topico3
* [Subtópico 1](#subtopico1)
* [Subtópico 2](#Subtopico2)
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam leo nibh, tempus sed rhoncus et, ultrices vitae orci. Donec erat mauris, laoreet in tortor vel.

##### Subtopico1
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam leo nibh, tempus sed rhoncus et, ultrices vitae orci. Donec erat mauris, laoreet in tortor vel.

##### Subtopico2
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam leo nibh, tempus sed rhoncus et, ultrices vitae orci. Donec erat mauris, laoreet in tortor vel.

### Tema3
#### Topico4
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam leo nibh, tempus sed rhoncus et, ultrices vitae orci. Donec erat mauris, laoreet in tortor vel, eleifend suscipit nibh. Mauris pharetra dui quis turpis rutrum blandit. Nunc tempor libero tortor, ac commodo erat porttitor ut. Donec vitae orci arcu. Nunc felis mi, maximus a turpis a, mollis pulvinar enim. Vivamus aliquam ante dui, a blandit massa rutrum et. Etiam hendrerit gravida ultrices.

***
### Exercícios 
* [Exercicio para sala](https://github.com/mflilian/repo-example/tree/main/exercicios/para-sala)
* [Exercicio para casa](https://github.com/mflilian/repo-example/tree/main/exercicios/para-casa)

### Material da aula 

### Links Úteis
- [Lorem Ipsum](https://www.lipsum.com/feed/html)
- [Lorem Ipsum](https://www.lipsum.com/feed/html)
- [Lorem Ipsum](https://www.lipsum.com/feed/html)
- [Lorem Ipsum](https://www.lipsum.com/feed/html)


<p align="center">
Desenvolvido com :purple_heart:  
</p>

