# ciencia-de-dados

## Trabalho de Ciência de Dados

Este repositório contém o processo de **limpeza e preparação de dados** para o e-commerce fictício **MegaSuper Vendas**, que enfrentava desafios significativos com dados desorganizados e inconsistentes. O objetivo é transformar esses dados em um formato estruturado e confiável para análises posteriores.

---

## 📊 Descrição do Projeto

A base de dados original do projeto apresenta diversos problemas, incluindo:

- Dados faltantes em colunas essenciais;
- Nomes de produtos despadronizados e inconsistentes;
- Cálculos incorretos no campo **"Total"**;
- Registros duplicados;
- CEPs e estados inválidos;
- Tipos de dados incorretos em várias colunas.

Este projeto aborda essas questões de forma sistemática, realizando a **limpeza, padronização e validação** dos dados, deixando o DataFrame pronto para análises mais avançadas.

---

## ⚙️ Tecnologias Utilizadas

- **Python 3.10+**
- **pandas** – Manipulação e limpeza dos dados
- **numpy** – Operações numéricas e arrays
- **datetime** – Conversão e formatação de datas
- **os** – Manipulação de arquivos e diretórios
- **Git e GitHub** – Versionamento e colaboração

---

## 🧪 Etapas de Limpeza

### 🔹 Leitura e Preparação Inicial
- Leitura do arquivo `.csv` com encoding **UTF-8**
- Renomeação das colunas para o formato `snake_case`

### 🔹 Tratamento de Dados Faltantes
- Substituição de valores ausentes (NaN) por padrões como `0` ou `"desconhecido"`
- Conversão de colunas de data/hora para formatos consistentes

### 🔹 Padronização de Dados
- Normalização de textos para letras minúsculas
- Padronização de nomes de produtos com expressões regulares
- Formatação e validação de CEPs

### 🔹 Validação e Correção de Cálculos
- Recalcular a coluna **Total** com base em `valor * quantidade + frete`
- Remoção de registros com valores inválidos

### 🔹 Remoção de Duplicatas
- Identificação e exclusão de registros duplicados
- Reset de índices para manter integridade

### 🔹 Geração de Relatório
- Impressão de um relatório final com estatísticas do processo de limpeza no console

---

## ✅ Resultado Esperado

Ao final do processo, espera-se um conjunto de dados limpo, estruturado e confiável. O DataFrame estará livre de erros como dados faltantes, duplicações e formatações inconsistentes — pronto para ser utilizado em análises exploratórias, visualizações e construção de modelos preditivos.
