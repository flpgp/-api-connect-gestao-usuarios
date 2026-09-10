# API Connect – Gestão de Usuários (MVP RESTful)

API RESTful desenvolvida em Python com o microframework Flask para servir como backend de gerenciamento de usuários de uma startup. O projeto adota arquitetura modular com separação de responsabilidades (SoC), validação rigorosa de payloads de entrada, persistência simulada em memória e envelopes padronizados de resposta em formato JSON.

---

## Tecnologias e Ferramentas

* **Linguagem:** Python 3.12
* **Framework Web:** Flask 3.0+
* **Controle de Origem:** Flask-CORS (habilitação de Cross-Origin Resource Sharing)
* **Gestão de Ambiente:** Python-dotenv
* **Padronização:** RESTful Architecture & JSON envelopes
* **Testes de Integração:** Postman / Insomnia / Thunder Client

---

## Estrutura do Projeto

```text
api-connect/
│
├── src/
│   ├── __init__.py
│   ├── app.py                     # Ponto de entrada e middlewares globais
│   ├── controllers/
│   │   ├── __init__.py
│   │   └── user_controller.py     # Lógica de negócio, validações e respostas
│   ├── routes/
│   │   ├── __init__.py
│   │   └── user_routes.py         # Mapeamento de rotas e verbos HTTP (Blueprints)
│   └── data/
│       ├── __init__.py
│       └── mock_users.py          # Camada de persistência provisória em memória
│
├── .env.example
├── .gitignore
├── requirements.txt
└── README.md
