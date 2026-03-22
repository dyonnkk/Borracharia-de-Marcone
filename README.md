## Projeto: Sistema Web para Borracharia
## Descrição

Este projeto tem como objetivo o desenvolvimento de um sistema web para uma borracharia, utilizando o framework Django, com foco na divulgação dos serviços, atendimento ao cliente e gerenciamento interno de solicitações.

A aplicação será responsiva, acessível via navegador e otimizada para dispositivos móveis, atendendo principalmente usuários em situações emergenciais.

## Objetivos

# Objetivo Geral

Desenvolver uma plataforma web robusta e escalável para melhorar a presença digital e otimizar o atendimento da borracharia.

# Objetivos Específicos

Divulgar serviços oferecidos
Facilitar contato com clientes (WhatsApp e formulário)
Exibir localização da empresa
Gerenciar solicitações de atendimento
Disponibilizar painel administrativo

# Stakeholders

Dono da borracharia
Clientes (motoristas, motociclistas, empresas)
Funcionários
Equipe de desenvolvimento

## Escopo do Sistema

# Módulo Público (Frontend)

Página inicial (Home)
Sobre a empresa
Serviços
Contato
Localização (Google Maps)
Botão de atendimento rápido (WhatsApp)

# Módulo Administrativo (Django Admin + Customizações)

Gerenciamento de serviços
Gerenciamento de solicitações
Cadastro de clientes (opcional)
Dashboard simples

## Para sistemas baseados no Debian (Ubuntu, Linux Mint, etc.)

# Pré-requisitos

Instale o Python e o módulo venv:

``
sudo apt update
sudo apt install python3 python3-venv python3-pip -y
`` 
Criar o ambiente virtual:

``
python3 -m venv .venv
`` 
Ativar o ambiente:

``
source venv/bin/activate
`` 
Após ativar, o terminal ficará assim:

``
(venv) usuario@maquina:~/projeto$
`` 
Desativar o ambiente:

``
deactivate
`` 
## Para sistemas Windows

# Pré-requisitos

Instalar o Python (recomenda-se via Python)
Durante a instalação, marcar: "Add Python to PATH"

# Criar o ambiente virtual

No Prompt de Comando (CMD) ou PowerShell:

``
python -m venv .venv
`` 
# Ativar o ambiente

CMD:

``
venv\Scripts\activate
`` 
PowerShell:

``
venv\Scripts\Activate.ps1
`` 
Caso dê erro de permissão no PowerShell:

``
Set-ExecutionPolicy RemoteSigned -Scope CurrentUser
`` 
Desativar:

``
deactivate
`` 

## Para sistemas macOS

# Pré-requisitos

Instalar Python via Homebrew (recomendado):

``
brew install python
`` 
Ou baixar direto do Python.

# Criar ambiente vitual

``
python3 -m venv .venv
`` 
# Ativar

``
source venv/bin/activate
`` 
# Desativar

``
deactivate
`` 

## Instalação de Dependências (Todos os Sistemas)

Com o ambiente ativado:

``
pip install django
``
Instalar dependências existentes:

``
pip install -r requirements/dev.txt
``
## Como Executar o Projeto

# Clonar o repositório
``
git clone <repo-url>
``

# Acessar diretório
``
cd projeto
``

# Aplicar migrações
``
python manage.py migrate
``

# Criar superusuário
``
python manage.py createsuperuser
``

# Criar o arquivo das variáveis de ambiente
``
cp .env-exemple .env
``

# Inicializa o servidor
``
python manage.py runserver
``

# Acesso
Sistema: http://localhost:8000
Admin: http://localhost:8000/admin