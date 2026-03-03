# Projeto ETL com Python – Ciência de Dados

## Objetivo

Este projeto tem como objetivo aplicar, na prática, o fluxo de ETL (Extração, Transformação e Carregamento) utilizando Python. O foco principal é compreender como os dados fluem entre cada etapa do processo, independentemente da fonte utilizada.

A proposta simula um cenário real de Ciência de Dados, onde é necessário lidar com indisponibilidade de fontes externas e buscar soluções alternativas.

## Conceito Central: ETL

ETL significa:

- **Extração (Extract):** Obter dados de uma fonte (API, CSV ou lista local).
- **Transformação (Transform):** Processar os dados e aplicar regras de negócio.
- **Carregamento (Load):** Salvar os dados tratados em um novo destino (arquivo, banco ou API).

## Estratégia Utilizada

Como a API pública utilizada no laboratório pode estar indisponível, foram consideradas duas alternativas práticas:

### Alternativa 1 – Lista em Python

Criação de uma lista de usuários diretamente no código, contendo dados fictícios como:

- Nome
- Conta
- Cartão

Essa abordagem elimina a dependência da API e permite focar na transformação e geração de mensagens.

### Alternativa 2 – Arquivo CSV Completo

Criação de um arquivo CSV contendo as colunas:

- Nome
- Conta
- Cartão

O fluxo do projeto segue:

1. Leitura do arquivo CSV (Extração)
2. Geração de mensagens personalizadas (Transformação)
3. Salvamento dos resultados em um novo arquivo CSV (Carregamento)

## Tecnologias Utilizadas

- Python 3
- Pandas
- OpenAI API (opcional, para geração de mensagens com IA)
- Jupyter Notebook (opcional)

## Estrutura do Projeto

```
etl-python/
│
├── dados_entrada.csv
├── dados_saida.csv
├── etl.py
└── README.md
```

## Fluxo do Processo

### Extração

Leitura dos dados via:
- API (quando disponível)
- Lista local
- Arquivo CSV

### Transformação

- Geração de mensagens personalizadas
- Aplicação de regras de negócio
- Padronização de dados

### Carregamento

- Salvamento dos resultados em novo CSV
- Preparação para envio a outro sistema

## Resultado Esperado

Ao final da execução, o sistema gera um novo arquivo contendo:

- Nome do usuário
- Dados da conta
- Mensagem personalizada gerada automaticamente

## Aprendizados

- Entendimento prático do fluxo ETL
- Manipulação de dados com Pandas
- Tratamento de dependência externa
- Organização de projeto para portfólio

## Próximos Passos

- Integração com banco de dados
- Deploy em ambiente cloud
- Automação do pipeline
- Monitoramento de execução

Desenvolvido como parte do desafio prático de Ciência de Dados.
