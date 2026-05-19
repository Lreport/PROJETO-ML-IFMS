# PROJETO-ML-IFMS

Projeto de Machine Learning usando o dataset
[Tracebase](https://github.com/areinhardt/tracebase).

## Objetivo

Classificar o tipo de eletrodomestico com base no padrao de consumo eletrico.

Nesta etapa, o projeto usa somente os dados da pasta:

```text
tracebase/complete/
```

## Preparacao do ambiente

No terminal do VS Code, dentro da pasta do projeto, ative o ambiente virtual:

```powershell
.\.venv\Scripts\Activate.ps1
```

Instale as dependencias, se ainda nao estiverem instaladas:

```powershell
python -m pip install -r requirements.txt
```

## Estrutura esperada do dataset

Baixe o Tracebase e coloque a pasta do dataset dentro deste projeto:

```text
PROJETO-ML-IFMS/
  tracebase/
    complete/
    incomplete/
    synthetic/
    australia/
```

Para esta etapa, use apenas `tracebase/complete`.

## Primeiro notebook

Abra e execute:

```text
notebooks/01_eda_tracebase_complete.ipynb
```

Esse notebook:

- carrega os arquivos CSV da pasta `complete`;
- cria a coluna `eletrodomestico`, que sera o target (`y`);
- transforma cada arquivo em uma linha de features;
- separa `X` e `y` para a futura etapa de modelagem.
