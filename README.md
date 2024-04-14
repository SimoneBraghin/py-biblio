# py-biblio

[![Main workflow](https://github.com/paulovitorweb/py-biblio/workflows/Main%20workflow/badge.svg)](https://github.com/paulovitorweb/py-biblio/actions/workflows/main.yml)

Uma aplicação escrita em Python com dataclasses para gerenciar referências bibliográficas.

## Build

### Requisitos

- Python >= 3.8

### Crie um ambiente virtual 

```
python -m venv venv
```

### Ative o ambiente virtual

```
No MacOS ou Linux ou PyCharm:
source venv/bin/activate

No Command Prompt (cmd):
venv\Scripts\activate

No PowerShell:
.\venv\Scripts\Activate.ps1
```

### Instale as dependências

```
pip install -r requirements.txt
```

### Suba a API

```
make dev
```

Ou, sem Makefile:

```
uvicorn src.pybiblio.api.main:app --reload
```

### Documentação

- Com Swagger: http://127.0.0.1:8000/docs
- Com ReDoc: http://127.0.0.1:8000/redoc

### Teste

Um conjunto de testes pode ser encontrado em `/tests`. Para executá-los, instale também as dependências de desenvolvimento:

```
pip install -r dev-requirements.txt
```

E, em seguida, execute:

```
make test
```

Visualize um relatório da cobertura de testes em `htmlcov/index.html`.

### Lint

Certifique-se de que usou boas práticas de escrita do código.

```
make lint
```
