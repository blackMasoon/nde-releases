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
generated_at: "2026-01-15T07:57:22.390Z"
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
# Regras em resumo

Automatic translation placeholder for <span class="rpg-token token-math">pt</span>

---



---

### 1) Herói em 1 minuto


* **Conceito:** quem você é e em que gênero está jogando (1 frase).
* **Função (escolha uma):**

  * **Assalto** – pressão, combate, superação de obstáculos
  * **Especialista** – furtividade, precisão, técnica, observação
  * **Adept** – poderes, conhecimento, influência, improvisação
* **Atributos (3):**

  * **Força (F)** – força física, resistência, combate corpo a corpo
  * **Destreza (D)** – reflexos, furtividade, tiro, pilotagem
  * **Poder (<span class="rpg-token token-stat">P</span>)** – magia/psionismo/tecnologia/blefe/ intuição (dependendo do mundo)
* **Dados de atributos:** um atributo **<span class="rpg-token token-d12">k12</span>**, um **<span class="rpg-token token-d8">k8</span>**, um **<span class="rpg-token token-d6">k6</span>** (escolha de acordo com a função).
* **Corações:** 5. **Pontos de Poder:** 3 (gaste em poderes e "jogadas especiais").
Abaixo você tem um trecho pronto para colar (variante A), no estilo de regras curtas "1-page".

**Dado da Sorte (como funciona):** gaste **1 DS**, para escolher uma:

* **Repetição** do seu teste (deixe o melhor resultado), ou
* **Aumento do dado em 1 nível** para essa única jogada (**<span class="rpg-token token-d6">k6</span>→<span class="rpg-token token-d8">k8</span>→<span class="rpg-token token-d12">k12</span>→<span class="rpg-token token-d20">k20</span>**), ou
* **Troca de falha por "sucesso com custo"** — a ação é bem-sucedida, mas o MJ imediatamente impõe um custo (por exemplo, você perde tempo, faz barulho, consome um recurso, termina em uma posição pior, atrai atenção, danifica equipamento).

**Recuperação de DS:** no início da próxima sessão, você volta ao limite. O MJ pode conceder **+1 DS** por risco ousado, excelente decisão narrativa ou jogando com consequências.

* **Equipamento:** 1 ferramenta "chave" (por exemplo, espada, rifle, kit de hacker), 1 proteção (armadura, escudo energético, camuflagem), 3 trinkets que se encaixam no conceito.

**Exemplo:** Especialista: F <span class="rpg-token token-d12">k12</span>, <span class="rpg-token token-stat">P</span> <span class="rpg-token token-d8">k8</span>, D <span class="rpg-token token-d6">k6</span>. No cyberpunk, <span class="rpg-token token-stat">P</span> é "Hackeamento/Influência"; na fantasia, <span class="rpg-token token-stat">P</span> é "Magia/Vontade".



---

### 2) Como resolver ações


1. O jogador diz **o que faz** e **como** (descrição no mundo do jogo).
2. O mestre determina a **Dificuldade** e a aposta ("o que acontece em caso de falha").
3. Role o dado de atributo (F/D/<span class="rpg-token token-stat">S</span>) e compare com a Dificuldade.

**Dificuldade (D):**

* **3** fácil, **4** padrão, **5** difícil, **6** muito difícil, **8** heroico, **12** lendário.

**Resultado do lançamento:**

* **1** – falha com consequência (a complicação acontece com certeza).
* **< D** – falha (mas a cena continua: perda de tempo, barulho, pior posição, perda de recurso).
* **≥ D** – sucesso.
* **<span class="rpg-token token-stat">M</span>áximo no dado** (por exemplo, 12 em <span class="rpg-token token-d12">k12</span>, 20 em <span class="rpg-token token-d20">k20</span>) – sucesso excepcional: você ganha um benefício adicional.

**Modificadores sem contagem:**

* **Melhor situação**: aumente o dado em 1 nível (<span class="rpg-token token-d6">k6</span>→<span class="rpg-token token-d8">k8</span>→<span class="rpg-token token-d12">k12</span>→<span class="rpg-token token-d20">k20</span>).
* **Pior situação**: diminua o dado em 1 nível (<span class="rpg-token token-d20">k20</span>→<span class="rpg-token token-d12">k12</span>→<span class="rpg-token token-d8">k8</span>→<span class="rpg-token token-d6">k6</span>→<span class="rpg-token token-d4">k4</span>).
* **Ajuda de um aliado** (custa a ação dele): aumente o dado em 1 nível.

**Exemplo:** O Adepto tenta fechar o portal (D <span class="rpg-token token-d8">k8</span>) sob alarme e estresse → pior situação, cai para <span class="rpg-token token-d6">k6</span>. D = 5. Lançamento 6: sucesso, mas o "alarme" permanece ao fundo como pressão narrativa.



---

### 3) Movimento e combate – por padrão sem grade, grade como opção

**Por padrão: teatro da mente (recomendado)**

* Distâncias são descritas como: **Próximo** (ao alcance), **Não muito longe** (alguns passos), **Longe** (do outro lado do palco), **Muito longe** (sniper/veículo).
* Em uma rodada você tem: **Movimento + 1 Ação**.

  * Movimento geralmente altera a distância em 1 “grau” (Não muito longe→Próximo etc.).
* **Ataque**: rolagem **<span class="rpg-token token-stat">S</span>** (corpo a corpo) ou **D** (distância) contra **Defesa** do alvo.

**Defesa dos oponentes (aproximadamente):**

* **Fraco** 4, **Típico** 5, **Elite** 6, **Chefe** 8 (chefe lendário 12).

**Efeitos de acerto (combate rápido):**

* Um acerto causa **1 Coração**.
* Um sucesso excepcional causa **2 Corações** ou dá um efeito forte (desarme, derrubada, distração).

**Cobertura e vantagem posicional:**

* Cobertura leve / ângulo ruim: diminua o dado do atacante em 1 grau.
* Boa posição / surpresa: aumente o dado em 1 grau.

**Opção: jogo em grade**

* 1 quadrado = 1–2 m. Movimento na rodada: **até 5 quadrados**. O resto das regras permanece inalterado.

**Exemplo:** O especialista atira de uma cobertura (D <span class="rpg-token token-d12">d12</span>) para a elite (Defesa 6). O alvo está em cobertura leve → D cai para <span class="rpg-token token-d8">d8</span>. Rolagem 7: sucesso, 1 Coração de dano.



---

### 4) Poderes, „feitiços” e jogadas especiais (universais)


Isso abrange magia, psionismo, cibernética, gadgets, truques de filme – dependendo do mundo.

* Quando você faz algo **acima do padrão**: gaste **Ponto de Poder** e role **<span class="rpg-token token-stat">M</span>**.
* Determine o nível do efeito:

**Níveis de poder (T / custo):**

* **Truque** (efeito curto, truque, "flash"): **T 4 / 0–1 PP**
* **Padrão** (ataque, escudo, impulso, controle menor): **T 5 / 1 PP**
* **Forte** (área, cura, paralisia, hack "ao vivo"): **T 6 / 2 PP**
* **Grande** (mudança de cena, intervenção poderosa): **T 8–12 / 3 PP**

**Falha:** PP é perdido, e a consequência é imediata (sobrecarga, rastro digital, falha no ritual, atenção indesejada).

**Recuperação:** após a cena de conflito, você recupera **1 PP**, após um descanso seguro – até o máximo.

**Exemplo:** Em uma space opera, o Adepto tenta "dobrar o sensor" de um drone: Padrão, T 5, custo 1 PP. Rolagem <span class="rpg-token token-stat">M</span> <span class="rpg-token token-d8">k8</span> = 8: sucesso excepcional – o drone perde o sinal e se confunde na trilha.



---

### 5) Queda, risco e cura

* Quando você cai para **0 Corações**, você está **fora de ação** (ferido, atordoado, em choque – de acordo com a convenção).
* Um aliado pode gastar uma ação para te colocar em **1 Coração** (primeiros socorros, adrenalina, reinicialização do sistema).
* Após a cena, se vocês tiverem um momento de descanso: vocês voltam para **Corações Cheios**, desde que tenham as condições (abrigo, curativo, manutenção, refeição).
* Se a cena foi excepcionalmente brutal ou se os inimigos têm vantagem, o Narrador pode exigir que um “reset completo” necessite de uma parada segura.

**Exemplo:** O Szturm cai para 0. O especialista o puxa para trás da cobertura e gasta uma ação: o Szturm volta para 1 Coração e pode agir na próxima rodada.



---

### 6) Desenvolvimento de personagem (campanha sem tabelas e contabilidade)


Após a aventura, escolha **uma**:

* **Aumente** um atributo em 1 ponto (máx. até <span class="rpg-token token-d20">k20</span>), ou
* **+1 Coração** (máx. 7), ou
* **+1 Ponto de Poder** (máx. 5), ou
* **Novo Traço** (uma regra curta, em uma frase, acordada com o Mestre).

**Exemplos de traços (universais):**

* **Ênfase:** uma vez por cena, quando você acerta corpo a corpo, causa +1 Coração de dano.
* **Sombra:** quando você age de forma furtiva, tem um aumento de dado de 1 ponto.
* **Faísca:** uma vez por cena, você pode gastar 1 PP para obter automaticamente um “sucesso com custo” sem rolar.

**Exemplo:** O Adepto aumenta <span class="rpg-token token-stat">M</span> de <span class="rpg-token token-d8">k8</span> para <span class="rpg-token token-d12">k12</span> – agora seus poderes se manifestam de forma mais estável em T 5–6.



---

### 7) Variante "somente <span class="rpg-token token-d6">k6</span>" no modo **2k6** (rápido e muito jogável)


Se você não tem um conjunto de dados ou deseja graus de resultado mais "narrativos":

* Cada teste é: **role 2k6 + modificador de atributo**.
* **Modificadores de atributos** escolha no início: um atributo **+2**, um **+1**, um **+0**.
* Resultado:

  * **6 ou menos** – falha com consequência
  * **7–9** – sucesso com custo (compromisso, perda de recurso, posição pior)
  * **10+** – sucesso total
  * **12** – sucesso excepcional (benefício adicional)

**Dificuldade da situação:** em vez de mudar os limites, adicione **+1 / -1** ao rolamento (ajuda / atrapalha) ou custo em caso de 7–9.

**Mapeamento para a versão de dados-atributos (se você quiser conformidade):**

* <span class="rpg-token token-d6">k6</span> ≈ +0, <span class="rpg-token token-d8">k8</span> ≈ +1, <span class="rpg-token token-d12">k12</span> ≈ +2, <span class="rpg-token token-d20">k20</span> ≈ +3 (para personagens muito experientes).

**Exemplo:** Especialista atira em movimento: <span class="rpg-token token-stat">Z</span> = +2, situação difícil (-1). Rolamento 2k6 = 8, soma 9: sucesso com custo – acerta, mas termina em uma posição exposta.

