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
t5-analise-de-dados-com-python/
├── README.md
├── 01_Introducao_Fundamentos_Analise_Dados/
│   ├── 02_aula_teorica.html      ← teoria + quiz interativo
│   └── 03_notebook_colab.ipynb   ← notebook prático (abra no Google Colab)
├── 02_..._ (próximas semanas, liberadas ao longo do curso)
└── alunos/
    ├── LEIA-ME.txt
    ├── <seu-nome>/                ← cada aluno cria a sua pasta aqui
    └── ...
```

> Cada semana publica aqui apenas os 2 arquivos de uso do aluno (`02_aula_teorica.html` e `03_notebook_colab.ipynb`). Planos de aula, listas de exercícios, atividades avaliativas e gabaritos são materiais internos do professor e não são publicados neste repositório.

---

## Como usar (alunos)

```bash
git clone https://github.com/cfneves/t5-analise-de-dados-com-python.git
cd t5-analise-de-dados-com-python
git checkout -b alunos/seu-nome
mkdir alunos/seu-nome
# adicione seus arquivos dentro de alunos/seu-nome/
git add alunos/seu-nome
git commit -m "Adiciona materiais de [seu nome]"
git push -u origin alunos/seu-nome
# depois, abra um Pull Request da sua branch para a main
```

Veja também `alunos/LEIA-ME.txt`.

---

## Regras de colaboração — o que você PODE e NÃO PODE fazer

| Você PODE | Você NÃO PODE |
|-----------|-----------------|
| Criar sua própria pasta em `alunos/<seu-nome>/` | Criar/editar arquivos dentro da pasta de outro colega |
| Adicionar, editar e organizar livremente os arquivos **dentro da sua pasta** | Editar, mover ou excluir arquivos do material oficial do curso (fora de `alunos/`) |
| Abrir Pull Requests para enviar suas mudanças | Excluir pastas ou arquivos de outros alunos |
| Sugerir melhorias via Pull Request/Issue | Fazer push direto na branch `main` (sempre via Pull Request) |
| Pedir revisão/ajuda ao professor ou colegas | Forçar push (`--force`) ou apagar branches de outras pessoas |

> A aprovação de Pull Requests segue o arquivo `.github/CODEOWNERS`: mudanças dentro da sua pasta podem ser aprovadas por você mesmo (uma vez configurado); qualquer mudança fora da sua pasta precisa de aprovação do professor.

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
