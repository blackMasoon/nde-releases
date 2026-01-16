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
generated_at: "2026-01-16T08:33:24.356Z"
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
# Guia do Mestre de Jogo

Automatic translation placeholder for <span class="rpg-token token-math">pt</span>

---



---

### 0) Regras de condução em 30 segundos

- **Comece pela ficção.** Primeiro descreva a situação e as ações dos jogadores, e só depois faça o teste.
- **Estabeleça a aposta antes da rolagem.** Diga: *o que está em jogo* e *o que acontecerá em caso de falha*.
- **Uma decisão → uma rolagem → efeito significativo.** Não divida uma intenção em 3 testes.
- **A falha impulsiona o jogo para frente.** Não "reinicie" a cena – altere-a com uma complicação, custo ou pressão.
- **Mantenha a consistência.** Mesmas condições → dificuldade semelhante, consequências semelhantes.
- **A grade é opcional.** Por padrão, o jogo funciona sem mapa: "Perto / Longe / Muito longe".



---

### 1.1. Quando lançar os dados?

Lançar os dados faz sentido apenas quando simultaneamente:
- o resultado **não é óbvio**,
- existe uma **aposta real** (algo vai mudar),
- ambas as partes aceitam que **a mecânica tem o direito de decidir**.

**Não lance os dados** quando:
- a ação é rotineira e sem pressão,
- o fracasso não trará nada interessante,
- o sucesso é certo e o preço já foi pago (por exemplo, os jogadores têm tempo, ferramentas e segurança).

**Exemplo (sem lançar dados):** Um especialista tem acesso administrativo e condições tranquilas – abrir uma porta padrão na base não requer teste.
**Exemplo (com lançamento de dados):** As mesmas portas, mas o alarme está ativo e uma patrulha se aproxima em 30 segundos – isso é um teste, pois a aposta é o tempo e a revelação.

### 1.2. Lista de verificação de resolução (procedimento de mesa)

1) O jogador diz: **o que faz** e **o que quer alcançar**.  
2) Você responde: **o que está no caminho** e **qual é a aposta**.  
3) Vocês escolhem um atributo: **Força (F)** / **Destreza (D)** / **Poder (<span class="rpg-token token-stat">P</span>)**.  
4) Você define a **Dificuldade (D)** ou **Defesa** (em combate).  
5) Você determina o modificador da situação: **aumentar/reduzir o dado** e possível **auxílio**.  
6) Jogada → resultado → consequência → atualização da cena.

Resumo: **Descrição → Aposta → Atributo → D/Defesa → Jogada → Consequência**.

### 1.3. Dificuldade (T): escala e regras práticas

Use uma única escala em todo o jogo. Isso constrói a confiança dos jogadores nas decisões do Mestre do Jogo.

- **T 3 – fácil:** condições favoráveis, sem pressão, resistência mínima.  
- **T 4 – padrão:** "trabalho normal" em uma aventura.  
- **T 5 – difícil:** pressão de tempo, risco, oponente, janela estreita.  
- **T 6 – muito difícil:** clara vantagem inimiga, alto risco, ação complexa sob estresse.  
- **T 8 – heroico:** feito acima da média; geralmente requer vantagem, plano ou recurso.  
- **T 12 – lendário:** momento “uau”; raramente sem preparação e muitas vezes com um grande custo.

**Regra prática:** se não souber o que definir – comece com **T 4** e só então justifique "para cima" ou "para baixo".

### 1.4. Modificadores sem Contagem: aumente/diminua o dado

Em vez de adicionar bônus e penalidades, em NDE você altera o **tamanho do dado** para um teste.

- **Situação Melhor:** aumente o dado em 1 grau  
  <span class="rpg-token token-<span class="rpg-token token-d4">d4</span>"><span class="rpg-token token-d4">d4</span></span>→<span class="rpg-token token-<span class="rpg-token token-d6">d6</span>"><span class="rpg-token token-d6">d6</span></span>→<span class="rpg-token token-<span class="rpg-token token-d8">d8</span>"><span class="rpg-token token-d8">d8</span></span>→<span class="rpg-token token-<span class="rpg-token token-d12">d12</span>"><span class="rpg-token token-d12">d12</span></span>→<span class="rpg-token token-<span class="rpg-token token-d20">d20</span>"><span class="rpg-token token-d20">d20</span></span>
- **Situação Pior:** diminua o dado em 1 grau (no sentido contrário).

**Ajuda de um aliado:** custa a ação dele e dá **aumento do dado em 1 grau** para o teste.

**Exemplo:** Castelo silencioso (D 4) vs castelo na chuva e sob ataque (D 5 + diminuição do dado, devido às mãos trêmulas e falta de visibilidade).
Isso geralmente funciona melhor do que "D 6 e +2 e -1".

### 1.5. Resultados dos testes: sucesso, falha e ritmo do jogo

- **1 no dado:** falha + complicação (complicação entra com certeza).  
- **Resultado < T:** falha (mas a situação muda).  
- **Resultado ≥ T:** sucesso.  
- **Resultado máximo no dado:** sucesso excepcional (benefício adicional).

#### Como projetar uma falha para não bloquear o jogo?

Antes que o jogador role o dado, estabeleça 1–2 tipos de custo:
- **tempo** (alguém consegue, algo se fecha),
- **posição** (mal posicionados, expostos),
- **recurso** (equipamento, munição, energia, Ponto de Poder),
- **atenção** (alarme, suspeitas, rastro).

**Exemplo (falha proativa):**  
O jogador quer forçar a porta. Falha não significa "não abrir".  
Falha significa: "você abre, mas faz barulho – a patrulha agora está Perto, e o nível de alarme aumenta".



---

### 2) Um Pouco de Sorte (Ł<span class="rpg-token token-stat">S</span>): como apoiar a dramaturgia sem estragar o jogo

Cada herói começa a sessão com **2 Ł<span class="rpg-token token-stat">S</span>**. É uma ferramenta dos jogadores, mas o Mestre de Jogo é responsável por sua "economia" na mesa.

### 2.1. Em que os jogadores gastam Ł<span class="rpg-token token-stat">S</span>?

Gaste 1 Ł<span class="rpg-token token-stat">S</span> para:
- realizar uma **re-rotação** (mantenha o melhor),
- **aumentar o dado em 1 grau** em um lance,
- transformar uma falha em um **sucesso com custo** (o Mestre de Jogo impõe um preço).

### 2.2. Quando atribuir LS adicional?

O MG pode atribuir **+1 LS** por:
- assumir conscientemente um risco que impulsiona a cena,
- aceitar as consequências sem "barganhar",
- encontrar uma solução criativa de acordo com a convenção,
- interpretar muito bem uma relação, motivação ou objetivo.

**Regra de higiene:** atribua de forma moderada (1–2 por sessão por pessoa em um jogo extremamente generoso). LS deve ser uma "faísca", não um combustível constante.

---



---

### 3) Conflito e luta

NDE deve lutar rapidamente. Se a luta durar 60 minutos, isso quase sempre significa: muitos inimigos 'com <span class="rpg-token token-heart">HP</span>' ou muitos lançamentos pequenos.

### 3.1. Padrão sem mapa: distâncias em cena

Use quatro distâncias:
- **Perto** – ao alcance da mão (corpo a corpo),
- **Não muito longe** – a alguns passos,
- **Longe** – do outro lado do palco,
- **Muito longe** – atirador/veicular.

Durante o turno, o personagem tem: **Movimento + 1 Ação**.
O movimento geralmente altera a distância em **1 nível** (Não muito longe→Perto).

**Exemplo:** O Guerreiro está Não muito longe. Durante o turno: ele avança (Perto) e ataca.

### 3.2. Opção: grade - quando você precisa de precisão

Se vocês jogam no mapa de grade: - movimento por turno: **até 5 quadrados**, - diagonais permitidas, - terreno difícil pode custar "2 quadrados por 1 entrada" (opcionalmente).

Todas as outras regras permanecem idênticas.

### 3.3. Defesa dos Oponentes e Dano

Na luta, em vez de Dificuldade, você usa a **Defesa** (uma espécie de "D para combate").  

**Defesa (aproximada):**  
- **Fraco** 4  
- **Típico** 5  
- **Elite** 6  
- **Chefe** 8 (chefe lendário 12)  

**Ataque:** jogada de **Força** (corpo a corpo) ou **Destreza** (à distância) contra a Defesa.  

**Dano (ritmo):**  
- um acerto causa **1 Coração**,  
- um sucesso excepcional causa **2 Corações** ou fornece um efeito poderoso (desarmamento, derrubada, desestabilização, dispersão).  

**Capangas e elites (modelo recomendado):**  
- **Capanga:** 1 acerto = desaparece da luta (derrotado, foge, imobilizado).  
- **Elite:** possui **2 Corações** (ou "2 acertos"), frequentemente tem uma vantagem tática.  
- **Chefe:** tem **3 Corações** + 1–2 "movimentos de chefe" (veja 3.6).  

Isso proporciona combates rápidos sem contagem de pontos.  

---

### 3.4. Abrigo, vantagem e 'terreno visível'

Em vez de multiplicar regras, use uma linguagem única: **dado para cima / dado para baixo**.

- Abrigo leve, fumaça, ângulo ruim: **reduza o dado do atacante** em 1 grau.
- Boa posição, surpresa, vantagem de altura: **aumente o dado** em 1 grau.
- Abrigo total: o ataque é impossível enquanto a situação não mudar.

**Exemplo:** Um sniper na janela está 'Longe' e tem vantagem de altura → o atacante sofre uma redução no dado.
A equipe muda a cena: granada de fumaça, flanqueamento, manobra – e a vantagem desaparece.

### 3.5. Ordem de combate sem contar a iniciativa

Esquema recomendado e rápido: 
1) **Os jogadores agem** (em qualquer ordem na mesa). 
2) **Os adversários agem**. 
3) Repita. 

Isso permite que os jogadores planejem combinações curtas sem sobrecarregar a mesa com a iniciativa.

### 3.6. Como conduzir um chefe para torná-lo interessante (e não apenas uma 'esponja de dano')

O chefe em NDE deve ter:
- **Defesa 8** (ou 12 na versão de 'final de temporada'),
- **3 Corações**,
- **1–2 movimentos únicos**, que mudem a cena.

**Movimentos de chefe exemplares (universais):**
- **Repulsão:** alguém atingido recua 1 distância (Perto→Longe) e perde a posição.
- **Quebra de guarda:** o chefe destrói a defesa ou força o adversário a sair da cobertura.
- **Chamada de reforços:** juntam-se 2 capangas ou uma elite (de preferência uma vez por luta).
- **Área de perigo:** a área se torna perigosa (fogo, eletricidade, runas) – quem permanecer nela arrisca um teste.

**Regra:** o movimento do chefe deve mudar o campo de jogo, não apenas 'causar mais dano'.

### 3.7. Moral e comportamento dos inimigos (procedimento leve)

Quando:
- o primeiro capanga cair, ou
- a elite perder seu primeiro Coração, ou
- o chefe perder seu segundo Coração,

lance <span class="rpg-token token-<span class="rpg-token token-d6">d6</span>"><span class="rpg-token token-d6">d6</span></span> e decida:
- **1–2:** retiram-se / procuram abrigo / negociam,
- **3–4:** mantêm a posição,
- **5–6:** avançam agressivamente.

Modifique com **+1** se tiverem vantagem, **-1** se estiverem assustados ou isolados.



---

### 4) Poderes (<span class="rpg-token token-stat">M</span>) do lado do Mestre: como avaliá-los e como não estragar o ritmo

No NDE, 'Poder' abrange magia, psionismo, cibernética, hacking, carisma 'nível de filme' – dependendo do mundo.

### 4.1. Escala de poder: Dificuldade e custo dos Pontos de Poder

- **Truque:** D 4, custo 0–1 PP (pequeno, efeito rápido).
- **Padrão:** D 5, custo 1 PP (alvo único, pequeno salto, escudo).
- **Forte:** D 6, custo 2 PP (área, controle, cura).
- **Grande:** D 8–12, custo 3 PP (efeito de mudança de cena).

**Dica:** se o efeito deve "mudar as regras da cena" (ponte de gelo, apagão no bairro) – isso é um Grande poder.

### 4.2. Consequências da falha de poder

A falha deve ser concreta e imediata: - perda de <span class="rpg-token token-power">PM</span> (sempre), - sobrecarga (queda de posição, exposição), - rastro (digital/astral), - efeito colateral no ambiente (ruído, brilho, cheiro, eco).

**Exemplo:** Hack "ao vivo" em combate. Falha: <span class="rpg-token token-power">PM</span> se perde e o sistema registra o intruso - inicia-se o contador "contra-ICE".

### 4.3. Defesa contra o poder

Se a ficção o justifica, permita um "contra-teste":
- **Destreza** (esquiva, reflexo) ou
- **Poder** (resistência, contra-ritual, barreira).

O contra-teste não deve multiplicar as rolagens. Use-o onde isso torna a cena mais interessante (por exemplo, paralisia, controle mental).




---

### 5.1. Construa cenas em 5 passos

1) **Objetivo da cena:** o que o grupo deve alcançar (específico).  
2) **Obstáculos:** 2-3 tipos diferentes (pessoas, dispositivos, ambiente).  
3) **Ameaça:** adversários, perigos, armadilhas, pressão do tempo.  
4) **Contador (opcional):** 3-5 campos; falhas movem o contador; no final, há uma grande consequência.  
5) **Recompensa e consequências:** o que muda com o sucesso, o que muda com o fracasso.

Este é o "motor de cena" mínimo - funciona em fantasia, sci-fi e crime.

### 5.2. Contadores (clocks) – versão simples

O contador tem 3–5 campos. Preenche-se quando:
- um teste termina em falha,
- alguém faz barulho,
- os inimigos têm tempo para reagir.

Quando o contador se preenche, ocorre um efeito:
- alarme,
- reforços,
- fechamento de caminho,
- perda de recurso,
- escalada de conflito.

**Exemplo:** "Alarme 0/4". Falha em furtividade = +1. Sucesso excepcional = -1 (opcionalmente).  
Quando chega a 4/4 – aparece uma patrulha e as portas se trancam.

---

### 5.3. Como ajustar a "dificuldade da cena" sem contar tudo

Para um grupo de 3–5 heróis: 

- **Fácil:** 3–5 lacaios ou um elite sem vantagens de terreno.  
- **Padrão:** 6–8 lacaios ou um elite + 2–4 lacaios, ou um perigo ambiental.  
- **Difícil:** chefe + 2–4 lacaios, ou 2 elites + 3–5 lacaios, ou um marcador 3.  
- **Heroico:** chefe + apoio + pressão de terreno + marcador 3–5.

**Mais importante:** o terreno e as coberturas frequentemente significam mais do que o número de inimigos.



---

### 6.1. Furtividade e infiltração: "Alarme"

1) Estabeleça o contador de **Alarme 0/3 a 0/5**. 
2) Cada falha = +1 alarme. 
3) Os jogadores podem reduzir o alarme com ações (ex.: sinal falso, sabotagem) – esses são testes normais. 
4) No máximo, entra em efeito: patrulha, trancamento, bloqueio.

**Exemplo:** A equipe caminha pelo corredor. O especialista quer contornar as câmeras (<span class="rpg-token token-stat">M</span>, D 5). Falha = +1 alarme. 
Antes de lançar, ele sabe o que está arriscando – e isso é a chave.

### 6.2. Perseguição: "Distância de perseguição"

Determine a **Distância** em passos, por exemplo, **3** (média).
Cada "turno de perseguição":
- o fugitivo faz um teste (<span class="rpg-token token-stat">Z</span> ou <span class="rpg-token token-stat">M</span> dependendo do método),
- o perseguidor faz um teste,
- o sucesso do fugitivo aumenta a distância, o sucesso do perseguidor diminui,
- quando a distância cair para **0** – captura,
- quando aumentar para **5** – fuga.

Adicione obstáculos (curva, multidão, barricada) como descrição + modificador de dados.

### 6.3. Investigação: "Pistas em vez de uma parede de testes"

Regra: **uma pista chave não pode ficar presa em um único teste**. 
Se a cena investigativa deve prosseguir, a pista chave está disponível:
- automaticamente (se os jogadores fizerem algo sensato),
- ou após um teste, mas o fracasso a fornece "com um custo" (tempo, pista falsa, alarme).

**Exemplo:** Examinando um corpo. Sucesso: eles descobrem a verdade. Fracasso: eles descobrem a verdade, mas a guarda chega ou alguém os nota.

### 6.4. Conflito social: aposta, pressão, consequência

Não transforme a conversa em uma "luta de dados". Determine: 
- o que o NPC quer, 
- o que os jogadores querem, 
- qual é a aposta, 
- quantos "movimentos" existem até o ponto de crise (contador de 3 a 5). 

Os testes **<span class="rpg-token token-stat">M</span>** (influência, blefe, autoridade) ou **<span class="rpg-token token-stat">Z</span>** (ler intenções) mudam a posição da conversa. 
Fracasso implica em custo (má impressão, perda de recurso, tempo, hostilidade).



---

### 7.1. Complicações em caso de falha (jogue <span class="rpg-token token-<span class="rpg-token token-d6">d6</span>"><span class="rpg-token token-d6">d6</span></span>)

1. Perda de tempo / alguém conseguiu reagir.  
2. Revelação da posição / aumento do alarme.  
3. Dano menor: -1 Coração ou perda de recurso.  
4. <span class="rpg-token token-stat">M</span>á posição: empurrão, queda, exposição.  
5. Perda ou dano de equipamento.  
6. Uma nova ameaça aparece na cena.

### 7.2. Benefícios em caso de sucesso excepcional (jogue <span class="rpg-token token-<span class="rpg-token token-d6">d6</span>"><span class="rpg-token token-d6">d6</span></span>)

1. Mais rápido (economiza tempo ou movimento). 
2. Mais silencioso (nenhum aumento de alarme). 
3. Sem custo (por exemplo, sem gastar <span class="rpg-token token-power">PM</span> / sem consequências de terreno). 
4. Maior efeito (maior alcance, alvo adicional). 
5. Melhor posição do aliado (alguém recebe um impulso de dados na próxima ação). 
6. Dica adicional ou vantagem narrativa.

### 7.3. Inserção rápida do inimigo (formato para anotações)

> **Nome — Defesa, Corações, Tática, Truque/Vantagem**

- **Capanga:** Defesa 4–5, 1 acerto = desaparece.  
- **Elite:** Defesa 6, 2 Corações, uma vantagem (mobilidade/contra/abrigo).  
- **Chefe:** Defesa 8 (ou 12), 3 Corações, 1–2 movimentos de chefe.

**Exemplo (universal):**  
> **Segurança — Defesa 5, 1 acerto, controla o corredor, granada de fumaça (uma vez)**



---

### 8) Segurança e acordo da mesa (mínimo)

- Decidam o que não será jogado (temas tabu) e o que será "passado rapidamente".
- Concordem com um sinal simples para interromper a cena (por exemplo, "pare" ou "pausa").
- Resolva os conflitos à mesa através de conversas fora da ficção, não com "decisões com raiva".

Isso melhora a qualidade do jogo mais do que qualquer mecânica.



---

### 9) Modularidade e desenvolvimento pela comunidade: como manter sob controle

Se você estiver construindo o NDE como um "motor", a maneira mais fácil de a comunidade desenvolvê-lo é por meio de pacotes:

- **Pacote de gênero** (fantasia/cyberpunk/terror): mapeamento de Poderes, lista de talentos, equipamento, adversários, 1–2 procedimentos (por exemplo, medo, perseguição). 
- **Pacote de adversários:** 10–20 entradas de capanga/elite/chefe + táticas.
- **Pacote de aventuras:** cenas de 1 página com contadores e apostas.

**Exigência de qualidade da contribuição:** cada nova regra deve ter:
- uma frase "para quê serve" (qual problema resolve),
- descrição curta da regra,
- exemplo de 3–5 linhas.

Dessa forma, os complementos não desestruturarão o núcleo e serão compreensíveis para novos jogadores.

