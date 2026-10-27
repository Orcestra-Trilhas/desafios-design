# 🎼 O Diapasão de Orc'estra

**Desafio 01 | Trilha Design | Orc'estra Gamificação**

> Antes de começar, leia o `README.md` da raiz do repositório: ele explica como fazer o fork, criar a branch `desafio01` e abrir o Pull Request.

---

## 📜 Anteriormente

No Vale de Orc'estra, os orcs não resolvem suas disputas com machados, e sim com música. Cada clã toca um instrumento, e é a **Grande Orquestra** que mantém o vale unido. A cada geração, quando o céu escurece no **Eclipse**, a orquestra inteira toca a Grande Peça, e é o som dela que renova a paz entre os clãs.

O Eclipse está a poucos dias. E a orquestra está em desordem.

O problema não é falta de talento. É que cada luthier forjou os seus instrumentos do seu jeito: o tambor do clã Rocha afina mais grave que o do clã Brasa, as flautas têm furos em lugares diferentes, e o cartaz de cada instrumento na Loja da Orquestra usa uma cor, uma letra e um tamanho. Quando tocam juntos, o resultado é **O Ruído**: uma cacofonia que cresce onde não existe padrão.

## 🧙 O Capítulo

**Brum**, jovem orc aprendiz de luthier, chegou à oficina antes do amanhecer e encontrou algo que não estava ali no dia anterior: um enorme **diapasão de bronze**, suspenso no ar, vibrando baixinho. Era **O Afinador**, espírito antigo da oficina.

"Aprendiz," ecoou o Afinador, "eu guardo uma verdade que os luthiers esqueceram: **sem um tom de referência, todo instrumento está certo e todos estão errados.** Quando precisaram trocar uma nota, refizeram a orquestra inteira. Nenhuma terminou a tempo."

Brum olhou para as prateleiras. Era verdade: o laranja do cartaz da flauta não era o mesmo laranja do cartaz do tambor.

"Forje o **Diapasão do Vale**," continuou o Afinador, "o guia de estilo ao qual todo instrumento e todo cartaz deverão obedecer. Depois, prove que ele funciona."

O bronze vibrou mais forte.

"Eu apontarei quatro dissonâncias no seu trabalho. E, no **Concerto Final**, o próprio Maestro virá tocar o seu Diapasão para ver se a orquestra o acompanha."

## 🎯 Sua missão

Você é a mão que forja o Diapasão. Num **arquivo Figma novo**, que será usado em todas as unidades da capacitação, crie a página `Design System` e monte o seu **style guide** usando a ferramenta de **Styles** do Figma. Depois, prove que ele funciona construindo um **mini card de produto**, o cartaz de um instrumento na Loja da Orquestra, usando apenas os styles que você criou.

### O que o Diapasão (style guide) precisa ter

| Seção | O que entregar |
|---|---|
| **Color style** | Primary, Secondary, Black/White |
| **Font style** | 1 família de fonte e ao menos 5 text styles: H1, H2, H3, Body e Caption |
| **Icons** | Ao menos 2 ícones, todos do mesmo estilo e tamanho |
| **Buttons** | Botão primário e botão secundário |

### O que o cartaz (mini card) precisa ter

Um **card de produto** com um instrumento da Loja da Orc'estra, por exemplo uma "Flauta de Osso" ou um "Alaúde Sangr'Alma":

- Imagem, ilustração ou forma
- Nome do instrumento
- Descrição curta
- Preço em **PTS** (Pontos)
- Botão de ação (ex.: "Comprar")

### Regra de ouro

> **Todo elemento do card deve usar um style do Diapasão.** Nenhuma cor ou texto solto.

**Liberdade criativa:** paleta, fonte e visual são seus. Pode seguir o clima do Vale, ou outro tema, como quiser. O que será avaliado é a organização, a consistência e o uso correto dos styles.

**Ainda não precisa:** componentes, variants ou variables. Isso vem nas próximas unidades, e o seu Diapasão será a base para evoluir.

## 🪕 As regras do duelo

Para ganhar o **Selo da Afinação**, o seu Diapasão precisa resistir a todas as dissonâncias:

| Dissonância | Nome | O que ela testa |
|---|---|---|
| 1 | A Dissonância do Caos | Página `Design System` organizada, com as seções em ordem e frames nomeados |
| 2 | A Dissonância Anônima | Styles com nomes claros e hierárquicos; nenhuma camada com nome padrão |
| 3 | A Dissonância Torta | Seções alinhadas e espaçamentos consistentes |
| 4 | A Dissonância do Vazio | Todas as categorias pedidas presentes, mais o card completo |
| ??? | O Concerto Final | Dissonâncias que você ainda não ouviu, aplicadas na correção |

> **Não existe vitória parcial.** Passar em 3 de 4 é derrota. E passar nas 4 visíveis ainda não garante o selo: o Concerto Final acontece na correção.

💡 *O Concerto Final existe para premiar quem entendeu para que serve um style guide, não quem apenas desenhou um quadro bonito.*

## 🗺️ Conhecendo o seu projeto

### No Figma

```
📁 Orc'estra – [Seu Nome]
└── 📄 Design System (Página)            ← você trabalha aqui
    ├── 🖼 Color style (Frames)
    ├── 🖼 Font style (Frames)
    ├── 🖼 Icons (Frames)
    ├── 🖼 Buttons (Frames)
    └── 🖼 Card (Frames)
```

As próximas unidades vão adicionar novas páginas ao mesmo arquivo. Por isso, **não crie um arquivo por entrega**.

| Item | O que é |
|---|---|
| **Frames de seção** | Um por categoria, nomeados como no esquema acima |
| **Local styles** | A lista que aparece no painel direito. Aqui nasce o seu Diapasão |
| **Card** | A prova de que os styles funcionam |

### Como nomear os styles

Use **barras** para criar hierarquia. O Figma agrupa automaticamente:

| Bom | Ruim |
|---|---|
| `Color/Primary` | `Color 1` |
| `Color/Neutral/200` | `cinza claro` |
| `Text/H1` | `Texto grande` |
| `Text/Body` | `Style 3` |

### No repositório

A entrega fica dentro da pasta do desafio, no seu fork, na branch `desafio01`:

```
desafio01/
├── README.md          # este arquivo (não altere)
├── ENTREGA.md         # você preenche
└── evidencias/        # você coloca os 3 prints aqui
    ├── design-system.png
    ├── card.png
    └── painel-styles.png
```

## 🧭 Como trabalhar, passo a passo

1. **Prepare o repositório.** Siga o `README.md` da raiz: fork, sincronização e branch `desafio01`.
2. **Prepare o arquivo Figma.** Crie o arquivo `Orc'estra – [Seu Nome]` e a página `Design System`.
3. **Crie os frames de seção** com os nomes: `Color style`, `Font style`, `Icons`, `Buttons` e `Card`.
4. **Monte as cores.** Desenhe os círculos ou quadrados e **crie um Fill style para cada um**, com nome hierárquico.
5. **Monte a tipografia.** Escolha uma família e crie os 5 Text styles.
6. **Monte os ícones.** Use um plugin ou biblioteca livre e mantenha tamanho e estilo iguais.
7. **Monte os botões** usando **apenas** os styles já criados.
8. **Monte o card.** Cada cor e cada texto vêm do Diapasão. Nada de "conta-gotas".
9. **Chame o Afinador** (checklist abaixo).
10. **Salve uma versão** em *File → Save to version history*, com o nome `Desafio 01`.
11. **Exporte três prints** para `desafio01/evidencias/`: o Design System completo, o card e o painel de **Local styles**.
12. **Preencha o `desafio01/ENTREGA.md`**, com o link do Figma.
13. **Faça commit e push** da branch `desafio01`, no padrão de commits do `README.md` da raiz.
14. **Abra o Pull Request** para a `main` original, com o título `[Desafio 01] Seu Nome Sobrenome`. Não faça o merge. Quem faz é o assessor.

## 🔎 Como ler o seu resultado (o Afinador)

Aqui, **você chama o Afinador**: percorra o checklist antes de entregar. O assessor usa o mesmo, mais as dissonâncias escondidas.

### Dissonância 1 – O Caos
- [ ] Existe a página `Design System` no seu arquivo
- [ ] As seções seguem a ordem: Color, Font, Icons, Buttons, Card
- [ ] Cada seção está dentro de um frame nomeado

### Dissonância 2 – A Anônima
- [ ] Todos os styles têm nomes hierárquicos (`Color/...`, `Text/...`)
- [ ] Nenhuma camada se chama `Frame NN`, `Rectangle NN` ou `Ellipse NN`

### Dissonância 3 – A Torta
- [ ] Os itens de cada seção estão alinhados entre si
- [ ] O espaçamento segue um padrão (ex.: múltiplos de 8)
- [ ] O card tem respiro interno consistente

### Dissonância 4 – O Vazio
- [ ] Cores: Primary, Secondary, Black/White
- [ ] Textos: H1, H2, H3, Body e Caption
- [ ] Ícones: no mínimo 2
- [ ] Botões: primário e secundário
- [ ] Card com imagem, nome, descrição, preço em PTS e botão

### Entrega
- [ ] Link do Figma com permissão "Qualquer pessoa com o link pode ver"
- [ ] Versão `Desafio 01` salva no histórico
- [ ] Três prints dentro de `desafio01/evidencias/`
- [ ] `desafio01/ENTREGA.md` preenchido
- [ ] Pull Request com o título `[Desafio 01] Seu Nome Sobrenome` e só arquivos da pasta `desafio01/`

> ⚠️ **Cuidado:** as dissonâncias 1 e 4 são fáceis de passar. Mas um Diapasão desenhado sem styles *parece* certo e não funciona. O Concerto Final descobre isso.

## 📜 Pergaminho de Dicas (abra só se travar)

<details>
<summary>Dica 1: como criar um Fill style</summary>

Selecione o elemento, clique nos quatro pontinhos ao lado da cor no painel direito e escolha o **+** para criar o style. Dê um nome com barra, como `Color/Primary`.

</details>

<details>
<summary>Dica 2: como saber se um elemento está usando style</summary>

Selecione-o e olhe o painel direito. Se aparecer o **nome do style**, está certo. Se aparecer só o código hexadecimal, a cor está solta.

</details>

<details>
<summary>Dica 3: como testar o seu próprio trabalho</summary>

Edite o style `Color/Primary` e mude para uma cor bem diferente. Se o botão e o card mudarem junto, o Diapasão funciona. Se algo ficar com a cor antiga, tem elemento solto. Depois use `Ctrl/Cmd + Z` para voltar.

</details>

Se continuar travado por mais de 40 minutos, escreva a sua dúvida no canal da trilha com o que já tentou.

## 📏 Regras

**Proibido:**
- copiar o style guide da aula, ou de um template, mudando só o nome
- deixar cor ou texto solto no card (sem style aplicado)
- usar *detach style* para "resolver" um problema
- criar um arquivo Figma novo a cada entrega (o arquivo é o mesmo ao longo do curso)
- entregar link com acesso restrito

**Permitido:** qualquer fonte, paleta e estilo; plugins de ícones e de cores; imagens de bancos livres, com crédito no `ENTREGA.md`.

**Ferramentas de IA:** podem ser usadas para tirar dúvida de conceito, sugerir paletas e criar imagens. Pedir o design pronto tira justamente o que este desafio quer treinar, e o Concerto Final mostra quando isso aconteceu.

Você precisa saber explicar qualquer escolha do seu Diapasão se o assessor perguntar.

## 🏆 Recompensas e pontuação

O **Selo da Afinação** só é concedido se o seu Diapasão passar nas 4 dissonâncias visíveis e em todo o Concerto Final. Quem ganha o selo avança na história para o próximo capítulo.

Além do selo, você soma **Pontos de Harmonia** para o ranking da EJ:

| Critério | Pontos |
|---|---|
| Selo conquistado (todas as dissonâncias) | 60 |
| Qualidade do design (hierarquia, consistência, legibilidade, contraste) | 20 |
| Estrutura e entrega (página organizada, link acessível, PR, commits no padrão) | 10 |
| `ENTREGA.md` preenchido e perguntas de reflexão | 10 |
| Bônus: botão com estados (padrão, hover e desabilitado) | 3 |
| Bônus: seção `Grid` com layout grid configurado | 2 |
| **Total** | **100 + 5** |

- **Atraso na entrega:** desconto de 10 pontos.
- **Design idêntico ao de outro membro:** zera o `ENTREGA.md` e a qualidade do design, e abre conversa individual.
- Todo membro recebe **3 pontos fortes e 3 pontos de melhoria** como comentários no Pull Request.

Boa sorte, aprendiz. O Eclipse não espera. 🌘