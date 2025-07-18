# Sistema de Gestão de Estoque (SGE)

## 📦 Descrição

O **SGE - Sistema de Gestão de Estoque** é uma aplicação web desenvolvida com Django e PostgreSQL, voltada para o gerenciamento eficiente de produtos, marcas, categorias e vendas. O sistema oferece uma interface moderna e intuitiva, além de métricas para controle de estoque e desempenho de vendas.

## ✨ Funcionalidades

- ✅ Cadastro, edição e exclusão de **produtos**
- ✅ Gerenciamento de **marcas** e **categorias**
- 📈 Relatórios com métricas de vendas e lucro
- 🔐 Autenticação via JWT
- 🖥️ Interface responsiva com Bootstrap
- 🐳 Ambiente Dockerizado

## 🛠 Tecnologias Utilizadas

- **Backend:** Django 5.2, Django REST Framework
- **Frontend:** HTML, CSS, Bootstrap
- **Banco de Dados:** PostgreSQL
- **Autenticação:** JWT (`djangorestframework-simplejwt`)
- **Ambiente:** Docker, Docker Compose
- **Outros:** `tzdata`, `sqlparse`, `pycodestyle`, `pyflakes`

---

## 🚀 Instalação

### ✅ Pré-requisitos

- [Python 3.12+](https://www.python.org/)
- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/)

### 🔧 Usando Docker (Recomendado)

```bash
# Clone o repositório
git clone https://github.com/CFBruna/sge.git
cd sge

# Construa os containers
docker-compose build

# Suba o ambiente
docker-compose up
```

Acesse o sistema em: [http://localhost:8000](http://localhost:8000)

---

### 🧪 Instalação Manual (opcional)

1. **Crie um ambiente virtual**:

   ```bash
   python -m venv venv
   # Linux/macOS
   source venv/bin/activate
   # Windows
   venv\Scripts\activate
   ```

2. **Instale as dependências**:

   ```bash
   pip install -r requirements.txt
   ```

3. **Configure o PostgreSQL**:
   - Crie um banco chamado `sge`
   - Atualize suas credenciais no arquivo: `app/settings.py`

4. **Aplique as migrações**:

   ```bash
   python manage.py migrate
   ```

5. **Inicie o servidor**:

   ```bash
   python manage.py runserver
   ```

---

## 🔑 Uso

- Acesse: [http://127.0.0.1:8000](http://127.0.0.1:8000)
- Página de login: `/login/`
- Dashboard: Visualize métricas e acesse os menus de gerenciamento
- Navegue pelas seções de Produtos, Marcas, Categorias e Relatórios

---


## 📄 Licença

Este projeto está licenciado sob a **MIT License**.  
Veja o arquivo [LICENSE](./LICENSE) para mais detalhes.

---

## 💡 Créditos

Desenvolvido por [Bruna (CFBruna)](https://github.com/CFBruna) com 💻 e ☕  
Este projeto foi desenvolvido como parte dos estudos durante o curso **Django Master**.
