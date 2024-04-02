# Documentação - Importação novas bases UFs

## 1. Criação das capas de estados não atendidos

Iniciamos esse novo projeto no dia 04/03/2024, com base na tabela de capas do Serve Bem (RJ) foram criadas as capas dos estados do quadro abaixo: 

|***ESTADO***  |***UF*** | ***IMPORTADO*** | 
| ----------| --------------| ----------|
| ACRE | AC | IMPORTADO |
| ALAGOAS | AL | TRATAR DADOS |
| AMAZONAS | AM | TRATAR DADOS |
| AMAPÁ | AP | IMPORTADO |
| MATO GROSSO DO SUL | MS | IMPORTADO |
| PARÁ | PA | TRATAR DADOS |
| PARAÍBA | PB | IMPORTADO |
| PIAUÍ | PI | IMPORTADO |
| RONDÔNIA | RO | TRATAR DADOS |
| TOCANTINS | TO | TRATAR DADOS |

- Totalizando a soma de 5 tabelas de capas importadas em nosso banco, isso se da por conta de tratar os dados conforme são identificados os benefícios de Cesta básica, Isenção, Redução específica, etc.

- Após essa coleta de dados as capas são montadas e identificadas com as numerações para criação da grade UF do estado.

**As capas de tributações importadas:** `AC, AP, MS, PB e PI.`

### 2. Grade de tributações desenvolvidas e importadas

Após o desenvolvimento das capas de tributações dos estados de AC, MS, PB, PI e MS, foram estruturadas as grades de tributações por UF e importadas no banco de dados.

Esta em andamento a grade de tributação de AP, assim que finalizado, será importada a grade ao banco.

> [!IMPORTANT]
> As bases de PB e PI não foram encontradas tributações com reduções de cesta básica, sendo um número menor de tributações!

**Observação:** AP e PI foram montadas tributações de bebidas frias considerando o MVA para `Indústria / Importador` ou `Distribuidor / depósito / estabelecimento atacadista`, assim também para ***TO*** quando for desenvolvida a base.

>![image](https://github.com/Wellingtondan/doc_projeto_uf/assets/119419112/d65a1dc7-a1fc-4976-9a57-b8c2eff26a23)

## 3. Base de tributações importadas de clientes

|***CLIENTE***  |***UF*** | 
| ----------| --------------|
| Meira | BA | 
| Big Box | DF | 
| Big Box | GO |
| Delmoro | MT | 
| Bonanza | PE | 
| Difal | PR | 
| Serve Bem | RJ | 
| Bom Preço | RN | 
| De Angelina | SC |
| Fonseca | SP |

- Faltando exportar MG (Fonseca) e RS (Coqueiros) para serem tratados os dados e importados em nosso banco.
- Totalizando a soma de 12 UFs de clientes em nosso banco.

> [!IMPORTANT]
> Para finalizar a base de tributação de SP, será necessário clonar os dados da Aba Indústria para a Aba distrbuidor, e considerar para a aba MIcro empresa o MVA Original nas linhas interestaduais e para a resolução 13, e realizar uma conferência das CST Entrada/Saída para finalizar!

## 4. Total de bases

Com a importação de 12 bases de tributação de clientes e o desenvolvimento de 5 novas bases, alcançamos até o momento um total de 17 bases de Unidades Federativas (UFs).

## 5. conclusão

Como temos um tempo de análise para os projetos tributários (Sofia), a estrutura da base de tributação contratada terá um período de validação dos dados informados na grade para conferência pelos analistas. Sendo assim, desenvolvi as capas ST com combinações de NCM e CEST, abrangendo os segmentos principais utilizados pelos nossos clientes. Baseando-me no cliente Serve Bem, por outro lado, foi necessário adicionar em alguns estados outras tributações, como a de "Carne", devido ter o alcance da Substituição Tributária (ST).

```Questionamentos para analisarmos em reunião```

Como serão feitas as conferências dos estados não atendidos?

E quanto às atualizações? Faremos em intervalos regulares? Mensal, trimestral, semestral ou anualmente? Ou apenas quando forem contratados novos serviços tributários?




