##**SIMULADOR DE INVESTIMENTOS EM FUNDOS DE INVESTIMENTOS IMOBILIÁRIOS (FIIs)**

Este projeto apresenta um simulador financeiro desenvolvido em Microsoft Excel, focado em auxiliar investidores iniciantes ou curiosos na análise e projeção de retorno de Fundos de Investimentos Imobiliários (FIIs). A ferramenta permite simular o desempenho de investimentos em FIIs, calculando rendimentos mensais, dividendos e o impacto de aportes recorrentes, fornecendo insights cruciais para a tomada de decisões, entre as quais “Qual impacto de investir mais dinheiro? ”.

##**OJBETIVO DO PROJETO**

O principal objetivo deste simulador é democratizar o acesso a análise financeira de FIIs para investidores com pouca ou nenhuma experiência. A ferramenta busca:

Simplificar Cálculos Financeiros 

Visualizar o Potencial de Retorno 

Auxiliar na Tomada de Decisão 

Responder a Perguntas Chaves  

##**COMO O SIMULADOR FUNCIONA (Etapas)**

O simulador é estruturado em diferentes etapas, guiando o investidor desde as configurações iniciais até as projeções de longo prazo e sugestões de alocações de forma intuitiva e eficaz.

**Etapa 1: Configurações Iniciais do Investidor**

Planilha dedicada à personalização dos parâmetros pessoais. Ela funciona como uma tabela de Dimensão. 
Aqui o investidor pode aportar seu salário caso assim desejar, o percentual de rendimento de carteira e sugestão de investimento mensal em relação ao salário em 30% para investir.

**Etapa 2: Simulador de Patrimônio**

Planilha principal do simulador, atuando como a Coluna Fato central do projeto. Aqui, os registros de entrada se transformam em projeções financeiras significativas. E nela, que as perguntas mais cruciais dos investidores são respondidas através de cálculos dinâmicos.

Quanto investir por mês? (Campo de entrada - Coluna Fato): Valor que pretende aportar mensalmente no investimento.

Por quanto Tempo? (Campo de entrada - Coluna Dimensão): Atributo que define a dimensão temporal do simulador. 

Taxa de Rendimento Mensal? (Campo de entrada como sugestão de 1,08% [alterável] – Coluna Dimensão): Atributo de dimensão crucial, pois impacta diretamente os cálculos de crescimento do patrimônio e dividendos.

Todos estes três Campos de entradas são dinâmicos, podem ser alterados conforme a necessidade do investidor.

Patrimônio Acumulado? (Coluna Calculada): Atributo gerado por uma fórmula que projeta o crescimento do Capital ao longo do tempo. 

Dividendos Mensais (Ganho Bruto – Coluna Calculada): Atributo que representa o ganho bruto mensal que o investidor receberia em dividendos.

Vale ressaltar que o Simulador Não apresenta cálculos de encargos, não considera impostos, taxas de corretagem, ou outras despesas financeiras associadas aos investimentos. Como também não considera variação do preço da cota. As projeções assumem uma taxa de rendimento mensal constante.

**Etapa 3: Simulador de Cenários e Projeção de Dividendos**

Esta planilha oferece uma visão estratégica ao investidor sobre o futuro do seu patrimônio e renda passiva, servindo como pontos de referência fixos para análise. 
As colunas calculadas ajudam a responder à pergunta: “E Se ___? ” em diferentes horizontes temporais.

Cenário de Tempo: Apresentam tempos pré-definidos como 2,5,10,20 e 30 anos. 

Patrimônio Acumulado por Cenário (Coluna Calculada): Projeta o valor de patrimônio por cada cenário, obtêm-se através da fórmula Valor Futuro do Excel (VF) que é ideal para esse tipo de projeção. O Valor Futuro (VF) calcula quanto um investimento valerá no futuro considerando o aporte e a taxa de juros.

Dividendos Relacionados por Cenários (Coluna Calculada): Projeta os dividendos mensais para cada cenário. Este é um registro que responde à pergunta do investidor: “Qual será minha renda passiva daqui a X anos? ”. 

**Etapa 4: Perfil do Investidor**

Nesta etapa o simulador se torna mais interativo e personalizado. 
Sugerindo alocações de investimento em diferentes Tipos de FIIs com base no perfil de risco do investidor.

Seleção do Perfil (Coluna Fato – Campo de Entrada): Através da ferramenta de dados – Validação de dados (Lista Suspensa), o investidor escolhe entre Conservador, Moderado e Agressivo. Este é um atributo de fato crucial, pois essa escolha influência diretamente o patrimônio.

Tipos de Fundos de Investimentos Imobiliários (FIIs) e Percentuais Sugeridos (Coluna Calculadas): Atributos de percentuais sugeridos para cada tipo de FII. Aqui a chave é a fórmula do PROCV (VLOOKUP), utilizada para buscar esses percentuais em uma tabela oculta, baseando-se no tipo de perfil escolhido.

Valores Calculados por Tipo de FII (Coluna Calculada): Calcula os valores em Reais a serem investidos em cada tipo de FII. 

Gráficos Demonstrativos

Gráfico tipo Pizza: Visualiza a distribuição percentual a serem investidos por tipo de FII.

Gráfico de Coluna: Apresenta os valores em reais a serem investidos por tipo de FII. 

##**DETALHES TÉCNICOS E RECURSOS DO EXCEL**

Este Simulador de Investimento apresenta a aplicação prática de diversas funcionalidades do Microsoft Excel, entre os quais:

Nomenclatura:
 Uso de Registros (Linhas) e Atributos (Colunas) para estruturar informações, diferenciando Colunas fato, onde dados mensuráveis como valores monetários são necessários, Colunas Dimensão, onde dados contextuais como períodos e perfis são necessários e Colunas Calculadas quando os valores derivados de fórmulas são necessários.

Fórmulas Estratégicas (uso):

Fixação de Células (F4 / $): garantem que importantes referências permaneçam estáticas ao manusear fórmulas, crucial para cálculos compostos.

Nomeação de Intervalos: Melhorar a legibilidade e a manutenção das fórmulas, exemplo – rendimento_carteira, utilizando a caixa de nome.

Valor Futuro (VF): fórmula essencial para projeções financeiras de longo prazo.
PROCV (VLOOKUP): permite a busca e associação dinâmica de dados, e permite a junção entre perfis e percentuais do FIIs.

Operador de Concatenação (&): permite unir textos e valores em fórmulas, criando mensagens dinâmicas para o usuário. 

Validação de Dados: implementada para controlar e restringir as entradas do usuário, garantindo a integridade dos cálculos, por exemplo, lista suspensa dos perfis de investidor.

Gráficos: transformam dados numéricos em insights visuais facilitando a compreensão, e tornando a análise mais acessível.

Formatação: Cor Cinza: utilizada de forma estratégica para indicar campos que são calculados automaticamente ou protegidos contra edições, guiando o usuário.

##**Como Usar**

Faça o download do arquivo .xlsx deste repositório

Abra o arquivo no Microsoft Excel

Navegue entre as abas

Preencha os campos em branco com seus dados e observe as projeções 

Experimente alterar os valores de entrada para simular diferentes cenários 

