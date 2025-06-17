# FakePinterest - Clone Simples do Pinterest com Flask
Este é um projeto de estudo desenvolvido com Flask que simula o funcionamento básico do Pinterest. Ele permite que usuários se cadastrem, façam login, façam upload de imagens e visualizem galerias, tanto pessoais quanto de outros usuários. Uma ótima forma de consolidar conhecimentos em autenticação, banco de dados e upload de arquivos em aplicações web Python.

# Funcionalidades
- Cadastro e login de usuários com validações
- Upload de fotos com armazenamento local
- Página de perfil com visualização de fotos enviadas
- Página de feed com imagens de todos os usuários
- Logout seguro
- Interface responsiva com HTML + CSS

# Tecnologias Utilizadas
- Python 3
- Flask
- Flask-WTF – Formulários e CSRF protection
- Flask-Login – Autenticação de usuários
- Flask-Bcrypt – Hash de senhas
- SQLite – Banco de dados local
- Jinja2 – Templates
- HTML/CSS

# Estrutura do Projeto
fakepinterest/
├── routes.py                  # Arquivo principal com as rotas
├── models.py                  # Definição das classes Usuario e Foto
├── forms.py                   # Formulários com validação
├── templates/                 # Templates HTML
    ├── navbar.html
│   ├── homepage.html
│   ├── criarconta.html
│   ├── perfil.html
│   └── feed.html
├── static/
│   ├── css/style.css          # Estilo customizado
│   └── fotos_posts/           # Imagens enviadas
├── database.db                # Banco de dados SQLite
└── README.md

# Como Executar o Projeto
1. Clone o repositório:

git clone https://github.com/seuusuario/fakepinterest.git
cd fakepinterest

2. Crie e ative o ambiente virtual:

python -m venv venv
venv\Scripts\activate  # Windows
source venv/bin/activate  # macOS/Linux

3. Instale as dependências:
pip install -r requirements.txt

4. Execute o projeto:

python app.py

# Exemplos de Uso
- Página Inicial: login com formulário integrado
- Cadastro: formulário com verificação de e-mail já existente
- Perfil: upload de imagens visíveis apenas ao usuário logado
- Feed: galeria pública com todas as fotos

# Aprendizados
Durante o desenvolvimento deste projeto, foi possível:
- Trabalhar com autenticação usando Flask-Login
- Proteger formulários com CSRF via Flask-WTF
- Criar relacionamento entre tabelas com SQLAlchemy
- Salvar e exibir arquivos no servidor
- Utilizar secure_filename para upload seguro