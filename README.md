## 📊 Simulador de Investimentos em Fundos Imobiliários (FIIs)


Este projeto apresenta um simulador financeiro desenvolvido em Microsoft Excel, focado em auxiliar investidores iniciantes ou curiosos na análise e projeção de retorno de Fundos de Investimentos Imobiliários (FIIs). A ferramenta permite simular o desempenho de investimentos em FIIs, calculando rendimentos mensais, dividendos e o impacto de aportes recorrentes, fornecendo insights cruciais para a tomada de decisões, entre as quais *Qual impacto de investir mais dinheiro?.*

## 🎯 Objetivo do Projeto
O principal objetivo deste simulador é democratizar o acesso à análise financeira de FIIs, mesmo para quem tem pouca ou nenhuma experiência.
A ferramenta busca:
-	✅ **Simplificar cálculos financeiros;**
-	✅ **Visualizar o potencial de retorno;**
-	✅ **Auxiliar na tomada de decisão;**
-	✅ **Responder a perguntas-chave**, como: *Qual o rendimento do meu investimento?*

###
<!--etapas de funcionamento-->
## ⚙️ Como o Simulador Funciona (Etapas)
### Etapa 1: Configurações Iniciais do Investidor
-	Planilha dedicada à personalização dos parâmetros pessoais
-	Permite incluir salário, taxa de rendimento e percentual do salário para investimento (sugestão: 30%)
-	Funciona como uma tabela de dimensão

###

### Etapa 2: Simulador de Patrimônio
-	Quanto investir por mês? (Campo de entrada - Coluna Fato)
-	Por quanto tempo? (Campo de entrada - Coluna Dimensão)
-	Taxa de rendimento mensal? (Sugestão: 1,08%, alterável - Coluna Dimensão)
-	Patrimônio acumulado? (Coluna Calculada)
-	Dividendos mensais? (Coluna Calculada)
ℹ️ *O simulador não considera **impostos**, **taxas de corretagem** ou **variação no preço da cota**. Assume uma taxa de rendimento constante.*

###

### Etapa 3: Simulador de Cenários e Projeção de Dividendos
-	Cenário de Tempo: 2, 5, 10, 20 e 30 anos
-	Patrimônio acumulado por cenário: Calculado com a fórmula VF (Valor Futuro)
-	Dividendos relacionados por cenário: Responde à pergunta “Qual será minha renda passiva daqui a X anos?”

###

### Etapa 4: Perfil do Investidor
-	Seleção do perfil: Conservador, Moderado ou Agressivo
-	Tipos de FIIs e percentuais sugeridos: Utiliza PROCV (VLOOKUP)
-	Valores calculados por tipo de FII
-	Gráficos Demonstrativos:
-	📈 Gráfico de Coluna: Valores em R$
-	🥧 Gráfico de Pizza: Distribuição percentual

###
<!--detalhes-->
## 🛠️ Detalhes Técnicos e Recursos do Excel
-	Colunas Fato / Dimensão / Calculadas
-	Fixação de Células (F4)
-	Nomeação de Intervalos
-	Funções: VF, PROCV, concatenação &
-	Validação de Dados (listas suspensas)
-	Gráficos ilustrativos
-	Formatação condicional (campos cinza = cálculo automático)

###

<!--como usar-->
## ▶️ Como Usar
- 1.	Faça o download do arquivo .xlsx deste repositório
- 2.	Abra o arquivo no Microsoft Excel
- 3.	Navegue entre as abas
- 4.	Preencha os campos em branco com seus dados
- 5.	Observe as projeções automaticamente
- 6.	Experimente diferentes cenários alterando os valores de entrada

###
<!--contribuições-->
## 🤝 Contribuições
Contribuições são bem-vindas!
Se você tiver ideias de melhoria, correções ou deseja expandir a funcionalidade, sinta-se à vontade para abrir uma issue ou enviar um *pull request.*

###
<!--Licença MIT-->

## 📄 Licença
Este projeto está licenciado sob os termos da **Licença MIT**.
Consulte o arquivo LICENSE para mais informações.


