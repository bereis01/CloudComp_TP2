# **Trabalho Prático 2:** DevOps

**Universidade Federal de Minas Gerais | Departamento de Ciência da Computação | 2024/02**

**Aluno:** Bernardo Reis de Almeida

**Professor:** Ítalo Fernando Scota Cunha

**Disciplina:** DCC030 Cloud Computing

## **Modelo**

A execução do modelo exige a declaração das seguintes variáveis de ambiente:

```
DATABASE_PATH="<caminho-para-a-base-de-dados>"
MODEL_PATH="<caminho-de-escrita-do-modelo>"
```

Na pasta ```model/```, primeiramente, deve-se criar um ambiente virtual Python por meio do comando:

```bash
python3 -m venv ./.venv
```

... e o ativar por meio do comando:

```bash
source ./.venv/bin/activate
```

Em seguida, as dependências do sistema devem ser instaladas por meio do comando:

```bash
pip install -r requirements.txt
```

A execução da aplicação pode ser feita por meio do seguinte comando:

```bash
python3 model.py
```

## **Back-End**

A execução do back-end exige a declaração das seguintes variáveis de ambiente:

```
MODEL_PATH="<caminho-de-leitura-do-modelo>"
```

Na pasta ```backend/```, primeiramente, deve-se criar um ambiente virtual Python por meio do comando:

```bash
python3 -m venv ./.venv
```

... e o ativar por meio do comando:

```bash
source ./.venv/bin/activate
```

Em seguida, as dependências do sistema devem ser instaladas por meio do comando:

```bash
pip install -r requirements.txt
```

A execução da aplicação pode ser feita por meio do seguinte comando:

```bash
fastapi run server.py
```

Ela ficará acessível pela rota ```http://0.0.0.0:8000/api/recommendation```.

## **Front-End**

A execução do front-end exige a declaração das seguintes variáveis de ambiente:

```
REC_ROUTE="http://<IP>:<PORT>/api/recommendation"
```

Na pasta ```frontend/```, primeiramente, deve-se criar um ambiente virtual Python por meio do comando:

```bash
python3 -m venv ./.venv
```

... e o ativar por meio do comando:

```bash
source ./.venv/bin/activate
```

Em seguida, as dependências do sistema devem ser instaladas por meio do comando:

```bash
pip install -r requirements.txt
```

A execução da aplicação pode ser feita por meio do seguinte comando:

```bash
streamlit run client.py
```

Ela ficará acessível pela rota ```http://127.0.0.1:8501/```.