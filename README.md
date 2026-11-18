
# 💬 Chat SQL – Consultas em Linguagem Natural com IA

## 📌 Sobre o projeto

O Chat SQL é uma aplicação desenvolvida em Python que permite consultar bancos de dados relacionais utilizando perguntas em linguagem natural.

A aplicação utiliza um Large Language Model (LLM) para interpretar as perguntas do usuário, gerar consultas SQL e recuperar informações diretamente do banco de dados SQLite.

O objetivo é facilitar o acesso aos dados sem exigir que o usuário escreva manualmente consultas SQL.

## 🚀 Funcionalidades

- Interpretação de perguntas em linguagem natural.
- Geração automática de consultas SQL utilizando LLM.
- Validação sintática e estrutural das consultas com SQLGlot.
- Restrição de operações para consultas de leitura.
- Execução das consultas no banco SQLite.
- Apresentação dos resultados reais retornados pelo banco.
- Histórico de conversas durante a sessão.
- Visualização da consulta SQL e dos resultados obtidos.

## 🛠️ Tecnologias utilizadas

- Python
- Streamlit
- LangChain
- OpenAI API
- GPT-4o-mini
- SQLite
- SQLGlot
- python-dotenv

## 🧠 Fluxo de funcionamento

1. O usuário envia uma pergunta em linguagem natural.
2. O LLM interpreta a solicitação e gera uma consulta SQL.
3. O SQLGlot analisa a consulta gerada.
4. A aplicação verifica se a operação permitida é somente de leitura.
5. A consulta validada é executada no SQLite.
6. O resultado retornado pelo banco é enviado ao LLM.
7. A aplicação apresenta uma resposta baseada nos dados recuperados.

## 🔒 Segurança

O projeto implementa validação das consultas SQL utilizando SQLGlot.

São permitidas consultas de leitura, como SELECT, UNION, INTERSECT e EXCEPT.

Operações de alteração de dados ou estrutura, como INSERT, UPDATE, DELETE, DROP, CREATE e ALTER, são bloqueadas pela validação implementada.

## 🗄️ Banco de dados

O projeto utiliza o banco de dados Sakila, um banco de exemplo que representa o funcionamento de uma locadora de filmes.

Entre as informações disponíveis estão:

- Atores
- Filmes
- Clientes
- Aluguéis
- Pagamentos
- Categorias

## ⚙️ Como executar o projeto

### 1. Clone o repositório

```bash
git clone [URL_DO_REPOSITORIO]
cd Streamlit
```

### 2. Crie um ambiente virtual

```bash
python -m venv venv
```

### 3. Ative o ambiente virtual

Windows:

```bash
venv\Scripts\activate
```

Linux / macOS:

```bash
source venv/bin/activate
```

### 4. Instale as dependências

```bash
pip install -r requirements.txt
```

### 5. Configure a chave da OpenAI

Crie um arquivo `.env` na raiz do projeto:

```env
OPENAI_KEY=sua_chave_api
```

### 6. Execute a aplicação

```bash
streamlit run app.py
```

## 🎯 Objetivo do projeto

Explorar a integração entre Inteligência Artificial e bancos de dados relacionais, utilizando LLMs para transformar perguntas em linguagem natural em consultas SQL, com validação antes da execução.

## 👨‍💻 Autor

William Alves

[GitHub](https://github.com/euwilliamalves)
