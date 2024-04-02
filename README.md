# Documentação - Importe Bases UFs

### 1. Criação das capas de estados não atendidos

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
>>As bases de PB e PI não foram encontradas tributações com reduções de cesta básica, sendo um número menor de tributações!

**Observação:** PI foram montadas tributações de bebidas frias considerando o MVA para Indústria ou Distribuidor, assim também para ***TO*** quando for montada a base.

### 2. Base de tributações importadas de clientes

|***CLIENTE***  |***UF*** | 
| ----------| --------------|
| Meira | BA | 
| Big Box | DF | 
| Big Box | GO |
| Delmoro | MT | 
| Bonanza | PE | 
| Difal | MT | 
| Serve Bem | RJ | 
| Bom Preço | RN | 
| De Angelina | SC | 

**Bases importadas de clientes:** BA (Meira), DF (Big Box), GO (Bog Box), MT (Delmoro), PE (Bonanza), PR (Difal), RJ (Serve Bem), RN (Bom Preço) e SC (De Angelina).

Faltando exportar MG (Fonseca) e RS (Coqueiros) para serem importados em nosso banco.

Para finalizar a base de tributação de SP, será necessário clonar os dados da Aba Indústria para a Aba distrbuidor, e considerar para a aba MIcro empresa o MVA Original nas linhas interestaduais e para a resolução 13, e realizar uma conferência das CST Entrada/Saída para finalizar!

