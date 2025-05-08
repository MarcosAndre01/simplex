# Simplex

Este repositório contém uma implementação do algoritmo Simplex para problemas de programação linear. Atividade realizada durante a disciplina de Pesquisa Operacional ministrada pelo
Prof. Dr. Anand Subramanian no Programa de Pós-Graduação em Informática da Universidade Federal da Paraíba (UFPB).

## Execução

1. Crie um ambiente virtual (opcional, mas recomendado):

   ```bash
   python -m venv venv
   source venv/bin/activate  # No Windows use: venv\Scripts\activate
   ```

2. Instale as dependências listadas no arquivo `requirements.txt` (numpy e jupyterlab):

   ```bash
   pip install -r requirements.txt
   ```

3. Inicie o Jupyter Lab:

   ```bash
   jupyter lab
   ```

4. Abra o notebook `simplex.ipynb`.

## Arquivo de Entrada

A entrada do problema pode ser configurada no arquivo `input.txt`. O formato de entrada é inspirado no LINDO. Os coeficientes de todas as variáveis
devem estar explícitos na função objetivo e em todas as restrições.

Exemplos:

```
max 3x1 + 5x2
st
x1 + 0x2 <= 32
0x1 + 2x2 <= 36
3x1 + 2x2 = 18
```

```
max x1 + x2 + x3
st
x1 + x2 + 0x3 <= 1
0x1 -1x2 + x3 <= 0
```

```
max 2x1 + 3x2
st
x1 + x2 <= 10
x1 + 2x2 >= 8
x1 - 1x2 = 2
```

```
min x1 - x2 + x3
st
x1 + x2 - x3 = 3
2x1 - x2 + 3x3 = 4
```
