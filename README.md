# Template para projetos do Observatório FIESC

Este repositório serve como um template padrão para iniciar novos projetos de Data Science. O objetivo é fornecer uma estrutura de diretórios organizada que promova a reprodutibilidade e facilite a colaboração.

## Estrutura de Diretórios

A estrutura de pastas foi pensada para separar de forma lógica os diferentes componentes de um projeto de dados:

```
.
├── Dados/
│   └── README.md  -> Armazene aqui os dados brutos e processados.
├── Imagens/
│   └── README.md  -> Guarde imagens e gráficos gerados/utilizados pelo projeto.
├── Modelos/
│   └── README.md  -> Salve os modelos treinados.
├── Notebooks/
│   └── README.md  -> Para prototipação e análises exploratórias.
├── Scripts/
│   └── README.md  -> Scripts para ETL, treinamento, inferência, etc.
├── requirements.txt -> Lista de dependências do projeto.
└── README.md        -> Este arquivo.
```

*   **`Dados/`**: Contém os datasets. É uma boa prática ter subpastas como `raw/` para dados brutos e `processed/` para dados limpos e transformados.
*   **`Imagens/`**: Ideal para salvar visualizações, como gráficos e plots, que podem ser usados em relatórios ou apresentações.
*   **`Modelos/`**: Local para armazenar os artefatos de modelos treinados (ex: arquivos `.pkl`, `.h5`, `.joblib`).
*   **`Notebooks/`**: Jupyter Notebooks para experimentação. Tente manter os notebooks focados em etapas específicas (ex: `01-exploracao-dados.ipynb`).
*   **`Scripts/`**: Código Python modularizado. Funções de pré-processamento, classes de modelos e pipelines de execução devem ser colocados aqui para serem reutilizados.

## Como Começar

Siga os passos abaixo para configurar o ambiente de desenvolvimento para um novo projeto usando este template.

### Pré-requisitos

-   Python 3.10+ instalado.

### 1. Crie o Ambiente Virtual

É uma prática essencial criar um ambiente virtual para isolar as dependências do seu projeto. Abra o terminal na raiz do projeto e execute:

```bash
# Cria um ambiente virtual na pasta venv
py -m venv venv
```

### 2. Ative o Ambiente Virtual

**No Windows (PowerShell/CMD):**
```powershell
.\venv\Scripts\activate
```

**No macOS/Linux:**
```bash
source ./venv/bin/activate
```

Após a ativação, o nome do ambiente (`.venv`) aparecerá no início da linha do seu terminal.

### 3. Instale as Dependências

Com o ambiente ativado, instale as bibliotecas necessárias para o projeto, que devem estar listadas no arquivo `requirements.txt`.

```bash
# Exemplo de instalação
pip install -r requirements.txt
```
