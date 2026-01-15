---
pdf_options:
  displayHeaderFooter: true
  headerTemplate: |-
    <div style="font-size: 8px; width: 100%; text-align: center; color: #b91c1c; font-family: 'Cinzel', serif; font-weight: 700; letter-spacing: 1px; padding-bottom: 5px;">
      NANO DUNGEON ENGINE v1.4
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
generated_at: "2026-01-15T08:02:46.231Z"
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
# Livro de Regras Básicas



---



---

### Coisas necessárias para o jogo

- Lápis e ficha de personagem.
- (Opcional) mapa/rede quadriculada e marcadores de personagem (papel quadriculado, tapete, VTT).
- Dados: **<span class="rpg-token token-d4">k4</span>, <span class="rpg-token token-d6">k6</span>, <span class="rpg-token token-d8">k8</span>, <span class="rpg-token token-d12">k12</span>, <span class="rpg-token token-d20">k20</span>**.
  - Na prática, basta **um de cada** (rola-se um dado por vez).
  - (Opcional) **k100** para tabelas aleatórias ou geradores.
- Se você tiver apenas **<span class="rpg-token token-d6">k6</span>**, use a variante **2k6** (no final).

---



---

### Dicionário de termos


Te palavras aparecem nas regras — aqui estão explicadas "de forma simples":

- **MJ (Mestre de Jogo)**: conduz o mundo, descreve situações, controla os oponentes, determina a Dificuldade e as consequências.
- **Jogador**: descreve as ações de seu personagem e realiza os testes.
- **Teste**: rolagem de dados que resolve um resultado incerto.
- **Atributos**: **Força (F)**, **Destreza (D)**, **Poder (<span class="rpg-token token-stat">P</span>)**. Dizem, *qual dado você rola*.
- **Dado de atributo**: tamanho do dado atribuído ao atributo (por exemplo, D = <span class="rpg-token token-d12">d12</span>).
- **Dificuldade (D)**: número que deve ser alcançado ou superado para que a ação tenha sucesso.
- **Sucesso**: resultado ≥ Dificuldade.
- **Sucesso excepcional**: **resultado máximo** no dado (por exemplo, 12 em <span class="rpg-token token-d12">d12</span>, 20 em <span class="rpg-token token-d20">d20</span>) — sucesso + benefício adicional.
- **Complicação**: problema adicional após uma falha (barulho, perda de tempo, pior posição, perda de recurso).
- **Sucesso com custo**: a ação tem sucesso, mas você paga um preço (compromisso, perda de recurso, revelação, risco).
- **Sorte (<span class="rpg-token token-stat">S</span>)**: recurso limitado que permite salvar cenas (rerolagem / aumento de dado / troca de falha por sucesso com custo).
- **Corações**: "vida" do personagem (resistência, ferimentos, condição — dependendo do mundo).
- **Pontos de Poder (PP)**: recurso para poderes e jogadas "acima do padrão" (magia, psionismo, gadgets, ações "cinematográficas").
- **Defesa**: limiar para atingir o oponente em combate (em vez de multiplicar regras sobre armadura, classe de armadura, etc.).
- **Obstáculo**: barreira entre você e o alvo. Geralmente dificulta ataques à distância ou ações de observação.

---



---

### 1. Personagem


Tworção de personagem é rápida. Um personagem é: **conceito + papel + características + recursos + equipamento**.

---

### 1.1 Conceito

Uma frase: quem você é e em que gênero você joga.

> Exemplo: "Era uma agente corporativa, hoje caçadora de recompensas, que age nas sombras e não confia em ninguém."


### 1.2 Papel (escolha um)


Role são intencionalmente "neutras para o mundo". Em fantasia você pode chamá-las de outra forma, em cyberpunk de outra, mas funcionam da mesma maneira.

- **Ataque** — pressão, combate, superação de obstáculos, rompimento de linhas.
- **Especialista** — furtividade, precisão, técnica, observação, planejamento.
- **Adept** — poderes, influência, conhecimento, improvisação (magia/psionismo/tecnologia dependendo do mundo).


### 1.3 Atributos e Dados


Você tem três atributos:

- **Força (F)** — força física, resistência, combate corpo a corpo, esforço.
- **Destreza (D)** — reflexos, precisão, furtividade, tiro, condução.
- **Poder (<span class="rpg-token token-stat">P</span>)** — "o que é especial": magia, psionismo, tecnologia avançada, blefe social, intuição — dependendo da convenção.

**No início, distribua os dados assim:**
- um atributo tem **<span class="rpg-token token-d12">d12</span>**,
- um tem **<span class="rpg-token token-d8">d8</span>**,
- um tem **<span class="rpg-token token-d6">d6</span>**.

**Distribuição sugerida por função (mais simples):**
- **Assalto:** F <span class="rpg-token token-d12">d12</span>, D <span class="rpg-token token-d8">d8</span>, <span class="rpg-token token-stat">P</span> <span class="rpg-token token-d6">d6</span>
- **Especialista:** D <span class="rpg-token token-d12">d12</span>, <span class="rpg-token token-stat">P</span> <span class="rpg-token token-d8">d8</span>, F <span class="rpg-token token-d6">d6</span>
- **Adept:** <span class="rpg-token token-stat">P</span> <span class="rpg-token token-d12">d12</span>, D <span class="rpg-token token-d8">d8</span>, F <span class="rpg-token token-d6">d6</span>

> Exemplo: se você tem D = <span class="rpg-token token-d12">d12</span>, então ao atirar, se esconder e desviar, você geralmente rola <span class="rpg-token token-d12">d12</span>.

### 1.4 Recursos

- **Corações:** 5.
- **Pontos de Poder (PP):** 3.
- **Sorte (<span class="rpg-token token-stat">S</span>):** no início de cada sessão você tem **2 <span class="rpg-token token-stat">S</span>**.

**Sorte (como funciona):** gaste **1 <span class="rpg-token token-stat">S</span>** para escolher uma das opções:
- **Repetição** do seu teste (você mantém o melhor resultado), ou
- **Aumento do dado em 1 nível** para essa única rolagem (**<span class="rpg-token token-d6">k6</span>→<span class="rpg-token token-d8">k8</span>→<span class="rpg-token token-d12">k12</span>→<span class="rpg-token token-d20">k20</span>**), ou
- **Transformar uma falha em “sucesso com custo”** — a ação é bem-sucedida, mas o MJ imediatamente impõe um custo (por exemplo, barulho, perda de tempo, perda de recurso, pior posição, atração de atenção, dano ao equipamento).

**Recuperação de <span class="rpg-token token-stat">S</span>:** no início da próxima sessão, você retorna ao limite. O MJ pode conceder **+1 <span class="rpg-token token-stat">S</span>** por risco ousado, excelente decisão narrativa ou por jogar com as consequências.

### 1.5 Talentos (opcionais, mas recomendados)

Talentos são **2 frases curtas** que descrevem em que sua personagem é boa (sem listas, sem tabelas).

- Exemplos: "Mecânico", "Explorador", "Negociador", "<span class="rpg-token token-stat">M</span>édico", "Hacker", "Veterano", "Descobridor".

**Como funcionam os Talentos:** se o Talento realmente ajudar em um teste, o MJ pode **aumentar o dado em 1 grau** (ou neutralizar a dificuldade).
- Talento não garante sucessos automáticos.
- Normalmente, **no máximo 1 Talento** influencia um teste.

### 1.6 Equipamento

Liste:
- 1 ferramenta "chave" (arma / conjunto / equipamento, sem o qual você não faz seu trabalho),
- 1 proteção (armadura, escudo, camuflagem — dependendo do mundo),
- 3 pequenos itens úteis na aventura.

O equipamento nas regras básicas é principalmente **uma permissão** (possibilita ações), e não um bônus numérico.

### 1.7 Exemplo de personagem completo

- Conceito: "Ladrã de informações que rouba dados de sistemas, e não de bolsos."
- Papel: Especialista
- Atributos: <span class="rpg-token token-stat">S</span> <span class="rpg-token token-d6">k6</span>, <span class="rpg-token token-stat">Z</span> <span class="rpg-token token-d12">k12</span>, <span class="rpg-token token-stat">M</span> <span class="rpg-token token-d8">k8</span>
- Recursos: 5 Corações, 3 <span class="rpg-token token-power">PM</span>, 2 LP
- Talentos: "Hacker", "Sombra"
- Equipamento: pistola, armadura leve, kit de arrombamento, corda, lanterna

---



---

### 2. Núcleo das regras: testes

Esta parte é a mais importante — se você a entende, entende o sistema.

### 2.1 Quando você faz um teste


Você faz um teste quando ambas as condições são atendidas:
1) o resultado é incerto (pode dar certo ou não), e
2) a aposta é real (uma falha muda algo / custa algo).

Se a ação for banal e sem pressão — o MJ pode dizer "deu certo" sem rolar.

### 2.2 Como realizar um teste (passo a passo)

1) O jogador diz **o que faz** e **por que**.
2) O mestre de jogo escolhe um atributo: **<span class="rpg-token token-stat">S</span>** ou **<span class="rpg-token token-stat">Z</span>** ou **<span class="rpg-token token-stat">M</span>**.
3) O mestre de jogo determina a **Dificuldade (D)** e diz o que significa falha (aposta).
4) O jogador rola **o dado do atributo**.
5) Compare o resultado com D e resolva as consequências.

### 2.3 Dificuldades (T)


Usamos limiares simples. Se você tiver dúvidas — escolha um limiar mais baixo, e a "dificuldade" será mostrada pela consequência.

- **T 3** – fácil (quase certeza, mas às vezes vale a pena verificar sob pressão)
- **T 4** – padrão (desafio típico)
- **T 5** – difícil (exige competência ou vantagem)
- **T 6** – muito difícil (sem vantagem é arriscado)
- **T 8** – heroico (para os melhores ou após boa preparação)
- **T 12** – lendário (raramente "limpo"; geralmente como um objetivo de campanha, plano, ritual, grandes condições)


### 2.4 Resultados do teste

- **Resultado ≥ T → Sucesso.** Você alcança o efeito desejado.
- **Resultado < T → Falha.** Você não alcança o efeito, e a situação muda (complicação ou custo).
- **Rolou 1 → Falha + complicação.** A complicação entra com certeza.
- **Resultado máximo nos dados → Sucesso excepcional.**
  - Além do sucesso, você recebe **um benefício adicional** (mais rápido, mais silencioso, mais forte, mais seguro, efeito adicional).

> Exemplo de sucesso com custo: "Você conseguiu forçar a porta, mas fez barulho e alguém vem verificar."

### 2.5 Facilidades e Dificuldades (sem contagem)


Zamiast dodawać +1/−1 do rzutów, zmieniamy **tamanho do dado**.

- **Situação Favorável** → **aumente o dado em 1 grau**  
<span class="rpg-token token-d6">k6</span> → <span class="rpg-token token-d8">k8</span> → <span class="rpg-token token-d12">k12</span> → <span class="rpg-token token-d20">k20</span>
- **Situação Desfavorável** → **reduza o dado em 1 grau**  
<span class="rpg-token token-d20">k20</span> → <span class="rpg-token token-d12">k12</span> → <span class="rpg-token token-d8">k8</span> → <span class="rpg-token token-d6">k6</span> → <span class="rpg-token token-d4">k4</span>

**Exemplos de facilidades:** preparação, boas ferramentas, vantagem de posição, surpresa, apoio.  
**Exemplos de dificuldades:** escuridão, escorregadio, pressão do tempo, barulho, distração, cobertura.

**Regra de Ordem:** para rapidez, assuma que para um único teste você geralmente aplica **no máximo 1 facilidade e 1 dificuldade** (podem se cancelar).

### 2.6 Ajuda do Aliado

Um aliado pode sacrificar sua ação (ou tempo na cena fora de combate) para ajudar.

**Efeito:** para este único teste, **aumente o dado em 1 grau**.

A ajuda deve ser descrita de forma sensata (cobertura, fornecimento de ferramentas, distração, estabilização, dicas).

### 2.7 Repetição de Testes


Se o teste falhar, não o repita "sem parar" sem mudar a situação.
- Ou você faz algo diferente (outra característica / outras ferramentas / outro caminho),
- ou você aceita o custo (tempo, alarme, recurso),
- ou você recua.

### 2.8 Exemplos de testes (fora de combate)

**Exemplo A — passagem silenciosa**
- Jogador: "Vou atravessar o pátio antes que o holofote volte."
- MJ: Agilidade (A). É sob pressão do tempo → Dificuldade **D 5**.
- O personagem tem o Talento "Sombra" → facilidade, dado aumentado em 1 grau.
- Rolagem: D <span class="rpg-token token-d12">d12</span> = 4 → falha. MJ: "Eles não te notam imediatamente, mas alguém ouve um ruído e começa a verificar a área (complicação: a pressão aumenta)."

**Exemplo B — forçar com força**
- Jogador: "Vou arrombar a porta de metal antes que a segurança chegue na esquina."
- MJ: Força (F), Dificuldade **D 6** (muito difícil sem ferramentas).
- Alguém ajuda, segurando a fechadura e fazendo pressão na porta → dado aumentado em 1 grau.
- Rolagem: F <span class="rpg-token token-d12">d12</span> = 12 → sucesso excepcional: a porta se abre imediatamente e você faz isso mais silenciosamente do que se esperava.



---

### 3. Movimento e distâncias (a grade é uma opção)

Por padrão, o NDE funciona sem um mapa: você descreve a cena e as posições dos personagens.

### 3.1 Padrão: distâncias descritivas


Usem quatro zonas:
- **Perto** — ao alcance da mão, combate corpo a corpo.
- **Não muito longe** — alguns passos, fácil aproximação.
- **Longe** — do outro lado da cena, requer um deslocamento claro.
- **Muito longe** — de sniper/veicular/"na borda da cena".

Em um turno, geralmente você pode mudar a distância em **uma zona** (por exemplo, Longe → Não muito longe).

### 3.2 Opção: jogo em grade (para táticas)


Se vocês preferem concretude:
- 1 quadrado = 1–2 m.
- Movimento na rodada: **até 5 quadrados**.
- Diagonais são permitidas (contam como um quadrado normal).


### 3.3 Cobertura e linha de ação

- **Cobertura total:** não é possível interagir "em linha" (tiro, observação, muitos poderes).
- **Cobertura parcial:** dificulta — geralmente **reduz o dado em 1 grau** para o atacante/observador.

---



---

### 4. Combate

Combate é uma cena comum com testes, apenas organizada em turnos.

### 4.1 Quando a luta começa

A luta começa quando:
- pelo menos uma das partes deseja ferir a outra, e
- é importante quem e quando age.

Se a situação for curta e óbvia, o Mestre do Jogo pode resolvê-la com um único teste.

### 4.2 Ordem das Turnos (versão simples)


O mais simples:
- Primeiro, todos os jogadores agem (em qualquer ordem),
- depois agem os oponentes,
- e assim por diante em um loop.

### 4.3 O que você faz na sua rodada


Na sua rodada, você tem:
- **Movimento** (mudança de zona / até 5 quadrados na variante de grade),
- **1 Ação** (ataque, teste, ajuda, uso de poder, equipamento, interação com o cenário).


### 4.4 Ataque: como funciona

1) Escolha um alvo e descreva o ataque.
2) Escolha um atributo:
   - **corpo a corpo** → teste de **Força (F)**,
   - **distância** → teste de **Destreza (D)**,
   - **poderes** → normalmente teste de **Poder (<span class="rpg-token token-stat">P</span>)** (veja o capítulo 5).
3) Determine a **Defesa** do alvo.
4) Role o dado e compare com a Defesa.

### 4.6 Dano e 'quanto aguentam'

- Um acerto causa **1 Coração**.
- **Sucesso excepcional** causa **2 Corações** *ou* provoca um efeito forte (desarmar, derrubar, empurrar para fora da cobertura) — escolha um.

Os arquetipos mais simples de inimigos:
- **Peão:** cai após 1 acerto.
- **Elite:** tem **2 Corações**.
- **Chefe:** tem **3 Corações** (ou 5 em cenas finais).

> Nota: "cai" não precisa significar morte. Pode estar inconsciente, ter fugido, se rendido, ou ter sido removido da ação.

### 4.5 Defesa dos Oponentes (orientativamente)

- **Fraco:** Defesa **4**
- **Típico:** Defesa **5**
- **Elite:** Defesa **6**
- **Chefe:** Defesa **8** (chefe lendário: **12**)

A cobertura e as condições geralmente alteram o tamanho dos dados do atacante (facilitações/dificuldades), e não a Defesa.

### 5.7 Alcance dos ataques (padrão)
Para não multiplicar números, use regras simples:
- Corpo a corpo: alvo na casa vizinha.
- Distância: alvo em "alcance visual" no tabuleiro.
  - Se o MJ quiser limitações: considere **até 10 casas** sem penalidade; acima de 10 casas <span class="rpg-token token-<span class="rpg-token token-math">tn</span>"><span class="rpg-token token-math">TN</span></span> +1 grau.

### 5.8 Vários oponentes ao mesmo tempo
Se vários lacaios estiverem "em combate" com uma única personagem, o GM pode:
- aumentar a <span class="rpg-token token-<span class="rpg-token token-math">tn</span>"><span class="rpg-token token-math">TN</span></span> em 1 grau (pressão), ou
- considerar que a falha significa uma complicação adicional (por exemplo, você perde a posição).

A regra deve ser rápida: **uma resolução → um efeito**.

### 4.7 Exemplos de combate

**Exemplo A — combate corpo a corpo com um capanga**
- Assaltante (<span class="rpg-token token-stat">S</span> <span class="rpg-token token-d12">k12</span>) ataca o capanga (Defesa 5).
- As condições são boas (surpresa) → o dado é aumentado em 1 grau, mas já é <span class="rpg-token token-d12">k12</span>, então o aumento dá <span class="rpg-token token-d20">k20</span>.
- Rolagem <span class="rpg-token token-d20">k20</span> = 7 → acerto, o capanga cai.

**Exemplo B — tiro na elite de trás de uma cobertura**
- Especialista (<span class="rpg-token token-stat">Z</span> <span class="rpg-token token-d12">k12</span>) atira na elite (Defesa 6).
- O alvo está parcialmente coberto → dificuldade, o dado cai para <span class="rpg-token token-d8">k8</span>.
- Rolagem <span class="rpg-token token-d8">k8</span> = 6 → acerto, a elite perde 1 Coração (fica com 1).

**Exemplo C — chefe e Sorte**
- Adepto (<span class="rpg-token token-stat">M</span> <span class="rpg-token token-d12">k12</span>) tenta desabilitar o chefe (Defesa 8) com poder.
- Rolagem <span class="rpg-token token-d12">k12</span> = 4 → falha. O jogador gasta 1 LS para rerolar.
- Reroll = 10 → sucesso. O chefe perde 1 Coração, mas o MJ adiciona o custo: “o efeito é barulhento, o alarme dispara.”



---

### 5. Poderes (<span class="rpg-token token-stat">P</span>) e Pontos de Poder (PP)

No NDE, "Poder" é uma categoria de efeitos especiais. Dependendo do mundo, pode significar:
- magia, psionismo, rituais,
- tecnologia avançada, drones, hacking "ao vivo",
- jogadas cinematográficas de heróis (por exemplo, "concentração magistral"),
- influência social em jogos onde a conversa é "poder".

### 5.1 Quando você gasta <span class="rpg-token token-power">PM</span>


Você gasta <span class="rpg-token token-power">PM</span> quando tenta obter um efeito **acima do padrão**.

---

### 5.2 Como usar o poder (passo a passo)

1) Descreva o efeito que você deseja obter.
2) O GM determina a Dificuldade e o custo de <span class="rpg-token token-power">PM</span>.
3) Gaste <span class="rpg-token token-power">PM</span>.
4) Role **<span class="rpg-token token-stat">M</span>** e compare com a Dificuldade.

**Falha:** o efeito não funciona; <span class="rpg-token token-power">PM</span> é perdido; uma complicação ocorre (sobrecarga, rastro, revelação, efeito colateral).

### 5.3 Níveis de Efeitos (Dificuldade / Custo)

- **Truque** (truque curto): **D 4 / 0–1 <span class="rpg-token token-power">PM</span>**  
  luz, som, pequena cortina, distração momentânea.
- **Padrão**: **D 5 / 1 <span class="rpg-token token-power">PM</span>**  
  projétil, escudo, impulso, salto, fortalecimento.
- **Forte**: **D 6 / 2 <span class="rpg-token token-power">PM</span>**  
  área, controle, cura, paralisia, "hack durante a luta".
- **Grande**: **D 8–12 / 3 <span class="rpg-token token-power">PM</span>**  
  efeito que muda a cena ou tem consequências de campanha.

### 5.4 Sucesso excepcional em poder

Se você tirar o máximo nos dados <span class="rpg-token token-stat">M</span>:
- aumente a escala (maior área / mais tempo / mais forte), ou
- adicione um benefício adicional (mais silencioso, mais preciso, mais seguro), ou
- o GM pode devolver **1 <span class="rpg-token token-power">PM</span>** (se se encaixar na ficção).

### 5.5 Recuperação de <span class="rpg-token token-power">PM</span>

- Após a cena de conflito, você recupera **1 <span class="rpg-token token-power">PM</span>**.
- Após um descanso seguro, você volta ao total.

### 5.6 Exemplos de Poderes

**Exemplo A — escudo para correr**
- Jogador: "Coloco uma proteção curta para correr até uma posição melhor."
- MJ: Padrão **D 5**, custo 1 <span class="rpg-token token-power">PM</span>.
- Rolagem <span class="rpg-token token-stat">M</span> <span class="rpg-token token-d12">d12</span> = 9 → sucesso: você corre em segurança.

**Exemplo B — falha com consequência**
- Jogador: "Impedir a elite no lugar."
- MJ: Forte **D 6**, custo 2 <span class="rpg-token token-power">PM</span>.
- Rolagem = 1 → falha + complicação: você perde 2 <span class="rpg-token token-power">PM</span>, e o efeito se reflete e revela sua posição.



---

### 6.1 0 Corações

Se você cair para 0 Corações:
- você está **desligado da ação** (ferido, atordoado, em choque — dependendo da convenção),
- um aliado pode sacrificar uma ação para te colocar de pé com **1 Coração**.

### 6.2 Descanso

- Após uma cena de conflito, se vocês tiverem um momento de descanso e condições básicas, podem retornar a seus Corpos Plenos.
- Em campanhas mais severas, o Mestre de Jogo pode exigir um local seguro para retornar à plenitude.

### 7.3 Descanso
Após uma cena de luta/conflito, se vocês tiverem um momento de descanso seguro (e as condições básicas), vocês retornam à plenitude:
- Corações,
- Mana.

Isso mantém o sistema ágil e não requer longos períodos de cura.



---

### 7. Desenvolvimento de Personagem

**Quando você cresce:** após uma aventura, missão ou importante capítulo da história (geralmente a cada 1–3 sessões).

Escolha **uma**:
- **Aumente** uma característica em 1 grau de dado (máx. até <span class="rpg-token token-d20">k20</span>), ou
- **+1 Coração** (máx. 7), ou
- **+1 <span class="rpg-token token-power">PM</span>** (máx. 5), ou
- **Novo Traço** (uma habilidade específica acordada com o GM).

> Exemplo: O especialista aumenta <span class="rpg-token token-stat">Z</span> de <span class="rpg-token token-d12">k12</span> para <span class="rpg-token token-d20">k20</span>, pois a campanha entrou na fase de perseguições e tiroteios.

---



---

### 8. Variante apenas <span class="rpg-token token-d6">k6</span>: 2k6

Se você não quiser usar diferentes dados, jogue com **2k6**.

### 8.1 Atributos como modificadores

Em vez de tamanhos de dados, divida os modificadores:
- um atributo tem **+2**
- um tem **+1**
- um tem **+0**

### 8.2 Teste


Rola **2d6 + modificador de atributo**.

**Resultado:**
- **6 ou menos** – falha com consequência
- **7–9** – sucesso com custo
- **10+** – sucesso completo
- **12** – sucesso excepcional (benefício adicional)


### 8.3 Dificuldade da Situação

Em vez de mudar os limiares, conceda:
- **+1** por vantagem, preparação, bom plano,
- **−1** por dificuldades, pressão, cobertura, caos.

### 8.4 Sorte de Sorte em 2k6


Gaste 1 Ponto de Sorte para:
- rerrolar 2k6, ou
- adicionar **+1** ao resultado do teste, ou
- transformar uma falha em sucesso com custo.

### 8.5 Mapeamento Rápido (opcional)

Se um dia você quiser "converter" um personagem entre variantes:
- <span class="rpg-token token-d6">k6</span> ≈ +0
- <span class="rpg-token token-d8">k8</span> ≈ +1
- <span class="rpg-token token-d12">k12</span> ≈ +2
- <span class="rpg-token token-d20">k20</span> ≈ +3 (para muito experientes)

---



---

[<span class="rpg-token token-math">PT</span>] Conteúdo em breve...




---

### 1. Introdução

7.2 Esses complementos não são obrigatórios, mas às vezes facilitam a condução.

### 9.1 Proteção (armadura) como um recurso simples


Se você quer que a "proteção" tenha um efeito claro:
- a personagem com proteção tem **1 ficha de Armadura por cena**,
- quando ela deveria perder 1 Coração, pode em vez disso gastar uma ficha de Armadura.

### 9.2 Pressão do tempo como cronômetro

Se a cena tiver um limite de tempo, o GM estabelece um "contador" (por exemplo, 3 passos). Cada falha move o contador em 1. Quando chegar ao fim — uma consequência ocorre (alarme, fuga do alvo, colapso da passagem).

---

### 9.3 Retaliação (variante de combate arriscado)

Se você quer que a luta seja mais "afiada" e rápida:
- quando **ataca corpo a corpo** e **erra**, você perde **1 Coração**, desde que o oponente pudesse realmente atingi-lo.
Isso é uma variante — no núcleo do NDE, as consequências das falhas em combate resultam principalmente da ficção e das decisões do GM.

