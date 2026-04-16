# Django Async Views

Exercício para estudo de requisições assíncronas e síncronas com Django + ASGI.

## Requisitos

- Python 3.10+
- pip

## Instalação

1. Clone o repositório:
```bash
git clone https://github.com/Reinaldo-Sn/Django-sync-async
cd async_views
```

2. Crie e ative o ambiente virtual:
```bash
python -m venv env

# Windows
env\Scripts\activate

# Linux/Mac
source env/bin/activate
```

3. Instale as dependências:
```bash
pip install django uvicorn httpx
```

## Iniciando o servidor

```bash
uvicorn --reload asyncviews.asgi:application
```

O servidor estará disponível em `http://127.0.0.1:8000`

## Rotas disponíveis

| Rota | Tipo | Descrição |
|------|------|-----------|
| `/api/` | Async | Requisição HTTP não bloqueante |
| `/sync/` | Sync | Requisição HTTP bloqueante |
| `/ex-async/` | Async | Exemplo de view assíncrona |
