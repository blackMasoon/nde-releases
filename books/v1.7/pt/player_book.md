---
pdf_options:
  displayHeaderFooter: true
  headerTemplate: |-
    <div style="font-size: 8px; width: 100%; text-align: center; color: #b91c1c; font-family: 'Cinzel', serif; font-weight: 700; letter-spacing: 1px; padding-bottom: 5px;">
      NANO DUNGEON ENGINE v1.7
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
generated_at: "2026-01-16T10:17:16.276Z"
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
# Manual do Jogador

Automatic translation placeholder for <span class="rpg-token token-math">pt</span>

---



---

### 1) Como é o jogo na mesa

- **Mestre do Jogo (MJ)** descreve a situação e diz o que é possível nesta cena. - **Você** diz: **o que faz** e **qual efeito deseja**. - Se o resultado for incerto ou arriscado, o MJ diz: 1) **qual atributo** você usa (F/I/C), 2) **qual é a Dificuldade** <span class="rpg-token token-t">D</span> (ou **Defesa** do alvo), 3) **o que ameaça em caso de falha** (consequência). Depois você lança o dado de atributo e imediatamente sabem o que acontece em seguida.

### A Regra Mais Curta

**Jogue o dado de atributo. Resultado ≥ <span class="rpg-token token-t">T</span> = sucesso.**



---

### 2) O que seu personagem tem

Seu personagem tem: - **Conceito** (1 frase: quem você é, em que mundo você atua), - **Papel** (Assalto / Especialista / Adepto), - 3 **atributos**: Força (F), Destreza (D), Poder (<span class="rpg-token token-stat">P</span>), - **Corações** (resistência) e **Pontos de Poder** (PP), - **Golpe de Sorte** (GS), - (opcionalmente) **Talentos**, - **equipamento**.

### 2.1 Características (F/D/<span class="rpg-token token-stat">P</span>) — para que servem

- **Força (F)**: combate corpo a corpo, arrombar, carregar, resistência. - **Destreza (D)**: tiro, precisão, furtividade, esquiva, acrobacia, condução de veículos. - **Poder (<span class="rpg-token token-stat">P</span>)**: "efeitos especiais" do mundo do jogo: magia, psionismo, fé, supertecnologia, hacking, influência, intuição — dependendo da convenção.

### 2.2 Dados de características — como funcionam

Cada característica tem um dado: <span class="rpg-token token-<span class="rpg-token token-d4">k4</span>"><span class="rpg-token token-d4">d4</span></span>, <span class="rpg-token token-<span class="rpg-token token-d6">k6</span>"><span class="rpg-token token-d6">d6</span></span>, <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">d8</span></span>, <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">d12</span></span> ou <span class="rpg-token token-<span class="rpg-token token-d20">k20</span>"><span class="rpg-token token-d20">d20</span></span>.  
Quando você usa uma característica, você lança **um dado** dessa característica.

- Dado maior = maior chance de sucesso e de sucesso excepcional (máximo no dado).

**Exemplo:** Você tem Destreza <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">d8</span></span>. Quando atira, escala ou se esgueira, geralmente você lança <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">d8</span></span>.

### 2.3 Recursos: Corações, Pontos de Poder e Golpes de Sorte

- **Corações:** 5 no início. Acertos e pressão tiram Corações.
- **Pontos de Poder (PP):** 3 no início. Você gasta-os em poderes e jogadas além do padrão.
- **Golpes de Sorte (GS):** 2 no início de cada sessão. É o seu "salvamento de cenas" e intensificação do drama.



---

### Passo 1: Conceito e papel

Escolha um papel – este é o estilo geral de ação (adequado para qualquer universo).

- **Assalto**: você se expõe ao risco e impulsiona as cenas para frente.  
  (ex.: guerreiro, fuzileiro, segurança, caçador, bárbaro)
- **Especialista**: você age com precisão, com um plano e ferramentas.  
  (ex.: ladrão, atirador de elite, batedor, hacker, piloto, rastreador)
- **Adepte**: você faz coisas 'além do padrão' – com poder, conhecimento, influência.  
  (ex.: mago, psíquico, sacerdote, alquimista, tecnomante, diplomata)

### Passo 2: Distribua os dados de atributos

Distribua os dados: um atributo <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>, um <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span>, um <span class="rpg-token token-<span class="rpg-token token-d6">k6</span>"><span class="rpg-token token-d6">k6</span></span>.

Dicas rápidas:
- **Assalto** geralmente tem F no máximo.
- **Especialista** geralmente tem H no máximo.
- **Adept** geralmente tem <span class="rpg-token token-stat">M</span> no máximo.

### Passo 3: Registre os recursos

- **Corações:** 5
- **Pontos de Poder:** 3
- **Golpe de Sorte:** 2 (restaurado no início da sessão)

### Passo 4 (opcional): Escolha 2 Talentos

Talentos são palavras curtas que descrevem no que você é bom (competências que frequentemente aparecem no jogo). 
- Exemplos: "Batedor", "Mecânico", "<span class="rpg-token token-stat">M</span>édico", "Negociador", "Atleta", "Analista", "Hacker", "Ritualista".

**Como funcionam os Talentos:** se o Talento realmente ajuda no teste, o Mestre do Jogo considera isso como uma situação melhor e você pode **aumentar o dado em 1 nível** para essa rolagem.
- Normalmente 1 Talento por 1 teste.
- O Talento não substitui a descrição da ação – é para fortalecer um plano razoável.

**Exemplo:** Você tem o Talento "Mecânico" e tenta iniciar o gerador em uma situação de emergência. O Mestre do Jogo reconhece que isso ajuda: você aumenta de <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span> para <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span> para este teste.

### Etapa 5: Equipamento

Liste:
- 1 ferramenta "chave" (arma ou equipamento profissional),
- 1 proteção (armadura, escudo, camuflagem – dependendo do mundo),
- 3 itens utilitários.

O equipamento geralmente funciona como **permissão**: se você tem algo, pode tentar ações adequadas. Uma boa ferramenta também pode criar uma situação melhor (aumentar os dados), se fizer sentido.

### Exemplo de personagem (universal)

- Papel: Especialista  
- F <span class="rpg-token token-<span class="rpg-token token-d6">k6</span>"><span class="rpg-token token-d6">k6</span></span>, A <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>, <span class="rpg-token token-stat">M</span> <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span>  
- Corações 5, <span class="rpg-token token-power">PM</span> 3, VE 2  
- Talentos: "Explorador", "Negociador"  
- Equipamento: arma de longo alcance, ferramentas de arrombamento / conjunto de ferramentas, corda, lanterna

---



---

### 4.1 Quando você lança

Você lança quando: - algo é **arriscado** ou incerto, - uma falha tem **consequência significativa**. Se algo for óbvio e sem pressão, o MJ pode dizer "você consegue" sem lançar.

### 4.2 Dificuldade <span class="rpg-token token-t">T</span>

MG escolhe a Dificuldade:

- <span class="rpg-token token-t">T 3</span> fácil  
- <span class="rpg-token token-t">T 4</span> padrão  
- <span class="rpg-token token-t">T 5</span> difícil  
- <span class="rpg-token token-t">T 6</span> muito difícil  
- <span class="rpg-token token-t">T 8</span> heroico  
- <span class="rpg-token token-t">T 12</span> lendário

Você não precisa "adivinhar" a Dificuldade — o MG a diz diretamente.

### 4.3 Resultados do lançamento

- **1**: falha com consequência (a complicação certamente ocorre). - **Resultado < <span class="rpg-token token-t">T</span>**: falha (mas a cena continua). - **Resultado ≥ <span class="rpg-token token-t">T</span>**: sucesso. - **<span class="rpg-token token-stat">M</span>áximo no dado** (por exemplo, 12 em <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>, 20 em <span class="rpg-token token-<span class="rpg-token token-d20">k20</span>"><span class="rpg-token token-d20">k20</span></span>): sucesso excepcional + benefício adicional.

**Benefício adicional** (exemplos): mais rápido, mais silencioso, mais seguro, maior efeito, melhor posição, detalhe adicional a seu favor.

### 4.4 Situação melhor/pior (sem bônus)

Ao invés de contar modificadores, jogue com a situação:

- **Situação melhor** → aumente o dado em 1 nível  
  (<span class="rpg-token token-<span class="rpg-token token-d6">k6</span>"><span class="rpg-token token-d6">k6</span></span>→<span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span>→<span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>→<span class="rpg-token token-<span class="rpg-token token-d20">k20</span>"><span class="rpg-token token-d20">k20</span></span>)
- **Situação pior** → diminua o dado em 1 nível  
  (<span class="rpg-token token-<span class="rpg-token token-d20">k20</span>"><span class="rpg-token token-d20">k20</span></span>→<span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>→<span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span>→<span class="rpg-token token-<span class="rpg-token token-d6">k6</span>"><span class="rpg-token token-d6">k6</span></span>→<span class="rpg-token token-<span class="rpg-token token-d4">k4</span>"><span class="rpg-token token-d4">k4</span></span>)

Seu papel como jogador: **crie melhores condições** por meio da descrição e decisões (cobertura, preparação, ferramentas, plano, reconhecimento).

### 4.5 Ajuda do aliado

O aliado pode usar a sua Ação para ajudá-lo. Então, para aquele único lançamento:
- você aumenta o dado em 1 grau.

A ajuda deve fazer sentido na descrição (distração, cobertura, fornecer ferramentas, apoio de fogo, segundo par de mãos).

### Exemplo de teste (claro e completo)

Você quer abrir uma porta bloqueada antes que os guardas cheguem.
- MG: "É Destreza. <span class="rpg-token token-t">T 5</span>. Falha: você faz barulho e perde tempo."
- Você tem D <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">k8</span></span>, mas está usando gazuas e tem o Talento "Especialista em fechaduras" → situação melhor, aumenta para <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>.
- Rolagem <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span> = 6 → sucesso: a porta se abre sem disparar o alarme.

---



---

### 5) Sorte (<span class="rpg-token token-stat">S</span>) — quando vale a pena usá-la

No início de cada sessão, você tem **2 <span class="rpg-token token-stat">S</span>**. A <span class="rpg-token token-stat">S</span> é para:
- salvar cenas importantes,
- adicionar dramaturgia,
- recompensar decisões corajosas.

Gaste **1 <span class="rpg-token token-stat">S</span>** para escolher uma das opções:
- **Rolar novamente** seu teste (ficando com o melhor resultado), ou
- **Melhorar o dado em 1 grau** para aquele único lance, ou
- **Transformar uma falha em “sucesso com custo”** — a ação é bem-sucedida, mas o MJ imediatamente aplica um preço.

**Recuperar <span class="rpg-token token-stat">S</span>:** no início da próxima sessão, você retorna ao limite. O MJ pode conceder **+1 <span class="rpg-token token-stat">S</span>** por riscos corajosos, decisões fabulosas de enredo ou por jogar com as consequências.

**Exemplo:** Uma falha ao pular entre telhados significaria cair na rua. Você gasta 1 <span class="rpg-token token-stat">S</span> e transforma a falha em sucesso com custo: você alcança, mas perde equipamento ou torce o tornozelo (pior situação na próxima cena).



---

### 6.1 Distâncias (padrão, sem mapa)

Descreva a distância com quatro palavras:
- **Perto** (ao alcance da mão),
- **Não muito longe** (alguns passos),
- **Longe** (do outro lado da cena),
- **Muito longe** (tiro de sniper / veículo).

No turno você tem: **Deslocamento + 1 Ação**.  
O deslocamento geralmente altera a distância em 1 grau (Não muito longe→Perto etc.).

### 6.2 Opção: jogo em grade

Se vocês estiverem jogando no mapa:
- 1 quadrado = 1–2 m,
- movimento por turno: **até 5 quadrados**,
- diagonais contam como 1 quadrado,
- o restante das regras funciona de forma idêntica.

### 6.3 Ataque

- **Corpo a Corpo:** teste de **Força (F)** contra a **Defesa** do alvo.  
- **Distância:** teste de **Destreza (D)** contra a **Defesa** do alvo.

**Defesa dos oponentes (aproximadamente):**
- <span class="rpg-token token-t">4</span> Fraco  
- <span class="rpg-token token-t">5</span> Típico  
- <span class="rpg-token token-t">6</span> Elite  
- <span class="rpg-token token-t">8</span> Chefe  
- <span class="rpg-token token-t">12</span> Chefe Lendário

### 6.4 Cobertura e posição

- Alvo sob cobertura / ângulo ruim / pressão → situação pior (baixe o dado).
- Boa posição / surpresa / vantagem numérica → situação melhor (aumente o dado).

### 6.5 Acerto e dano

- Um acerto causa **1 Coração**.
- Um sucesso excepcional causa **2 Corações** ou produz um efeito forte (desarmamento, derrubada, empurrão, retirada da cobertura).

### 6.6 0 Corações

Quando você cai para **0 Corações**, está fora de ação (ferido, atordoado, em choque – conforme a convenção). - Um aliado pode usar uma Ação para colocá-lo em **1 Coração**. - Se a pressão continua, sua prioridade é proteção e evacuação, não 'tankar'.

### Exemplo de rodada curta (sem grade)

- Você está **Perto** da elite.
- Deslocamento: você se move **Perto** atrás da coluna (cobertura).
- Ação: ataque corpo a corpo (<span class="rpg-token token-stat">S</span>). A defesa da elite é <span class="rpg-token token-t">6</span>. Você tem <span class="rpg-token token-stat">S</span> <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">k12</span></span>.
  Jogada 9: sucesso, a elite perde 1 Coração.

---



---

### 7) Poderes e ações além do padrão (Pontos de Poder)

O que chamamos de "poder" depende do mundo: magia, psionismo, fé, gadgets, hacking, supertruques.

### 7.1 Como você usa o poder

1) Descreva o efeito.  
2) O MJ diz a Dificuldade e o custo em <span class="rpg-token token-power">PM</span>.  
3) Gaste <span class="rpg-token token-power">PM</span> e lance **Poder (<span class="rpg-token token-stat">P</span>)**.

### 7.2 Níveis de efeito (T / custo)

- **Truque:** efeito curto, truque → <span class="rpg-token token-t">T 4</span>, custo 0–1 <span class="rpg-token token-<span class="rpg-token token-power">pm</span>"><span class="rpg-token token-power">PM</span></span>
- **Padrão:** ataque, escudo, impulso → <span class="rpg-token token-t">T 5</span>, custo 1 <span class="rpg-token token-<span class="rpg-token token-power">pm</span>"><span class="rpg-token token-power">PM</span></span>
- **Forte:** área, cura, paralisia, hack "ao vivo" → <span class="rpg-token token-t">T 6</span>, custo 2 <span class="rpg-token token-<span class="rpg-token token-power">pm</span>"><span class="rpg-token token-power">PM</span></span>
- **Grande:** mudança de cena, intervenção poderosa → <span class="rpg-token token-t">T 8–12</span>, custo 3 <span class="rpg-token token-<span class="rpg-token token-power">pm</span>"><span class="rpg-token token-power">PM</span></span>

### 7.3 Falha e sucesso excepcional

- Falha: os <span class="rpg-token token-<span class="rpg-token token-power">pm</span>"><span class="rpg-token token-power">PM</span></span> gastos são perdidos, e a consequência ocorre (sobrecarga, rastro, perda de posição, efeito colateral). - <span class="rpg-token token-stat">M</span>áximo no dado: sucesso excepcional + benefício adicional (alcance maior, tempo prolongado, efeito mais forte, ou menos "efeitos colaterais").

### 7.4 Recuperação de <span class="rpg-token token-power">PM</span>

- Após uma cena de conflito, você recupera **1 <span class="rpg-token token-power">PM</span>**.
- Após um descanso seguro – até a capacidade máxima (se o mundo do jogo permitir).

**Exemplo (fantasia):** "Salto Curto" – Padrão, <span class="rpg-token token-t">T 5</span>, custo 1 <span class="rpg-token token-power">PM</span>.  
**Exemplo (sci-fi):** "Sobrecarga em Fechadura Eletrônica" – Padrão, <span class="rpg-token token-t">T 5</span>, custo 1 <span class="rpg-token token-power">PM</span>.



---

### 8) Descanso e Regeneração

Se vocês têm um momento seguro (abrigo, curativo, serviço, refeição):
- vocês recuperam todos os **Corações**,
- e reabastecem **<span class="rpg-token token-power">PM</span>** de acordo com a regra de descanso em sua convenção.

Em campanhas mais rigorosas, o MM pode exigir uma parada completa para recuperar tudo.



---

### 9) Desenvolvimento de Personagem (quando você 'nívela')

O desenvolvimento ocorre **após a aventura** (geralmente após 1–3 sessões, dependendo do ritmo da campanha).  
Você escolhe **um**: 
- aumente um atributo em 1 grau de dado (máx. até <span class="rpg-token token-<span class="rpg-token token-d20">k20</span>"><span class="rpg-token token-d20">d20</span></span>), ou 
- +1 Coração (máx. 7), ou 
- +1 <span class="rpg-token token-power">PM</span> (máx. 5), ou 
- Novo Talento (uma regra curta de uma linha acordada com o Mestre).

**Exemplo:** Destreza aumenta de <span class="rpg-token token-<span class="rpg-token token-d8">k8</span>"><span class="rpg-token token-d8">d8</span></span> para <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">d12</span></span>. A partir de agora, todos os testes de D você faz em <span class="rpg-token token-<span class="rpg-token token-d12">k12</span>"><span class="rpg-token token-d12">d12</span></span>.

---



---

### 10) Variante "apenas <span class="rpg-token token-d6">d6</span>": 2d6

Se quiserem jogar apenas com <span class="rpg-token token-d6">d6</span>:

- Cada teste é **2d6 + modificador de atributo**.
- Modificadores de atributos no início: um atributo **+2**, um **+1**, um **+0**.

**Resultado:**

- **6 ou menos** – falha com consequência  
- **7–9** – sucesso com custo  
- **10+** – sucesso completo  
- **12** – sucesso excepcional

**Situação:** adicionar **+1 / -1** ao lançamento (ajuda / atrapalha), em vez de alterar os limites.

**Sorte em 2d6:** funciona da mesma forma, apenas "aumentar o dado" se transforma em **+1 ao lançamento**.

---



---

### 11) Bons hábitos do jogador

- Fale: **o que você faz + por quê**. O objetivo das ações facilita para o mestre definir a aposta. - Se a Dificuldade for alta: não "insista no dado" — **mude a situação** (preparação, ferramenta, cobertura, ajuda, outro caminho). - Colabore: a ajuda de um aliado é uma das alavancas mais fortes e simples no sistema. - Na batalha, a posição vence: cobertura, distância e vantagem situacional são frequentemente mais importantes do que as estatísticas.

