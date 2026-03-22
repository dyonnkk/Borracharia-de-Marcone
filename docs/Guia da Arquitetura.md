## Arquitetura do Sistema

## O sistema seguirá o padrão MVT (Model-View-Template) do Django.

# Tecnologias

Backend: Django 5 + Django REST Framework (opcional)
Frontend: Django Templates ou integração com Vue.js, Angular ou Bootstrap
Banco de Dados: PostgreSQL
Containerização: Docker + Docker Compose

## Estrutura do Projeto

borracharia/
├── core/              # Configurações do projeto
├── pages/
├── servicos/
├── clientes/
├── solicitacoes/
├── templates/
├── static/
├── manage.py
├── docs/
├── requirements/
|   ├── base.txt
|   ├── dev.txt
|   └── prod.txt
├── .env_exemple
└── README.md

## Modelagem Inicial (Entidades)

# Serviço

nome
descrição
preço (opcional)

# Cliente

nome
telefone
email (opcional)

# Solicitação

cliente
serviço
descrição
status (pendente, em andamento, concluído)
data/hora

# Fluxo do Sistema

Usuário acessa o site
Visualiza serviços
Entra em contato via WhatsApp ou formulário
Registra solicitação
Administrador gerencia via painel Django Admin

# Segurança

Proteção CSRF (nativa do Django)
Autenticação via Django Admin ou via SSO
Validação de formulários
Uso de HTTPS (via Nginx Proxy Manager)