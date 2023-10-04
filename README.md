# Análise exploratória: série temporal dos dados de postagem dos Correios para o estado do RJ

**Projeto - Estatística I**
Instrutor: Felipe Yoshimoto
**Equipe: Gabriel Miranda, Marcus Thadeu, Ruann Campos e Thiago Caveglion**

# Objetivo geral
Analisar, de forma exploratória, os dados referente à série temporal de postagens de uma agência dos Correios do estado do Rio de Janeiro (2023-01 a 2023-09).

# Objetivos específicos
No desenvolvimento de nossa análise, buscamos responder às seguintes perguntas:
* Qual a distribuição dos valores de postagem por estado?
* Qual o ticket médio por cliente?
* Qual o ticket médio tipo de serviço?
* Qual a distribuição de postagem por mês e dia?
* O valor das postagens é maior na Segunda-feira?
* A média de postagens na Segunda-Feira é significativamente diferente da média de postagens no restante da semana?
* O valor médio do número de postagens mais baratas que 20 reais é significativamente diferente do valor médio do número de postagens mais caras que 20 reais?
* A média de postagens nos primeiros 15 dias é significativamente diferente da média de postagens no restante do mês?
* Qual a distribuição do número de postagens por estado?
* Percentualmente, o quão varia o número de postagens entre os estados do sudeste?
* Como se caracteriza a distribuição de valores de postagem para os estados da região sudeste?
* A média de valor dos pacotes enviados para dentro do estado do RJ é igual à média dos pacotes enviados para outros estados do Brasil?
* A média de valor dos pacotes enviados para dentro do estado do RJ é igual à média dos pacotes enviados para outros estados do Sudeste?
* A média de valor dos pacotes enviados para o ES é igual à média dos pacotes enviados para SP?
* Como se configura a distribuição de valor médio de envio por região?
* Valor médio de envio da região Norte é igual ao valor médio de envio da região Nordeste?
* E para as outras regiões? A região Norte apresenta um valor médio igual ao valor médio das outras regiões?
* O valor médio de envio da região Centro-Oeste é igual ao valor médio de envio da região Sul?
* Qual a distribuição da quantidade de envios por região?

# Execução
Para executar o notebook localmente, certifique-se de, logo no início do arquivo `analise-exploratoria-correios-rj.ipynb`, alterar a seguinte linha de código: `df = pd.read_parquet("caminho")`.
* O argumento da função `read_parquet()` deve conter o caminho para o arquivo referente ao nosso dataset (`operations_base.parquet`).
