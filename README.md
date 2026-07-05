# Análise de Dados com Python — Turma T5
## Repositório da Turma — SENAI / LAB365

**Prof. Especialista Cláudio F. Neves**

---

## Sobre o curso

| | |
|---|---|
| **Nome do Produto** | Análise de Dados com Python |
| **Carga Horária Total** | 300 horas, em 2 módulos de 150h |
| **CBO** | 2112-20 — Cientista de Dados |
| **Modalidade** | Qualificação Profissional, a distância, online |
| **Público-alvo** | Estudantes de tecnologia, profissionais em transição de carreira e entusiastas de Python e dados |
| **Pré-requisito obrigatório** | Ter no mínimo 14 anos |

**Objetivo:** capacitar profissionais para coletar, tratar, analisar, visualizar e interpretar dados utilizando Python e ferramentas modernas de análise, aplicando boas práticas de programação, estatística, limpeza de dados, exploração, modelagem básica e comunicação de insights.

### Matriz Curricular

| Módulo | Unidade Curricular | CH | Status |
|--------|---------------------|:--:|--------|
| **Básico** | Manipulação de Dados com Python e SQL | 150h | **Este repositório** |
| Específico | Gestão de Dados com Arquitetura Moderna | 150h | Próxima etapa do curso |

> Aprovação: aproveitamento mínimo **≥ 7,0** em cada Unidade Curricular. Não há obrigatoriedade de frequência mínima para aprovação.

---

## O que é este repositório

Espaço de colaboração da **Turma T5** durante o Módulo Básico (*Manipulação de Dados com Python e SQL*). Aqui ficam:

- O material de estudo de cada semana (teoria + notebook prático)
- A pasta `alunos/`, onde cada estudante organiza seus próprios materiais e exercícios

---

## Estrutura do repositório

```
turma05-analise-de-dados-com-python/
├── README.md
├── 01_Introducao_Fundamentos_Analise_Dados/
│   ├── aula_teorica.html      ← teoria + quiz interativo
│   └── notebook_colab.ipynb   ← notebook prático (abra no Google Colab)
├── 02_Logica_de_Programacao/
│   ├── aula_teorica.html      ← teoria + quiz interativo
│   └── notebook_colab.ipynb   ← notebook prático (abra no Google Colab)
├── 03_Versionamento_e_Python_Local/
│   ├── aula_teorica.html      ← teoria + quiz interativo
│   └── notebook_colab.ipynb   ← notebook prático (abra no Google Colab)
├── 04_Manipulacao_Arquivos_e_Modularizacao/
│   ├── aula_teorica.html      ← teoria + quiz interativo
│   └── notebook_colab.ipynb   ← notebook prático (abra no Google Colab)
├── 05_Pandas_e_NumPy/
│   ├── aula_teorica.html      ← teoria + quiz interativo
│   └── notebook_colab.ipynb   ← notebook prático (abra no Google Colab)
├── 06_..._ (próximas semanas, liberadas ao longo do curso)
└── alunos/
    ├── LEIA-ME.txt
    ├── <seu-nome>/                ← cada aluno cria a sua pasta aqui
    └── ...
```

---

## Notebooks do curso

Clique em **Open in Colab** para abrir o notebook da semana diretamente no Google Colab — sem instalar nada, sem navegar por pastas:

| Semana | Tema | Notebook |
|:------:|------|:--------:|
| 01 | Introdução e Fundamentos da Análise de Dados | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/cfneves/turma05-analise-de-dados-com-python/blob/main/01_Introducao_Fundamentos_Analise_Dados/notebook_colab.ipynb) |
| 02 | Lógica de Programação | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/cfneves/turma05-analise-de-dados-com-python/blob/main/02_Logica_de_Programacao/notebook_colab.ipynb) |
| 03 | Versionamento e Python Local | *em breve* |
| 04 | Manipulação de Arquivos e Modularização | *em breve* |
| 05 | Pandas e NumPy | *em breve* |
| 06 | Limpeza e Transformação de Dados | *em breve* |
| 07 | Visualização e Pipelines | *em breve* |

> Os badges acima abrem a versão do professor diretamente no Colab. Para trabalho persistente entre sessões, configure o ambiente abaixo (faça uma vez).

---

## Configuração do ambiente — faça uma vez

O Colab começa do zero a cada sessão — qualquer arquivo some ao encerrar. Solução: clonar o repositório dentro do **Google Drive** (uma vez), onde tudo fica salvo permanentemente.

**Célula 1 — clone inicial (só na primeira vez):**

```python
from google.colab import drive
drive.mount('/content/drive')      # autorize quando o link aparecer

import os
os.makedirs('/content/drive/MyDrive/Turma05', exist_ok=True)
%cd /content/drive/MyDrive/Turma05

!git clone https://github.com/cfneves/turma05-analise-de-dados-com-python.git
!ls    # deve aparecer: turma05-analise-de-dados-com-python/
```

**Célula 2 — início de cada nova sessão (toda vez):**

```python
from google.colab import drive
drive.mount('/content/drive')

%cd "/content/drive/MyDrive/Turma05/turma05-analise-de-dados-com-python"
!ls                            # semanas disponíveis

%cd "01_Introducao_Fundamentos_Analise_Dados"
!ls
!pwd
```

**Quando uma nova semana for liberada — baixar o conteúdo:**

```python
%cd "/content/drive/MyDrive/Turma05/turma05-analise-de-dados-com-python"
!git pull
```

> Passo a passo detalhado com explicações no [GUIA_GITHUB.md](GUIA_GITHUB.md) — Caminho C.

---

## Como usar o material de cada semana

### Notebook prático

Configure o ambiente acima (clone inicial) e execute a Célula 2 a cada sessão para ir direto à pasta da semana.

### Aula teórica (HTML)

1. Clique no arquivo `aula_teorica.html` na pasta da semana
2. Clique no ícone de download (↓ no canto superior direito) → salve o arquivo
3. Abra no navegador — a aula com quiz interativo funciona completamente offline

---

## Como enviar seus exercícios para o repositório

Para o setup completo (criar conta no GitHub, aceitar convite, criar sua pasta), veja o **[GUIA_GITHUB.md](GUIA_GITHUB.md)**. Resumo:

### Pelo navegador — sem Git instalado (Blocos 1 e 2, Google Colab)

Ideal para quem trabalha no Google Colab e ainda não configurou o Git localmente:

1. No Colab, faça **Arquivo → Fazer download → Fazer download do .ipynb**
2. Acesse o repositório no GitHub → navegue até `alunos/seu-nome/`
3. Clique em **"Add file → Upload files"** → selecione o arquivo baixado
4. Em "Commit changes", selecione **"Create a new branch and start a pull request"** e use `alunos/seu-nome` como nome da branch
5. Clique em **"Propose changes"** → **"Create pull request"**
6. Aguarde a aprovação do professor (*"Review required"* é normal — não é erro)

### Via Git local (a partir do Bloco 2, Semana 03)

```bash
git clone https://github.com/cfneves/turma05-analise-de-dados-com-python.git
cd turma05-analise-de-dados-com-python
git checkout -b alunos/seu-nome
mkdir alunos/seu-nome
# adicione seus arquivos dentro de alunos/seu-nome/
git add alunos/seu-nome
git commit -m "Adiciona materiais de [seu nome]"
git push -u origin alunos/seu-nome
# depois, abra um Pull Request da sua branch para a main
```

Veja também `alunos/LEIA-ME.txt` e o [GUIA_GITHUB.md](GUIA_GITHUB.md) completo.

---

## Regras de colaboração — o que você PODE e NÃO PODE fazer

| Você PODE | Você NÃO PODE |
|-----------|-----------------|
| Criar sua própria pasta em `alunos/<seu-nome>/` | Criar/editar arquivos dentro da pasta de outro colega |
| Adicionar, editar e organizar livremente os arquivos **dentro da sua pasta** | Editar, mover ou excluir arquivos do material oficial do curso (fora de `alunos/`) |
| Abrir Pull Requests para enviar suas mudanças | Excluir pastas ou arquivos de outros alunos |
| Sugerir melhorias via Pull Request/Issue | Fazer push direto na branch `main` (sempre via Pull Request) |
| Pedir revisão/ajuda ao professor ou colegas | Forçar push (`--force`) ou apagar branches de outras pessoas |

> A branch `main` é protegida: **todo Pull Request precisa da aprovação do professor** antes do merge (o GitHub nunca permite que o autor aprove o próprio PR, então a aprovação sempre vem de outra pessoa — por padrão, o professor).

---

## Tecnologias e Ferramentas

| Ferramenta | Uso |
|-----------|-----|
| Python 3.x | Linguagem principal |
| Google Colab | Ambiente de desenvolvimento inicial |
| VS Code | Ambiente de desenvolvimento local (a partir do Bloco 2) |
| Git / GitHub | Versionamento e colaboração — este repositório |
| Pandas / NumPy | Manipulação e análise de dados |
| Matplotlib / Seaborn | Visualização de dados |
| PostgreSQL | Integração Python-SQL |
| Discord / AVA | Comunicação e ambiente virtual de aprendizagem |

---

*SENAI / LAB365 — Análise de Dados com Python*
*Prof. Especialista Cláudio F. Neves*
