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
generated_at: "2026-01-12T20:14:08.531Z"
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
# Guia do Mestre de Jogo

Automatic translation placeholder for pt

---



---

### 7.2 Comunique claramente a taxa.

- **Comunique claramente a dificuldade.** Antes de fazer o teste, diga: característica, <span class="rpg-token token-tn">TN</span>, consequência da falha, chance de ajuda.
- **Descrição → mecânica → resultado.** Sempre comece pela ficção, só depois faça o teste.
- **Cenas rápidas.** Mantenha o ritmo: um teste = um efeito razoável.
- **A falha impulsiona a ação.** A complicação muda a situação, e não "reinicia" a cena.
- **Coerência.** As mesmas circunstâncias → as mesmas <span class="rpg-token token-tn">TN</span> e consequências.



---

### 1. Introdução

1) O jogador diz o que faz e o que deseja alcançar.  
2) Escolha uma característica: **S** (força), **Z** (precisão/rápido), **M** (efeitos especiais).  
3) Estabeleça **<span class="rpg-token token-tn">TN</span>**: 4 fácil, 6 normal, 8 difícil, 12 heroico.  
4) Diga o que está em risco em caso de falha e se alguém pode **ajudar** (aumentando o dado em 1 tamanho).  
5) O jogador rola o dado da característica e compara com a <span class="rpg-token token-tn">TN</span>.  
6) Resolva o resultado e atualize a situação.  

Resumo para a mesa: “Características/<span class="rpg-token token-tn">TN</span>/Rolagem/Consequência”.



---

### 4 (fácil):

- **4 (fácil):** as condições são favoráveis, o alvo não oferece resistência.
- **6 (normal):** padrão na aventura sem vantagem.
- **8 (difícil):** pressão do tempo, má posição, cobertura, ferramentas complexas.
- **12 (heroico):** desafio acima da média; geralmente requer preparação ou um dado alto.

Modificação situacional: ajuste o <span class="rpg-token token-tn">TN</span> **em 1 grau** (máx. 2 em extremos).
- Pior: escuro, escorregadio, cobertura, alarme → <span class="rpg-token token-tn">TN</span> +1.
- Melhor: tempo, ferramentas, vantagem de posição, surpresa → <span class="rpg-token token-tn">TN</span> −1.

Intuições rápidas de eficácia (aproximações):
- <span class="rpg-token token-d6">d6</span> vs TN6 ≈ 17%; <span class="rpg-token token-d8">d8</span> vs 6 ≈ 38%; <span class="rpg-token token-d10">d10</span> vs 6 ≈ 50%; <span class="rpg-token token-d12">d12</span> vs 6 ≈ 58%.
- <span class="rpg-token token-d10">d10</span> vs TN8 ≈ 30%; <span class="rpg-token token-d12">d12</span> vs 8 ≈ 42%; <span class="rpg-token token-d20">d20</span> vs 12 ≈ 45%.
Use esses números como referência, não conte em tempo real.

Quando não rolar:
- Quando o resultado é óbvio e não há aposta.
- Quando a rolagem não mudará nada (é melhor passar para o próximo desafio).



---

### 1 na kości

- **1 nos dados**: falha + complicação. Exemplos: barulho, perda de tempo, pista errada, ferimento leve (−1 Coração), recurso perdido, posição pior.
- **Falha (resultado < <span class="rpg-token token-tn">TN</span>)**: sem efeito e eventual "retaliação" (em combate) ou progresso da ameaça (fora do combate).
- **Sucesso excepcional (máximo nos dados)**: sucesso + benefício adicional: mais rápido/mais silencioso/sem custo/maior efeito.

Checklist para criar complicações:
1) Atinja um recurso (tempo, posição, corações, mana, equipamento).
2) Mude a disposição no tabuleiro (novos obstáculos, caminhos bloqueados, escudos reforçados).
3) Aumente a pressão (contador, alarme, fortalecimento dos oponentes).



---

### Ruch:

- **Movimento:** até 5 quadrados por turno; movimento diagonal permitido.
- **Cobertura:** parcial → ataques à distância <span class="rpg-token token-tn">TN</span> +1; total → sem linha de visão.
- **Terreno difícil (opcional):** entrar em um quadrado custa 2 de 5 pontos de movimento.
- **Empurrar/mover:** teste S vs <span class="rpg-token token-tn">TN</span> 6 (modifique conforme a situação). Sucesso: mova o alvo 1–2 quadrados; excepcional: +1 quadrado.
- **Alcances:** considere até 10 quadrados como "sem penalidade"; além disso → <span class="rpg-token token-tn">TN</span> +1.
A velocidade é mais importante do que a contagem meticulosa — mantenha as regras leves.



---

### Kolejność:

- **Ordem:** jogadores → oponentes → repetir.
- **Ataque:** corpo a corpo = S, distância = Z; <span class="rpg-token token-tn">TN</span> do oponente: peão 6, elite 8, chefe 12.
- **Acerto:** peão cai; elite/chefe recebe 1 Ferida (chefe tem 3). Sucesso excepcional = normalmente 2 Feridas.
- **Erros:** se o oponente poderia alcançar → o herói perde 1 Coração (retaliação). Em cobertura/distante — normalmente sem retaliação.

Escalonamento de pressão:
- Muitos peões "em combate" → <span class="rpg-token token-tn">TN</span> +1 ou complicação adicional em caso de erro.
- Mude o terreno a cada turno: obstáculos aparecem, gargalos, oportunidades de vantagem.



---

### 1. Introdução

Construa cenas em 5 etapas:
1) **Objetivo**: para que serve a cena (por exemplo, transição, obtenção de itens, desativação de ameaças).
2) **Obstáculos**: 2–3 tipos diferentes (guarda, castelo, alarme, terreno perigoso).
3) **Ameaça**: lacaios/elites/boss, perigos, armadilhas.
4) **Contador (opcional)**: 3–5 etapas; falhas o movem; no final, uma consequência negativa.
5) **Recompensa/Consequência**: o que o sucesso traz, o que a falha muda.

Limites de tamanho do confronto (para 3–5 heróis):
- **Fácil:** 3–5 lacaios ou elite sem apoio.
- **Padrão:** 6–8 lacaios ou elite + 2–4 lacaios.
- **Difícil:** boss + 2–4 lacaios ou 2 elites + 3–5 lacaios.
- **Heroico:** boss + 4–6 lacaios e/ou elite.
Ajuste para a mesa: o terreno e as coberturas têm grande impacto.



---

### 1. Introdução

Formato (exemplo, sem clima):
> **Nome — <span class="rpg-token token-tn">TN</span>, Feridas, Tática, Especial**
- **Peão:** <span class="rpg-token token-tn">TN</span> 6, sem Feridas; tática simples.
- **Elite:** <span class="rpg-token token-tn">TN</span> 8, 2 Feridas; tem uma clara vantagem (por exemplo, mobilidade, cobertura, controle de campo).
- **Chefe:** <span class="rpg-token token-tn">TN</span> 12, 3 Feridas; 1–2 movimentos únicos (por exemplo, empurrão, convocação de apoio).

Reação e moral (sistema leve):
- Quando o primeiro peão cair ou a elite sofrer uma Ferida, role **<span class="rpg-token token-d6">d6</span>**:
  - 1–2: recuo/emboscada; 3–4: mantêm a posição; 5–6: atacam.
- Modifique ±1 por vantagem/medo/chefe nas proximidades.



---

### 1. Introdução

Magia é "efeitos especiais". Atribua <span class="rpg-token token-tn">TN</span> e custo de Mana de acordo com a escala:
- **Truque:** <span class="rpg-token token-tn">TN</span> 4, custo 0–1 (efeito curto, pequeno).
- **Padrão:** <span class="rpg-token token-tn">TN</span> 6, custo 1 (alvo único, salto curto, barreira).
- **Forte:** <span class="rpg-token token-tn">TN</span> 8, custo 2 (área, controle, cura +2 Corações).
- **Grande poder:** <span class="rpg-token token-tn">TN</span> 12, custo 3 (efeito cênico).

Regras auxiliares:
- **Múltiplos alvos:** ou +1 custo de Mana, ou <span class="rpg-token token-tn">TN</span> +1 grau.
- **Manutenção do efeito:** a cada turno pague 1 Mana ou ocupa uma Ação.
- **Contra-ataque/esquiva de feitiço:** permita que o herói faça o teste apropriado (Z ou M) contra a mesma <span class="rpg-token token-tn">TN</span>, para reduzir ou evitar o efeito (dependendo da ficção).



---

### 7.2. Skrytobójstwo/przemykanie: ustaw „poziom alarmu” jako **licznik 3–5**

- **Assassinato/Esquiva:** defina o “nível de alerta” como **contador 3–5**; falhas aumentam-no; ao atingir o máximo, um patrulha aparece, a porta se tranca, etc.
- **Perseguição:** determine a distância em “passos de perseguição” (por exemplo, 3). A cada turno: ambos os lados fazem testes; o sucesso do perseguidor encurta, o do fugitivo alonga. Quando chegar a 0 → alcance; ao 5 → fuga.
- **Obstáculos ambientais:** comunique claramente o custo do risco (por exemplo, queda = -1 Coração e pior posição), <span class="rpg-token token-tn">TN</span> dependente das descrições.



---

### Desenvolvimento:

- **Desenvolvimento:** após a aventura, cada um escolhe uma: aumentar o tamanho do dado de atributo, +1 Coração (máx 7) ou +1 Mana (máx 5).
- **Recompensas materiais:** concedem "permissões" (novas ações) ou vantagens únicas ("uma vez por cena, reduza a <span class="rpg-token token-tn">TN</span> em 1"). Evite modificadores permanentes.
- **Economia (opcional):** limiares simples: barato/padrão/caro — resolva com um teste de recursos em vez de contar moeda.



---

### 1. Introdução

- Estabeleça com os jogadores o escopo do conteúdo (o que é OK, do que devemos evitar).
- Combine um sinal simples de "pare"/"avance" para situações desconfortáveis.
- Resolva conflitos na ficção, não à mesa.



---

### 1. Introdução

1) **Gancho:** problema em uma frase.
2) **3 locais** com características táticas (coberturas, alturas, passagens estreitas).
3) **3 obstáculos:** castelo, guarda, ameaça ambiental.
4) **Recursos em jogo:** tempo, ruído, atenção do oponente.
5) **Lista de complicações** (5 itens) e **contador** para a cena.
6) **Inimigos:** entradas de 1 linha (peões/elites/boss) + tática simples.



---

### 1. Introdução

Komplikacje — <span class="rpg-token token-d6">d6</span> (universais):
1. Perda de tempo / vantagem do oponente.
2. Revelação de posição / aumento do alarme.
3. Pequeno dano: −1 Coração ou recurso.
4. Posição ruim: empurrão/atrapalhamento.
5. Perda/atrapalhamento de equipamento.
6. Nova ameaça aparece na cena.

Benefícios em caso de sucesso excepcional — <span class="rpg-token token-d6">d6</span>:
1. Mais rápido.
2. Mais silencioso.
3. Sem custo (por exemplo, sem Mana/sem retaliação).
4. Maior efeito (área/alcance).
5. Melhor posição dos aliados.
6. Dica/informação adicional.



---

### Cel graczy

- Objetivo dos jogadores: passar pela passagem segura.
- MG: fechadura (<span class="rpg-token token-tn">TN</span> 6), patrulha (contador 3), passagem estreita (coberturas).
1) Jogador A: "Eu abro a fechadura" (Z, <span class="rpg-token token-tn">TN</span> 6). Falha = +1 no contador. Rolagem 5 → falha, contador 1/3.
2) Jogador B ajuda (aumenta o dado). A: novamente (novas ferramentas, melhor posição), rolamento <span class="rpg-token token-d12">d12</span>=9 → sucesso.
3) A patrulha se aproxima (contador 2/3). Jogador C cobre a saída (S, <span class="rpg-token token-tn">TN</span> 6). Sucesso excepcional → vantagem de posição para o grupo.
Cena resolvida rapidamente, com apostas claras.

---
Isso é tudo que você precisa para conduzir. O restante (mundo, monstros, tesouros) é modular e deve ser adaptado ao universo escolhido.

