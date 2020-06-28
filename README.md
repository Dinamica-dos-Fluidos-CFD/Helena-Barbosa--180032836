# Helena-Barbosa--180032836

**Nota escolhida para substituição:** Nota do Laboratório 

**Problema escolhido:** Problema 1 

Problema 1: Uma instalação de bombeamento tem apresentado problemas em uma seção de tubulação de 1 metro de comprimento e 40 mm de diâmetro. A perda de carga foi medida usando sensores de pressão, e mensurou-se uma queda de pressão de 2 Pa. A bomba que supre esta tubulação com água está operando em potência máxima. Também mediu-se a vazão deste escoamento, obtendo um valor de 0,0001 metro cúbico por segundo na saída do tubo. O projeto de CFD deve:

- Determinar se estes valores de vazão e perda de carga estão coerentes ou não, e o motivo para isto.
- Apresentar possibilidades de problemas em caso dos valores colocados acima não estarem coerentes.
- Usando a simulação apresentada, realizar um estudo paramétrico do fator de atrito para avaliar se o cenário acima é normal ou não para esta instalação.

# 1. Modelagem: 

A primeira etapa deverá conter as respostas para as seguintes perguntas:

## Qual é o objetivo do projeto?
    
### Objetivo geral:

 O projeto consiste em analisar a instalação de bombeamento apontada no Problema 1 a qual apresenta problemas em uma determinada seção da tubulação. O objetivo geral deste projeto é obter uma simulação do tubo em questão através da Dinâmica dos Fluidos Computacional do problema, utilizando o Software Ansys Student. Como uma boa prática para Projetos em CFD para a etapa de modelagem do problema, é importante apresentar e listar objetivos específicos para melhor entendimento das necessidades do projeto e decisões tomadas posteriormente. 
    
### Os objetivos específicos:
        
   * Comparar os resultados de vazão e perda de carga obtidos na simulação com os resultados teóricos, para avaliar se são consistentes com a realidade.
   * Apresentar possibilidades de problemas caso os valores obtidos não sejam coerentes.
   * Analisar o parâmetro fator de atrito através de um estudo paramêtrico para definir a normalidade do cenário da instalação apresentada.

## Quais são seus requisitos de solução?

 O requisito de solução do Projeto de CFD é o fator de atrito ou o seu cálculo por meio dos parâmetros determinados pela simulação, tais como a velocidade do escoamento, o diâmetro do tubo na seção mencionada, a viscosidade do fluido e a sua massa específica.    
    
## Qual é a finalidade do projeto?

 O projeto tem finalidade acadêmica para demonstração e visualização do escoamento citado e do parâmetro escolhido, no caso deste projeto é o fator de atrito. Através da simulação computacional e de cálculos feitos previamente utilizando a teoria de Dinâmica dos Fluidos será possível caracterizar o escoamento e confirmar os resultados obtidos por ambas as formas.
    
## Que hipóteses de simplificação podem ser adotadas?

  1) O escoamento será considerado laminar devido às características do fluido e do tubo e para a facilitação dos cálculos do             problema.
  2) A geometria do tubo é considerada simples, possibilitando a criação de uma malha boa e fiel para análise e simulação porém não       complexa demais para a demanda do problema.
  3) O problema considera regime permanente.
  4) Trocas de calor não serão consideradas.
  5) Filtrar os parâmetros que necessitam de simulação para averiguar o problema e efetuar os cálculos, para assim não haver simulações desnecessárias.
    
## Que hipóteses de simplificação devem ser adotadas?

  1) O escoamento será considerado laminar devido às características do fluido e do tubo.
  2) A geometria do tubo é considerada simples, possibilitando a criação de uma malha boa e fiel para análise e simulação porém não       complexa demais para a demanda do problema.
  3) O problema considera regime permanente.
  4) Trocas de calor não serão consideradas.
    
## Qual é a precisão requerida nos resultados do projeto?

 Devido ao projeto possuir um formato não muito complexo e ser caracterizado como um projeto acadêmico para simulação e comparação de dados, a precisão necessária será definida através dos cálculos e será o suficiente para a avaliação do problema.
    
## Qual é o prazo de entrega do projeto?

  O projeto será dividido em 3 etapas: 
    
   1- Modelagem: 1 semana;
    
   2- Pré- processamento: 1 semana;
    
   3- Processamento e pós-processamento: 1 semana;
    
  A etapa de Modelagem, assim como as demais etapas tem o prazo de aproximandamente uma semana até o recebimento do Feedback e a partir da efetuação das correções necessárias as etapas seguintes apresentarão novos prazos de acordo com a necessidade.
    
## Há outra metodologia mais adequada do que CFD?
    
 O projeto consiste em uma análise e comparação das simulações feitas em CFD e os cálculos. Perante a isso, para um resultado sólido os cálculos de perda de carga, número de Reynolds e sua relação com o fator de atrito já são suficientes, porém por conta da natureza do projeto a simulação é importante para esta comparação, mas não necessariamente a mais adequada para apresentar os resultados pedidos.

## O projeto deverá conter nesta etapa:

- Desenhos CAD mostrando a geometria do problema.
- Desenho esquemático da modelagem do problema.

A seguir, a imagem do Sketch com cotagem do diâmetro do tubo:

![Design_Modeler_Cotagem_Diâmetro](https://user-images.githubusercontent.com/62161754/85886441-81583e00-b7bc-11ea-87c2-479a7a8b610a.png)



Extrude do Sketch --> geometria final do tubo:

![Design_Modeler_Extrude](https://user-images.githubusercontent.com/62161754/85886469-8f0dc380-b7bc-11ea-9fdb-ef9cef544848.png)



Desenho esquemático da modelagem do problema, elaborado no AutoCAD:

![Esquemático do problema Autocad 2D](https://user-images.githubusercontent.com/62161754/83933377-3f6c4700-a77e-11ea-9e10-a04fa9279dfd.PNG)


# 2. Pré-Processamento:

 A segunda etapa deverá conter as respostas para as seguintes perguntas:

## Quanto detalhado o domínio de cálculo precisa ser?

 O domínio de cálculo não necessita de um detalhamento elevado devido à baixa complexidade do problem. A geometria da tubulação será feita de maneira simplificada utilizando apenas o diâmetro da tubulação e seu comprimento. Conforme apresentado anteriormente a intenção é reproduzir uma simulação na qual os resultados possam ser observados e comparados com os cálculos teóricos. O objetivo é avaliar a normalidade da situação. Neste sentido, é importante encontrar o equilíbrio entre a demanda de tempo para os cálculos teóricos e o detalhamento da simulação do problema.

## A geometria está adequada?

 A tubulação em questão apresenta uma secção transversal circular com diâmetro de 40 mm e comprimento de 1000 mm, não possuindo elementos que necessitam de uma maior simplificação, logo a geometria produzida apresenta-se adequada para o problema.
    
## Que tipo de malha e método usar? Estruturada ou não-estruturada? Volumes Finitos ou Elementos Finitos?

 A escolha realizada para a simulação foi a malha automática gerada pelo próprio Ansys Student. A malha resultada é estruturada, ou seja, apresenta um menor número de elementos, o que permite um menor tempo de simulação. Além disso a malha obtida permite que seus elementos possam alinhar-se com a direção dos gradientes do escoamento, ou seja, é possível obter uma melhor precisão nos resultados.
 
 O método utilizado será MVF (Método dos Volumes Finitos) por ser mais adequado para a Mecânica dos Fluidos. O método no software se baseia em, de forma geral, decompor o domínio em volumes de controle na malha computacional, utilizar as equações integrais de conservação para cada volume de controle, aproximar em valores numéricos as integrais, aproximar os valores das variáveis nas faces e as derivadas com a informação das variáveis nodais e por último montar e solucionar o sistema algébrico obtido.
    
## Geração da malha e sua qualidade:

 A malha foi gerada automaticamente através do botão "generate":
    
   ![meshing_cursor_generate](https://user-images.githubusercontent.com/62161754/85912059-d23d5600-b7ff-11ea-811f-ecf64b90e647.png)
    
  Dessa forma o programa analisa a geometria apresentada e escolhe o método mais adequado para a geração da malha, o resultado é mostrado na imagem a seguir:
    
   ![meshing_view](https://user-images.githubusercontent.com/62161754/85896545-06e4e980-b7cf-11ea-8f64-a887b5f66310.png)
    
 Como é possivel notar, a malha possui um alinhamento com o comprimento do tubo e com os gradientes de escoamento. No entanto faz-se necessária a análise da qualidade da malha. Os principais fatores são a Dissimetria (Skewness) e a Qualidade Ortogonal (Orthogonal Quality). Estes valores são muito importantes para a garantia de resultados confiáveis e mais precisos, os parâmetros para classificação da qualidade da malha através destes valores são:
    
  Qualidade da malha de acordo com os valores de Dissimetria:
    
   * Excelente: 0 - 0,25;
   * Muito Bom: 0,25 - 0,50;
   * Bom: 0,50 - 0,80;
   * Aceitável: 0,80 - 0,94;
   * Ruim: 0,95 - 0,97;
   * Inaceitável: 0,98 - 1;
    
   Qualidade da malha de acordo com os valores de Qualidade Ortogonal:
    
   * Excelente: 0,95 - 1;
   * Muito Bom: 0,70 - 0,95;
   * Bom: 0,20 - 0,69;
   * Aceitável: 0,15 - 0,20;
   * Ruim: 0,001 - 0,14;
   * Inaceitável: 0 - 0,001;
    
 Abaixo encontram-se as tabelas com os valores obtidos da malha gerada referentes a esses parâmetros:
    
   ![meshing_quality_skewness](https://user-images.githubusercontent.com/62161754/85899056-da7f9c00-b7d3-11ea-8a41-ca39015e304c.png)
    
    
   ![meshing_quality_orthogonal](https://user-images.githubusercontent.com/62161754/85899079-e4090400-b7d3-11ea-9d5b-06b30a18b8f9.png)

    
 A partir desses valores a malha gerada foi classificada de maneira positiva. Como pode ser visto o valor máximo de Dissimetria se encontra em 0,47313 e o valor mínimo da Qualidade Ortogonal em 0,82069, classificando ambos na margem do Muito Bom nas escalas de qualidade.
    
    
## Quais são as informações de entrada (Input) do problema?

 As informações de entrada do problema são a pressão relativa na saída, que será considerada zero, e a velocidade de entrada do problema, a qual foi calculada utilizando o valor da vazão volumétrica fornecido e a Equação da Continuidade, como demonstrado a seguir:
    
  O somatório das vazões mássicas de entrada são iguais ao somatório das vazões mássicas de saída, consequentemente, o mesmo vale para a vazão volumétrica.
    
   ![CodeCogsEqn_eq_continuidade](https://user-images.githubusercontent.com/62161754/85890783-6e496c00-b7c4-11ea-854b-e90ff9427b99.gif)
    

   ![CodeCogsEqn_vazões](https://user-images.githubusercontent.com/62161754/85890830-802b0f00-b7c4-11ea-9b0c-f587844c9333.gif)
    
 A partir disso, para obter o valor da velocidade de entrada do problema é necessário usar a equação a seguir, na qual a vazão volumétrica é resultada da multiplicação entre a velocidade média e a área da secção transversal do tubo. Como a aréa é constante ao longo do tubo, a velocidade média também será a mesma na entrada e na saída.
    
   ![CodeCogsEqn_vazão_volum](https://user-images.githubusercontent.com/62161754/85891295-32fb6d00-b7c5-11ea-9acb-d221bcd8ca1e.gif)
    

   ![CodeCogsEqn_expressao_velocidade](https://user-images.githubusercontent.com/62161754/85892640-ad2cf100-b7c7-11ea-8cc9-55a175b8829a.gif)
    
    
   ![CodeCogsEqn_velocidade](https://user-images.githubusercontent.com/62161754/85891418-6ccc7380-b7c5-11ea-8b1f-782c08bc05e8.gif)
    
    
## Que escolhas devem ser feitas em relação ao processamento da solução?

 Após a escolha da malha, foi feito o estabelecimento das regiões que receberão as condições de contorno, ou seja, onde será a entrada e a saída do escoamento. Primeiramente foi necessário escolher as faces do sólido, utilizando o recurso a seguir:
    
   ![meshing_select_face](https://user-images.githubusercontent.com/62161754/85899984-5c23f980-b7d5-11ea-859c-b89ee906fc9c.png)
    
Depois de selecionar a face escolhida para a entrada do escoamento, utilizou-se o botão direito do mouse para criar uma "Named Selection" na face selecionada para entrada:
    
  ![meshing_botao_direito_face](https://user-images.githubusercontent.com/62161754/85900158-b58c2880-b7d5-11ea-90c4-a720b67d1cf3.png)
    
  ![meshing_entrada](https://user-images.githubusercontent.com/62161754/85900324-0439c280-b7d6-11ea-9a40-8f5f473a6dc8.png)

O mesmo processo foi feito para a saída do escoamento. Resultando na seguinte Árvore de projeto:
    
   ![meshing_arvore](https://user-images.githubusercontent.com/62161754/85900463-419e5000-b7d6-11ea-8ede-9f8b963594e2.png)
    
 Após as faces serem escolhidas e nomeadas, a próxima etapa consiste em estabelecer o Dominio Padrão do escoamento, no qual as escolhas consistiram na definição do material como água, a pressão de referência como 1 atm, a desconsideração de trocas de calor e a caracterização do escoamento como laminar.
    
   ![CFX-Pre_water_and_reference_pressure](https://user-images.githubusercontent.com/62161754/85911299-da46c700-b7fa-11ea-8fc2-0581659433e5.png)
    
   ![CFX-Pre_Domain_heat_transfer](https://user-images.githubusercontent.com/62161754/85911301-dca92100-b7fa-11ea-8732-c5249705757f.png)
    
  Consequentemente foram definidos os detalhes das condições de contorno na entrada e na saída do tubo, primeiro foram atribuídos o parâmetro de velocidade para a entrada do escoamento e a pressão estática relativa na saída.
    
   ![CFX-Pre_Boundary_entrada](https://user-images.githubusercontent.com/62161754/85911165-cfd7fd80-b7f9-11ea-88bc-f53fb38c7161.png)
    
   ![CFX-Pre_Boundary_entrada_Details_Speed](https://user-images.githubusercontent.com/62161754/85911168-d49cb180-b7f9-11ea-921e-1b49c128702d.png)
       
   ![CFX-Pre_Boundary_Saida](https://user-images.githubusercontent.com/62161754/85911346-1712be00-b7fb-11ea-8ed8-2d4d4e7190f5.png)
    
   ![CFX-Pre_Boundary_Saida_details_pressure](https://user-images.githubusercontent.com/62161754/85911349-19751800-b7fb-11ea-8c16-accfda5e3ea6.png)
    
 Após a conclusão dessas definições o próximo passo foi definir os controles de solução, os quais permaneceram no padrão fornecido pelo programa, finalizando a parte do pré-processamento das condições de contorno.
    
   ![CFX-PRE_Solver_Control_Default](https://user-images.githubusercontent.com/62161754/85911469-d2d3ed80-b7fb-11ea-8211-87c2ae69ae87.png)
    
   ![CFX-PRE_Solver_Control_Default - Copia](https://user-images.githubusercontent.com/62161754/85911473-d5cede00-b7fb-11ea-8564-acd189ac0581.png)

    
## Quais são os prazos e disponibilidade de capacidade computacional para a análise em questão? 
    
 O prazo para realização da etapa de pré-processamento é de aproximadamente uma semana, sendo suficiente devido à complexidade da simulação.
    
 A capacidade computacional disponível para a análise segue abaixo:
    
   * Processador: Intel(R) Core(TM) i7-7500 
   * Memória RAM: 8 GB DDR4 2133 MHz
   * Sistema Operacional: Windows 10 
    

## O projeto deverá conter nesta etapa:

- Descrição do pré-processamento feito no ANSYS.
- Imagens da malha de cálculo do problema.


# 3. Processamento e Pós-Processamento:

A terceira etapa deverá conter as respostas para as seguintes perguntas:

## O histórico de convergência do cálculo está adequado?
## Quanto tempo a simulação está levando para ser processada?
## Os resíduos estão em valores aceitáveis?
## A simulação fornece resultados qualitativos?
## É possível calcular resultados quantitativos e qualitativos com o que a simulação calculou?
## Os resultados estão de acordo com a realidade física do escoamento?

## O projeto deverá conter nesta etapa:

- Análise dos resultados obtidos.
- Comparação dos resultados numéricos com os resultados analíticos de cada problema.
- Imagens de visualização do escoamento.
- Análise dos resultados obtidos pelo estudo paramétrico.



