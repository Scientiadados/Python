# 📊 Notebook: Comandos Básicos do Pandas

Este notebook contém uma coleção de comandos essenciais do **Pandas** para manipulação e análise de dados. É um guia prático que cobre desde operações básicas até transformações mais avançadas.

## 📋 Conteúdo

O notebook está organizado nas seguintes seções:

### 1️⃣ Inspeção Inicial
Comandos fundamentais para entender seus dados:
- `head()` - Primeiras linhas
- `tail()` - Últimas linhas
- `shape` - Dimensões do DataFrame
- `columns` - Nomes das colunas
- `info()` - Informações sobre tipos e valores nulos
- `describe()` - Estatísticas descritivas

### 2️⃣ Seleção de Colunas
Como selecionar colunas específicas:
- Seleção de uma coluna
- Seleção de múltiplas colunas
- Seleção usando variáveis

### 4️⃣ Filtros
Filtragem de dados com condições:
- Filtros simples (`>`, `<`, `==`)
- Filtros compostos (`&`, `|`)
- Filtros com `isin()`

### 5️⃣ Criando Colunas Novas
Transformações e criação de novas colunas:
- Operações matemáticas
- Extração de componentes de data (ano, mês)
- Conversão de tipos de data

### 6️⃣ Alterando Valores
Modificação de valores existentes:
- Transformação de strings (`.str.upper()`)
- Atualização condicional com `loc`

### 7️⃣ Ordenação
Ordenação de dados:
- `sort_values()` - Ordenação crescente
- `sort_values(ascending=False)` - Ordenação decrescente

### 8️⃣ Agrupamentos (groupby)
Agregações e análises por grupos:
- Soma por grupo
- Múltiplas agregações com `.agg()`

### 🔟 Valores Nulos
Tratamento de dados faltantes:
- `isna().sum()` - Contagem de valores nulos
- `fillna()` - Preenchimento de valores nulos
- `dropna()` - Remoção de linhas com valores nulos

### 1️⃣1️⃣ Conversão de Tipos
Conversão entre tipos de dados:
- `pd.to_datetime()` - Conversão para data
- `.astype()` - Conversão de tipos numéricos

### 1️⃣2️⃣ Renomear Colunas
Renomeação de colunas com `rename()`

### 1️⃣3️⃣ Exportar Dados
Exportação para diferentes formatos:
- `.to_excel()` - Exportar para Excel
- `.to_csv()` - Exportar para CSV

## 🚀 Como Usar

### Pré-requisitos

```bash
# Instalar dependências (se usar Poetry)
poetry install

# Ou instalar manualmente
pip install pandas openpyxl
```

### Executar o Notebook

1. Abra o notebook `notebook/01_basic_command.ipynb` no Jupyter Notebook ou JupyterLab
2. Execute as células na ordem
3. O notebook carrega dados de uma planilha do Google Sheets automaticamente

### Dados de Exemplo

O notebook utiliza dados de vendas com as seguintes colunas:
- `data` - Data da venda
- `vendedor` - Nome do vendedor
- `cidade` - Cidade da venda
- `produto` - Nome do produto
- `quantidade` - Quantidade vendida
- `preco` - Preço unitário

## 📁 Estrutura do Projeto

```
.
├── notebook/
│   └── 01_basic_command.ipynb  # Este notebook
├── data/
│   ├── resultado.csv           # Arquivo CSV exportado
│   └── resultado.xlsx          # Arquivo Excel exportado
└── README.md                   # Este arquivo
```

## 💡 Dicas

- Sempre comece com a **inspeção inicial** dos dados antes de fazer transformações
- Use `df.copy()` quando quiser criar uma cópia independente do DataFrame
- Para filtros compostos, use parênteses: `(condição1) & (condição2)`
- O método `inplace=True` modifica o DataFrame original (use com cuidado)

## 📚 Recursos Adicionais

- [Documentação oficial do Pandas](https://pandas.pydata.org/docs/)
- [10 minutos para Pandas](https://pandas.pydata.org/docs/user_guide/10min.html)
- [Pandas Cheat Sheet](https://pandas.pydata.org/Pandas_Cheat_Sheet.pdf)

## 📝 Notas

- Os dados são carregados diretamente de uma planilha do Google Sheets
- Os arquivos exportados são salvos na pasta `data/`
- O notebook demonstra operações comuns, mas pode ser adaptado para seus próprios dados

---

**Última atualização:** 2024
