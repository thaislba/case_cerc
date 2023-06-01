### Intro

Este repositório contém os artefatos e recursos necessários para a execução do código de análise do dataset chicago.csv.
Esse dataset é um subconjunto do dataset Chicago bikeshare e possui os seguintes campos:

|        Campo       |   Descrição    |
---------------------|-----------------
| Start Time         | Data e hora do início da corrida      |
| End Time           | Data e hora do fim da corrida         |
| Trip Duration      | Duração da corrida                    |
| Start Station      | Estação de início da corrida          |
| End Station        | Estação de fim da corrida             |
| User Type          | Tipo de ciclista                      |
| Gender             | Genêro do ciclista membro             |
| Birth Year;;;;;;;  | Ano de nascimento do ciclista membro  |

### Estrutura do repositório
 - ````.venv````virtual environment com bibliotecas necessárias para a execução do código
 - ````chicago.csv```` arquivo do dataset analisado
 - ````chicago_bikeshare_pt.py```` código Python proposto
 - ````case_cerc_formatted.ipynb````jupyter notebook contendo o código de chicago_bikeshare_pt apresentado de forma visual

### Execução
O código pode ser executado de duas maneiras:
  1. execução de ````chicago_bikeshare_pt.py```` pela linha de comando
  2. execução do jupyter notebook ````case_cerc_formatted.ipynb````

Siga o passo a passo respectivo para executar o código.
  1. execução de ````chicago_bikeshare_pt.py````
      * Abra o terminal e navegue até a pasta python_challenge
      * Ative o ambiente virtual ````source .venv/bin/activate````
      * Execute o comando python3 ````chicago_bikeshare_pt.py````
 2. execução de ````case_cerc_formatted.ipynb````
      * Abra o terminal e navegue até a pasta python_challenge
      * Ative o ambiente virtual ````source .venv/bin/activate````
      * Execute o comando ````jupyter notebook```` uma página localhost deve abrir
      * Abra o notebook e execute as células na ordem em que aparecem
