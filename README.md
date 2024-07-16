## Requisitos

- Python 3.12.3
- Pip
- Virtualenv
- Git

## Instruções de Instalação

### 1. Clonar o Repositório

Primeiro, clone o repositório para a sua máquina local usando o comando:

```bash
git clone https://github.com/igormartins0301/Movies-API.git
```

### 2. Criar e Ativar um Ambiente Virtual
Navegue até o diretório do projeto:

```bash
Copiar código
cd SeuProjeto
```

Crie um ambiente virtual:

```bash
Copiar código
python -m venv venv
```

Ative o ambiente virtual:

No Windows:
```bash
venv\Scripts\activate
```
No Mac/Linux:
```bash
source venv/bin/activate
```

### 3. Instalar Dependências
Com o ambiente virtual ativado, instale as dependências do projeto usando o pip:

```bash
pip install -r requirements.txt
```

### 4. Configurar o Banco de Dados
Execute as migrações para configurar o banco de dados:

```bash
python manage.py migrate
```

### 5. Criar um Superusuário
Crie um superusuário para acessar o admin do Django:


```bash
python manage.py createsuperuser
```

### 6. Rodar o Servidor de Desenvolvimento
Inicie o servidor de desenvolvimento do Django:

```bash
python manage.py runserver
```

### Agora, você pode acessar o projeto no seu navegador em 
```bash
http://127.0.0.1:8000/api/v1/genres
http://127.0.0.1:8000/api/v1/actors
http://127.0.0.1:8000/api/v1/movies
http://127.0.0.1:8000/api/v1/reviews
```