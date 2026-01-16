---
pdf_options:
  displayHeaderFooter: true
  headerTemplate: |-
    <div style="font-size: 8px; width: 100%; text-align: center; color: #b91c1c; font-family: 'Cinzel', serif; font-weight: 700; letter-spacing: 1px; padding-bottom: 5px;">
      NANO DUNGEON ENGINE v1.5
    </div>
  footerTemplate: |-
    <div style="font-size: 8px; width: 100%; display: flex; justify-content: space-between; padding: 0 20px; color: #78716c; font-family: 'Cinzel', serif;">
      <span>Nano Dungeon Engine</span>
      <span>Page <span class="pageNumber"></span> of <span class="totalPages"></span></span>
    </div>
  margin:
    top: "20mm"
    bottom: "20mm"
    left: "20mm"
    right: "20mm"
generated_at: "2026-01-16T08:50:46.371Z"
---


<style>
    body > h1:first-of-type, .markdown-body > h1:first-of-type { 
        text-align: center; 
        font-size: 2.5em; 
        border-bottom: 2px solid #b91c1c; 
        padding-bottom: 0.5em;
        margin-bottom: 2em;
    }
</style>

<style>
    h1 { color: #1c1917; }
    
    /* Dice & Tokens */
    .rpg-token {
        display: inline-block;
        padding: 0 0.3em;
        border-radius: 0.25em;
        font-weight: bold;
        font-family: 'Courier New', Courier, monospace;
        white-space: nowrap;
        font-size: 0.9em;
    }
    .token-d4 { background-color: #fef08a; color: #854d0e; border: 1px solid #eab308; }
    .token-d6 { background-color: #e2e8f0; color: #1e293b; border: 1px solid #94a3b8; }
    .token-d8 { background-color: #bfdbfe; color: #1e40af; border: 1px solid #60a5fa; }
    .token-d10 { background-color: #d8b4fe; color: #6b21a8; border: 1px solid #c084fc; }
    .token-d12 { background-color: #fbcfe8; color: #9d174d; border: 1px solid #f472b6; }
    .token-d20 { background-color: #bbf7d0; color: #166534; border: 1px solid #4ade80; }
    .token-tn { background-color: #451a03; color: #ea580c; border: 1px solid #9a3412; }
    .token-luck { background-color: #fef08a; color: #854d0e; border: 1px solid #eab308; }
    .token-power { background-color: #e9d5ff; color: #6b21a8; border: 1px solid #c084fc; }
    .token-heart { background-color: #fecaca; color: #991b1b; border: 1px solid #ef4444; }
    .token-stat { background-color: #451a03; color: #ea580c; border: 1px solid #9a3412; }
    .token-math { background-color: #1e293b; color: #38bdf8; border: 1px solid #0f172a; }
    
    /* Footer Styling */
    .pdf-footer {
        font-family: 'System-ui', sans-serif;
        font-size: 9px;
        color: #78716c;
        width: 100%;
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 0 20px;
        border-top: 1px solid #e7e5e4;
        padding-top: 8px;
    }
    .footer-logo { height: 16px; vertical-align: middle; opacity: 0.6; margin-left: 10px; }
    
    /* Density Adjustments */
    h1, h2, h3, h4 { margin-top: 1em; margin-bottom: 0.5em; }
    p, ul, ol, blockquote { margin-bottom: 0.6em; }
    hr { margin: 1.5em 0; border: 0; border-top: 1px solid #e7e5e4; }
</style>
# Manual dos Monstros

Automatic translation placeholder for <span class="rpg-token token-math">pt</span>

---



---

### Para que serve este livro

Este livro é um conjunto de **ferramentas** para criar oponentes e ameaças em NDE:
- rapidamente (em 2–5 minutos),
- sem calcular estatísticas,
- de forma consistente com as regras dos **Regras Básicas** e do **Livro do Mestre**.

**O principal pressuposto do NDE:** *apenas os jogadores rolam os dados.*
Os oponentes não 'atacam com lançamentos' — atacam através da **pressão na ficção**: colocando obstáculos, forçando testes, criando ameaças e consequências.



---

### 0. Glossário (termos neste livro)

- **Defesa**: limiar para acertar/contornar o oponente em combate. O jogador lança e compara o resultado com a Defesa.
- **Dificuldade (D)**: limiar de teste contra o ambiente, fenômeno, movimento especial ou "truque" do inimigo.
- **Corações**: quantos danos uma criatura pode suportar nesta cena.
- **Pião / Elite / Chefe**: três níveis de "importância" do oponente na cena.
- **Facilidade / Dificuldade**: alteração do tamanho do dado do jogador em 1 nível (**<span class="rpg-token token-d6">d6</span>→<span class="rpg-token token-d8">d8</span>→<span class="rpg-token token-d12">d12</span>→<span class="rpg-token token-d20">d20</span>** / para baixo).
- **Movimento especial**: habilidade ativa do inimigo que muda a situação (frequentemente exige um teste F/D/A do jogador).
- **Característica (passiva)**: propriedade constante do inimigo (armadura, voo, resistência, zona de perigo), que geralmente fornece facilidade/dificuldade ou muda a aposta.



---

### 1. Como funciona o oponente no NDE (em resumo)

No NDE, o oponente é simples, mas "vivo" devido ao comportamento.

1) **O jogador age → o jogador faz um lançamento.**
   - Ataque corpo a corpo: Força (F) vs **Defesa** do alvo.
   - Ataque à distância: Destreza (D) vs **Defesa** do alvo.
   - Poderes: Poder (<span class="rpg-token token-stat">P</span>) vs **Dificuldade (D)** ou vs Defesa (se for ataque/imobilização).

2) **Se o jogador erra/perde o teste**, a cena continua: surge um custo ou complicação.
   Na luta, o custo pode significar:
   - perda de posição,
   - perda de tempo,
   - entrada no alcance de uma zona perigosa,
   - ou **Coração perdido**, se fizer sentido (por exemplo, luta corpo a corpo, fogo cruzado, campo de explosão).

3) **O oponente "age" sem lançamento:**
   O Mestre descreve o que o inimigo faz e, se isso realmente ameaça os heróis, então:
   - força um teste (F/D/<span class="rpg-token token-stat">P</span>) contra a **Dificuldade (D)**,
   - ou impõe uma condição ("até que...", "quando você entrar em...", "quem está Perto..."),
   - ou altera os dados dos jogadores (facilidade/dificuldade).

4) **A luta é compreensível quando o inimigo tem uma tática de uma linha.**
   Cada bloco de estatísticas deve conter: "o que esse inimigo faz na primeira rodada" e "o que faz quando leva um golpe na cara".



---

### 2. Ficha de personagem — formato e campos

O ficheiro mínimo de estatísticas tem apenas o que é necessário na cena.

> **Nome — Classe, Defesa, Corações, Papel, Mobilidade, Habilidades, Movimentos, Tática**

### 2.1 Campos obrigatórios

- **Classe:** Pajem | Elite | Chefe  
- **Defesa:** número que precisa ser superado para acertar/evitar o inimigo.  
- **Corações:** quantos acertos aguenta (no NDE "acerto" padrão = 1 Coração).  
- **Função:** qual pressão cria na luta (veja capítulo 4).  
- **Mobilidade:** como se move (descritivamente por zonas; a grade é uma opção).  
- **Habilidades (passivas):** 1–2 características curtas.  
- **Movimentos (ativos):** 1 movimento (Elite) ou 2–3 movimentos (Chefe).  
- **Tática:** 1–3 frases para que o Mestre de Jogo guie o inimigo de forma consistente.

### 2.2 Campos Opcionais (vale a pena ter, se encaixarem)

- **Alcance:** se o inimigo for à distância (por exemplo, "Longe", "Muito longe").  
- **Zona:** se o inimigo criar uma área perigosa (fumaça, fogo, campo de força).  
- **Fraqueza:** uma "alavanca" clara para os jogadores (água, luz UV, interferência de sinal).  
- **Recompensa / Pista:** o que permanece após ser derrotado (saque, pista, informação).  
- **Variações:** 1–2 substituições rápidas (por exemplo, "em vez de voo tem salto"; "em vez de fogo tem ácido").

### 2.3 Exemplo de statblock (universal)

**Guarda — Capanga, Defesa 5, Corações 1, Bruto, Mobilidade: Perto→Próximo, Habilidades: Escudo, Movimentos: Investida, Tática: bloqueia a passagem e empurra fora da cobertura.**

- **Escudo (passivo):** enquanto estiver **Próximo** da cobertura ou do escudeiro, o atacante tem **desvantagem** (dado rebaixado em 1 nível).
- **Investida (movimento):** se o Guarda atingir em combate corpo a corpo (ou se o jogador errar um ataque corpo a corpo contra ele), o Mestre pode empurrar o herói 1 zona (Próximo→Longe) ou 1-2 quadrados na variante de grade.
- **Tática:** entra em combate corpo a corpo com o alvo mais fraco, defende o corredor, não recua.



---

### 3. Classes of Opponents: Peão, Elite, Boss

Na NDE, a "dificuldade" de um oponente é composta de duas coisas:
- **quão difícil é atingi-lo** (Defesa),
- **quanto ele aguenta** (Corações),
- além de **qual a pressão que ele exerce** (papel + movimentos).

### 3.1 Capanga (minion)

- **Defesa:** normalmente **5** (mais fácil: 4, mais difícil: 6).  
- **Corações:** **1** (cai após ser atingido).  
- **Movimentos:** normalmente 0–1 (simples, evidente).  
- **Propósito:** proporciona ritmo, fundo e sensação de "luta em grupo".  
- **Como conduzir:** entra em números de 3–8, morre rápido, mas faz barulho e ocupa espaço.

> Boa regra: o capanga deve ter principalmente uma *posição* (cobertura, vantagem numérica, terreno alto), e não uma "mecânica complexa".

### 3.2 Elite

- **Defesa:** geralmente **6** (elite mais fácil: 5, "elite dura": 8).  
- **Corações:** **2**.  
- **Movimentos:** 1 movimento característico + 1 característica passiva.  
- **Propósito:** é um "mini-chefe" na cena, força a adaptação.

> A elite deve fazer *uma coisa claramente*: "quebra barreiras", "define zonas", "salta pelas paredes", "cura lacaios".

### 3.3 Boss

- **Defesa:** geralmente **8** (lendário: 12).
- **Corações:** **3** (final: 5).
- **Movimentos:** 2–3 movimentos + 1–2 características passivas.
- **Para que serve:** é uma cena em si - afeta o terreno e o ritmo.

**Um boss sem artifícios é chato.** Para que o boss seja "jogável", dê a ele pelo menos um dos seguintes:
- um movimento que força um teste em vários heróis,
- uma zona (terreno que precisa ser gerido),
- ou uma mecânica de "fase" (após perder 1 Coração muda o comportamento).

### 3.4 "Lendário" (nível opcional)

Se você precisa de um oponente para a campanha:
- **Defesa 12**, **Corações 5**, 3–4 movimentos, zonas e fases.
Este é o "chefe para o final do ato" — não use isso aleatoriamente.



---

### 4. Papéis dos oponentes (pressão clara)

Os papéis existem para que o Mestre de Jogo saiba imediatamente "como jogar com isso". O papel não é uma estatística — é um **estilo de ameaça**.

- **Brutamontes (pressão corpo a corpo):** entra para Perto, empurra, derruba, quebra a linha de frente.  
  *Pergunta para os jogadores:* "quem está na frente e o que está arriscando?"

- **Combatente (móvel):** entra, faz o que tem que fazer e foge; pune a solidão.  
  *Pergunta:* "quem está separado do grupo?"

- **Artilharia (distância):** dispara de trás das coberturas; força o movimento e a mudança de posição.  
  *Pergunta:* "onde é seguro e onde está a linha de tiro?"

- **Controlador (controle):** zonas, fumaça, terreno pegajoso, armadilhas, pressão sobre objetivos.  
  *Pergunta:* "como contornar a zona em vez de lutar dentro dela?"

- **Apoio (suporte):** fortalece, cura, desloca, fornece coberturas.  
  *Pergunta:* "quem desabilitar primeiro para simplificar a luta?"

---



---

### 5. Facilidades/Dificuldades em monstros — regra de condução

No NDE **não complicamos os números**.  
Em vez de: "+2 para acertar, -1 para danos, bônus para CA" — fazemos:

- **facilidade:** aumente o dado do jogador em 1 nível,
- **dificuldade:** diminua o dado do jogador em 1 nível,
- **mudança de abordagem:** o sucesso funciona, mas requer uma abordagem diferente (por exemplo, primeiro remover a cobertura).

### 5.1 Quando mudar Defesa e quando o dado

- **Com maior frequência, altere o dado do jogador** (facilitando/dificultando). 
- **Altere a Defesa raramente**, principalmente quando:
  - o inimigo possui "armadura/invisibilidade/campo de força", que *realmente* o torna mais difícil de atingir,
  - ou quando isso faz parte da mecânica da fase do chefe.

### 5.2 Exemplos de dificuldades 'puras'

- 'O inimigo está parcialmente coberto' → o atacante tem **dificuldade**. - 'O inimigo está atordoado / amarrado' → o atacante tem **facilidade**. - 'O inimigo é rápido e salta pelas paredes' → o atacante tem **dificuldade**, até que ele seja bloqueado.



---

### 6. Habilidades Passivas (Características) — Catálogo para Anexar

Abaixo você tem características que pode anexar ao bloco de estatísticas. Escolha **1–2** (chefe: 2–3). Sempre descreva-as no mundo do jogo.

### 6.1 Proteção e dureza

- **Armadura Leve:** o primeiro acerto nesta cena causa 1 Coração a menos (ou seja, 0) *ou* requer "especificação" (o sucesso só causa Coração quando o ataque contorna a armadura).  
  *Versão mais simples:* "o primeiro acerto não causa Coração".

- **Armadura Pesada:** enquanto não contornar a armadura (flanco, explosão, gancho, magia), os ataques têm **desvantagem**.  
  *Nota:* ofereça aos jogadores um caminho claro para contornar.

- **Resistente:** após perder 1 Coração, o inimigo não muda de posição (não pode ser facilmente empurrado/derrubado).  
  Bom para colossos e chefes.

### 6.2 Mobilidade

- **Rápido:** uma vez por rodada pode mudar a distância em uma zona adicional (por exemplo, Distante→Perto).
  Na grade: +1–2 quadrados.

- **Saltador / Escalador:** trata obstáculos verticais como normais.
  Oferece "atalhos viáveis" para as costas inimigas.

- **Voo:** ignora obstáculos do terreno, mas requer coberturas "de cima" ou força testes de reação (por exemplo, <span class="rpg-token token-stat">Z</span>, para evitar bombardeios).

### 6.3 Percepção e Furtividade

- **Explorador:** a primeira tentativa de aproximação furtiva tem **dificuldade**.
- **Sentinelas:** se alguém realizar uma ação barulhenta na cena, o inimigo muda imediatamente para uma posição melhor (entra na cobertura / chama reforços).

### 6.4 Resistências e Vulnerabilidades (simples)

- **Resistência [tipo]:** pela primeira vez na cena, quando o inimigo deveria receber um determinado efeito (fogo, gelo, psíquico, elétrico), o efeito é **enfraquecido** (menor área / duração mais curta / sem perda de Coração).
- **Vulnerabilidade [tipo]:** contra este tipo de ataques, o jogador tem uma **vantagem**.

> Princípio da transparência: resistência e vulnerabilidade só fazem sentido se os jogadores puderem descobrir e aproveitar isso.

### 6.5 "Enxame" e pressão numérica

- **Enxame:** se pelo menos duas dessas criaturas estiverem Perto de um herói, o herói terá uma **desvantagem** nos testes de movimento/fuga até que mude de zona.



---

### 7. Movimentos ativos — como escrever e como conduzir

Um movimento ativo deve responder a 3 perguntas: 1) **O que ele faz na ficção?** (descrição) 2) **Quem é afetado e quando?** (gatilho) 3) **Como é resolvido mecanicamente?** (teste / efeito / custo)

### 7.1 Formato simples de movimento

- **Nome do movimento:** uma frase de descrição. - **Gatilho:** quando isso ocorre (por exemplo, "quando o herói está Perto", "quando alguém atira de cobertura"). - **Teste:** qual atributo e qual Dificuldade. - **Consequência do fracasso:** o que você perde, o que muda. - **Consequência do sucesso:** geralmente você evita a consequência ou ganha uma vantagem.

### 7.2 Como determinar a Dificuldade de movimento do inimigo (sem tabelas)

Se o movimento for 'ofensivo' e direcionado a um único alvo:
- defina **T do movimento = Defesa do inimigo** (isso é consistente e fácil de lembrar).

Se o movimento for em área ou 'grande':
- defina T um nível acima do padrão da cena (normalmente **T 6** ou **T 8**).

### 7.3 Movimentos Exemplares (módulos)

**Investida (Brute)**  
- **Descrição:** o inimigo entra em combate corpo a corpo e empurra.  
- **Gatilho:** quando o inimigo está Perto do herói.  
- **Teste:** o herói faz um teste de **F ou D** contra **Dificuldade = Defesa do inimigo**.  
- **Falha:** o herói perde 1 Coração *ou* é empurrado para 1 zona (o Mestre do Jogo escolhe o que faz sentido).  
- **Sucesso:** evita danos e mantém a posição.

**Rajada (Artillery)**  
- **Descrição:** uma série de tiros/estilhaços em uma área.  
- **Gatilho:** quando pelo menos 2 heróis estão na mesma zona e não estão em cobertura.  
- **Teste:** cada alvo testa **D** contra **Dificuldade 6** (ou Dificuldade = Defesa do inimigo, se o inimigo for uma elite).  
- **Falha:** −1 Coração e 



---

### 8.1 Padrão: zonas de distância

Em combate descritivo, use: **Perto / Longe / Muito longe / Extremamente longe**.

No bloco de estatísticas, registre a mobilidade como:
- "**Mobilidade:** muda de zona em 1 (padrão)"
- ou "**Mobilidade:** Rápido (muda de zona em 2)"
- ou "**Mobilidade:** Voa (ignora obstáculos, mas exige testes durante ataques aéreos)".

### 8.2 Opção: grade (se a mesa gostar de tática)

Se vocês estiverem jogando em um mapa: 
- movimento padrão = **5 quadrados**, 
- Rápido = **6–7**, 
- Salto = 3 quadrados "verticalmente" ou sobre obstáculos. 

**Todas as habilidades descritivas funcionam da mesma forma** — a grade apenas "fornece uma medida métrica".



---

### 9. Construção de Oponente em 2 Minutos (Procedimento)

1) **Escolha a classe**: Pajem / Elite / Chefe.
2) **Defina Defesa**: 5 / 6 / 8 (lendário: 12).
3) **Defina Corações**: 1 / 2 / 3 (final: 5).
4) **Escolha o papel**: Bruto / Espadachim / Artilharia / Controlador / Suporte.
5) **Adicione 1–2 características passivas** (chefe: 2–3).
6) **Adicione movimentos**: Elite 1, Chefe 2–3.
7) **Escreva a tática em 2 frases** (primeira rodada + reação à ameaça).
8) (Opcional) Adicione **fraqueza** e **recompensa**.

> Teste prático: se você consegue conduzir o inimigo sem olhar para a tabela — o bloco de estatísticas está bom.



---

### 10. Templates prontos (para reskin em qualquer mundo)

As entradas a seguir são propositalmente "sem cor". Você muda o nome e a descrição — a mecânica permanece.

### 10.1 Peões

- **Guarda — Peão, Defesa 5, Corações 1, Bruto, Mobilidade: padrão, Habilidades: Escudo, Movimentos: Impulso, Tática: bloqueia e empurra.**
- **Explorador — Peão, Defesa 5, Corações 1, Combatente, Mobilidade: Rápida, Habilidades: Explorador, Movimentos: Fuga, Tática: aproxima-se, marca alvos e desaparece.**
- **Atirador — Peão, Defesa 5, Corações 1, Artilheiro, Mobilidade: padrão, Habilidades: Cobertura, Movimentos: Tiroteio, Tática: mantém à Distância e força a correr.**
- **Controlador — Peão, Defesa 5, Corações 1, Controlador, Mobilidade: padrão, Habilidades: Área, Movimentos: Âncora, Tática: divide a equipe.**
- **Apoio — Peão, Defesa 5, Corações 1, Suporte, Mobilidade: padrão, Habilidades: <span class="rpg-token token-stat">M</span>édico, Movimentos: Reforço, Tática: protege a elite.**

**Movimentos rápidos para peões:**
- **Fuga:** quando atingido (mas ainda "não eliminado" na ficção, por exemplo, armadura), afasta-se 1 zona.
- **Tiroteio:** se alguém está em campo aberto, dá-lhe desvantagem na próxima ação ("balas, estilhaços, medo").
- **Área:** uma vez por cena, cria uma pequena área de dificuldade (fumaça, óleo, lama).

### 10.2 Elites

- **Durão — Elite, Defesa 6, Corações 2, Bruto, Mobilidade: padrão, Habilidades: Armadura Leve, Movimentos: Investida, Tática: aproxima-se e segura a linha.**
- **Assassino — Elite, Defesa 6, Corações 2, Skirmisher, Mobilidade: Rápido + Saltador, Habilidades: Explorador, Movimentos: Corte de flanco, Tática: ataca pela retaguarda e recua.**
- **Sniper — Elite, Defesa 6, Corações 2, Artilharia, Mobilidade: Distante, Habilidades: Cobertura, Movimentos: Tiro preciso, Tática: força o movimento e pune a falta de cobertura.**
- **Manipulador de Terreno — Elite, Defesa 6, Corações 2, Controlador, Mobilidade: padrão, Habilidades: Zona (2×), Movimentos: Âncora, Tática: corta o caminho de fuga.**
- **Comandante — Elite, Defesa 6, Corações 2, Suporte, Mobilidade: padrão, Habilidades: Sentinelas, Movimentos: Reforço, Tática: fortalece aliados e posiciona-os em coberturas.**

### 10.3 Chefes

- **Líder — Chefe, Defesa 8, Corações 3, Suporte, Mobilidade: padrão, Habilidades: Vigia + Escudo, Movimentos: Reforço + Evocação + Barreira, Tática: mantém o suporte e controla o ritmo.** - **Colosso — Chefe, Defesa 8, Corações 3, Bruto, Mobilidade: padrão, Habilidades: Resistência + Armadura Pesada, Movimentos: Abalo + Avanço, Tática: quebra a formação e força testes.** - **Caçador — Chefe, Defesa 8, Corações 3, Atirador, Mobilidade: Rápido + Saltador, Habilidades: Explorador, Movimentos: Emboscada + Corte + Fuga, Tática: isola e elimina.** - **Arquiteto das Zonas — Chefe, Defesa 8, Corações 3, Controlador, Mobilidade: padrão, Habilidades: Zona (2×) + Resistência [tipo], Movimentos: Âncora + Salva + Deslocamento, Tática: divide a equipe e força decisões.**



---

### 11. Ameaças Ambientais (Riscos)

Perigo é um 'adversário sem vontade' ou um mecanismo de cena: torre de vigilância, fogo, avalanche, alarme.

**Formato: Nome — Dificuldade (D), Quando atua, Efeito, Como desativar / evitar**

### 11.1 Exemplos de Perigos (universais)

**Torreta / Drone de defesa — D 6**
- **Quando ativa:** no final da rodada, se alguém estiver na linha.
- **Efeito:** teste **A vs D 6**; falha: −1 Coração e você deve procurar cobertura.
- **Desativação:** teste **<span class="rpg-token token-stat">P</span> ou A vs D 6** no painel / interferência / desligamento de energia.

**Armadilha / Mina / Laço — D 5**
- **Quando ativa:** ao entrar na área.
- **Efeito:** teste **A vs D 5**; falha: −1 Coração ou imobilização (você perde movimento).
- **Desativação:** ferramentas + teste **A vs D 4–5**.

**Gás / Fumaça / Contaminação — D 5**
- **Quando ativa:** no início do turno, se você estiver na área.
- **Efeito:** teste **R ou <span class="rpg-token token-stat">P</span> vs D 5**; falha: −1 Coração ou dificuldade nos testes para sair.
- **Desativação:** ventilação, máscaras, vedação.

**Alarme / Contagem regressiva — D (dependendo da cena)**
- **Quando ativa:** quando ocorre uma complicação ou alguém faz barulho.
- **Efeito:** surge pressão de tempo (próxima onda, porta trancada, reforços).
- **Desativação:** teste **<span class="rpg-token token-stat">P</span>** (hack/ritual) ou “fisicamente” teste **R/A**.



---

### 12. Gerador de cena de combate (rápido, claro)

Escolha 1 de cada linha (ou jogue <span class="rpg-token token-<span class="rpg-token token-d6">d6</span>"><span class="rpg-token token-d6">d6</span></span>):

1) **Objetivo da cena:** passagem / recuperação / desativação / escolta / roubo / defesa  
2) **Terreno:** aberto / gargalos / multi-nível / muitas coberturas / bordas / neblina-fumaça  
3) **Oponentes:** 6× capanga / 4× capanga + elite / 2× elite / chefe / chefe + 2× capanga / elite + risco  
4) **Vantagem do inimigo:** cobertura / altura / mobilidade / tempo limitado / emboscada / apoio à distância  
5) **Vantagem dos jogadores:** surpresa / ferramentas / atalho / aliado neutro / terreno oferece cobertura / informação (sabem quem é o inimigo)



---

### 13. Equilíbrio na prática (sem matemática)

No NDE, o equilíbrio é feito com *ritmo* e *pressão*, e não com 'CR'.

### 13.1 Regras rápidas para definir a dificuldade da cena

- **Cena fácil:** 4–6 lacaios ou 1 elite.  
- **Cena padrão:** 4 lacaios + 1 elite, ou 2 elites.  
- **Cena difícil:** chefe + 2–4 lacaios, ou chefe + perigo.  
- **Final:** chefe (5 Corações) + elite + pressão de tempo.

### 13.2 Se a luta estiver durando pouco

- Envie uma **onda de lacaios** (2–3 por rodada durante 2 rodadas).  
- Aumente a pressão do terreno: área de fumaça, alarme, falta de cobertura.  
- Mude a tática: o inimigo deixa de lutar "honestamente" (recuar, pegar um refém, bloquear a saída).

### 13.3 Se a luta se prolongar

- Dê aos jogadores uma "alavanca": um tanque exposto, painel, ritual, fraqueza. - Permita **benefícios por sucesso excepcional**: quebrar cobertura, desarmar, dispersar suporte. - Reduza o número de Corações do chefe de 5 para 3, se não for a final.



---

### 14. Reskin: como transformar um inimigo para cada ambientação

Você tem o bloco de estatísticas 'Explorador'. Agora, você só precisa mudar a descrição:

- **Fantasia:** arqueiro goblin explorador (Explorador + Tiro).  
- **Ficção científica:** drone de reconhecimento (Explorador + Sensores).  
- **Cyberpunk:** batedor de gangue de skate (Rápido + Escape).  
- **Eslavo:** demônio que segue trilhas (Vulnerabilidade: ferro; Resistência: medo).

A mecânica permanece a mesma. Isso permite que a comunidade adicione centenas de entradas sem comprometer a coesão do núcleo.

