---
pdf_options:
  displayHeaderFooter: true
  headerTemplate: |-
    <div style="font-size: 8px; width: 100%; text-align: center; color: #b91c1c; font-family: 'Cinzel', serif; font-weight: 700; letter-spacing: 1px; padding-bottom: 5px;">
      NANO DUNGEON ENGINE v1.2
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
generated_at: "2026-01-12T20:14:32.274Z"
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

Automatic translation placeholder for pt

---



---

### MG descreve a situação e diz o que é possível.
- Você diz **o que faz** e **qual é o efeito que deseja**.
- Se o resultado for incerto, MG diz.

- MG descreve a situação e diz o que é possível.
- Você diz **o que faz** e **qual efeito deseja**.
- Se o resultado for incerto, o MG diz:
  1) qual característica você está usando (S/Z/M),
  2) qual é a dificuldade (<span class="rpg-token token-tn">TN</span>),
  3) o que pode acontecer em caso de falha.
- Você rola **um dado** da sua característica e verifica se o resultado ≥ <span class="rpg-token token-tn">TN</span>.

### A Regra Mais Curta



---

### 1. Introdução

Sua personagem tem:
- **Função** (Guerreiro / Ladino / Mago),
- 3 **atributos**: Força (F), Destreza (D), Magia (M),
- **Vida** (Corações) e **Mana**,
- 2 **Talentos** (opcionais, mas recomendados),
- equipamento.

### 2.1 Atributos (F/D/M) — para que servem
- **Força (F)**: combate corpo a corpo, arrombamento, levantamento, resistência.
- **Destreza (D)**: tiros, precisão, furtividade, esquiva, acrobacias.
- **Magia (M)**: efeitos "especiais" (feitiços/psionismo/tecnologia — dependendo do jogo).

### 2.2 Dados de características
Cada característica tem seu dado (por exemplo, <span class="rpg-token token-d6">d6</span>, <span class="rpg-token token-d8">d8</span>, <span class="rpg-token token-d10">d10</span>, <span class="rpg-token token-d12">d12</span>, <span class="rpg-token token-d20">d20</span>). Você sempre rola **um** dado.
- Dado maior = maior chance de resultados altos.

### 2.3 Vida e Mana
- **Vida:** 5 Corações (início).
- **Mana:** 3 (início). Você a gasta ao usar Magia.



---

### Passo 1: Escolha um papel
Escolha um papel. Define os dados iniciais das características:
- **Guerreiro:** S <span class="rpg-token token-d10">d10</span>, Z <span class="rpg-token token-d6">d6</span>, M <span class="rpg-token token-d6">d6</span>
- **Ladrão:** S <span class="rpg-token token-d6">d6</span>, Z <span class="rpg-token token-d10">d10</span>, M <span class="rpg-token token-d6">d6</span>
- **Mago:** S <span class="rpg-token token-d6">d6</span>, Z <span class="rpg-token token-d6">d6</span>, M <span class="rpg-token token-d10">d10</span>

### Passo 2: Registre os recursos

### Passo 3: Escolha 2 Talentos (opcional)
Talentos são frases curtas que descrevem em que você é bom.
- Exemplos neutros: “Negociador”, “Explorador”, “Mecânico”, “Médico”, “Atleta”, “Analista”, “Hacker”.

**Como funcionam os Talentos:** se um Talento realmente ajudar no teste, o MG pode **reduzir a dificuldade (<span class="rpg-token token-tn">TN</span>) em 1 grau**.
- Normalmente, 1 Talento por teste.
- O Talento não substitui a descrição da ação — ajuda quando realmente faz sentido.

### Passo 4: Equipamento
Liste:
- 1 ferramenta de combate (corpo a corpo ou à distância),
- proteção (se aplicável),
- 3 itens utilitários.

O equipamento neste jogo geralmente funciona como **"permissão"**: você tem algo, então pode tentar realizar ações específicas.

### Exemplo de personagem
- Papel: Ladino
- Força <span class="rpg-token token-d6">d6</span>, Destreza <span class="rpg-token token-d10">d10</span>, Magia <span class="rpg-token token-d6">d6</span>
- Vida 5, Mana 3
- Talentos: “Explorador”, “Negociador”
- Equipamento: ferramenta de longo alcance, ganchos, corda, lanterna



---

### 4.1 Quando você joga
Você joga quando:
- algo é **arriscado** ou incerto,
- e a falha tem consequências.

Se algo é óbvio e sem pressão, o MG pode dizer "sucesso" sem jogar.

### 4.2 Dificuldades (<span class="rpg-token token-tn">TN</span>)
São utilizados 4 níveis:
- **<span class="rpg-token token-tn">TN</span> 4 — Fácil**
- **<span class="rpg-token token-tn">TN</span> 6 — Normal**
- **<span class="rpg-token token-tn">TN</span> 8 — Difícil**
- **<span class="rpg-token token-tn">TN</span> 12 — Heroico**

O MG escolhe a <span class="rpg-token token-tn">TN</span>. Você não precisa "adivinhar" — o MG simplesmente diz qual é a dificuldade.

### Wyniki Testu

> **Nível de Dificuldade (<span class="rpg-token token-tn">TN</span>)**: 4 (Fácil), 6 (Normal), 8 (Difícil).
> 
> **Resultado do Lançamento:**
> - **1**: Falha + Complicação.
> - **< <span class="rpg-token token-tn">TN</span>**: Falha.
> - **≥ <span class="rpg-token token-tn">TN</span>**: Sucesso.
> - **Max (10/20)**: Sucesso + Benefício.

---

### 4.3 Resultados do lançamento
- **Resultado ≥ <span class="rpg-token token-tn">TN</span>:** sucesso.
- **Resultado < <span class="rpg-token token-tn">TN</span>:** falha.
- **Rolou 1:** falha com complicação.
- **Máximo nos dados** (por exemplo, 10 em <span class="rpg-token token-d10">d10</span>): sucesso excepcional + benefício adicional.

**Benefício adicional** (exemplos): mais rápido, mais silencioso, mais seguro, maior efeito, melhor posição.

### 4.4 Mudanças de dificuldade "um grau"
Em vez de contar bônus, o MG às vezes altera a <span class="rpg-token token-tn">TN</span> em 1 grau:
- condições piores → <span class="rpg-token token-tn">TN</span> mais alta (por exemplo, 6 → 8),
- condições melhores → <span class="rpg-token token-tn">TN</span> mais baixa (por exemplo, 8 → 6).

Seu papel como jogador: **crie melhores condições** através de descrição e decisões (cobertura, preparação, ferramentas, plano).

### 4.5 Ajuda do aliado
Um aliado pode usar sua Ação para te ajudar. Nesse caso, para essa única rolagem você pode:
- aumentar o dado em 1 tamanho: **<span class="rpg-token token-d6">d6</span>→<span class="rpg-token token-d8">d8</span>→<span class="rpg-token token-d10">d10</span>→<span class="rpg-token token-d12">d12</span>→<span class="rpg-token token-d20">d20</span>**.

A ajuda deve fazer sentido na descrição (por exemplo, proteger, distrair, fornecer ferramentas).

### Exemplo de teste
Você quer abrir rapidamente uma passagem bloqueada.
- MG: "Isso é Agilidade, <span class="rpg-token token-tn">TN</span> 6."
- Você rola 1d10 e sai 7 → sucesso: passagem aberta.



---

### 1. Kratka

- **1 quadrado** é a unidade básica de distância.
- Em uma rodada, você tem **movimento de até 5 quadrados**.
- Você pode andar na diagonal (a diagonal conta como 1 quadrado).
- A cobertura é importante: se algo te protege de um ataque à distância, geralmente fica mais difícil acertar.



---

### 6.1 Como é a vez
Na sua vez, você tem:
- **Movimento** (até 5 quadrados),
- **1 Ação**.

Ação pode ser, por exemplo: ataque, uso de equipamento, teste de atributo, ajuda, uso de Magia.

### Atak

> 1) Escolha um alvo (dentro do alcance e na linha de visão).
> 2) Escolha a arma/magia.
> 3) Verifique qual Atributo é utilizado (por exemplo, Força corpo a corpo, Destreza à distância, Magia para o feitiço).
> 4) **Role.** Compare com a **<span class="rpg-token token-tn">TN</span>** do oponente.

---

### 6.2 Ataque
- **Corpo a corpo:** teste de **Força (F)**.
- **Distância:** teste de **Destreza (D)**.
- O mestre do jogo diz a <span class="rpg-token token-tn">TN</span> do oponente.

<span class="rpg-token token-tn">TN</span> padrão dos oponentes:
- **Peão:** <span class="rpg-token token-tn">TN</span> 6
- **Elite:** <span class="rpg-token token-tn">TN</span> 8
- **Chefe:** <span class="rpg-token token-tn">TN</span> 12

### Trafienie

> - **Pachołek**: Morre (ou sai da luta).
> - **Elita/Boss**: Perde **1 Coração**.
> - **Jogador**: Perde **1 Coração** (a menos que tenha Armadura — nesse caso, a Armadura absorve o golpe, mas se desgasta).

---

### 6.3 O que significa um acerto
- Você acerta o marcador → sai da luta.
- Você acerta uma elite/boss → recebe uma Ferida (o Boss normalmente tem 3 Feridas).
- Sucesso excepcional contra uma elite/boss → geralmente você causa +1 Ferida (totalizando 2), ou ganha uma vantagem situacional (por exemplo, empurrar para fora da cobertura).

### Pudło i Odwet

> Walka ma ryzyko. Jeśli **não acertar** (resultado < <span class="rpg-token token-tn">TN</span>) ou tirar **1**:
> - O oponente contra-ataca: você perde **1 Coração**.
> - Ou ocorre outra complicação lógica (por exemplo, você perde a arma, é derrubado).
> 
> *Esta não é a vez do oponente — é o efeito do seu ataque malsucedido.*

---

### 6.4 Erro e "retaliação"
Se você **erra** (resultado < <span class="rpg-token token-tn">TN</span>) e o oponente poderia realmente te atingir, você perde **1 Coração**.
- Isso é comum em combate corpo a corpo.
- Em ataques à distância, muito depende da cobertura e da situação.

Sua lição tática: **posicione-se de forma que, ao errar, não receba retaliação** (cobertura, distância, plano, ajuda).

### 0 Serc

> Se você cair para 0 Corações:
> - Você está **Derrubado**.
> - Você não pode realizar ações (apenas rastejar e falar com o que resta de força).
> - Um aliado pode "te levantar" (ação de Ajuda), restaurando 1 Coração.
> - Se você receber dano enquanto estiver Derrubado — **Você Morre**.

---

### 6.5 0 Serc
Quando você cai para 0 Serc:
- você está caído e não realiza ações,
- um aliado pode usar uma Ação para te colocar de pé com **1 Serc**.

### Exemplo de uma ação curta
- Movimento: você corre 3 quadrados até a cobertura.
- Ação: você atira (Z). MG: "<span class="rpg-token token-tn">TN</span> 6, mas o alvo está atrás da cobertura → <span class="rpg-token token-tn">TN</span> 8". Você rola <span class="rpg-token token-d10">d10</span>=9 → acerto.



---

### 1. Introdução

Magia e mecanismo de "efeitos especiais". Você descreve o efeito, o MG determina a <span class="rpg-token token-tn">TN</span> e o custo de Mana.

### 7.1 Custos e níveis
- **Truque:** <span class="rpg-token token-tn">TN</span> 4, custo 0–1
- **Padrão:** <span class="rpg-token token-tn">TN</span> 6, custo 1
- **Efeito forte:** <span class="rpg-token token-tn">TN</span> 8, custo 2
- **Grande poder:** <span class="rpg-token token-tn">TN</span> 12, custo 3

### 7.2 Falha na Magia
Quando a Magia falha:
- você perde a Mana gasta,
- uma consequência aparece (por exemplo, -1 Coração, perda de posição, ameaça adicional).

### 7.3 Sucesso excepcional
O máximo nos dados de Magia oferece um benefício adicional:
- maior alcance/área,
- maior duração,
- maior eficácia,
- ou menor custo (o MJ pode devolver 1 Mana).

### Exemplo de Magia
Você quer fazer um "salto" curto de 5 quadrados.
- MG: "É Padrão: <span class="rpg-token token-tn">TN</span> 6, custo 1."
- Você paga 1 Mana, rola M <span class="rpg-token token-d10">d10</span>=7 → sucesso: você salta por trás da cobertura.



---

### 1. Introdução

Após o conflito, se vocês tiverem um momento seguro e as condições básicas para descansar:
- Vida e Mana retornam ao máximo.



---

### 1. Introdução

Após a aventura, você escolhe **uma**:
- aumentar S/Z/M em 1 tamanho de dado: <span class="rpg-token token-d6">d6</span>→<span class="rpg-token token-d8">d8</span>→<span class="rpg-token token-d10">d10</span>→<span class="rpg-token token-d12">d12</span>→<span class="rpg-token token-d20">d20</span>,
- ou +1 Coração (máx 7),
- ou +1 Mana (máx 5).

Isso significa desenvolvimento sem adicionar mais dados às jogadas.



---

### 1. Introdução

Se houver apenas um [token:<span class="rpg-token token-d6">d6</span>] na mesa, em vez do tamanho do dado, você tem um limiar de sucesso:
- Mestre 3+, Treinado 4+, Novato 5+, Sem proficiência 6.

O GM pode aumentar/diminuir o limiar em 1 grau por situação ou ajuda.



---

### Zawsze mów

- Sempre diga: **o que você faz** + **para que**. "Quero apertar a alavanca" está ok, mas "quero apertar a alavanca para fechar a passagem" é ainda melhor.
- Se o <span class="rpg-token token-tn">TN</span> for alto: não "force o teste" — mude a situação (cobertura, ferramentas, ajuda, outro caminho).
- Estabeleçam a cooperação: uma pessoa ajuda, a outra realiza o teste.
- Em combate, respeite a cobertura e a posição — muitas vezes é mais importante do que o próprio teste.

---
Fim do livro do jogador.

