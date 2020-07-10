# Helena-Barbosa--180032836

**Nota escolhida para substituição:** Nota do Laboratório 

**Problema escolhido:** Problema 1 

Problema 1: Uma instalação de bombeamento tem apresentado problemas em uma seção de tubulação de 1 metro de comprimento e 40 mm de diâmetro. A perda de carga foi medida usando sensores de pressão, e mensurou-se uma queda de pressão de 2 Pa. A bomba que supre esta tubulação com água está operando em potência máxima. Também mediu-se a vazão deste escoamento, obtendo um valor de 0,0001 metro cúbico por segundo na saída do tubo. O projeto de CFD deve:

- Determinar se estes valores de vazão e perda de carga estão coerentes ou não, e o motivo para isto.
- Apresentar possibilidades de problemas em caso dos valores colocados acima não estarem coerentes.
- Usando a simulação apresentada, realizar um estudo paramétrico do fator de atrito para avaliar se o cenário acima é normal ou não para esta instalação.

# 1. Modelagem:

## Objetivos:
    
### Objetivo geral:

 O projeto consiste em analisar a instalação de bombeamento apontada no problema, a qual apresenta problemas em uma determinada seção da tubulação. O objetivo geral deste projeto é obter uma simulação do tubo em questão através da Dinâmica dos Fluidos Computacional do problema, utilizando o Software Ansys Student para auxiliar no estudo paramétrico. 
    
### Objetivos específicos:
        
   * Comparar os resultados de vazão e perda de carga obtidos na simulação com os resultados teóricos, para avaliar se são consistentes com a realidade.
   * Apresentar possibilidades de problemas caso os valores obtidos não sejam coerentes.
   * Analisar o parâmetro fator de atrito através de um estudo paramêtrico para definir a normalidade do cenário da instalação apresentada.

## Requisitos de solução:

 O requisito de solução do Projeto de CFD é o fator de atrito ou o seu cálculo por meio dos parâmetros determinados pela simulação, tais como a velocidade do escoamento, o diâmetro do tubo na seção mencionada, a viscosidade do fluido e a sua massa específica.    
    
## Finalidade do projeto:

 O projeto tem finalidade acadêmica para demonstração e visualização do escoamento citado e do parâmetro escolhido, no caso deste projeto é o fator de atrito. Através da simulação computacional e de cálculos feitos previamente utilizando a teoria de Dinâmica dos Fluidos será possível caracterizar o escoamento e confirmar os resultados obtidos por ambas as formas.
    
## Hipóteses de simplificação que podem ser adotadas:

  1) O escoamento será considerado laminar devido às características do fluido e do tubo e para a facilitação dos cálculos do             problema.
  2) A geometria do tubo é considerada simples, possibilitando a criação de uma malha boa e fiel para análise e simulação, porém, não       complexa demais para a demanda do problema.
  3) O problema considera regime permanente.
  4) Trocas de calor não serão consideradas.
  5) Filtrar os parâmetros que necessitam de simulação para averiguar o problema e efetuar os cálculos, para assim não haver simulações desnecessárias.
    
## Hipóteses de simplificação que devem ser adotadas:

  1) O escoamento será considerado laminar devido às características do fluido e do tubo.
  2) A geometria do tubo é considerada simples, possibilitando a criação de uma malha boa e fiel para análise e simulação, porém, não       complexa demais para a demanda do problema.
  3) O problema considera regime permanente.
  4) Trocas de calor não serão consideradas.
    
## Precisão requerida:

 Devido ao projeto possuir um formato não muito complexo e ser caracterizado como um projeto acadêmico para simulação e comparação de dados, a precisão necessária será definida através dos cálculos e será o suficiente para a avaliação do problema.
    
## Prazo de entrega do projeto:

  O projeto será dividido em 3 etapas: 
    
   1- Modelagem: 1 semana;
    
   2- Pré- processamento: 1 semana;
    
   3- Processamento e pós-processamento: 1 semana;
    
  A etapa de Modelagem, assim como as demais etapas, tem o prazo de aproximandamente uma semana até o recebimento do Feedback e a partir da efetuação das correções necessárias as etapas seguintes apresentarão novos prazos de acordo com a necessidade.
    
## Há outra metodologia mais adequada do que CFD?
    
 O projeto consiste em uma análise e comparação das simulações feitas em CFD e os cálculos. Perante a isso, para um resultado sólido os cálculos de perda de carga, número de Reynolds e sua relação com o fator de atrito já são suficientes, porém por conta da natureza do projeto a simulação é importante para esta comparação, mas não necessariamente a mais adequada para apresentar os resultados pedidos.

## Imagens da modelagem do projeto:

   * Cotagem do diâmetro do tubo:

![Design_Modeler_Cotagem_Diâmetro](https://user-images.githubusercontent.com/62161754/85886441-81583e00-b7bc-11ea-87c2-479a7a8b610a.png)



   * Geometria final do tubo:

![Design_Modeler_Extrude](https://user-images.githubusercontent.com/62161754/85886469-8f0dc380-b7bc-11ea-9fdb-ef9cef544848.png)



   * Desenho esquemático da modelagem do problema, elaborado no AutoCAD:

![Esquemático do problema Autocad 2D](https://user-images.githubusercontent.com/62161754/83933377-3f6c4700-a77e-11ea-9e10-a04fa9279dfd.PNG)


# 2. Pré-Processamento:


## Detalhamento no domínio de cálculo:

 O domínio de cálculo não necessita de um detalhamento elevado devido à baixa complexidade do problema. A geometria da tubulação será feita de maneira simplificada utilizando apenas o diâmetro da tubulação e seu comprimento. Conforme apresentado anteriormente a intenção é reproduzir uma simulação na qual os resultados possam ser observados e comparados com os cálculos teóricos. O objetivo é avaliar a normalidade da situação. Neste sentido, é importante encontrar o equilíbrio entre a demanda de tempo para os cálculos teóricos e o detalhamento da simulação do problema.

## Geometria:

 A tubulação em questão apresenta uma secção transversal circular com diâmetro de 40 mm e comprimento de 1000 mm, não possuindo elementos que necessitam de uma maior simplificação, logo a geometria produzida apresenta-se adequada para o problema.
    
## Malha:

 A escolha realizada para a simulação foi a malha automática gerada pelo próprio Ansys Student. A malha resultada é estruturada, ou seja, apresenta um menor número de elementos, permitindo um menor tempo de simulação. Além disso, a malha obtida permite que seus elementos possam alinhar-se com a direção dos gradientes do escoamento, ou seja, é possível obter uma melhor precisão nos resultados.
 
 ## Método:
 
 O método utilizado será o MVF (Método dos Volumes Finitos) por ser mais adequado para a Mecânica dos Fluidos. O método no software se baseia em, de forma geral, decompor o domínio em volumes de controle na malha computacional, utilizar as equações integrais de conservação para cada volume de controle, aproximar em valores numéricos as integrais, aproximar os valores das variáveis nas faces e as derivadas com a informação das variáveis nodais e por último montar e solucionar o sistema algébrico obtido.
    
## Geração e qualidade da malha:

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

    
 A partir desses valores a malha gerada foi classificada de maneira positiva. Como pode ser visto, o valor máximo de Dissimetria se encontra em 0,47313 e o valor mínimo da Qualidade Ortogonal em 0,82069, classificando ambos na margem do Muito Bom nas escalas de qualidade.
    
    
## Informações de entrada (Input) do problema:

 As informações de entrada do problema são a pressão relativa na saída, que será considerada zero, e a velocidade de entrada do problema, a qual foi calculada utilizando o valor da vazão volumétrica fornecido e a Equação da Continuidade, como demonstrado a seguir:
    
  O somatório das vazões mássicas de entrada são iguais ao somatório das vazões mássicas de saída, consequentemente, o mesmo vale para a vazão volumétrica.
    
   ![CodeCogsEqn_eq_continuidade](https://user-images.githubusercontent.com/62161754/85890783-6e496c00-b7c4-11ea-854b-e90ff9427b99.gif)
    

   ![CodeCogsEqn_vazões](https://user-images.githubusercontent.com/62161754/85890830-802b0f00-b7c4-11ea-9b0c-f587844c9333.gif)
    
 A partir disso, para obter o valor da velocidade de entrada do problema é necessário usar a equação a seguir, na qual a vazão volumétrica é resultada da multiplicação entre a velocidade média e a área da secção transversal do tubo. Como a aréa é constante ao longo do tubo, a velocidade média também será a mesma na entrada e na saída.
    
   ![CodeCogsEqn_vazão_volum](https://user-images.githubusercontent.com/62161754/85891295-32fb6d00-b7c5-11ea-9acb-d221bcd8ca1e.gif)
    

   ![CodeCogsEqn_expressao_velocidade](https://user-images.githubusercontent.com/62161754/85892640-ad2cf100-b7c7-11ea-8cc9-55a175b8829a.gif)
    
    
   ![CodeCogsEqn_velocidade](https://user-images.githubusercontent.com/62161754/85891418-6ccc7380-b7c5-11ea-8b1f-782c08bc05e8.gif)
    
    
## Escolhas para o processamento da solução:

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

    
## Prazos:
    
 O prazo para realização da etapa de pré-processamento é de aproximadamente uma semana, sendo suficiente devido à complexidade da simulação.

##  Capacidade computacional:

 A capacidade computacional disponível para a análise segue abaixo:
    
   * Processador: Intel(R) Core(TM) i7-7500 
   * Memória RAM: 8 GB DDR4 2133 MHz
   * Sistema Operacional: Windows 10 
    

# 3. Processamento e Pós-Processamento:


## Simulação preliminar:


### Histórico de convergência:

Na etapa do processamento de solução foi obtido o gráfico de convergência da simulação, como pode ser visto, o histórico de convergência encontra-se adequado devido ao fato de  todas as curvas estarem direcionadas para baixo.

![Solver_Manager_Time - Copia](https://user-images.githubusercontent.com/62161754/86939287-c31ba980-c117-11ea-88ce-07c9acb9850a.png)



### Tempo de processamento da simulação:

A simulação apresentou um tempo de processamento de aproximadamente 4 segundos. Consequente da simplicidade na geometria adotada e da malha utilizada.

![Solver_Manager_Time](https://user-images.githubusercontent.com/62161754/86954231-ff590500-c12b-11ea-9f5d-69192250f28b.png)

### Resíduos:

Os resíduos, ou seja, o erro da simulação, encontram-se acetáveis, uma vez que a malha adotada possui valores de qualidade ortogonal e de dissimetria na escala do Muito Bom. Permitindo resultados potencialmente condizentes para os requisitos de solução apresentados.

## Resultados preliminares:

Após o processamento, utilizou-se o pacote CFD-Post para obter os resultados da simulação, inicialmente foi inserido um plano de referência entre a entrada e a saída do tubo.

![CFD-Post_Location_Plane_Cursor](https://user-images.githubusercontent.com/62161754/86946078-3aedd200-c120-11ea-8f6e-667c9de0e188.png)

![CFD-Post_Plane1_config](https://user-images.githubusercontent.com/62161754/86946095-417c4980-c120-11ea-9e27-c93c07ab9299.png)


Consecutivamente foram adicionadas uma linha horizontal e outra vertical para a geração dos gráficos de perfil de velocidade e de perda de carga.

![CFD-Post_Location_line1](https://user-images.githubusercontent.com/62161754/86947408-214d8a00-c122-11ea-8bd8-cf40edbb85db.png)

![CFD-Post_Line1](https://user-images.githubusercontent.com/62161754/86947453-2e6a7900-c122-11ea-9bb2-e0a73783594a.png)

![CFD-Post_Line2](https://user-images.githubusercontent.com/62161754/86947461-2f9ba600-c122-11ea-9b3f-531a0f005f31.png)


### Resultados qualitativos e quantitativos:

Nessa etapa do pós-processamento, após a criação do plano de referência e das linhas, foram obtidos resultados qualitativos característicos de engenharia, como:

   * Vetores de velocidade do escoamento, inseridos através da ferramenta "Vector":
   
   ![CFD-Post_Vector1](https://user-images.githubusercontent.com/62161754/86953049-41814700-c12a-11ea-91a4-97d8e922a5a3.png)
   
   ![CFD-Post_Vector2_simulation](https://user-images.githubusercontent.com/62161754/86952853-f9622480-c129-11ea-8138-6da759c10a01.png)
   
   

   * Contorno de perfil de velocidade com 15 amostras, utilizando a ferramenta "Contour":
   
   ![CFD-Post_Contour_cursor](https://user-images.githubusercontent.com/62161754/86953204-77263000-c12a-11ea-8a9f-cb9b4ae9f05c.png)
   
   ![CFD-Post_Velocity_contour_15](https://user-images.githubusercontent.com/62161754/86952897-0bdc5e00-c12a-11ea-8a06-bdcfd210b33a.png)
   
   
   
   * Contorno de pressão com 15 amostras:
   
   ![CFD-Post_Pressure_contour_15](https://user-images.githubusercontent.com/62161754/86953335-ad63af80-c12a-11ea-9c7c-5303db7fcd39.png)
   
   
   * Gráfico de perfil de velocidade com 100 amostras, gerado pela ferramenta "Chart":
   
   ![CFD-Post_Chart_cursor](https://user-images.githubusercontent.com/62161754/86973946-cc266e00-c14b-11ea-9482-76d4bed07feb.png)
   
   
   ![CFD-Post_Chart2_Velocity](https://user-images.githubusercontent.com/62161754/86952921-14cd2f80-c12a-11ea-9c84-73b5d9b82505.png)
   
   
   
   * Gráfico de perda de carga, apresentando a perda de pressão de acordo com o escoamento, da entrada para a saída respectivamente:
   
   ![CFD-Post_Chart1_Pressure](https://user-images.githubusercontent.com/62161754/86952932-172f8980-c12a-11ea-91de-cac1c165c13c.png)
   
   

A partir do processamento da simulação, efetuou-se a inserção de paramêtros de entrada e de saída para o cálculo de valores para o Número de Reynolds de acordo com diferentes valores de velocidade média e da Perda de carga. Com base nisso, permite-se avaliar o perfil do escoamento e consequentemente aferir os valores necessários para o estudo paramétrico do Fator de Atrito.


   #### Número de Reynolds:
   
   O Número de Reynolds (![CodeCogsEqn_Re](https://user-images.githubusercontent.com/62161754/87058404-6d5e0480-c1de-11ea-8b69-a48e6d09cf1b.gif)) será importante para o cálculo e análise do estudo paramétrico do Fator de Atrito, para isso, seu cálculo é realizado da seguinte maneira:
   
   ![CodeCogsEqn_n_reynolds](https://user-images.githubusercontent.com/62161754/86963484-fe7b9f80-c13a-11ea-903a-659f8a3d2513.gif)

Onde ![CodeCogsEqn_rho](https://user-images.githubusercontent.com/62161754/86963801-734ed980-c13b-11ea-8607-2d63465484e0.gif) , ![CodeCogsEqn_v](https://user-images.githubusercontent.com/62161754/86963546-13f0c980-c13b-11ea-8050-63bfec6b6913.gif) , ![CodeCogsEqn_D](https://user-images.githubusercontent.com/62161754/86963552-16ebba00-c13b-11ea-86e8-d1ad8c8761bd.gif) , ![CodeCogsEqn_mu](https://user-images.githubusercontent.com/62161754/86963562-1b17d780-c13b-11ea-9aae-fcf80ca984a6.gif) respectivamente são:

   * Massa específica da água:
   
   ![CodeCogsEqn_massaesp](https://user-images.githubusercontent.com/62161754/86963907-a6916880-c13b-11ea-83b3-5941cf2ef37d.gif)
   
   * Velocidade: 
   
   ![CodeCogsEqn_velocity](https://user-images.githubusercontent.com/62161754/86963920-ac874980-c13b-11ea-805d-930e8f540b97.gif)
   
   * Diâmetro do tubo:
   
   ![CodeCogsEqn_diametro](https://user-images.githubusercontent.com/62161754/86963930-b01ad080-c13b-11ea-8039-c53a07348e92.gif)
   
   * Viscosidade dinâmica da água:
   
   ![CodeCogsEqn_viscosity](https://user-images.githubusercontent.com/62161754/86963953-b8730b80-c13b-11ea-8a1e-b18ad5b20f7a.gif)

Logo:

![CodeCogsEqn_n_reynolds_numbers](https://user-images.githubusercontent.com/62161754/86964204-1142a400-c13c-11ea-8a87-2284f859344a.gif)

![CodeCogsEqn_n_reynolds_result](https://user-images.githubusercontent.com/62161754/86964268-333c2680-c13c-11ea-8817-ed3551b4bcc2.gif)
   
   
 Com os cálculos realizados, elaborou-se uma tabela com as comparações entre os valores para o Número de Reynolds (![CodeCogsEqn_Re](https://user-images.githubusercontent.com/62161754/87058404-6d5e0480-c1de-11ea-8b69-a48e6d09cf1b.gif)) calculados e os valores obtidos pela simulação de acordo com a variação de velocidade:
   
   | Velocidade (m/s) | ![CodeCogsEqn_Re](https://user-images.githubusercontent.com/62161754/87058404-6d5e0480-c1de-11ea-8b69-a48e6d09cf1b.gif) teórico | ![CodeCogsEqn_Re](https://user-images.githubusercontent.com/62161754/87058404-6d5e0480-c1de-11ea-8b69-a48e6d09cf1b.gif) simulado | Erro percentual |
   |:----------------------------:|:---------------------------:|:---------------------------------:|:--------------------------------:|
   | 0,02 | 895,17 | 893,53 | 0,1835% |
   | 0,05 | 2237,93 | 2236,2 | 0,0773% |
   | 0,0795 | 3558,31 | 3556,5 | 0,0508% |
   | 0,1 | 4475,86 | 4474,1 | 0,0393% |
   
   
   #### Perda de carga:
   
   A perda de carga (![CodeCogsEqn_hf](https://user-images.githubusercontent.com/62161754/87077393-6bee0580-c1f9-11ea-82bf-84183ce8faf2.gif)) mensurada na tubulação com uma velocidade média do escoamento de 0,0795 m/s foi de 2 Pa. Assim como para o Número de Reynolds, foram inseridos diferentes valores de velocidade média para uma análise breve da perda de carga na tubulação simulada.

| Velocidade (m/s) | ![CodeCogsEqn_hf](https://user-images.githubusercontent.com/62161754/87077393-6bee0580-c1f9-11ea-82bf-84183ce8faf2.gif) (Pa) simulado |  
|:--------------------:|:--------------------:|
| 0,02 | 0,42433 |
| 0,05 | 1,1608 |
| 0,0795 | 1,8326 |
| 0,1 | 2,4963 |


## Estudo paramétrico preliminar:

Em escoamentos podem ocorrer diversas perdas energéticas, entre elas há o Fator de Atrito através das forças de cisalhamento do fluido. Para calcular o Fator de Atrito é necessário previamente analisar o comportamento do escoamento, o qual pode ser classificado como em regime laminar, de transição ou turbulento. Estas regiões possuem valores limites característicos para o Número de Reynolds, são eles:

   * Regime laminar: ![CodeCogsEqn_Re](https://user-images.githubusercontent.com/62161754/86964518-9201a000-c13c-11ea-829e-d4d213d85e9b.gif) < 2100;
   * Regime de transição entre laminar e turbulento: 2100 < ![CodeCogsEqn_Re](https://user-images.githubusercontent.com/62161754/86964518-9201a000-c13c-11ea-829e-d4d213d85e9b.gif) < 4000;
   * Regime turbulento: ![CodeCogsEqn_Re](https://user-images.githubusercontent.com/62161754/86964518-9201a000-c13c-11ea-829e-d4d213d85e9b.gif) > 4000;
   

Para cada região de escoamento há uma forma de calcular o Fator de Atrito. No escoamento laminar o fator de atrito de Darcy (![CodeCogsEqn_f](https://user-images.githubusercontent.com/62161754/86968811-28d15b00-c143-11ea-94d7-0103baca53c1.gif)
) depende apenas do Número de Reynolds:

![CodeCogsEqn_atrito_laminar](https://user-images.githubusercontent.com/62161754/86968814-2969f180-c143-11ea-9bd0-c71eec996e61.gif)


Para os demais escoamentos faz-se importante a consideração de outro fator, a rugosidade (![CodeCogsEqn_E_rugosidade](https://user-images.githubusercontent.com/62161754/86966121-f6256380-c13e-11ea-9ab2-7eb127fa0991.gif)), podendo variar de acordo com o material da tubulação, a maneira como foi fabricada e o tempo de utilização. A rugosidade absoluta possui unidade de medida de comprimento e a rugosidade relativa é adimensional.

Para os escoamentos turbulentos a expressão mais usual para o Fator de Atrito (![CodeCogsEqn_f](https://user-images.githubusercontent.com/62161754/86969713-9c279c80-c144-11ea-9d71-559956255946.gif)
) é a de Colebrook.

![CodeCogsEqn_Colebrook](https://user-images.githubusercontent.com/62161754/86969679-8914cc80-c144-11ea-8267-5799699d6e67.gif)

É possível notar que a equação de Colebrook é implícita em ![CodeCogsEqn_f](https://user-images.githubusercontent.com/62161754/86969713-9c279c80-c144-11ea-9d71-559956255946.gif) , sendo possível calcular através de Softwares para cálculo numérico ou realizando apenas algumas iterações.

Outra expressão aceita para casos onde ![CodeCogsEqn_Re](https://user-images.githubusercontent.com/62161754/86970337-98e0e080-c145-11ea-971c-e55cd92bb3e2.gif) > 3000 é a equação de Haaland.

![CodeCogsEqn_Haaland](https://user-images.githubusercontent.com/62161754/86969681-89ad6300-c144-11ea-9e54-249641a9bb8e.gif)

A equação de Haaland é explícita em ![CodeCogsEqn_f](https://user-images.githubusercontent.com/62161754/86969713-9c279c80-c144-11ea-9d71-559956255946.gif) , porém os resultandos diferem cerca de 2% dos resultados obtidos através da equação de Colebrook.

Além disso, para casos em que a superfície da tubulação é considerada lisa, outra equação aceita é a de Prandtl.

![CodeCogsEqn_Prandtl](https://user-images.githubusercontent.com/62161754/86971333-5f10d980-c147-11ea-837d-426760d69145.gif)

Baseado na expressão de Colebrook, traçou-se o Diagrama de Moody, tal gráfico mostra as relações entre o Fator de Atrito, Número de Reynolds e a rugosidade relativa. A partir do diagrama é possível estimar os valores para o Fator de Atrito e compará-los com os resultados teóricos obtidos.

![Diagrama_de_Moody_2](https://user-images.githubusercontent.com/62161754/86973362-d72cce80-c14a-11ea-8241-d6e45652dcce.jpg)

Como pode ser visto acima, o comportamento do escoamento, ou seja, o Número de Reynolds, pode variar facilmente de acordo com a velocidade do escoamento, consequentemente o mesmo vale para o fator de atrito na tubulação. Para a análise do estudo paramétrico serão observadas as mudanças no Fator de Atrito de acordo com diferentes valores para a velocidade média e para diferentes materiais. Serão considerados os seguintes materiais e seus respectivos valores de rugosidade absoluta em metros. O objetivo é avaliar a influência do tipo de material da tubulação e a velocidade do fluido, nos valores do Fator de Atrito.

| Material | Rugosidade absoluta (m) |
|:-----:|:--------------------:|
| Aço galvanizado com costura  | 0,00015   |
| Aço galvanizado sem costura  | 0,00006|
| Ferro fundido novo  | 0,00025 |
| Ferro fundido com leve oxidação  | 0,0003 |
| Ferro fundido velho  | 0,003 |
| PVC, plásticos em geral  | 0,0000015 |
| "liso"  | 0 |
 
 
   #### Fator de Atrito:
   
   Inseriram-se tabelas comparativas entre os valores teóricos e simulados do Fator de Atrito de acordo com os materiais selecionados e a variação da velocidade.
   
   * ![CodeCogsEqn_v1](https://user-images.githubusercontent.com/62161754/87051052-75fe0d00-c1d5-11ea-877a-ae1e21390aaa.gif)
   
   | ![CodeCogsEqn_f](https://user-images.githubusercontent.com/62161754/87052238-ec4f3f00-c1d6-11ea-890e-21ce86ea7511.gif) teórico | ![CodeCogsEqn_f](https://user-images.githubusercontent.com/62161754/87052238-ec4f3f00-c1d6-11ea-890e-21ce86ea7511.gif) simulado | Erro percentual |
   |:---------------------------------:|:--------------------------------:|:----------------------------:|
   | 0,07149480 | 0,071626023 | 0,1832% |
   
   
   


   * ![CodeCogsEqn_v2](https://user-images.githubusercontent.com/62161754/87051054-75fe0d00-c1d5-11ea-942b-9da3d07dbb3e.gif)
   
   | Material | ![CodeCogsEqn_E_rugosidade](https://user-images.githubusercontent.com/62161754/87052231-ea857b80-c1d6-11ea-999b-0f913f72a9e0.gif) (m) | ![CodeCogsEqn_f](https://user-images.githubusercontent.com/62161754/87052238-ec4f3f00-c1d6-11ea-890e-21ce86ea7511.gif) teórico | ![CodeCogsEqn_f](https://user-images.githubusercontent.com/62161754/87052238-ec4f3f00-c1d6-11ea-890e-21ce86ea7511.gif) simulado | Erro percentual |
   |:------------------------------------:|:---------------------:|:--------------------:|:-----------------------:|:---------------------:|
   | Aço galvanizado com costura | 0,00015 | 0,0506346 | 0,0506456 | 0,0217% |
   | Aço galvanizado sem costura | 0,0006 | 0,0488869 | 0,0488983 | 0,0233% |
   | Ferro fundido novo | 0,00025 | 0,0535383 | 0,0525387 | 0,0197% |
   | Ferro fundido com leve oxidação | 0,0003 | 0,0534576 | 0,0534679 | 0,0192% |
   | Ferro fundido velho | 0,003 | 0,0950876 | 0,0950934 | 0,0061% |
   | PVC, plásticos em geral | 0,0000015 | 0,0477268 | 0,0477385 | 0,0245% |
   | "liso" | 0 | 0,0476968 | 0,0477085 | 0,0245% |
   
   
   
   
   * ![CodeCogsEqn_vmd](https://user-images.githubusercontent.com/62161754/87051048-75657680-c1d5-11ea-9bf2-5f3ef739e690.gif)
   
   | Material | ![CodeCogsEqn_E_rugosidade](https://user-images.githubusercontent.com/62161754/87052231-ea857b80-c1d6-11ea-999b-0f913f72a9e0.gif) (m) | ![CodeCogsEqn_f](https://user-images.githubusercontent.com/62161754/87052238-ec4f3f00-c1d6-11ea-890e-21ce86ea7511.gif) teórico | ![CodeCogsEqn_f](https://user-images.githubusercontent.com/62161754/87052238-ec4f3f00-c1d6-11ea-890e-21ce86ea7511.gif) simulado | Erro percentual |
   |:------------------------------------:|:---------------------:|:--------------------:|:-----------------------:|:------------------------:|
   | Aço galvanizado com costura | 0,00015 | 0,0448128 | 0,0448184 | 0,0124% |
   | Aço galvanizado sem costura | 0,0006 | 0,0427494 | 0,0427554 | 0,0140% |
   | Ferro fundido novo | 0,00025 | 0,0470113 | 0,0470166 | 0,0112% |
   | Ferro fundido com leve oxidação | 0,0003 | 0,0480778 | 0,0480829 | 0,0106% |
   | Ferro fundido velho | 0,003 | 0,0922701 | 0,0922726 | 0,0027% |
   | PVC, plásticos em geral | 0,0000015 | 0,0413589 | 0,0413652 | 0,0152% |
   | "liso" | 0 | 0,0413226 | 0,0413290 | 0,0154% |
  
  
  
  
   * ![CodeCogsEqn_v4](https://user-images.githubusercontent.com/62161754/87051046-74cce000-c1d5-11ea-8fc0-8f6cfef3884f.gif)

  | Material | ![CodeCogsEqn_E_rugosidade](https://user-images.githubusercontent.com/62161754/87052231-ea857b80-c1d6-11ea-999b-0f913f72a9e0.gif) (m) | ![CodeCogsEqn_f](https://user-images.githubusercontent.com/62161754/87052238-ec4f3f00-c1d6-11ea-890e-21ce86ea7511.gif) teórico | ![CodeCogsEqn_f](https://user-images.githubusercontent.com/62161754/87052238-ec4f3f00-c1d6-11ea-890e-21ce86ea7511.gif) simulado | Erro percentual |
   |:------------------------------------:|:---------------------:|:--------------------:|:-----------------------:|:------------------------:|
   | Aço galvanizado com costura | 0,00015 | 0,0424226 | 0,0424264 | 0,0089% |
   | Aço galvanizado sem costura | 0,0006 | 0,0401788 | 0,0401830 | 0,0104% |
   | Ferro fundido novo | 0,00025 | 0,0447875 | 0,0447910 | 0,0078% |
   | Ferro fundido com leve oxidação | 0,0003 | 0,0459265 | 0,0459299 | 0,0074% |
   | Ferro fundido velho | 0,003 | 0,0912639 | 0,0912654 | 0,0016% |
   | PVC, plásticos em geral | 0,0000015 | 0,0386512 | 0,036556 | 0,0113% |
   | "liso" | 0 | 0,0386112 | 0,0386156 | 0,0113% |




### Análise preliminar:

#### Fator de Atrito:

A partir do resultados apresentados é possível notar que, à medida que ocorre o aumento da velocidade média do escoamento e do número de Reynolds, os valores do Fator de Atrito decrescem, quando isso ocorre a espessura da fina camada viscosa próxima à parede do tubo diminui. Sendo assim os elementos de rugosidade partem a emergir através desta camada, tornando o efeito da rugosidade importante para esses casos. Como mencionado anteriormente, quando o escoamento passa a apresentar comportamento de regime turbulento, o Fator de Atrito não depende mais apenas do Número de Reynolds, mas também da rugosidade. Observa-se que quando o valor da rugosidade absoluta aumenta, para o mesmo tubo circular com a área de secção transversal constante, o valor do Fator de Atrito também aumenta.

Ao analisar o efeito da mudança de material da tubulação nota-se que determinados tipos de materiais possuem valores de rugosidade maiores e consequentemente aumentam os efeitos do Fator de Atrito, assim como outros materiais possuem valores menores e causam efeitos menores no Fator de Atrito. Comparando os valores de rugosidade para o mesmo material porém produzidos de maneira distinta, no caso o aço galvanizado, nota-se que o tubo com costura foi fabricado através da soldagem de uma chapa de metal, dessa maneira as extremidades foram unidas pelo calor e instrumentos de soldagem, e portanto, possui um valor de rugosidade mais elevado, resultando em valores maiores para o Fator de Atrito em regimes turbulentos. Um pouco diferente do tubo sem costura, o qual sua fabricação consiste na perfuração de um cilindro de metal aquecido, resultando em uma rugosidade menor. Para o ferro fundido foi analisada a influência do tempo de uso da tubulação perante os valores de rugosidade e Fator de Atrito. Para uma tubulação mais velha a rugosidade tende a aumentar, o mesmo ocorre para o Fator de Atrito.

#### Perfil de velocidade:


#### Perda de carga:


#### Número de Reynolds:





## O projeto deverá conter nesta etapa:

- Análise dos resultados obtidos.
- Comparação dos resultados numéricos com os resultados analíticos de cada problema.
- Imagens de visualização do escoamento.
- Análise dos resultados obtidos pelo estudo paramétrico.

