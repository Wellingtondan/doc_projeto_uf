# Documentação - Importação novas bases UFs

## 1. Criação das capas dos estados ainda não atendidos

Iniciamos esse novo projeto no dia 01/03/2024, com base na tabela de capas do Serve Bem (RJ) foram criadas as capas dos estados do quadro abaixo: 

|***ESTADO***  |***UF*** | ***IMPORTADO*** | 
| ----------| --------------| ----------|
| ACRE | AC | **SIM** |
| ALAGOAS | AL | **NÃO** |
| AMAZONAS | AM | **NÃO** |
| AMAPÁ | AP | **SIM** |
| MATO GROSSO DO SUL | MS | **SIM** |
| PARÁ | PA | **NÃO** |
| PARAÍBA | PB | **SIM** |
| PIAUÍ | PI | **SIM** |
| RONDÔNIA | RO | **NÃO** |
| TOCANTINS | TO | **NÃO** |

- Totalizando a soma de 5 tabelas de capas importadas em nosso banco, isso se da por conta de tratar os dados conforme são identificados os benefícios de Cesta básica, Isenção, Redução específica, etc.

- Após essa coleta de dados as capas são montadas e identificadas com as numerações para criação da grade UF do estado.

**As capas de tributações importadas:** `AC, AP, MS, PB e PI.`

### 2. Grade de tributações desenvolvidas e importadas

Após o desenvolvimento das capas de tributações dos estados de AC, AP, MS, PB e PI, foram estruturadas as grades de tributações por UF e importadas no banco de dados.

`Observação:` Das capas que ```NÃO``` foram importadas ao banco conforme citadas no quadro acima, já foram coletadas todas as NCM e CEST com previsão de ST, faltando verificar quais serão utilizadas como capas, quais são as alíquotas, quais as MVAs e quais os benefícios fiscais, e assim dar andamento ao próximo estado.

> [!IMPORTANT]
> As bases de PB e PI não foram encontradas tributações ST com reduções de cesta básica, dessa forma contêm um número menor de tributações para essas bases!

**Observação:** AP e PI foram montadas tributações dos segmentos `Cervejas, chopes, refrigerantes, águas e outras bebidas` considerando o MVA para `Indústria / Importador` ou `Distribuidor / depósito / estabelecimento atacadista`, assim também para ***TO*** quando for desenvolvida a base.

>![image](https://github.com/Wellingtondan/doc_projeto_uf/assets/119419112/d65a1dc7-a1fc-4976-9a57-b8c2eff26a23)

> [!NOTE]
> - Para criar a grade de tributação foi utilizada a ferramenta Power Query para duplicar o número de tributação para cada UF;
> 
> - Com a ferramenta aberta, adicione uma nova coluna em "Adicionar Coluna - Coluna Personalizada" e insere o comando "= {"AC", "AL", "AM", "AP", "BA", "CE", "DF", "ES", "EX", "GO", "MA", "MG", "MS", "MT", "PA", "PB", "PE", "PI", "PR", "RJ", "RN", "RO", "RR", "RS", "SC", "SE", "SP", "TO"}";
> 
> - E para duplicar as UFs para os tipos de tributações foi utilizado esse comando para inserir "= {"EI", "ED", "EM", "SC", "SN"}".

## 3. Base de tributações importadas de clientes

|***CLIENTE***  |***UF*** | ***ESTADO*** | ***CONFERÊNCIA***|
| ----------| --------------| --------------| --------------|
| BIG BOX | BA | BAHIA | **CONFERIDO** | 
| DE ANGELINA | SC | SANTA CATARINA | **REVISAR** |
| DELMORO | MT | MATO GROSSO | **REVISAR** |
| BIG BOX | DF | DISTRITO FEDERAL | **CONFERIDO** |
| BIG BOX | GO | GOIÁS | **CONFERIDO** |
| BONANZA | PE | PERNAMBUCO | **CONFERIDO** |
| DIFAL | PR | PARANÁ | **REVISAR** |
| SERVE BEM | RJ | RIO DE JANEIRO | **CONFERIDO** |
| BOM PREÇO | RN | RIO GRANDE DO NORTE | **CONFERIDO** |
| COQUEIROS | RS | RIO GRANDE DO SUL | **CONFERIDO** |
| FONSECA | SP | SÃO PAULO | **FINALIZAR** |

- Faltando exportar MG (Fonseca), assim que extraída do cliente irei tratar os dados e importar em nosso banco.
- Totalizando a soma de 12 UFs de clientes em nosso banco.

> [!IMPORTANT]
> Para finalizar a base de tributação de SP, será necessário clonar os dados da Aba Indústria para a Aba distrbuidor, e considerar para a aba Micro empresa o MVA Original nas linhas interestaduais e para a resolução 13, e realizar uma conferência das CST Entrada/Saída para finalizar!
> 
> Não foi finalizada devido o início do desenvolvimento das novas bases para esse projeto, priorizei as novas bases, e assim que possível farei a atualização!

## 4. Total de bases

Com a importação de 12 bases de tributação de clientes e o desenvolvimento de 5 novas bases, alcançamos até o momento um total de 17 bases de Unidades Federativas (UFs).

## 5. conclusão

Como temos um tempo de análise para os projetos tributários (Sofia), a estrutura da base de tributação contratada terá um período de validação dos dados informados na grade para conferência pelos analistas. Sendo assim, desenvolvi as capas ST com combinações de NCM e CEST, abrangendo os segmentos principais utilizados pelos nossos clientes. Baseando-me no cliente Serve Bem, por outro lado, foi necessário adicionar em alguns estados outras tributações, como a de "Carne", devido o alcance da Substituição Tributária (ST).

```Questionamentos para analisarmos em reunião```

- Como serão feitas as conferências dos estados não atendidos?

- E quanto às atualizações? Faremos em intervalos regulares? Mensal, trimestral, semestral ou anualmente? Ou apenas quando forem contratados novos serviços tributários?

6. Relatório (Sofia)



