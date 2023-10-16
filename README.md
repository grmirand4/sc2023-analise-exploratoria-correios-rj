# [Análise exploratória: série temporal dos dados de postagem de uma empresa de logística do estado do RJ](https://github.com/grmirand4/sc2023-analise-exploratoria-logistica-rj)

**Projeto - Estatística I**

Instrutor: Felipe Yoshimoto

**Equipe: [Gabriel Miranda](https://www.linkedin.com/in/grmiranda/), [Marcus Thadeu](https://www.linkedin.com/in/marcus-thadeu/), [Ruann Campos](https://www.linkedin.com/in/ruann-campos/) e [Thiago Caveglion](https://www.linkedin.com/in/thiago-caveglion/)**

## 🎯 Objetivo geral
Analisar, de forma exploratória, os dados referentes à série temporal de postagens de uma empresa de logística do estado do Rio de Janeiro (2023-01 a 2023-09).

## 📊 Sobre o data set

O data set `operations_base.parquet` contém informações de pacotes que foram enviados por uma agência de logística localizada na cidade do Rio de Janeiro (RJ). Em nosso recorte, os envios ocorreram entre os meses de Janeiro e Setembro de 2023. As colunas do arquivo incluem:
* `Data`: data de postagem do pacote;
* `Objeto`: código de rastreamento;
* `CEP`: CEP do destino;
* `Serviço`: tipo de serviço (expresso ou econômico);
* `Valor`: valor da postagem (em reais);
* `Cliente`: nome do cliente;
* `Postagem`: tipo de postagem;
* `Destino`: cidade de destino;
* `UF`: estado de destino.

## 📝 Perguntas de negócio
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

## 💡 Principais conclusões
* Rondônia é o estado com o maior valor de ticket médio (R$ 77,16).
* Enquanto o cliente Mesbla possui o menor valor de ticket médio (R$ 11,76), o cliente Arapuã está no extremo oposto (R$ 42,98).
* O serviço expresso possui um ticket médio de R$ 21,56 enquanto o do serviço econômico está definido em R$ 25,42.
* Observa-se um pico de envio de postagens nos meses de Julho e Agosto.
* Considerando os dias do mês, o pico de postagem ocorre no dia 13.
* A quantidade total de produtos despachados é maior na segunda-feira.
* A maior parte dos produtos despachados custa menos de 20 reais.
* A maior parte dos produtos despachados dessa agência de logística vai para o próprio estado do RJ (49% das postagens totais). Logo após, temos os estados da região sudeste (MG, ES e SP, respectivamente).
* O valor médio de envio para a região norte é superior à todas as outras regiões.
* A região sul é a que menos recebe pacotes dessa agência de logística.

## 👨‍💻 Execução
Para executar o notebook localmente, certifique-se de, logo no início do arquivo `analise-exploratoria-logistica-rj.ipynb`, alterar a seguinte linha de código: `df = pd.read_parquet("caminho")`.
* O argumento da função `read_parquet()` deve conter o caminho para o arquivo referente ao nosso data set (`operations_base.parquet`).

## 💻 Principais linguagens
- Python
  - Pandas
  - Numpy
  - OS
  - Locale
  - Plotly
  - Matplotlib
  - Scipy

###### Tags: `python` `data-science` `logistica` `ciencia-de-dados` `analise-exploratoria`
