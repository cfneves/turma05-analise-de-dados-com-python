# Guia — Configurando seu acesso ao GitHub da Turma

**Prof. Especialista Cláudio F. Neves**

> Este guia não está amarrado a uma semana específica. Faça-o com calma, **antes da sua primeira entrega** que precise ir para o repositório — sem pressa e sem prazo de uma única aula. Se travar em qualquer passo, peça ajuda no Discord da turma antes de continuar.

---

## Antes de começar, alguns nomes que você vai ver o tempo todo

| Termo | O que significa |
|---|---|
| **Git** | O programa que guarda o "histórico de versões" dos seus arquivos — como um Ctrl+Z gigante, que lembra de cada mudança feita, por quem e quando. |
| **GitHub** | O site que guarda esse histórico na internet (na nuvem) e permite que várias pessoas trabalhem no mesmo projeto, cada uma na sua parte. |
| **Repositório ("repo")** | A "pasta do projeto" versionada — no nosso caso, o repositório da Turma T5. |
| **Branch** | Uma "cópia paralela" do repositório, só sua, onde você trabalha sem risco de estragar o trabalho dos colegas. |
| **Commit** | Um "ponto de salvamento" das suas mudanças, com uma mensagem curta explicando o que mudou. |
| **Push** | Enviar os seus commits do seu computador para o GitHub (a nuvem) — antes do push, suas mudanças existem só na sua máquina. |
| **Pull Request (PR)** | Um pedido formal: "professor, pode revisar e aceitar essa mudança que eu fiz?" — nada entra na pasta oficial da turma sem passar por um PR aprovado. |

---

## Pré-requisitos

- Computador com acesso à internet
- Uma conta no GitHub (gratuita — se ainda não tem, o Passo 1 abaixo ensina a criar)
- Ter enviado seu nome de usuário do GitHub para o professor no Discord, para ser adicionado como colaborador do repositório (sem isso, nenhum dos dois caminhos abaixo funciona)
- Escolher um caminho: **Caminho A — GitHub Desktop** (programa com botões, recomendado para quem nunca usou Git) ou **Caminho B — Terminal/Git Bash** (digitando comandos)

---

## Caminho C — Google Colab (para os primeiros encontros, sem instalar nada)

Use este caminho enquanto o curso utilizar o **Google Colab** como ambiente principal (Blocos 1 e 2). Você não precisa instalar nada — só de um navegador, uma conta Google e uma conta GitHub.

1. **Criar sua conta no GitHub.** Acesse `github.com/join`, informe e-mail, senha e escolha um nome de usuário (ex.: `joao-silva`). Guarde esse nome de usuário — você vai precisar dele.

2. **Avisar o professor e aceitar o convite.** Mande seu nome de usuário do GitHub no Discord da turma. O professor te adiciona como colaborador. Você receberá um e-mail/notificação do GitHub com o convite — abra e clique em **"Accept invitation"**.

3. **Abrir o notebook da semana no Google Colab.** Três formas:

   - **Link direto (Semana 01):**
     `https://colab.research.google.com/github/cfneves/turma05-analise-de-dados-com-python/blob/main/01_Introducao_Fundamentos_Analise_Dados/notebook_colab.ipynb`

   - **Pelo Colab:** acesse `colab.research.google.com` → **Arquivo → Abrir notebook → aba GitHub** → busque `cfneves/turma05-analise-de-dados-com-python` → clique no `notebook_colab.ipynb` da semana

   - **Clonar o repositório dentro do Colab:** crie uma nova célula de código e execute:
     ```python
     !git clone https://github.com/cfneves/turma05-analise-de-dados-com-python.git
     %cd turma05-analise-de-dados-com-python
     !ls
     ```
     O repositório aparece no painel de arquivos (ícone de pasta, à esquerda). Navegue até a semana e clique no `notebook_colab.ipynb`.

4. **Salvar uma cópia no Drive.** O notebook aberto via link ou pelo menu do Colab é somente leitura — é a versão do professor. Clique em **Arquivo → Salvar uma cópia no Drive** para criar a sua versão editável no Google Drive. Trabalhe sempre nessa cópia.

5. **Fazer o exercício.** O Colab salva automaticamente no Drive enquanto você trabalha.

6. **Baixar seu notebook quando terminar.** Clique em **Arquivo → Fazer download → Fazer download do .ipynb** — salva o arquivo no seu computador.

7. **Fazer upload no GitHub.** Acesse o repositório em `github.com/cfneves/turma05-analise-de-dados-com-python`:
   - Navegue até `alunos/` → entre na sua pasta `alunos/seu-nome/` (se ainda não tiver sua pasta, veja abaixo)
   - Clique em **"Add file → Upload files"**
   - Selecione o arquivo `.ipynb` que você baixou
   - Em "Commit changes", selecione **"Create a new branch and start a pull request"**
   - Digite `alunos/seu-nome` como nome da branch (ex.: `alunos/joao-silva`)
   - Clique em **"Propose changes"**

8. **Abrir o Pull Request.** Na tela seguinte, escreva um título curto (ex.: *"Adiciona notebook Semana 01 — João Silva"*) e clique em **"Create pull request"**.

9. **Aguardar a aprovação.** A PR fica marcada como *"Review required"* — não é erro. O professor revisa e aprova.

> **Ainda não tem sua pasta criada em `alunos/`?** Na primeira vez, clique em **"Add file → Create new file"**, digite `alunos/seu-nome/README.md` no campo do nome (o GitHub cria a pasta automaticamente ao digitar a barra `/`), escreva qualquer coisa no arquivo e siga os passos 7 a 9 para criar a pasta via PR. Depois disso, use o upload normalmente.

---

## Caminho A — GitHub Desktop (recomendado para iniciantes)

1. **Criar sua conta no GitHub.** O GitHub funciona como uma "rede social" para projetos de código — você precisa de uma conta lá, assim como tem uma conta de e-mail. Acesse `github.com/join`, informe e-mail, senha e escolha um nome de usuário (ex.: `joao-silva`). Esse nome de usuário é o que você vai mandar para o professor.

2. **Avisar o professor o seu usuário do GitHub e aceitar o convite.** O professor precisa te adicionar como "colaborador" do repositório da turma. Sem isso, mesmo fazendo tudo certo nos próximos passos, você recebe erro de permissão. Mande seu usuário (@seu-usuario) no Discord da turma. Você vai receber um e-mail/notificação do GitHub com um convite — abra e clique em **"Accept invitation"**.

3. **Instalar o GitHub Desktop.** Um programa com botões e telas (sem precisar digitar comandos) que conversa com o Git e o GitHub por trás dos panos. Acesse `desktop.github.com`, baixe a versão para o seu sistema (Windows/Mac), abra o instalador e siga as opções padrão.

4. **Fazer login no GitHub Desktop.** Abra o GitHub Desktop → na tela inicial, clique em **"Sign in to GitHub.com"** → faça login com a conta criada no Passo 1.

5. **Clonar (baixar) o repositório da turma.** "Clonar" é baixar uma cópia completa do repositório da turma para o seu computador, já conectada ao GitHub. File → **Clone Repository** → aba "GitHub.com" → procure `turma05-analise-de-dados-com-python` → escolha uma pasta no seu PC → **Clone**.

6. **Criar a sua branch.** Trabalhar direto na `main` (a pasta "oficial") é bloqueado de propósito — toda mudança precisa passar por revisão. Criando sua própria branch, você tem liberdade total para trabalhar sem afetar ninguém. Clique em **"Current Branch"** (topo) → **"New Branch"** → nome: `alunos/seu-nome` (ex.: `alunos/joao-silva`, sem espaços ou acentos) → **Create Branch**.

7. **Criar sua pasta e colocar seus arquivos.** Cada aluno trabalha isolado dentro da própria pasta em `alunos/` — isso evita que um aluno sobrescreva o material de outro. No GitHub Desktop, Repository → **Show in Explorer** (abre a pasta clonada). Dentro de `alunos/`, crie uma pasta com o seu nome (igual ao usado na branch). Copie para lá os arquivos que quiser guardar.

8. **Commit — salvar uma versão com explicação.** Um commit é um "ponto de salvamento" das suas mudanças, junto com uma mensagem curta dizendo o que foi feito — assim, qualquer pessoa (inclusive você, no futuro) entende o histórico. Volte ao GitHub Desktop — a aba **"Changes"** já mostra os arquivos novos. Escreva uma frase no campo "Summary" (ex.: *"Adiciona meus primeiros materiais"*) e clique em **"Commit to alunos/seu-nome"**.

9. **Push — enviar para o GitHub.** Até aqui, tudo ficou só no seu computador. O push é o que efetivamente manda suas mudanças para a nuvem, onde o professor e a turma conseguem ver. Clique no botão **"Push origin"** no topo do GitHub Desktop.

10. **Abrir o Pull Request.** O pedido formal para o professor revisar e aprovar sua mudança antes dela entrar de fato na pasta oficial (`main`) da turma. Depois do push, aparece um botão **"Create Pull Request"** — clique (abre o navegador), escreva um título/descrição curtos e clique em **"Create pull request"**.

11. **Aguardar a aprovação.** Sua PR vai aparecer marcada como *"Review required"* — não é erro, é a proteção que existe para todo o material da turma. O professor revisa, e só depois disso seu conteúdo entra na pasta oficial.

---

## Caminho B — Terminal / Git Bash

1. **Instalar o Git.** O "motor" por trás de tudo isso — o programa que de fato versiona os arquivos (o GitHub Desktop é só uma interface bonita por cima dele). Acesse `git-scm.com/downloads`, baixe para o seu sistema, abra o instalador e siga com as opções padrão (Next, Next... Install).

2. **Abrir o Git Bash.** Depois de instalar, procure "Git Bash" no menu Iniciar do Windows e abra — é nele que você vai digitar os comandos dos próximos passos.

3. **Configurar seu nome e e-mail (uma única vez).** Toda vez que você salva uma versão (commit), o Git anota quem fez aquela mudança. Esse passo configura essa "assinatura" — só precisa fazer uma vez por computador.
   ```bash
   git config --global user.name "Seu Nome"
   git config --global user.email "seu-email@exemplo.com"
   ```

4. **Clonar o repositório.** "Clonar" é baixar uma cópia completa do repositório da turma para o seu computador.
   ```bash
   git clone https://github.com/cfneves/turma05-analise-de-dados-com-python.git
   cd turma05-analise-de-dados-com-python
   ```

5. **Criar sua branch.** A `main` é protegida de propósito — criar sua própria branch te dá um espaço livre para trabalhar sem afetar ninguém.
   ```bash
   git checkout -b alunos/seu-nome
   ```
   (troque `seu-nome` pelo seu nome, sem espaços/acentos — ex.: `alunos/joao-silva`)

6. **Criar sua pasta e adicionar arquivos.** Cada aluno trabalha isolado na própria pasta dentro de `alunos/`.
   ```bash
   mkdir alunos/seu-nome
   ```
   Copie seus arquivos para dentro dessa pasta (pelo Explorador de Arquivos mesmo, ou pelo terminal).

7. **Commit.** `add` seleciona o que vai entrar no "ponto de salvamento"; `commit` de fato salva essa versão, com uma mensagem explicando o que foi feito.
   ```bash
   git add alunos/seu-nome
   git commit -m "Adiciona meus primeiros materiais"
   ```

8. **Push.** Envia sua branch (com os commits) do seu computador para o GitHub — antes disso, tudo existia só na sua máquina.
   ```bash
   git push -u origin alunos/seu-nome
   ```

9. **Abrir o Pull Request.** O pedido formal para o professor revisar e aprovar sua mudança antes dela entrar na `main` oficial. O terminal mostra um link parecido com `https://github.com/.../pull/new/alunos/seu-nome` — copie e cole no navegador. Ou acesse o repositório no GitHub: vai aparecer um aviso amarelo **"Compare & pull request"** — clique nele. Escreva um título/descrição curtos e clique em **"Create pull request"**.

10. **Aguardar a aprovação.** Sua PR aparece marcada como *"Review required"* — é a proteção que existe para o material de toda a turma. Aguarde a revisão do professor.

> **Usa Mac?** O instalador do Git para Mac não tem a opção "Add to PATH" do Windows — normalmente já funciona direto no Terminal após a instalação. Se o comando `git` não for reconhecido, instale via [Homebrew](https://brew.sh) com `brew install git`.

---

## Erros comuns

| Mensagem / Situação | O que significa | O que fazer |
|---|---|---|
| "Permission denied" / "Repository not found" ao clonar ou dar push | Você ainda não foi adicionado como colaborador | Avise seu usuário do GitHub no Discord da turma |
| Pediu usuário/senha e não aceitou | O GitHub não usa mais senha simples para Git — precisa logar pelo navegador | Siga o fluxo de login que aparecer na tela (GitHub Desktop) ou pelo navegador (terminal) |
| Sua Pull Request mostra "Review required" e não tem botão de merge | Normal! É a proteção da branch principal | Aguardar o professor revisar — não é erro |
| Não aparece nada para "commitar" no GitHub Desktop | Os arquivos não foram salvos dentro de `alunos/seu-nome/` | Confirme o caminho da pasta com Repository → Show in Explorer |

---

## Checklist final

- [ ] Tenho conta no GitHub
- [ ] Fui adicionado como colaborador (recebi e aceitei o convite)
- [ ] Instalei o GitHub Desktop OU o Git
- [ ] Clonei o repositório da turma
- [ ] Criei minha branch `alunos/<meu-nome>`
- [ ] Criei minha pasta dentro de `alunos/`
- [ ] Fiz commit e push
- [ ] Abri o Pull Request e vi a mensagem "Review required" (sei que isso é normal)

---

*Prof. Especialista Cláudio F. Neves*
