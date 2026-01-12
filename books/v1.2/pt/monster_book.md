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
generated_at: "2026-01-12T20:14:22.038Z"
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
# Manual dos Monstros

Automatic translation placeholder for pt

---



---

### 1. Introdução

- Usamos os mesmos conceitos que nas regras básicas e no livro MG.
- **Apenas os jogadores rolam.** Os oponentes exercem pressão através da <span class="rpg-token token-tn">TN</span> e movimentos; os danos geralmente resultam de "retaliação" ou testes forçados aos jogadores.



---

### 1. Introdução

> Nome — Classe, <span class="rpg-token token-tn">TN</span>, Ferimentos, Papel, Movimento, Especial

- **Classe:** Peão | Elite | Chefe
- **<span class="rpg-token token-tn">TN</span>:** número 4/6/8/12 que determina a dificuldade de atingir/desviar do oponente.
- **Ferimentos:** apenas para Elite e Chefe (Elite: 2, Chefe: 3 por padrão). Peão não tem Ferimentos (cai após ser atingido).
- **Papel:** Bruto (luta), Atirador (móvel), Artilharia (distância), Controlador (controle de campo), Suporte (apoio).
- **Movimento:** padrão de 5 quadrados. Altere se a mobilidade for única (por exemplo, 6 Rápido, Voo, Salto 3).
- **Especial:** 1–2 habilidades descritivas curtas (veja as seções “Características” e “Movimentos”).

Exemplo de anotação: “Guardião Elite — Elite, <span class="rpg-token token-tn">TN</span> 8, Ferimentos 2, Bruto, Movimento 5, Especial: Escudo Pesado; Investida”.



---

### Pachołek (minion):

- **Minion (pachołek):** <span class="rpg-token token-tn">TN</span> 6, cai após 1 acerto. Em quantidade, cria pressão. Retaliação ao errar: −1 Coração.
- **Elite:** <span class="rpg-token token-tn">TN</span> 8, 2 Feridas. Geralmente tem 1 característica defensiva ou mobilidade. Retaliação ao errar: −1 Coração; às vezes um efeito situacional adicional.
- **Chefe:** <span class="rpg-token token-tn">TN</span> 12, 3 Feridas. Tem 2–3 movimentos especiais e influencia o terreno/ritmo. Pode provocar testes nos jogadores (por exemplo, esquiva, estabilização).



---

### Bruto (luta corpo a corpo):

- **Brutamontes (combate corpo a corpo):** pressiona no corpo a corpo, empurra para fora da cobertura.
- **Skirmisher (móvel):** entra/sai do contato, pune a solidão.
- **Artilharia (distância):** atira de trás da cobertura, força o movimento.
- **Controlador (controle):** cria zonas de perigo, fumaças, campos de empurrão.
- **Suporte (apoio):** fortalece aliados, reduz a <span class="rpg-token token-tn">TN</span> dos aliados ou aumenta a <span class="rpg-token token-tn">TN</span> dos heróis em 1 grau situacionalmente.



---

### 1. Introdução

Adicione 1–2 ao statblock. Sempre funcionam descritivamente; mudam a <span class="rpg-token token-tn">TN</span> em 1 grau apenas quando faz sentido.
- **Escudo Natural:** a uma distância do oponente, ele geralmente tem cobertura parcial (ataque contra ele → <span class="rpg-token token-tn">TN</span> +1 grau).
- **Armadura Leve:** a primeira perda de 1 Coração em retaliação contra esta unidade na cena é ignorada.
- **Duro:** o primeiro sucesso contra esta unidade não causa Ferida (apenas empurra/posição) — bom para chefes.
- **Rápido (Movimento 6):** ignora 1 quadrado de terreno difícil por turno.
- **Escalador/Saltador:** move-se verticalmente/sobre obstáculos como se estivesse em terreno plano, salto de 3 quadrados.
- **Voo:** ignora obstáculos de terreno (o MJ cuida de coberturas razoáveis).
- **Explorador:** é mais difícil de surpreender; a primeira tentativa de furtividade contra ele tem <span class="rpg-token token-tn">TN</span> +1.
- **Resistência [tipo]:** o primeiro efeito de um determinado tipo na cena é reduzido (o MJ explica: alcance mais fraco, tempo mais curto).
- **Vulnerabilidade [tipo]:** contra este tipo de ataques, a <span class="rpg-token token-tn">TN</span> é 1 grau mais baixa.
- **Enxames:** quando está ao lado do alvo, a retaliação em um erro pode atingir dois heróis em alcance 1.



---

### 1. Introdução

Escolha 1–2 características. Os movimentos descrevem o efeito; se ameaçarem os heróis, o MJ pode pedir que eles façam o teste apropriado (Z ou M) contra a <span class="rpg-token token-tn">TN</span> do oponente.
- **Empurrão (Brute):** após atingir o herói, mova-o adicionalmente de 1 a 2 quadrados.
- **Quebra de Escudo:** quando esta unidade atinge, o escudo do alvo deixa de funcionar até o final do próximo turno.
- **Arrancada (Skirmisher):** entrar/sair do combate corpo a corpo não provoca retaliação.
- **Salva (Artillery):** área 3×3; todos na área fazem teste Z contra <span class="rpg-token token-tn">TN</span>; falha: −1 Coração e empurrão de 1 quadrado.
- **Âncora (Controller):** área 3×3 se torna "terreno pegajoso" (entrar custa toda a Ação) até o final do próximo turno.
- **Reforço (Support):** um aliado tem um bônus de 1 grau até o final da rodada (aqueles que o atacam têm <span class="rpg-token token-tn">TN</span> +1).
- **Invocação (Boss):** uma vez no início, invoca 2 lacaios em quadrados livres.
- **Barreira (Boss):** até o final da rodada do lado divino, os heróis realizam ataques à distância com <span class="rpg-token token-tn">TN</span> +1.
- **Impacto (Boss):** todos dentro de 2 quadrados fazem teste S vs <span class="rpg-token token-tn">TN</span>; falha: −1 Coração ou queda (você perde Movimento neste turno).



---

### 1. Introdução

1) **Escolha a classe:** Cone / Elite (2 Ferimentos) / Chefe (3 Ferimentos).
2) **Defina o <span class="rpg-token token-tn">TN</span>:** 6 / 8 / 12 (excepcionalmente 4 para muito fracos ou 10 para elites duras).
3) **Atribua um papel:** Bruto, Atirador, Artilharia, Controlador, Suporte.
4) **Adicione 1–2 características** e **1 movimento especial** (Chefe: 2–3 movimentos).
5) **Movimento:** normalmente 5; mude apenas se for crucial.

Pronto. Este esqueleto funciona em todas as realidades.



---

### 1. Introdução

Poniższe wpisy podmieniaj nazwami/kolorami świata.

### 7.1 Pachoquinhos
- **Guarda Pachoquinho — Pachoquinho, <span class="rpg-token token-tn">TN</span> 6, —, Bruto, Movimento 5, Especial: Escudo Natural.**
- **Explorador Pachoquinho — Pachoquinho, <span class="rpg-token token-tn">TN</span> 6, —, Patrulheiro, Movimento 6, Especial: Explorador.**
- **Atirador Pachoquinho — Pachoquinho, <span class="rpg-token token-tn">TN</span> 6, —, Artilharia, Movimento 5, Especial: Salva (pequena área 2×2, apenas avisa: em falha −1 Coração).**
- **Controlador Pachoquinho — Pachoquinho, <span class="rpg-token token-tn">TN</span> 6, —, Controlador, Movimento 5, Especial: Âncora (por 1 turno, uma vez).**
- **Apoio Pachoquinho — Pachoquinho, <span class="rpg-token token-tn">TN</span> 6, —, Suporte, Movimento 5, Especial: Reforço (uma vez por cena).**

### 7.2 Elites
- **Guarda Elite — Elite, <span class="rpg-token token-tn">TN</span> 8, Ferimentos 2, Bruto, Movimento 5, Especial: Armadura Leve; Apressar.**
- **Assassino Elite — Elite, <span class="rpg-token token-tn">TN</span> 8, Ferimentos 2, Skirmisher, Movimento 6, Especial: Arrancada; Vulnerabilidade [observação] (mais fácil de detectar).**
- **Atirador Elite — Elite, <span class="rpg-token token-tn">TN</span> 8, Ferimentos 2, Artilharia, Movimento 5, Especial: Cobertura Natural; Salva (3×3 após preparação).**
- **Controlador Elite — Elite, <span class="rpg-token token-tn">TN</span> 8, Ferimentos 2, Controlador, Movimento 5, Especial: Âncora; Empurrão de 1 quadrado em caso de sucesso excepcional.**
- **Médico Elite — Elite, <span class="rpg-token token-tn">TN</span> 8, Ferimentos 2, Suporte, Movimento 5, Especial: Reforço; ao acertar, remove 1 complicação de um aliado (descritivamente).**

### 7.3 Chefes
- **Líder — Chefe, <span class="rpg-token token-tn">TN</span> 12, Ferimentos 3, Suporte, Movimento 5, Especial: Invocação; Fortalecimento; Barreira.**
- **Colosso — Chefe, <span class="rpg-token token-tn">TN</span> 12, Ferimentos 3, Bruto, Movimento 5, Especial: Investida (até 2 quadrados); Resistente; Impacto.**
- **Caçador — Chefe, <span class="rpg-token token-tn">TN</span> 12, Ferimentos 3, Atacante, Movimento 6, Especial: Arrancada; Explorador; Salva (saltatória — após o movimento).**
- **Tático — Chefe, <span class="rpg-token token-tn">TN</span> 12, Ferimentos 3, Controlador, Movimento 5, Especial: Âncora (manutenção por 1 Mana/recurso por turno); Barreira; Invocação (1 peão/ turno até um máximo de 3).**



---

### 1. Introdução

Perigo é um "inimigo sem cérebro" ou efeito ambiental. Funciona em turnos ou por gatilho.  
Formato: **Nome — <span class="rpg-token token-tn">TN</span>, Efeito, Como desativar**  
- **Torre — <span class="rpg-token token-tn">TN</span> 8, Efeito: no turno dos oponentes, cada um na linha de tiro faz teste Z vs <span class="rpg-token token-tn">TN</span>, falha: −1 Coração; Desativação: teste M ou Z <span class="rpg-token token-tn">TN</span> 8 no painel.**  
- **Tranca — <span class="rpg-token token-tn">TN</span> 6, Efeito: entrar no campo força um teste Z; falha: imobilização ou −1 Coração; Desativação: Z <span class="rpg-token token-tn">TN</span> 6 com ferramentas.**  
- **Campo Repulsivo — <span class="rpg-token token-tn">TN</span> 8, Efeito: no início do turno, move 2 quadrados em direção à borda; Desativação: M <span class="rpg-token token-tn">TN</span> 8 (dispersão) ou corte de energia (S <span class="rpg-token token-tn">TN</span> 6).**  
- **Gás/Fumaça — <span class="rpg-token token-tn">TN</span> 6, Efeito: na área 3×3 teste M ou Z; falha: ponto cego/−1 Coração; Desativação: ventilação (S) ou vedação (Z).**



---

### 1. Introdução

Escolha 1 de cada linha (ou role [token:<span class="rpg-token token-d6">d6</span>]):
1. Objetivo da cena: passagem / recuperação / desativação / escolta / roubo / defesa
2. Terreno principal: aberto / corredores estreitos / múltiplos níveis / coberturas modulares / bordas perigosas / névoa-fumaça
3. Oponentes: 6× capanga / 4× capanga + elite / 2× elite / chefe / chefe + 2× capanga / elite + azar
4. Vantagem do oponente: cobertura / altura / mobilidade / contagem regressiva / gargalos / suporte remoto
5. Vantagem dos jogadores: surpresa / nível superior / ferramentas / barreira curta / atalho / aliado neutro



---

### 1. Introdução

Em vez de <span class="rpg-token token-tn">TN</span> numéricos, use graus:
- **Peão:** "Normal" (equivalente a <span class="rpg-token token-tn">TN</span> 6)
- **Elite:** "Difícil" (+1 grau)
- **Chefe:** "Heroico" (+2 graus) e 3 Ferimentos
As características e movimentos funcionam da mesma forma; quando "<span class="rpg-token token-tn">TN</span> +1" na descrição, aumente o grau.



---

### 7.2 Se a luta durar muito pouco

- Se a luta durar muito pouco: adicione lacaios em ondas (2 por turno) ou aumente a <span class="rpg-token token-tn">TN</span> em 1 grau para os oponentes que têm vantagem de posição.
- Se a luta se arrastar: permita um sucesso excepcional com mais frequência criando oportunidades (melhor posição), ou diminua a <span class="rpg-token token-tn">TN</span> para inimigos enfraquecidos.
- Duas elites ≈ pequeno chefe; chefe + 4 lacaios ≈ confronto final em uma sessão de 2 horas.



---

### Straż Obronny — Pachołek, <span class="rpg-token token-tn">TN</span> 6, —, Artilharia, Movimento 5, Especial: Proteção Natural.

- **Guarda de Defesa — Pachołek, <span class="rpg-token token-tn">TN</span> 6, —, Artilharia, Movimento 5, Especial: Proteção Natural.**
- **Patrulha Móvel — Pachołek, <span class="rpg-token token-tn">TN</span> 6, —, Atirador, Movimento 6, Especial: Explorador.**
- **Ataque Pesado — Elite, <span class="rpg-token token-tn">TN</span> 8, Ferimentos 2, Bruto, Movimento 5, Especial: Armadura Leve; Impulso.**
- **Tático de Campo — Elite, <span class="rpg-token token-tn">TN</span> 8, Ferimentos 2, Controlador, Movimento 5, Especial: Âncora; Fortalecimento.**
- **Líder de Campo — Chefe, <span class="rpg-token token-tn">TN</span> 12, Ferimentos 3, Suporte, Movimento 5, Especial: Invocação; Barreira; Fortalecimento.**
- **Colosso Terreno — Chefe, <span class="rpg-token token-tn">TN</span> 12, Ferimentos 3, Bruto, Movimento 5, Especial: Resistente; Impacto; Impulso.**

---
Este é um conjunto de ferramentas para criar rapidamente inimigos. Defina o <span class="rpg-token token-tn">TN</span>, escolha a classe e o papel, adicione 1–2 características e movimento — e você terá um inimigo jogável pronto para o tabuleiro.

