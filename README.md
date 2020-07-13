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
    
   ![CFX-Pre_water_and_reference_pressure](https://user-images.githubusercontent.com/62161754/87212999-0896cd00-c2f8-11ea-9b11-24539bf16334.png)
    
   ![CFX-Pre_Domain_heat_transfer](https://user-images.githubusercontent.com/62161754/85911301-dca92100-b7fa-11ea-8732-c5249705757f.png)
    
  Consequentemente foram definidos os detalhes das condições de contorno na entrada e na saída do tubo, primeiro foram atribuídos o parâmetro de velocidade para a entrada do escoamento e a pressão estática relativa na saída.
    
   ![CFX-Pre_Boundary_entrada](https://user-images.githubusercontent.com/62161754/85911165-cfd7fd80-b7f9-11ea-88bc-f53fb38c7161.png)
    
   ![CFX-Pre_Boundary_entrada_Details_Speed](https://user-images.githubusercontent.com/62161754/87213041-514e8600-c2f8-11ea-8305-1922ea0675bf.png)
       
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
    

# 3. Processamento:


## Histórico de convergência:

Na etapa do processamento de solução foi obtido o gráfico de convergência da simulação, como pode ser visto, o histórico de convergência encontra-se adequado devido ao fato de  todas as curvas estarem direcionadas para baixo.

![Solver_Manager_Time - Copia](https://user-images.githubusercontent.com/62161754/86939287-c31ba980-c117-11ea-88ce-07c9acb9850a.png)



## Tempo de processamento da simulação:

A simulação apresentou um tempo de processamento de aproximadamente 4 segundos. Consequente da simplicidade da geometria adotada e da malha utilizada.

![Solver_Manager_Time](https://user-images.githubusercontent.com/62161754/86954231-ff590500-c12b-11ea-9f5d-69192250f28b.png)

## Resíduos:

Os resíduos, ou seja, o erro da simulação, encontram-se aceitáveis, uma vez que a malha adotada possui valores de qualidade ortogonal e de dissimetria na escala do Muito Bom. Permitindo resultados potencialmente satisfatórios para os requisitos de solução apresentados.


Utilizou-se o pacote CFD-Post para obter os resultados da simulação. Inicialmente foi inserido um plano de referência entre a entrada e a saída do tubo.

![CFD-Post_Location_Plane_Cursor](https://user-images.githubusercontent.com/62161754/86946078-3aedd200-c120-11ea-8f6e-667c9de0e188.png)

![CFD-Post_Plane1_config](https://user-images.githubusercontent.com/62161754/86946095-417c4980-c120-11ea-9e27-c93c07ab9299.png)


Consecutivamente foram adicionadas uma linha horizontal e outra vertical para a geração dos gráficos de perfil de velocidade e de perda de carga.

![CFD-Post_Location_line1](https://user-images.githubusercontent.com/62161754/86947408-214d8a00-c122-11ea-8bd8-cf40edbb85db.png)

![CFD-Post_Line1](https://user-images.githubusercontent.com/62161754/86947453-2e6a7900-c122-11ea-9bb2-e0a73783594a.png)

![CFD-Post_Line2](https://user-images.githubusercontent.com/62161754/86947461-2f9ba600-c122-11ea-9b3f-531a0f005f31.png)


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
   
   
# 4. Pós-processamento:

## Resultados preliminares:

   Foram obtidos resultados quantitativos após o processamento, efetuou-se a inserção de paramêtros de entrada e de saída para o cálculo do Número de Reynolds e da Perda de carga de acordo com diferentes valores de velocidade média.
   
   ### Número de Reynolds:
   
   O Número de Reynolds (![CodeCogsEqn_Re](https://user-images.githubusercontent.com/62161754/87058404-6d5e0480-c1de-11ea-8b69-a48e6d09cf1b.gif)) permite avaliar o perfil do escoamento. O qual pode ser classificado como regime laminar, regime de transição ou regime turbulento. Estas regiões possuem valores limites característicos para o Número de Reynolds, são eles:

   * Regime laminar: ![CodeCogsEqn_Re](https://user-images.githubusercontent.com/62161754/86964518-9201a000-c13c-11ea-829e-d4d213d85e9b.gif) < 2100;
   * Regime de transição entre laminar e turbulento: 2100 < ![CodeCogsEqn_Re](https://user-images.githubusercontent.com/62161754/86964518-9201a000-c13c-11ea-829e-d4d213d85e9b.gif) < 4000;
   * Regime turbulento: ![CodeCogsEqn_Re](https://user-images.githubusercontent.com/62161754/86964518-9201a000-c13c-11ea-829e-d4d213d85e9b.gif) > 4000;
   
   O cálculo do Número de Reynolds é realizado da seguinte maneira:
   
   ![CodeCogsEqn_n_reynolds](https://user-images.githubusercontent.com/62161754/86963484-fe7b9f80-c13a-11ea-903a-659f8a3d2513.gif)

Onde ![CodeCogsEqn_rho](https://user-images.githubusercontent.com/62161754/86963801-734ed980-c13b-11ea-8607-2d63465484e0.gif) , ![CodeCogsEqn_v](https://user-images.githubusercontent.com/62161754/86963546-13f0c980-c13b-11ea-8050-63bfec6b6913.gif) , ![CodeCogsEqn_D](https://user-images.githubusercontent.com/62161754/86963552-16ebba00-c13b-11ea-86e8-d1ad8c8761bd.gif) , ![CodeCogsEqn_mu](https://user-images.githubusercontent.com/62161754/86963562-1b17d780-c13b-11ea-9aae-fcf80ca984a6.gif) respectivamente, são:

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
   
   Os valores apresentam baixo erro percentual entre os valores simulados e teóricos. De acordo com a tabela elaborada, a velocidade do escoamento e o número de Reynolds são diretamente proporcionais. À medida que a velocidade aumenta de 0,02 m/s para 0,05 m/s, o fluido começa a adotar a transição entre regime laminar e turbulento, notório pelo número de Reynolds. Quando a velocidade atinge 0,0795 m/s, o fluido apresenta comportanto próximo ao turbulento. Portanto, os resultados para o número de Reynolds obtidos apresentam-se coerentes com a realidade física do escoamento.
   
   ### Perda de carga:
   
   Para o cálculo teórico da Perda de carga (![CodeCogsEqn_hl](https://user-images.githubusercontent.com/62161754/87109340-c3f92c00-c23a-11ea-86f3-8022ef4eeb87.gif)) em Pa, utilizou-se a seguinte expressão:
   
   ![CodeCogsEqn_pressureloss_up](https://user-images.githubusercontent.com/62161754/87317096-ee7a0c00-c4fc-11ea-8e67-0aa02367e8dd.gif)
   
   Onde ![CodeCogsEqn_f](https://user-images.githubusercontent.com/62161754/87108383-8f847080-c238-11ea-9077-d87850297b36.gif) e ![CodeCogsEqn_L](https://user-images.githubusercontent.com/62161754/87108360-82678180-c238-11ea-9c26-d4c67627341b.gif) são, respectivamente:
   
   * Fator de Atrito, para este cálculo inicial da Perda de carga na tubulação, adotou-se a superfície do cano como "lisa", resultando no seguinte valor:
   
   ![CodeCogsEqn_f_number](https://user-images.githubusercontent.com/62161754/87108825-8ba51e00-c239-11ea-86d0-a5f086093802.gif)
   
   * Comprimento do tubo.
   
   ![CodeCogsEqn_L_m](https://user-images.githubusercontent.com/62161754/87108541-f570f800-c238-11ea-8358-090e487445bf.gif)
   
   Utilizando estes e outros valores apresentados ateriormente, foi possível chegar ao valor teórico da Perda de carga:
   
   ![CodeCogsEqn_pressureloss_number](https://user-images.githubusercontent.com/62161754/87108286-50561f80-c238-11ea-9fae-c2b69d3cb999.gif)
   
   ![CodeCogsEqn_pressureloss_result](https://user-images.githubusercontent.com/62161754/87108290-53e9a680-c238-11ea-9aa7-ce0624e29866.gif)
   
   A perda de carga mensurada na tubulação com a velocidade média do escoamento de 0,0795 m/s foi de 2 Pa. Assim como para o Número de Reynolds, foram inseridos diferentes valores de velocidade média para uma análise breve da perda de carga na tubulação simulada.

| Velocidade (m/s) | ![CodeCogsEqn_hl](https://user-images.githubusercontent.com/62161754/87109340-c3f92c00-c23a-11ea-86f3-8022ef4eeb87.gif) (Pa) teórico | ![CodeCogsEqn_hl](https://user-images.githubusercontent.com/62161754/87109340-c3f92c00-c23a-11ea-86f3-8022ef4eeb87.gif) (Pa) simulado  | Erro percentual |
|:--------------------:|:--------------------:|:-------------------------:|:--------------:|
| 0,02 | 0,2058 | 0,42433 | 51,500%  |
| 0,05 | 1,2867 | 1,1608 | 9,784% |
| 0,0795 | 3,2530 | 1,8326 | 43,664% |
| 0,1 | 5,1470 | 2,4963 | 51,499% |

Nota-se que os erros percentuais obtidos são elevados. Os valores de perda de carga para o escoamento em questão apresentou erro de 43,664% entre o valor simulado e o teórico. Não caracterizando o escoamento simulado de acordo com a sua realidade física.

 ### Fator de Atrito:

Em escoamentos podem ocorrer diversas perdas energéticas, entre elas, o Fator de Atrito. Através das forças de cisalhamento do fluido. Para cada regime de escoamento há uma forma de calcular o Fator de Atrito. 

No escoamento laminar, o Fator de Atrito de Darcy (![CodeCogsEqn_f](https://user-images.githubusercontent.com/62161754/86968811-28d15b00-c143-11ea-94d7-0103baca53c1.gif)
) depende apenas do Número de Reynolds:

![CodeCogsEqn_atrito_laminar](https://user-images.githubusercontent.com/62161754/86968814-2969f180-c143-11ea-9bd0-c71eec996e61.gif)


Para os demais escoamentos faz-se importante a consideração de outro fator, a rugosidade (![CodeCogsEqn_E_rugosidade](https://user-images.githubusercontent.com/62161754/86966121-f6256380-c13e-11ea-9ab2-7eb127fa0991.gif)), podendo variar de acordo com o material da tubulação, a maneira como foi fabricada e o tempo de utilização. A rugosidade absoluta (![CodeCogsEqn_E_rugosidade](https://user-images.githubusercontent.com/62161754/86966121-f6256380-c13e-11ea-9ab2-7eb127fa0991.gif)) possui unidade de medida de comprimento e a rugosidade relativa (![CodeCogsEqn_E_rugosidade](https://user-images.githubusercontent.com/62161754/86966121-f6256380-c13e-11ea-9ab2-7eb127fa0991.gif)/![CodeCogsEqn_D](https://user-images.githubusercontent.com/62161754/86963552-16ebba00-c13b-11ea-86e8-d1ad8c8761bd.gif)) é adimensional.

Para escoamentos turbulentos a expressão mais usual para o Fator de Atrito (![CodeCogsEqn_f](https://user-images.githubusercontent.com/62161754/86969713-9c279c80-c144-11ea-9d71-559956255946.gif)
) é a de Colebrook.

![CodeCogsEqn_Colebrook](https://user-images.githubusercontent.com/62161754/86969679-8914cc80-c144-11ea-8267-5799699d6e67.gif)

É possível notar que a equação de Colebrook é implícita em ![CodeCogsEqn_f](https://user-images.githubusercontent.com/62161754/86969713-9c279c80-c144-11ea-9d71-559956255946.gif) , sendo possível calculá-la através de Softwares de cálculo numérico ou realizando algumas iterações.

Outra expressão aceita para casos onde ![CodeCogsEqn_Re](https://user-images.githubusercontent.com/62161754/86970337-98e0e080-c145-11ea-971c-e55cd92bb3e2.gif) > 3000 é a equação de Haaland.

![CodeCogsEqn_Haaland](https://user-images.githubusercontent.com/62161754/86969681-89ad6300-c144-11ea-9e54-249641a9bb8e.gif)

A equação de Haaland é explícita em ![CodeCogsEqn_f](https://user-images.githubusercontent.com/62161754/86969713-9c279c80-c144-11ea-9d71-559956255946.gif) , porém os resultandos diferem cerca de 2% dos resultados obtidos através da equação de Colebrook.

Além disso, para casos em que a superfície da tubulação é considerada lisa, outra equação aceita é a de Prandtl.

![CodeCogsEqn_Prandtl](https://user-images.githubusercontent.com/62161754/86971333-5f10d980-c147-11ea-837d-426760d69145.gif)

Serão considerados os seguintes materiais e seus respectivos valores de rugosidade absoluta em metros. O objetivo é avaliar a tendência do Fator de Atrito de acordo com o tipo de material da tubulação, a técnica de fabricação (para o caso do Aço galvanizado), a idade da tubulção (analisando o ferro fundido) e a velocidade do fluido.

| Material | Rugosidade absoluta (m) |
|:-----:|:--------------------:|
| Aço galvanizado com costura  | 0,00015   |
| Aço galvanizado sem costura  | 0,00006|
| Ferro fundido novo  | 0,00025 |
| Ferro fundido com leve oxidação  | 0,0003 |
| Ferro fundido velho  | 0,003 |
| PVC, plásticos em geral  | 0,0000015 |
| "liso"  | 0 |
 
 Tal escolha de parâmetros e variáveis, possui as seguintes finalidades:
 
   * Analisar os efeitos causados por materiais diferentes.E assim, comprovar a influência da rugosidade no cálculo do Fator de Atrito.
   * Avaliar a mudança no Fator de Atrito, de acordo com a diferença da rugosidade entre processos de fabricação distintos, para o mesmo material.
   * Calcular os efeitos da oxidação no mesmo material, porém, com tempos de utilização distintos.
   * Observar o Fator de Atrito e sua relevância no escoamento, de acordo com a variação da velocidade, e consequentemente, o regime do escoamento.
   
  Foram estabelecidas tabelas comparativas entre os valores teóricos e simulados do Fator de Atrito (![CodeCogsEqn_f](https://user-images.githubusercontent.com/62161754/87052238-ec4f3f00-c1d6-11ea-890e-21ce86ea7511.gif)), de acordo com os materiais selecionados e a variação da velocidade.
   
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


# 5. Estudo Paramétrico:

 O Diagrama de Moody mostra as relações entre o Fator de Atrito ( ![CodeCogsEqn_f](https://user-images.githubusercontent.com/62161754/87052238-ec4f3f00-c1d6-11ea-890e-21ce86ea7511.gif)), Número de Reynolds (![CodeCogsEqn_Re](https://user-images.githubusercontent.com/62161754/86964518-9201a000-c13c-11ea-829e-d4d213d85e9b.gif)) e a rugosidade relativa (![CodeCogsEqn_E_rugosidade](https://user-images.githubusercontent.com/62161754/86966121-f6256380-c13e-11ea-9ab2-7eb127fa0991.gif)/![CodeCogsEqn_D](https://user-images.githubusercontent.com/62161754/86963552-16ebba00-c13b-11ea-86e8-d1ad8c8761bd.gif)). A partir do diagrama é possível estimar os valores para o Fator de Atrito e compará-los com os resultados teóricos obtidos.


![Diagrama_de_Moody_3](https://user-images.githubusercontent.com/62161754/87110939-97dfaa00-c23e-11ea-9775-454d4cd43e8d.jpg)

Como pode ser visto acima, o comportamento do escoamento e o Número de Reynolds podem variar facilmente de acordo com a velocidade do escoamento, consequentemente o mesmo vale para o fator de atrito na tubulação. 




***Para a análise do estudo paramétrico serão observadas as mudanças no Fator de Atrito de acordo com diferentes valores para a velocidade média e para diferentes materiais. ***


# 6. Análise preliminar:

### Número de Reynolds:

Para a simulação realizada, foi adotado para o escoamento o regime laminar. Porém, a partir do cálculo do Número de Reynolds para a realização do estudo paramétrico, conclui-se que o escoamento apresenta um comportamento mais turbulento. O valor de ![CodeCogsEqn_Re](https://user-images.githubusercontent.com/62161754/87111638-36b8d600-c240-11ea-98ba-7f5325b05069.gif) foi de 3558,31, caracterizando um regime de transição para turbulento, tornando a simulação efetuada não coerente com a física do escoamento. Tal fato, no entanto, não causou um erro percentual elevado entre o resultado simulado no pós-processamento através da inserção de parâmetros, e os resultados teóricos obtidos através dos cálculos. 

 | Velocidade (m/s) | ![CodeCogsEqn_Re](https://user-images.githubusercontent.com/62161754/87058404-6d5e0480-c1de-11ea-8b69-a48e6d09cf1b.gif) teórico | ![CodeCogsEqn_Re](https://user-images.githubusercontent.com/62161754/87058404-6d5e0480-c1de-11ea-8b69-a48e6d09cf1b.gif) simulado | Erro percentual |
   |:----------------------------:|:---------------------------:|:---------------------------------:|:--------------------------------:|
   | 0,0795 | 3558,31 | 3556,5 | 0,0508% |

Consequentemente, o baixo valor de erro percentual foi aceitável para a comparação preliminar dos valores para o Fator de Atrito e suas correlações. Porém, para o perfil de velocidade e a perda de carga, a caracterização do regime como laminar ao invés de turbulento, afetou ambos resultados de maneira mais acentuada.

### Fator de Atrito:

A partir do resultados apresentados é possível notar que, à medida que ocorre o aumento da velocidade média do escoamento e do número de Reynolds, os valores do Fator de Atrito (![CodeCogsEqn_f](https://user-images.githubusercontent.com/62161754/87112513-6963ce00-c242-11ea-87de-3ccd84d13fb1.gif)) decrescem, quando isto ocorre, a espessura da fina camada viscosa próxima à parede do tubo diminui. Sendo assim, os elementos de rugosidade (![CodeCogsEqn_E_rugosidade](https://user-images.githubusercontent.com/62161754/87112534-7680bd00-c242-11ea-8c25-6dd760907016.gif)) passam a emergir através desta camada, tornando o efeito da rugosidade relevante para estes casos. 

Como mencionado anteriormente, quando o escoamento passa a apresentar comportamento turbulento, o Fator de Atrito não depende mais apenas do Número de Reynolds, mas também da rugosidade. Observa-se que quando o valor da rugosidade absoluta aumenta, para o mesmo tubo circular com a área de secção transversal constante, o valor do Fator de Atrito também aumenta.

Ao analisar o efeito da mudança de material da tubulação nota-se que determinados tipos de material possuem valores de rugosidade elevados e consequentemente aumentam os efeitos do Fator de Atrito, assim como outros materiais possuem valores menos elevados e causam efeitos menores. Comparando os valores de rugosidade para tubulações do mesmo material porém, produzidas de maneira distinta, no caso o aço galvanizado, nota-se que o tubo com costura foi fabricado através da soldagem de uma chapa de metal. Desta maneira as extremidades foram unidas pelo calor e instrumentos de soldagem, e portanto, possui um valor de rugosidade maior, causando efeitos maiores no Fator de Atrito em regimes turbulentos. Um pouco diferente do tubo sem costura, o qual sua fabricação consiste na perfuração de um cilindro de metal aquecido, gerando uma rugosidade menor. Para o ferro fundido foi analisada a influência do tempo de uso da tubulação na rugosidade e no Fator de Atrito. Para uma tubulação mais velha a rugosidade tende a aumentar, o mesmo ocorre para o Fator de Atrito. Sendo assim, os resultados preliminares obtidos, para este estudo paramétrico, correspondem com a realidade física, apesar da caracterização do escoamento não ter sido adequada.

### Perfil de velocidade:

Ao considerar o escoamento como laminar, nota-se a diferença gráfica entre o perfil de velocidade obtido e o esperado. O perfil deve apresentar formato parabólico quando encontrado em regime laminar, no qual os maiores valores de velocidade encontram-se no centro do tubo e diminuem gradativamente ao aproximarem-se da parede da tubulação. A velocidade varia com o raio do tubo, essa variação de velocidade e a viscosidade do fluido resultam em uma tensão de cisalhamento na parede tubo. 

![perfil_velocidade_laminar_sist](https://user-images.githubusercontent.com/62161754/87111181-1c322d00-c23f-11ea-917c-7f19b7c63b12.png)

![perfil_velocidade_laminar_sist2](https://user-images.githubusercontent.com/62161754/87111183-1ccac380-c23f-11ea-820e-e23855ad75da.png)

O perfil de velocidade simulado apresenta formato próximo ao parabólico porém, mais achatado, não caracterizando um escoamento laminar. Com isto, a realização de uma nova simulação considerando o regime como turbulento pode ser útil para uma melhor análise deste parâmetro.

![CFD-Post_Chart2_Velocity](https://user-images.githubusercontent.com/62161754/87111197-23f1d180-c23f-11ea-81cb-271cfc051a73.png)


### Perda de carga:

Os valores de perda de carga (![CodeCogsEqn_hl](https://user-images.githubusercontent.com/62161754/87114354-bba6ee00-c246-11ea-8541-f60c20af5ca6.gif)
) simulados apresentaram os maiores erros percentuais em relação aos cálculos teóricos, ao compará-los com os demais parâmetros analisados. O escoamento laminar simulado não apresentou valores próximos aos valores calculados, adotando um comportamento não correspondente a realidade física do escoamento.

| Velocidade (m/s) | ![CodeCogsEqn_hl](https://user-images.githubusercontent.com/62161754/87109340-c3f92c00-c23a-11ea-86f3-8022ef4eeb87.gif) (Pa) teórico | ![CodeCogsEqn_hl](https://user-images.githubusercontent.com/62161754/87109340-c3f92c00-c23a-11ea-86f3-8022ef4eeb87.gif) (Pa) simulado  | Erro percentual |
|:--------------------:|:--------------------:|:-------------------------:|:--------------:|
| 0,0795 | 3,2530 | 1,8326 | 43,664% |


O gráfico apresenta um comportamento linear. Apesar dos valores teóricos e simulados terem apresentado diferença percentual elevada, a perda de carga simulada aproxima-se do valor medido através dos sensores de pressão na tubulação.

![CFD-Post_Chart1_Pressure](https://user-images.githubusercontent.com/62161754/87111209-28b68580-c23f-11ea-9b62-8fec0a50bf6d.png)

| ![CodeCogsEqn_hl](https://user-images.githubusercontent.com/62161754/87114354-bba6ee00-c246-11ea-8541-f60c20af5ca6.gif) medido (Pa)| ![CodeCogsEqn_hl](https://user-images.githubusercontent.com/62161754/87114354-bba6ee00-c246-11ea-8541-f60c20af5ca6.gif) simulado (Pa) | Erro percentual |
|:-------------------:|:----------------------:|:--------------------:|
| 2,0 | 1,8326 | 8,37% |



# 7. Referências:

MORAN , Michael J. et al. Introdução à engenharia de Sistemas Térmicos: Termodinâmica, Mecânica dos Fluidos e Transferência de Calor. Jonh Wiley & Sons, Inc. 2003.
 
FOX, Robert W. et al. Introdução á Mecânica dos Fluidos. 8ª ed. LTC, 2014.

WHITE, Frank M. Fluid Mechanics. 7ª ed. New York: McGraw-Hill, 2011.


