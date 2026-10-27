# 🎼 A Pauta do Eclipse

**Desafio 02 | Trilha Design | Orc'estra Gamificação**

**Prazo:** (definir)

> Antes de começar, releia o `README.md` da raiz: ele explica o fork, a branch `desafio02` e o Pull Request.

## 🎬 Aulas de apoio (Udemy)

Seção 4: Landing Page XP Zone

| Aulas | Foco |
|---|---|
| 16 a 21 | Grids, Auto Layout e componentes base |
| 22 a 27 | Image Settings, Effects e protótipo básico |

Sua landing page **não pode ser uma cópia** da Landing Page XP Zone da aula.

## 📜 O Capítulo

O Eclipse chegou, e o Maestro quer anunciar o Concerto num painel na praça. Mas os cartazes foram pendurados cada um numa altura, e os retratos dos instrumentos estão esticados.

**A Pauta**, espírito das linhas de prata, avisa: "Sem grade, as notas flutuam. Monte o painel sobre a minha pauta, com fios que se ajustam sozinhos, e deixe o Maestro clicar nele."

## 🎯 Sua missão

Monte uma **landing page simples** da Loja da Orquestra, com **2 telas ligadas por um protótipo**. Escolha **uma** versão:

- **Desktop:** frame de 1440 px, grid de 12 colunas
- **Mobile:** frame de 390 px, grid de 4 colunas

**Onde fazer:** o indicado é o **mesmo arquivo Figma do Desafio 01**, em uma **nova página** chamada `Landing Page`. Se precisar, pode criar outro arquivo (avise no `ENTREGA.md`).

### O que entregar

| Tela | Conteúdo |
|---|---|
| `Home` | Header (logo e links), Hero (título, texto, botão e imagem) e uma linha com 3 cards de instrumentos |
| `Detalhe` | Imagem, nome, descrição, preço em **PTS**, botão "Comprar" e botão "Voltar" |

| Ferramenta | O que usar |
|---|---|
| **Grid** | Layout grid aplicado nos dois frames |
| **Auto Layout** | Header, hero, linha de cards e o interior do card |
| **Componente** | O card como componente, usado 3 vezes (instâncias) |
| **Mídia** | Ao menos 4 imagens (hero e cards), com Image Settings corretos, sem esticar |
| **Effects** | Ao menos 1 efeito aplicado (ex.: sombra nos cards ou blur no header) |
| **Protótipo** | Ponto de partida na `Home`; clicar em um card abre o `Detalhe`; "Voltar" retorna |

**Regra de ouro:** nada posicionado "no olho". Use Auto Layout e instâncias do componente.

**Liberdade criativa:** tema, textos, cores, fonte e imagens são seus. Usar o Diapasão do Desafio 01 é bem-vindo, mas não é obrigatório.

**Ainda não precisa:** variants, variables, componentes interativos e Design System novo.

## 🪕 As regras do duelo

Para ganhar o **Selo da Pauta**, o seu trabalho precisa resistir a todos os desalinhos:

| Desalinho | Nome | O que ele testa |
|---|---|---|
| 1 | O Caos | Página `Landing Page` com frames `Home` e `Detalhe` nomeados |
| 2 | O Anônimo | Camadas e componente com nomes claros; nada de `Frame NN` ou `Rectangle NN` |
| 3 | O Torto | Conteúdo alinhado à grade; Auto Layout com espaçamentos consistentes |
| 4 | O Vazio | Todas as telas, itens e o protótipo presentes |
| ??? | O Ensaio Geral | Desalinhos que você ainda não ouviu, aplicados na correção |

> **Não existe vitória parcial.** Passar em 3 de 4 é derrota. E passar nos 4 visíveis ainda não garante o selo: o Ensaio Geral acontece na correção.

## 🗺️ Estrutura

### No Figma

```
📁 Orc'estra – [Seu Nome]
├── 📄 Design System        ← Desafio 01 (não apague)
└── 📄 Landing Page         ← você trabalha aqui
    ├── 🖼 Home
    └── 🖼 Detalhe
```

Nomeie as camadas (`Header`, `Hero`, `Cards`, `Info`) e o componente (`Card/Produto`).

### No repositório

```
desafio02/
├── README.md          # este arquivo (não altere)
├── ENTREGA.md         # você preenche
└── evidencias/
    ├── landing.png
    ├── detalhe.png
    └── prototipo-fluxo.png
```

## 🧭 Passo a passo

1. **Prepare o repositório:** sincronize o fork e crie a branch `desafio02`.
2. **Prepare o Figma:** crie a página `Landing Page` e os frames `Home` e `Detalhe` (1440 ou 390 px de largura).
3. **Aplique o grid** nos dois frames.
4. **Monte o card** em Auto Layout e transforme-o em componente.
5. **Monte a `Home`** em Auto Layout, com 3 instâncias do card.
6. **Trate as imagens** com Fill ou Crop, sem esticar.
7. **Monte o `Detalhe`.**
8. **Monte o protótipo:** ponto de partida, card → `Detalhe`, "Voltar" → `Home`.
9. **Chame a Pauta** (checklist abaixo).
10. **Salve uma versão** em *File → Save to version history*, com o nome `Desafio 02`.
11. **Exporte três prints** para `desafio02/evidencias/`: a `Home` com a grade visível, o `Detalhe` e a aba de protótipo com as conexões.
12. **Preencha o `desafio02/ENTREGA.md`**, com o link do Figma e do protótipo.
13. **Commit, push e Pull Request** com o título `[Desafio 02] Seu Nome Sobrenome`. Não faça o merge.

## 🔎 A Pauta (checklist)

**Desalinho 1 – O Caos**
- [ ] Página `Landing Page` com os frames `Home` e `Detalhe`
- [ ] A página `Design System` do Desafio 01 continua intacta (se estiver no mesmo arquivo)

**Desalinho 2 – O Anônimo**
- [ ] Componente com nome claro (`Card/Produto`)
- [ ] Nenhuma camada chamada `Frame NN`, `Rectangle NN`, `Group NN` ou `Ellipse NN`

**Desalinho 3 – O Torto**
- [ ] Grid aplicado e conteúdo alinhado às colunas
- [ ] Header, hero, linha de cards e interior do card em Auto Layout
- [ ] Gaps e paddings consistentes (ex.: múltiplos de 8)

**Desalinho 4 – O Vazio**
- [ ] `Home` com header, hero e 3 cards de instrumentos diferentes
- [ ] `Detalhe` com imagem, nome, descrição, preço em PTS e dois botões
- [ ] Card como componente, usado 3 vezes
- [ ] 4 ou mais imagens, sem esticar
- [ ] Ao menos 1 efeito aplicado
- [ ] Protótipo: início definido, card leva ao detalhe e "Voltar" retorna

**Entrega**
- [ ] Links do Figma e do protótipo com permissão "Qualquer pessoa com o link pode ver"
- [ ] Versão `Desafio 02` salva
- [ ] Três prints em `desafio02/evidencias/`
- [ ] `ENTREGA.md` preenchido
- [ ] PR com o título correto e só arquivos da pasta `desafio02/`

> ⚠️ Os desalinhos 1 e 4 são fáceis de passar. Mas uma tela montada "no olho" *parece* certa e não aguenta nenhuma mudança. O Ensaio Geral descobre isso.

## 📜 Dicas (abra só se travar)

<details>
<summary>Dica 1: como aplicar o grid</summary>

Selecione o frame, clique no **+** ao lado de *Layout grid* e escolha **Columns**. Configure colunas, gutter e margem. Use `Ctrl + G` para mostrar ou esconder a grade.

</details>

<details>
<summary>Dica 2: como saber se o Auto Layout funciona</summary>

Troque o nome de um instrumento por um texto bem comprido. Se o card cresce sozinho e nada sobrepõe, está certo. **Hug** abraça o conteúdo, **Fill** preenche o espaço e **Fixed** trava o tamanho.

</details>

<details>
<summary>Dica 3: como evitar imagem esticada</summary>

No preenchimento da imagem, use **Fill** (preenche e corta o excesso) ou **Fit** (mostra inteira), e não **Stretch**. Use **Crop** para ajustar o enquadramento.

</details>

<details>
<summary>Dica 4: como testar o seu trabalho</summary>

(1) Edite o componente do card: as 3 instâncias devem mudar juntas. (2) Duplique um card: a linha deve se ajustar sozinha. (3) Abra o modo *Present* e clique em tudo.

</details>

Se travar por mais de 40 minutos, escreva a sua dúvida no canal da trilha com o que já tentou.

## 📏 Regras

**Proibido:**
- copiar a Landing Page XP Zone da aula ou um template, mudando só os textos
- posicionar elementos "no olho" no lugar de usar Auto Layout
- usar *detach instance* para "resolver" um problema
- esticar imagens
- entregar link com acesso restrito

**Permitido:** qualquer fonte, paleta e estilo; plugins; imagens de bancos livres, com crédito no `ENTREGA.md`.

**Ferramentas de IA:** podem ser usadas para tirar dúvida de conceito, sugerir textos e criar imagens. Pedir o design pronto tira o que este desafio quer treinar, e o Ensaio Geral mostra quando isso aconteceu.

Você precisa saber explicar qualquer escolha do seu trabalho se o assessor perguntar.

## 🏆 Pontuação

O **Selo da Pauta** só é concedido se você passar nos 4 desalinhos visíveis e em todo o Ensaio Geral.

| Critério | Pontos |
|---|---|
| Selo conquistado | 60 |
| Qualidade do design (hierarquia, consistência, legibilidade, contraste, imagens) | 20 |
| Estrutura e entrega (página organizada, links acessíveis, PR, commits no padrão) | 10 |
| `ENTREGA.md` preenchido e perguntas de reflexão | 10 |
| Bônus: fazer as duas versões (Desktop e Mobile) | 3 |
| Bônus: interação extra no protótipo (ex.: overlay ao clicar em "Comprar") | 2 |
| **Total** | **100 + 5** |

- **Atraso na entrega:** desconto de 10 pontos.
- **Design idêntico ao de outro membro:** zera o `ENTREGA.md` e a qualidade do design, e abre conversa individual.
- Todo membro recebe **3 pontos fortes e 3 pontos de melhoria** no Pull Request.
