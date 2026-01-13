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
generated_at: "2026-01-13T09:31:02.905Z"
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
# Regras em resumo

Automatic translation placeholder for pt

---



---

### 1) Herói em 1 minuto

- Papel (escolha um):
  - Guerreiro — mestre da força e do combate corpo a corpo
  - Ladino — mestre da velocidade, furtividade e tiros
  - Mago — mestre de feitiços e conhecimento
- Atributos e dados: Força (F), Destreza (D), Magia (M).
  - Guerreiro: F <span class="rpg-token token-d10">d10</span>, D <span class="rpg-token token-d6">d6</span>, M <span class="rpg-token token-d6">d6</span>
  - Ladino: F <span class="rpg-token token-d6">d6</span>, D <span class="rpg-token token-d10">d10</span>, M <span class="rpg-token token-d6">d6</span>
  - Mago: F <span class="rpg-token token-d6">d6</span>, D <span class="rpg-token token-d6">d6</span>, M <span class="rpg-token token-d10">d10</span>
- Vida: 5 Corações. Mana: 3 (usada em feitiços).
- Equipamento: arma, armadura leve, 3 itens adequados ao papel.
Exemplo: Ladino tem Destreza <span class="rpg-token token-d10">d10</span>, então usa <span class="rpg-token token-d10">d10</span> para tiros.



---

### 2) Como você executa ações

1. Escolha a característica apropriada (S/Z/M) e role o dado dessa característica.
2. Compare com o nível de dificuldade (<span class="rpg-token token-tn">TN</span>):
   - Fácil 4, Normal 6, Difícil 8, Heroico 12.
3. Resultado:
   - 1 no dado — falha com complicação (barulho, perda de tempo, ferimento leve, etc.).
   - Resultado < <span class="rpg-token token-tn">TN</span> — falha.
   - Resultado ≥ <span class="rpg-token token-tn">TN</span> — sucesso.
   - Máximo no dado (por exemplo, 10 em <span class="rpg-token token-d10">d10</span>, 20 em <span class="rpg-token token-d20">d20</span>) — sucesso excepcional com benefício adicional.
Melhorias sem contagem:
- Situação melhor/pior: diminua/aumente a <span class="rpg-token token-tn">TN</span> em 1 grau (por exemplo, 6 → 8 por cobertura).
- Ajuda de um aliado (com sua ação): para este lançamento, "aumente" o dado em um tamanho (<span class="rpg-token token-d6">d6</span>→<span class="rpg-token token-d8">d8</span>→<span class="rpg-token token-d10">d10</span>→<span class="rpg-token token-d12">d12</span>→<span class="rpg-token token-d20">d20</span>).
Exemplo: O Guerreiro arromba a porta (Normal 6). Ele rola <span class="rpg-token token-d10">d10</span> e tira 10 — sucesso excepcional: a porta voa, e o guarda atrás dela cai.



---

### 3) Movimento e luta no tabuleiro

- Movimento: até 5 quadrados (diagonais permitidas).
- Sua vez: Movimento + 1 Ação (por exemplo, ataque, feitiço, busca, levantar alavanca).
- Ataque:
  - Corpo a corpo (C): rolagem contra a <span class="rpg-token token-tn">TN</span> do oponente.
  - Distância (D): a cobertura do alvo aumenta a <span class="rpg-token token-tn">TN</span> em 1 grau.
- <span class="rpg-token token-tn">TN</span> dos oponentes: Peão 6, Elite 8, Chefe 12.
- Efeitos do acerto: Peão — cai após ser atingido; Elite — o GM pode exigir condições favoráveis; Chefe — tem 3 Feridas (acerto = 1 Ferida). Sucesso excepcional contra o Chefe = 2 Feridas.
- Retaliação: se você errar em combate corpo a corpo ou em alcance de retaliação, perde 1 Coração (a menos que tenha cobertura total).
Exemplo: Mago (D <span class="rpg-token token-d6">d6</span>) atira com uma funda em um peão atrás de uma caixa: <span class="rpg-token token-tn">TN</span> 6 + cobertura → 8. O Mago pede ajuda ao Ladino (aumenta o dado para <span class="rpg-token token-d8">d8</span>) e muda de posição para uma melhor (<span class="rpg-token token-tn">TN</span> cai para 6). <span class="rpg-token token-d8">d8</span>=7 — atingido.



---

### 4) Magia (prosto)

- Lançar um feitiço: descreva o efeito, gaste Mana, lance Magia (M).
  - Truque (chama, estrondo, névoa) — <span class="rpg-token token-tn">TN</span> 4, custo 0–1 Mana.
  - Projétil/Barreira/Salto de 5 quadrados — <span class="rpg-token token-tn">TN</span> 6, custo 1 Mana.
  - Área/Cura +2 Corações/Paralisia — <span class="rpg-token token-tn">TN</span> 8, custo 2 Mana.
  - Grande poder (ponte de gelo, tempestade de fogo) — <span class="rpg-token token-tn">TN</span> 12, custo 3 Mana.
- Falha: Mana é perdida; ocorre uma pequena consequência (falta de ar -1 Coração ou atenção indesejada dos inimigos).
- Descanso após a batalha: você recupera toda a Mana; um descanso seguro também restaura Corações.
Exemplo: “Relâmpago” (teleporte curto de 5 quadrados): <span class="rpg-token token-tn">TN</span> 6, custo 1 Mana. O mago <span class="rpg-token token-d10">d10</span> rola 7 — salto bem-sucedido para a barreira.



---

### 5) Queda e tratamento

- 0 Coração: derrubado (não está funcionando). Um aliado pode usar uma ação para te levantar para 1 Coração.
- Após o combate, com um breve descanso e uma refeição, vocês retornam à plenitude de Corações e Mana.
Exemplo: O Ladino cai para 0. O Guerreiro o ajuda a se levantar — o Ladino volta para 1 Coração.



---

### 6) Desenvolvimento de PERSONAGENS

Após a aventura, escolha uma:
- Aumente um atributo em um tamanho de dado: <span class="rpg-token token-d6">d6</span>→<span class="rpg-token token-d8">d8</span>→<span class="rpg-token token-d10">d10</span>→<span class="rpg-token token-d12">d12</span>→<span class="rpg-token token-d20">d20</span>,
- ou +1 Coração (máx 7),
- ou +1 Mana (máx 5).
Exemplo: O Guerreiro aumenta a Força de <span class="rpg-token token-d10">d10</span> para <span class="rpg-token token-d12">d12</span> — fica mais fácil atingir <span class="rpg-token token-tn">TN</span> 12.



---

### 7) Wariant só-<span class="rpg-token token-d6">d6</span>

Quando você tem apenas um dado <span class="rpg-token token-d6">d6</span>:
- Em vez de tamanhos de dados, cada atributo tem um limiar de sucesso:
  - Mestre 3+, Treinado 4+, Novato 5+, Sem proficiência 6.
- A <span class="rpg-token token-tn">TN</span> ainda muda a situação em 1 grau (mais fácil/difícil).
- Ajuda: reduza o limiar em 1 (por exemplo, de 4+ para 3+ para este teste).
- Desenvolvimento: aumente o nível de um atributo (por exemplo, Treinado 4+ → Mestre 3+) ou +1 Coração/Mana.
Exemplo: Tiro do Ladrão (Treinado 4+) em um alvo com leve cobertura (um grau mais difícil) requer 5+. Rolagem <span class="rpg-token token-d6">d6</span>=5 — acerto.

