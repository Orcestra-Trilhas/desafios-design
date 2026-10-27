# Desafios Semanais: Trilha Design

Orc'estra Gamificação | Trilha Design

Este repositório reúne os desafios semanais da trilha de Design. Toda semana aparece aqui uma pasta nova com o enunciado do desafio. Você resolve no seu fork e entrega por Pull Request (PR).

```
<repositorio>/
├── README.md          # este arquivo
├── .gitignore
├── desafio01/         # enunciado e kit do desafio 1
├── desafio02/         # aparece quando o desafio 2 for liberado
└── desafioN/
```

## 1. Como funciona

| Etapa | Quando | O que você faz |
|---|---|---|
| Fork | Uma única vez | Cria a sua cópia do repositório no seu GitHub |
| Sincronizar | Toda semana, antes de começar | Traz para o seu fork a pasta do desafio novo |
| Resolver | Toda semana | Cria uma branch e entrega dentro da pasta do desafio |
| Entregar | Toda semana | Abre um Pull Request do seu fork para este repositório |

**Regra de ouro:** a `main` do seu fork deve ficar idêntica à `main` deste repositório. Você nunca trabalha nela. Todo trabalho acontece em uma branch.

**O que fica onde:** o design em si vive no **Figma** (um único arquivo, usado em todas as unidades). O que vai para o repositório é a **prova da entrega**: o `ENTREGA.md` preenchido (com o link do Figma) e os prints na pasta `evidencias/`.

## 2. Antes de começar

- Conta no GitHub
- Conta no Figma
- Git instalado e configurado com o seu nome e email:

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu-email@exemplo.com"
```

O que cada desafio exigir de ferramentas (por exemplo, plugins do Figma) está descrito no `README.md` da pasta do desafio.

## 3. Passo 1: Fazer o fork (só uma vez)

1. Abra a página deste repositório no GitHub e clique em **Fork**, no canto superior direito.
2. Mantenha o nome padrão e clique em **Create fork**. Você vai parar no repositório `<seu-usuario>/<repositorio>`.
3. Clone o **seu fork** (não o repositório original):

```bash
git clone https://github.com/<seu-usuario>/<repositorio>.git
cd <repositorio>
```

4. Aponte para o repositório original com o nome `upstream`. É por ele que você vai receber os desafios novos:

```bash
git remote add upstream https://github.com/<organizacao>/<repositorio>.git
git remote -v
```

O resultado deve mostrar dois remotos:

| Nome | Aponta para |
|---|---|
| `origin` | O seu fork |
| `upstream` | O repositório original da Orc'estra |

Se `origin` e `upstream` estiverem apontando para o mesmo endereço, você clonou o repositório errado. Apague a pasta e refaça o passo 3.

## 4. Passo 2: Ciclo de cada semana

### 4.1 Sincronize o seu fork

**Opção A: pelo site (a mais simples)**

1. Abra o seu fork no GitHub.
2. Clique em **Sync fork** e depois em **Update branch**.
3. No terminal, traga a atualização para o seu computador:

```bash
git checkout main
git pull origin main
```

**Opção B: só pelo terminal**

```bash
git checkout main
git fetch upstream
git merge --ff-only upstream/main
git push origin main
```

Depois de sincronizar, a pasta do desafio novo (por exemplo, `desafio02/`) deve aparecer no seu computador. Se ela não apareceu, o desafio ainda não foi liberado ou a sincronização falhou.

Se o `--ff-only` der erro, veja a seção 7.

### 4.2 Crie a branch do desafio

Sempre a partir da `main` sincronizada:

```bash
git checkout -b desafio01
```

O nome da branch é `desafio` mais o número com dois dígitos (`desafio01`, `desafio02`, e assim por diante).

### 4.3 Resolva o desafio

1. Entre na pasta do desafio: `cd desafio01`.
2. Leia o `README.md` da pasta. Ele explica a história, as regras e o que entregar.
3. Faça o design no Figma, conforme o enunciado.
4. Na pasta do desafio, preencha o `ENTREGA.md` e coloque os prints dentro de `evidencias/`.
5. Trabalhe somente dentro da pasta do desafio.
6. Faça commits pequenos e frequentes, no padrão da seção 5.

```bash
git add .
git commit -m "docs: adiciona prints do design system"
```

Antes de cada commit, rode `git status` e confira que você não está versionando arquivos que não fazem parte da entrega (como `.DS_Store` ou arquivos temporários).

### 4.4 Envie a sua branch

```bash
git push -u origin desafio01
```

### 4.5 Abra o Pull Request

1. Abra o seu fork no GitHub. Vai aparecer um aviso amarelo com o botão **Compare & pull request**. Clique nele.
2. Confira os quatro campos no topo da tela:

| Campo | Valor correto |
|---|---|
| base repository | `<organizacao>/<repositorio>` (o original) |
| base | `main` |
| head repository | `<seu-usuario>/<repositorio>` (o seu fork) |
| compare | `desafio01` (a sua branch) |

3. Título: `[Desafio 01] Seu Nome Sobrenome`
4. Preencha o checklist da descrição.
5. Clique em **Create pull request**.
6. Abra a aba **Files changed** e confira: só devem aparecer arquivos da pasta do seu desafio. Se aparecerem arquivos a mais, veja a seção 7.

### 4.6 Ajustes depois do feedback

Se o assessor pedir mudanças, **não abra outro PR**. Faça novos commits na mesma branch e envie:

```bash
git add .
git commit -m "fix: atualiza prints apos ajuste dos styles"
git push
```

O PR se atualiza sozinho. Se a mudança for no Figma, lembre de salvar uma nova versão e de atualizar os prints.

### 4.7 O seu PR não será mesclado (e isso é normal)

O assessor vai revisar a entrega, comentar e depois fechar o PR. O PR é a entrega, não precisa virar parte da `main`. Isso evita que as entregas de todos os membros entrem na mesma pasta e causem conflitos.

## 5. Padrões

| Item | Regra |
|---|---|
| Branch | `desafioNN` (exemplo: `desafio01`) |
| Título do PR | `[Desafio NN] Seu Nome Sobrenome` |
| Um PR por desafio | Sempre da branch do desafio para a `main` original |
| O que mexer | Só a pasta `desafioNN/` do desafio em andamento (`ENTREGA.md` e `evidencias/`) |
| O que nunca mexer | A `main` do seu fork, o `README.md` da raiz, o `.gitignore`, as pastas de outros desafios e o `README.md` do desafio (a menos que o enunciado diga o contrário) |
| Nunca versionar | `.DS_Store`, arquivos temporários, senhas e tokens |
| Arquivo Figma | Um único arquivo para todo o curso. Não crie um arquivo novo por entrega |
| Link do Figma | Sempre com permissão "Qualquer pessoa com o link pode ver" |

### Padrão de commits

Formato: `tipo: descrição curta no presente`

| Tipo | Quando usar | Exemplo |
|---|---|---|
| `feat` | adicionou algo novo à entrega | `feat: adiciona print do card` |
| `fix` | corrigiu um erro | `fix: corrige link do Figma` |
| `docs` | preencheu ou ajustou o `ENTREGA.md` | `docs: preenche ENTREGA.md` |
| `chore` | organização de arquivos, sem mudar o conteúdo | `chore: renomeia prints das evidencias` |

Mensagens como `ajustes`, `final` ou `asdf` perdem pontos.

## 6. Prazo e visibilidade

- **Prazo:** o horário limite de cada desafio está no `README.md` da pasta. O que vale é o conteúdo que estiver no PR até esse horário.
- **Tudo é público.** Um fork de repositório público é público, e os PRs ficam visíveis para todos. Qualquer pessoa pode ver a sua entrega, e você pode ver a dos outros.
- Não coloque dados pessoais, senhas ou tokens em nenhum arquivo.
- **Copiar o design de outro membro não vale.** O enunciado de cada desafio explica como isso é tratado, e a correção e as perguntas de reflexão existem justamente para isso.

## 7. Se eu errei

| Situação | O que fazer |
|---|---|
| Fiz commits direto na `main` do meu fork | Veja o bloco de recuperação logo abaixo |
| `git merge --ff-only upstream/main` deu erro | A sua `main` divergiu da original. Veja o bloco de recuperação logo abaixo |
| O PR mostra arquivos de mais | Remova do versionamento com `git rm -r --cached caminho/do/arquivo`, depois `git commit -m "chore: remove arquivos extras"` e `git push`. Confira se o `.gitignore` da raiz está no seu fork |
| Abri o PR com a base ou a branch erradas | Feche o PR (**Close pull request**) e abra outro seguindo a seção 4.5 |
| Mexi em arquivo de outro desafio | Restaure o arquivo: `git checkout main -- caminho/do/arquivo`, depois commit e push |
| Não aparece a pasta do desafio novo | Sincronize o fork de novo (seção 4.1) e confira com `git log --oneline -3` |
| O botão **Compare & pull request** não aparece | Abra a aba **Pull requests** do repositório original e clique em **New pull request**, depois **compare across forks** |
| O link do Figma abre pedindo acesso | Em **Share**, mude para "Qualquer pessoa com o link pode ver" e teste em uma janela anônima |

### Bloco de recuperação: devolver a `main` do fork ao estado do original

Isso guarda o seu trabalho em uma branch e depois limpa a `main`:

```bash
git branch desafio01-salvo
git fetch upstream
git checkout main
git reset --hard upstream/main
git push --force-with-lease origin main
git checkout desafio01-salvo
```

A partir daí, continue o trabalho na branch `desafio01-salvo` (ou renomeie com `git branch -m desafio01`, se não existir outra com esse nome). Atenção: `reset --hard` apaga alterações não commitadas, então faça commit antes.

## 8. Glossário rápido

| Termo | O que é |
|---|---|
| Fork | Sua cópia pessoal de um repositório, hospedada no seu GitHub |
| Clone | Baixar um repositório para o seu computador |
| `origin` | O apelido do seu fork |
| `upstream` | O apelido do repositório original |
| Branch | Uma linha de trabalho separada, para não mexer na `main` |
| Commit | Um registro das suas alterações, com uma mensagem |
| Push | Enviar os seus commits para o GitHub |
| Pull Request | O pedido para o assessor olhar o seu trabalho. É a sua entrega |

## 9. Índice de desafios

| Desafio | Tema | Prazo | Pasta |
|---|---|---|---|
| 01 | O Diapasão de Orc'estra (Figma, Styles e style guide) | (definir) | `desafio01` |

## 10. Dúvidas

Escreva no canal da trilha de Design com o que você tentou e, se for sobre Git, o resultado do terminal. Se travar com o Git, avise antes do prazo, não no dia da entrega.
