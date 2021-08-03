# Detecção de fraude de transações
Um projeto de ciência de dados para prever se uma transação é uma fraude ou não.
![image](https://user-images.githubusercontent.com/82065728/128082588-65389cd4-e967-4837-bbc8-caae021a5812.png)
# 1.0 Problema de Negócio
A Blocker Fraud Company é uma empresa especializada em detectar fraudes em transações financeiras feitas por meio de dispositivos móveis. A empresa possui um serviço chamado "Fraude de Bloqueador" que garante o bloqueio de transações fraudulentas.
O modelo de negócio da empresa é do tipo De Serviço com a monetização feita pela realização do serviço prestado, ou seja, o usuário paga uma taxa fixa sobre o sucesso na detecção de fraudes nas transações do cliente.

No entanto, a Blocker Fraud Company está se expandindo no Brasil e, para adquirir clientes mais rapidamente, adotou uma estratégia muito agressiva. A estratégia funciona da seguinte forma:
 1.A empresa receberá 25% do valor de cada transação verdadeiramente detectada como fraude;
 2.A empresa receberá 5% do valor de cada transação detectada como fraude, mas a transação é verdadeiramente legítima.
 3.A empresa devolverá 100% do valor ao cliente, para cada transação detectada como legítima, porém a transação é realmente uma fraude.
 
 Com essa estratégia agressiva, a empresa assume os riscos de não detectar fraudes e é remunerada pela detecção assertiva de fraudes.
 
Para o cliente, é um excelente negócio contratar a Blocker Fraud Company. Embora a taxa cobrada seja muito alta no sucesso, 25%, a empresa reduz seus custos com transações fraudulentas detectadas corretamente e até mesmo os danos causados por um erro no serviço antifraude serão cobertos pela própria Blocker Fraud Company.
 
Para a empresa, além de conseguir muitos clientes com essa estratégia arriscada para garantir o reembolso em caso de falha na detecção de fraudes de clientes, depende apenas da precisão e precisão dos modelos construídos por seus Cientistas de Dados, ou seja, quanto mais preciso o modelo "Fraude de Bloqueador", maior a receita da empresa. No entanto, se o modelo tiver baixa precisão, a empresa pode ter uma grande perda.

# 2.0 Pressupostos Empresariais

Fraud prevention is the implementation of a strategy to detect fraudulent transactions or banking actions and prevent these actions from causing financial damage and the reputation of the client and the financial institution.

There are always financial frauds and They can happen through virtual and physical ways. So the investment in security has been increasing.

Os prejuízos causados pelas fraudes podem chegar a R$ 1 bilhão - o que corresponde à metade do valor que as instituições investem em sistemas tecnológicos voltados para a segurança da informação todos os anos, segundo a https://blog.simply.com.br/tecnologia-bancaria-2020/ .

# 3.0 Estratégia de Solução

Minha solução para resolver esse problema será o desenvolvimento de um projeto de ciência de dados. Este projeto terá um modelo de aprendizado de máquina que pode prever se uma transação é fraudulenta ou não.

Passo 01. Descrição dos dados: Nesta primeira seção os dados serão coletados e estudados. Os valores perdidos serão ameaçados ou removidos. Finalmente, uma descrição inicial dos dados será realizada para saber os dados. Portanto, alguns cálculos de estatísticas descritivas serão feitos, como kurtose, distorção, mídia, moda, mediana e desviação padrão.

Passo 02. Engenharia de Características: Nesta seção, será criado um mapa mental para auxiliar a criação da hipótese e a criação de novos recursos. Essas suposições ajudarão na análise exploratória de dados e podem melhorar os escores do modelo.

Passo 03. Filtragem de dados: A filtragem de dados é usada para remover colunas ou linhas que não fazem parte do negócio. Por exemplo, colunas com ID do cliente, código hash ou linhas com idade que não consistem na idade humana.

Passo 04. Análise exploratória de dados: A seção de análise exploratória de dados consiste em análise univariada, análise bivariada e análise multivariada para auxiliar na compreensão da base de dados. A hipótese criada na etapa 02 será testada na análise bivariada.

Passo 05. Preparação de dados: Nesta quinta seção, os dados serão preparados para modelagem de machine learning. Portanto, eles serão transformados para melhorar o aprendizado do modelo de aprendizagem de máquina, assim eles podem ser codificados, superamostrados, subamostrados ou redimensionados.

Passo 07. Modelagem de Machine Learning: Passo 07 visa treinar os algoritmos de aprendizagem de máquina e como eles podem prever os dados. Para validação o modelo é treinado, validado e aplicado à validação cruzada para saber a capacidade de aprendizagem do modelo.

Passo 08. Ajuste fino do hyparameter: Em primeiro lugar, selecionou o melhor modelo a ser aplicado no projeto, é importante fazer um ajuste fino dos parâmetros para melhorar suas pontuações. Os mesmos métodos de desempenho do modelo na etapa 07 são usados.

Passo 09. Conclusões: Esta é uma fase de conclusão que o modelo de capacidade de geração é testado usando dados invisíveis. Além disso, algumas perguntas de negócios são respondidas para mostrar a aplicabilidade do modelo no contexto empresarial.

Passo 10. Model Deploy: Esta é a etapa final do projeto de ciência de dados. Então, nesta etapa o flask api é criado e o modelo e as funções são salvos para serem implementados na api.

# 4.0 Top 3 Data Insights

* Todo o valor da fraude é maior que 10.000.
# Verdade: Os valores são superiores a 10.000. Mas é importante notar que os valores sem fraude também são superiores a 100.000.
