# Helena-Barbosa--180032836

**Nota escolhida para substituição:** Nota do Laboratório 

**Problema escolhido:** Problema 1 

Problema 1: Uma instalação de bombeamento tem apresentado problemas em uma seção de tubulação de 1 metro de comprimento e 40 mm de diâmetro. A perda de carga foi medida usando sensores de pressão, e mensurou-se uma queda de pressão de 2 Pa. A bomba que supre esta tubulação com água está operando em potência máxima. Também mediu-se a vazão deste escoamento, obtendo um valor de 0,0001 metro cúbico por segundo na saída do tubo. O projeto de CFD deve:

- Determinar se estes valores de vazão e perda de carga estão coerentes ou não, e o motivo para isto.
- Apresentar possibilidades de problemas em caso dos valores colocados acima não estarem coerentes.
- Usando a simulação apresentada, realizar um estudo paramétrico do fator de atrito para avaliar se o cenário acima é normal ou não para esta instalação.

### 1. Modelagem: 

A primeira etapa deverá conter as respostas para as seguintes perguntas:

- Qual é o objetivo do projeto?
    
    O projeto consiste em analisar a instalação de bombeamento apontada no Problema 1 a qual apresenta problemas em uma determinada seção da tubulação. O objetivo geral deste projeto é obter uma simulação do tubo em questão através da Dinâmica dos Fluidos Computacional do problema, utilizando o Software Ansys Student.
    
    Os objetivos específicos são:
        
     1) Comparar os resultados de vazão e perda de carga obtidos na simulação com os resultados teóricos, para avaliar se são consistentes com a realidade.
     2) Apresentar possibilidades de problemas caso os valores obtidos não sejam coerentes.
     3) Analisar o parâmetro fator de atrito através de um estudo paramêtrico para definir a normalidade do cenário da instalação apresentada.

- Quais são seus requisitos de solução?

    O requisito de solução do Projeto de CFD é o fator de atrito ou o seu cálculo por meio dos parâmetros determinados pela simulação, tais como a velocidade do escoamento, o diâmetro do tubo na seção mencionada, a viscosidade do fluido e a sua massa específica.    
    
- Qual é a finalidade do projeto?

    O projeto tem finalidade acadêmica para demonstração e visualização do escoamento citado e do parâmetro escolhido,no caso deste projeto é o fator de atrito, através da simulação computacional e de cálculos feitos previamente utilizando a teoria de Dinâmica dos Fluidos será possível caracterizar o escoamento e confirmar os resultados obtidos por ambas as formas.
    
- Que hipóteses de simplificação podem ser adotadas?

    1) O escoamento será considerado laminar devido às características do fluido e do tubo e para a facilitação dos cálculos do             problema.
    2) A geometria do tubo é considerada simples, possibilitando a criação de uma malha boa e fiel para análise e simulação porém não       complexa demais para a demanda do problema.
    3) O problema considera regime permanente.
    4) Trocas de calor não serão consideradas.
    5) Filtrar os parâmetros que necessitam de simulação para averiguar o problema e efetuar os cálculos, para assim não haver simulações desnecessárias.
    
- Que hipóteses de simplificação devem ser adotadas?

    1) O escoamento será considerado laminar devido às características do fluido e do tubo.
    2) A geometria do tubo é considerada simples, possibilitando a criação de uma malha boa e fiel para análise e simulação porém não       complexa demais para a demanda do problema.
    3) O problema considera regime permanente.
    4) Trocas de calor não serão consideradas.
    
- Qual é a precisão requerida nos resultados do projeto?

    Devido ao projeto possuir um formato não muito complexo e ser caracterizado como um projeto acadêmico para simulação e comparação de dados, a precisão necessária será definida através dos cálculos e será o suficiente para a avaliação do problema.
    
- Qual é o prazo de entrega do projeto?

    O projeto será dividido em 3 etapas: 
    
    1- Modelagem;
    
    2- Pré- processamento;
    
    3- Processamento e pós-processamento.
    
    A etapa de Modelagem tem o prazo de aproximandamente uma semana até o recebimento do Feedback e a partir da efetuação das correções necessárias as etapas seguintes apresentarão novos prazos de acordo com a necessidade.
    
- Há outra metodologia mais adequada do que CFD?
    
    O projeto consiste em uma análise e comparação das simulações feitas em CFD e os cálculos, portanto para o resultado sólido, os cálculos utilizando equação de Bernoulli, número de Reynolds e sua relação com o fator de atrito já são suficientes, porém por conta da natureza do projeto a simulação é importante para esta comparação, mas não necessariamente a mais adequada para apresentar os resultados pedidos.

O projeto deverá conter nesta etapa:

- Desenhos CAD mostrando a geometria do problema.
- Desenho esquemático da modelagem do problema.

I) Imagem 1: Sketch com cotagem do diâmetro do tubo.

![Print CFX Design Modeler Cotagem Diâmetro](https://user-images.githubusercontent.com/62161754/83933354-1946a700-a77e-11ea-9623-c4fbcc055ad4.png)

II) Imagem 2: Extrude do Sketch --> geometria final do tubo.

![Print CFX Design Modeler Extrude](https://user-images.githubusercontent.com/62161754/83933373-31b6c180-a77e-11ea-9d74-1203cfd97dc0.png)


III) Imagem 3: Desenho esquemático da modelagem do problema, elaborado no AutoCAD.

![Esquemático do problema Autocad 2D](https://user-images.githubusercontent.com/62161754/83933377-3f6c4700-a77e-11ea-9e10-a04fa9279dfd.PNG)


### 2.	Pré-Processamento:

A segunda etapa deverá conter as respostas para as seguintes perguntas:

- Quanto detalhado o domínio de cálculo precisa ser?
- A geometria está adequada?
- Que tipo de malha e método usar? Estruturada ou não-estruturada? Volumes Finitos ou Elementos Finitos?
- Quais são as informações de entrada (Input) do problema?
- Que escolhas devem ser feitas em relação ao processamento da solução?
- Quais são os prazos e disponibilidade de capacidade computacional para a análise em questão? 

O projeto deverá conter nesta etapa:

- Descrição do pré-processamento feito no ANSYS.
- Imagens da malha de cálculo do problema.



