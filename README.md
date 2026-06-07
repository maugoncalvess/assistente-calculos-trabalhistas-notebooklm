# assistente-calculos-trabalhistas-notebooklm
Assistente para Cálculos Trabalhistas

------------------------ CONTEXTO E OBJETIVOS ------------------------

Diante da necessidade e exigência por partes do Tribunais em estimar os valores que são devidos numa eventual reclamação trabalhista, bem como os altos custos perito ou contador judicial, 
este projeto de NotebookLM foi criado para auxiliar o advogado na realização de cálculos trabalhistas para conseguir liquidar o valor das verbas rescisórias que serão pleiteadas em uma petição inicial trabalhista.

------------------------ FONTES -----------------------------

o projeto foi alimentado com manuais, guias e decisões relevantes no âmbito da jurisprudência trabalhista, observando a boa prática forense. Foram utilizadas as seguintes fontes:

 1) Guia de cálculos trabalhistas [recurso eletrônico] : entenda e esteja em Compliance com o eSocial e a Fiscalização / editorial Equipe Técnica IOB. – São Paulo : IOB, 2020. 1867 Kb ; PDF.
 2) Apostila de Cálculos Trabalhistas - COORDENAÇÃO DO CURSO DE DIREITO PROFESSOR: Eduardo Antônio Dória de Carvalho
 3) Rocha, Gisele Mariano da Cálculos trabalhistas para rotinas, liquidação de sentenças e atualização de débitos judiciais / Gisele Mariano da Rocha. – 5ª ed. rev. atual. Porto Alegre: Livraria do Advogado Editora, 2014. 150 p.; 21 cm. ISBN 978-85-7350-152-0
 4)  7.ed. Santos, José Aparecido dos Estrutura e desenvolvimento dos cálculos / José Aparecido dos Santos. - 7.ed. - Curitiba
 5)  https://www.jota.info/trabalho/nova-decisao-de-moraes-impede-condenacao-trabalhista-acima-do-valor-pedido-na-inicial

----------------------------- ENGENHARIA DE PROMPT -------------------------------

para que o modelo responda de forma assertiva, é necessário que o comando dado pelo advogado traga as informações mais importantes de acordo com o caso. Por exemplo, no prompt utilizado abaixo
a hipótese versava sobre um caso de um empregado exposto a periculosidade e acumulo de função em seu trabalho e que pleitearia o referido adicional na Justiça. 
Para isso, o modelo deverá apresentar o valor devido para acrescentar nos pedidos:

Exemplo de Prompt Utilizado:

"Faça o cálculo de acordo com o seguinte caso: O funcionário laborou no período de 13/03/2023 a 11/03/2025. Seu último salário de acordo com o TRCT era de R$ 2.043,40. 
Ele acumulou funções durante todo o período contratual. Além disso, não recebeu a periculosidade durante o período em que ficou exposto ao risco, isto é, de Dezembro/2023 a Março/2025, bem como 21 dias sem período específico. 
Com base na legislação trabalhista brasileira, elabore os cálculos acerca da diferença salarial de quanto o cliente deve receber em razão do acumulo (utilizar percentual de 40%) e da periculosidade (utilizar percentual de 30%). 
Não deixe de indicar os reflexos nas demais verbas. Por fim, deverá apresentar memória de cálculo para analisar se o resultado está correto."

A resposta trazida pelo Modelo foi a seguinte:

"Para elaborar os cálculos solicitados com base nas fontes e na legislação trabalhista, consideraremos o funcionário como mensalista, utilizando o divisor de 30 dias para valores diários e a jornada padrão de 220 horas mensais
.
1. Parâmetros e Bases de Cálculo
Período Contratual: 13/03/2023 a 11/03/2025 (23 meses e 29 dias).
Último Salário Base: R$ 2.043,40.
Adicional de Acúmulo de Função (40%): R$ 817,36 mensais
.
Adicional de Periculosidade (30%): R$ 613,02 mensais (incidente sobre o salário básico)
.

--------------------------------------------------------------------------------
2. Memória de Cálculo: Verbas Principais (Diferenças)
A. Diferença por Acúmulo de Função (40%)
O funcionário acumulou funções durante todo o contrato (23 meses e 29 dias).
Meses Integrais (23 meses): 23 x R817,36=∗∗R 18.799,28**
Proporcional Março/2023 (18 dias): (R817,36÷30)x18=∗∗R 490,42**
Proporcional Março/2025 (11 dias): (R817,36÷30)x11=∗∗R 299,70**
Subtotal Acúmulo: R$ 19.589,40
B. Adicional de Periculosidade (30%)
Devido de Dezembro/2023 a Março/2025, mais 21 dias avulsos.
Meses Integrais (Dez/23 a Fev/25 = 15 meses): 15 x R613,02=∗∗R 9.195,30**
Proporcional Março/2025 (11 dias): (R613,02÷30)x11=∗∗R 224,77**
Dias Avulsos (21 dias): (R613,02÷30)x21=∗∗R 429,11**
Subtotal Periculosidade: R$ 9.849,18

--------------------------------------------------------------------------------
3. Reflexos nas Demais Verbas
Os adicionais de acúmulo e periculosidade possuem natureza salarial e devem refletir nas demais verbas
.
13º Salário Proporcional
Reflexo do Acúmulo (24/12 avos totais): R817,36x2anos=∗∗R 1.634,72**
Reflexo da Periculosidade:
2023 (1/12 - Dezembro): R$ 51,08
2024 (12/12): R$ 613,02
2025 (2/12 - Jan e Fev): R$ 102,17
Obs: Março/25 não conta como avo pois teve menos de 15 dias
.
Férias + 1/3 Constitucional
1º Período (2023/2024 - Vencidas):
Reflexo Acúmulo: R817,36+1/3(R 272,45) = R$ 1.089,81
Reflexo Periculosidade (prop. 3/12 de exposição): (R613,02÷4)+1/3=∗∗R 204,34**
2º Período (2024/2025 - Proporcionais 12/12):
Reflexo Acúmulo: R817,36+1/3=∗∗R 1.089,81**
Reflexo Periculosidade: R613,02+1/3=∗∗R 817,36**
Obs: Pela projeção do aviso prévio, completa-se o 12º mês de férias
.
Aviso Prévio Indenizado (33 dias)
O funcionário trabalhou quase 2 anos, fazendo jus a 33 dias de aviso
.
Reflexo Acúmulo: (R817,36÷30)x33=∗∗R 899,10**
Reflexo Periculosidade: (R613,02÷30)x33=∗∗R 674,32**
FGTS (8%) e Multa Rescisória (40%)
O FGTS incide sobre todas as diferenças salariais e reflexos (exceto férias indenizadas)
.
Base de Cálculo Estimada (Diferenças + Reflexos salariais): R$ 33.734,12
FGTS (8%): R$ 2.698,73
Multa de 40% sobre o FGTS: R$ 1.079,49

--------------------------------------------------------------------------------
4. Resumo Geral dos Valores Devidos
Descrição da Verba
Valor Principal
Reflexos Estimados
Acúmulo de Função (40%)
R$ 19.589,40
R$ 4.713,44
Adicional Periculosidade (30%)
R$ 9.849,18
R$ 2.462,16
FGTS + Multa 40%
-
R$ 3.778,22
TOTAL ESTIMADO
R$ 29.438,58
R$ 10.953,82
Valor Bruto Total a Receber: R$ 40.392,40
Nota: Estes cálculos são estimativos com base nas informações fornecidas.
Valores exatos podem variar dependendo do fechamento da folha de cada mês e de possíveis faltas ou convenções coletivas específicas não citadas."

------------------------ CONCLUSÃO/AVALIAÇÃO GERAL ------------------------------------------

O modelo seguiu corretamente a metodologia de cálculo usada comumente na prática forense, entretanto, em uma eventual contestação acerca dos valores é necessário que o advogado realize a revisão ou alimente
com mais fontes daquele tribunal em específico, uma vez que a metologia de cálculo utilizada pelos tribunais podem divergir em alguns pontos. Entretanto, de maneira geral, o modelo mostrou-se um excelente 
assistente na liquidação dos pedidos, o que diminui consideravelmente a margem de erro e eventual impugnação.

