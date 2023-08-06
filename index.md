<style>
  section {
    background: #fff url(./img/background.png) no-repeat center center;
    background-size: cover;
  }

  .transparent {
    background-color: transparent!important;
  }

  .cabecalho {
    position: absolute;
    top: 10%;
    margin-left: 5%;
    margin-right: 10%;
    font-size: 48px;
    font-weight: bold;
  }

  .conteudo {
    top: 30%;
    margin-left: 5%;
    margin-right: 10%;
    font-size: 28px;
    text-align: justify;
  }

  .conteudo-absoluto {
    position: absolute;
    top: 30%;
    margin-left: 5%;
    margin-right: 10%;
    font-size: 28px;
    text-align: justify;
  }
  
  .large {
    font-size: 36px;
  }

  .normal {
    font-size: 22px;
  }
  .regular {
    font-size: 18px;
  }
  .small {
    font-size: 16px;
  }
  .footnotesize {
    font-size: 14px;
  }
  .scriptsize {
    font-size: 12px;
  }
  .tiny {
    font-size: 10px;
  }
  .bold {
    font-weight: bold;
  }
  .center {
    text-align: center;
  }
  section.lead p {
    text-align: justify;
  }
  section.lead h1 {
    text-align: center;
  }
  section.lead h2 {
    text-align: center;
  }
  .two-columns-33-66 {
    position: absolute;
    top: 30%;
    margin-left: 5%;
    margin-right: 10%;
    display: grid;
    grid-template-columns: 1fr 2fr;
    font-size: 28px;
    text-align: justify;
  }
  .two-columns-66-33 {
    position: absolute;
    top: 30%;
    margin-left: 5%;
    margin-right: 10%;
    display: grid;
    grid-template-columns: 2fr 1fr;
    font-size: 28px;
    text-align: justify;
  }

  .two-columns-50-50 {
    position: absolute;
    top: 30%;
    margin-left: 5%;
    margin-right: 10%;
    display: grid;
    grid-template-columns: 1fr 1fr;
    font-size: 28px;
    text-align: justify;
  }
</style>

<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>


# Análise de Circuitos Elétricos
## Aula 02 - Resistência em Série, Resistência em Paralelo, Divisores de Tensão e Divisores de Corrente
 
Prof. M.Sc. Diego Ascânio Santos (ascanio@cefetmg.br)

Aula baseada sobre o material do professor Dr. Emerson Gonçalves de Melo (emerdemelo@usp.br - DEMAR EEL USP) e da Khan Academy.

Divinópolis, 2023.


---

# Roteiro

1. Revisão Lei de Ohm
2. Resistência Equivalente
3. Resistência Equivalente Para Resistores em Série
4. Resistência Equivalente Para Resistores em Paralelo
5. Simplificação de Redes de Resistores
6. Divisão da Tensão
7. Divisão da Corrente
8. Lista 2


---

<div class="cabecalho large">

Revisão - Lei de Ohm

</div>
<div class="two-columns-50-50">

<div class="regular">

- Da definição de $J$ é obtida a lei de Ohm

Parâmetros distribuídos:

$$
J = \sigma E \rightarrow E = {J \over \sigma} \text{ ou } E = \rho J
$$

Parâmetros concentrados:

$$
I = GV \rightarrow V = {I \over G} \text{ ou } V = RI
$$

Lei de Ohm:

$$
V = RI \text{ ou } I = {V \over R} \text{ ou } R = {V \over I}
$$

<center>

Essas relações entre Tensão, Corrente, Resistência e Condutividade Elétrica são fundamentais para o entendimento da aula de hoje e de todas as outras!

</center>

</div>

<div class="regular">
    <center>
        <img class="transparent" src="./img/ohm.png" width=75% >
    </center>
</div>

</div>



---

<div class="cabecalho">
    Equivalência de Resistências
</div>

<div class="two-columns-50-50">
<div class="regular">

- Em muitos circuitos, a norma é que existam vários resistores;
- Frequentemente é necessário saber a resistência total do circuito:
    - Causada por todos os resistores;
- Ou a parcial:
    - Restrita a apenas segmentos dos circuitos;
- Existem resistências em série, paralelas e mistas;
- A resistência total (ou parcial) — equivalente — é determinada pela CONTRIBUIÇÃO DE TODOS OS RESISTORES do circuito (ou do segmento).

</div>
<div>
    <center>
        <img class="transparent" src="./img/equivalencia_resistores.png" width=50%>
    </center>
</div>
</div>


---

<div class="cabecalho">
    Equivalência de Resistências - Resistores em Série
</div>

<div class="two-columns-50-50">
<div class="small">

- Quando existem $n$ resistores em série, a resistência equivalente é a soma das resistências de cada um dos resistores:
    - $R_{eq} = \sum_{i = 1}^{n}{R_{i}}$
- Em resistores em série, a corrente $i$ é igual em todas as resistências.
    - Porquê a carga elétrica não pode se acumular em um resistor, sempre fluindo do ponto de maior potencial elétrico para o ponto de menor potencial.
- Pela lei de Ohm, $V = RI$. Como a corrente é igual em todos os resistores, logo, a diferença de potencial em cada resistor é dada por;
    - $V_{i} = R_{i} I; \text{ } \forall i = {1, \cdots, n}$
- Cada resistor $i$, por ser um elemento de oposição ao fluxo da carga elétrica, faz com que a diferença de potencial diminua em $R_{i}I$ na sua saída.

</div>
<div>
    <center>
        <img class="transparent" src="./img/resistores_equivalencia_serie.png">
    </center>
</div>
</div>


---

<div class="cabecalho large">
    Equivalência de Resistências - Resistores em Paralelo 
</div>

<div class="two-columns-50-50">
<div class="small">

- Em resistores paralelos, a tensão $V$ que chega aos resistores é igual em todas as resistências.
    - Porquê o mesmo potencial elétrico se aplica a todos os resistores ao mesmo tempo.
- Considerando que a tensão $V$ em todos os resistores é igual, mas, seus valores de resistência são distintos, pela lei de Ohm, a corrente $i_{1}$ que passa pelo resistor $R_{1}$, quando multiplicada por $R_{1}$ é: $R_{1}i_{1} = V$. Entretanto, isto equivale para todas as outras resistências:
    - $R_{1}i_{1} = \cdots = R_{n}i_{n} = V$
- Como $V$ é constante e os valores de $R_{1}, \cdots, R_{n}$ sao variáveis, logo, os valores $i_{1}, \cdots, i_{n}$ também devem ser variáveis.
- Temos uma fonte variável de corrente que fornece uma corrente $I_{S}$ para o sistema.
    - Pela conservação da energia, sabemos que a soma das correntes $i_{1}, \cdots, i_{n}$ tem que ser igual a corrente total $I_{S}$:
        - $(\sum_{j = 1}^{n}{i_{j}}) = I_{S}$ 


</div>
<div style="margin: auto;">
    <center>
        <img class="transparent" src='img/equivalencia_resistores_paralelos.svg'>
    </center>
</div>
</div>


---

<div class="cabecalho large">
    Equivalência de Resistências - Resistores em Paralelo 
</div>

<div class="two-columns-50-50">
<div class="small">

- Pela conservação da energia, sabemos que a soma das correntes $i_{1}, \cdots, i_{n}$ tem que ser igual a corrente total $I_{S}$:
    - $(\sum_{j = 1}^{n}{i_{j}}) = I_{S}$
- Pela Lei de Ohm:
    - $R_{1}i_{1} = \cdots = R_{n}i_{n} = V$
- Logo:
    - $i_{1} = {{V} \over {R_{1}}}$; $i_{2} = {{V} \over {R_{2}}}$; $\cdots$; $i_{n} = {{V} \over {R_{n}}}$; 
- Pela Conservação da energia:
    - $(\sum_{j = 1}^{n}{i_{j}}) = I_{S} = (\sum_{j = 1}^{n}{{V} \over {R_{j}}}) = V (\sum_{j = 1}^{n}{{1} \over {R_{j}}})$
- Novamente, pela lei de Ohm:
    - $R_{\text{parallel}} = {V \over I_{S}}$
- Como $I_{S} = V (\sum_{j = 1}^{n}{{1} \over {R_{j}}})$, logo:
    - $R_{\text{parallel}} = {{V} \over {V \sum_{j = 1}^{n} {{{1} \over {R_{j}}}}}} =  {{1} \over {\sum_{j = 1}^{n} {{{1} \over {R_{j}}}}}}$
$$
\therefore {1 \over R_{\text{parallel}}} = {1 \over {R_{1}}} + \cdots + {1 \over {R_{n}}} = {\sum_{i = 1}^{n} {{{1} \over {R_{i}}}}}
$$

</div>
<div style="margin: auto;">
    <center>
        <img class="transparent" src='img/equivalencia_resistores_paralelos.svg'>
    </center>
</div>
</div>


---

<div class="cabecalho large">
    Equivalência de Resistências - Exercícios Resolvidos
</div>

<div class="two-columns-50-50">
<div class="small">

1. (FEI-SP) Qual a Resistência equivalente da associação a seguir?

    <center>
        <img class="transparent" src='img/exercicio_01.png'>
    </center>

    - a) $80 \Omega$ b) $100 \Omega$ c) $90 \Omega$ d) $62 \Omega$ e) $84 \Omega$ 

Resolvendo os resistores em paralelo:

$$
\begin{align}
{1 \over {R_{eq}}} &= {1 \over 20} + {1 \over 30} \rightarrow \\
{1 \over {R_{eq}}} &= {30 \over 600} + {20 \over 600} \rightarrow \\
50 R_{eq} &= 600 \rightarrow \\
R_{eq} &= 12 \Omega
\end{align}

$$

</div>
<div class="small">

Agora que temos a resistência paralela equivalente, devemos calcular a resistência paralela em série, que é:

$$ R_{eq} = 12 \Omega + 50 \Omega = 62 \Omega $$

Sendo a resposta correta, letra d)

<hr>

2. (F.M. Itajubá-MG) Abaixo temos esquematizada uma associação de resistências. Qual é o valor da resistência equivalente entre os pontos A e B?

<center>
    <img class="transparent" src='img/exercicio_02.png'>
</center>

</div>
</div>


---

<div class="cabecalho large">
    Equivalência de Resistências - Exercícios Resolvidos
</div>
<div class="conteudo regular">

- Para facilitar a resolução, é melhor redesenhar o circuito de outra forma:

<center>
    <img class="transparent" src="img/desenho.png" width=50%>
</center>

- Assim, temos três resistências em série de $1 \Omega, 3 \Omega, 6 \Omega$ em paralelo com uma de $2.5 \Omega$. A resistência equivalente destas resistências também está em série com outras resistências de $1 \Omega$ e $0.5 \Omega$.

- Resolvendo: $R = [0.5 + ({1 \over {{1 \over 2.5} + {1 \over {1 + 3 + 6}}}}) + 1] \Omega \rightarrow R = 3.5 \Omega$

</div>


---

# Simplificação de Redes de Resistores


---

<div class="cabecalho">
    Simplificando Redes de Resistores
</div>

<div class="two-columns-50-50">
<div class="small">

- Existem redes de resistores complicadas, como a da imagem abaixo:

<img class="transparent" src="https://cdn.kastatic.org/ka-perseus-images/16b4aecbaae9e2a5e0b50fc70ace724f471ad0c0.svg">

- Diante disso, qual a melhor estratégia para extrair a resistência equivalente deste circuito?

</div>
<div class="small">

## Estratégia de Simplificação de Redes de Resistores

1. Comece o mais longe possível da fonte do circuito em questão.
2. Substitua resistores em série ou em paralelo por sua resistência equivalente.
3. Continue movendo-se à esquerda até que um único resistor equivalente represente a rede inteira de resistores.

- Faremos a simplificação deste circuito no quadro. No slide a seguir existe um vídeo da Khan Academy explicando o procedimento.

</div>
</div>


---

<div class="conteudo regular">
    <video width=100% height=100% controls>
        <source src="./videos/simplificando_resistores.mp4" type="video/mp4">
    </video>

[Simplificando redes de resistores](https://pt.khanacademy.org/science/electrical-engineering/ee-circuit-analysis-topic/ee-resistor-circuits/v/ee-simplifying-resistor-networks) por [Khan Academy](https://pt.khanacademy.org/) licenciado sob [CC BY-NC-SA 3.0](https://creativecommons.org/licenses/by-nc-sa/3.0/)

</div>


---

<!-- _class: lead -->
# Transformação $\Delta - Y | Y - \Delta$


---

<div class="cabecalho large">

Transformação $\Delta - Y | Y - \Delta$

</div>
<div class="two-columns-50-50">
<div class="small">

- Técnicas de simplificação nem sempre conseguem calcular resistência equivalente:

<center>
    <img class="transparent" src="https://cdn.kastatic.org/ka-perseus-images/5d6b711e0f765ad7e88a6d18b39bf20850ac8e18.svg">
</center>

- Quantos resistores estão em paralelo? Quantos estão em série? Como calcular a resistência equivalente deste circuito?
    - Através da transformação $\Delta - Y$ (Delta - Y).

</div>
<div class="small">

<!-- _class: lead -->
## $\Delta - Y$

- Delta e Ípsilon vêm do formato do esquema, que lembra essas letras:

<center>
    <img class="transparent "src="https://cdn.kastatic.org/ka-perseus-images/801966b0b8e1e43a390d1975a0bdee3d3b59259f.svg">
</center>

- Permite trocar três resistores num formato $\Delta$ por outros três num formato $Y$ (e vice-versa).

</div>
</div>


---

<div class="cabecalho large">

Transformação $\Delta - Y | Y - \Delta$

</div>
<div class="conteudo small">

- Permite trocar três resistores num formato $\Delta$ por outros três num formato $Y$ (e vice-versa).
    - Isso é útil para transformar a disposição dos resistores e poder determinar com clareza quem está em série e quem está em paralelo.
        - O que antes não era simplificável, agora se torna!

- Circuito do exemplo após passar por uma transformação $\Delta - Y$:

<div class="two-columns-50-50" style="position: relative; top: 0%">
    <div>
        <center>
            <img class="transparent" src="https://cdn.kastatic.org/ka-perseus-images/5d6b711e0f765ad7e88a6d18b39bf20850ac8e18.svg">
        </center>
    </div>
    <div>
        <center>
            <img class="transparent" src="https://cdn.kastatic.org/ka-perseus-images/8b336f68ba2a02ea0c5a9b25b4eb91c0e041bead.svg">
        </center>
    </div>
</div>

Agora é possível calcular sua resistência equivalente!

</div>


---

<div class="cabecalho large">

Transformação $\Delta - Y | Y - \Delta$

</div>
<div class="conteudo normal">

- Permite trocar três resistores num formato $\Delta$ por outros três num formato $Y$ (e vice-versa).
- Aplicável apenas a configurações com três terminais.
- Deve-se observar que as duas configurações possuem um número diferente de nós:
    - $\Delta$ possui três nós.
    - $Y$ possui quatro (com um nó no centro).

<center>
    <img class="transparent" src="https://cdn.kastatic.org/ka-perseus-images/801966b0b8e1e43a390d1975a0bdee3d3b59259f.svg">
</center>

</div>


---

<div class="cabecalho" style="font-size: 26px;">

Transformação $\Delta - Y | Y - \Delta$

</div>
<div class="conteudo regular">

Para ocorrer a transformação, a resistência entre cada par de terminais deve ser igual, antes e depois.

<center>
    <img class="transparent" width=35% src="https://cdn.kastatic.org/ka-perseus-images/05cc24f20113bc6937dec9b8e85ee09e032d2a66.svg">
</center>

Considerando os terminais $x$ e $y$ (e que $z$ não está conectado a nada):
- Na configuração $\Delta$ a resistência entre $x$ e $y$ é dada por:
    - $R_{xy} = {{{1} \over {{{1} \over {R_{c}}} + {{1} \over {R_{a} + R_{b}}}}}} = {{R_{c} (R_{a} + R_{b})} \over {R_{a} + R_{b} + R_{c}}}$
- Na configuração $Y$ a resistência entre $x$ e $y$ é dada por:
    - $R_{xy} = R_{1} + R_{2}$
- Logo:

$$
R_{xy} = {{{1} \over {{{1} \over {R_{c}}} + {{1} \over {R_{a} + R_{b}}}}}} = {{R_{c} (R_{a} + R_{b})} \over {R_{a} + R_{b} + R_{c}}} = R_{1} + R_{2}
$$

</div>


---

<div class="cabecalho">

Transformação $\Delta - Y | Y - \Delta$

</div>
<div class="conteudo normal">

Aplicando os mesmos princípios para todos os terminais:

$$
\begin{align}
R_{xy} &= {{{1} \over {{{1} \over {R_{c}}} + {{1} \over {R_{a} + R_{b}}}}}} = {{R_{c} (R_{a} + R_{b})} \over {R_{a} + R_{b} + R_{c}}} = R_{1} + R_{2} \\
R_{xz} &= {{{1} \over {{{1} \over {R_{b}}} + {{1} \over {R_{a} + R_{c}}}}}} = {{R_{b} (R_{a} + R_{c})} \over {R_{a} + R_{b} + R_{c}}} = R_{1} + R_{3} \\
R_{yz} &= {{{1} \over {{{1} \over {R_{a}}} + {{1} \over {R_{b} + R_{c}}}}}} = {{R_{a} (R_{b} + R_{c})} \over {R_{a} + R_{b} + R_{c}}} = R_{2} + R_{3}
\end{align}
$$

</div>


---

<div class="cabecalho">

Transformação $\Delta \rightarrow Y$

</div>
<div class="conteudo normal">

Aplicando manipulações algébricas nas equações anteriores, que vocês deverão desenvolver, temos na transformação $\Delta \rightarrow Y$ as seguintes equivalências entre resistências:

$$
\begin{align}
R_{1} &= {{R_{b}R_{c}} \over {R_{a} + R_{b} + R_{c}}} \\
R_{2} &= {{R_{a}R_{c}} \over {R_{a} + R_{b} + R_{c}}} \\
R_{3} &= {{R_{a}R_{b}} \over {R_{a} + R_{b} + R_{c}}} 
\end{align}
$$

E ao transformar $\Delta$ para $Y$, se introduz um nó adicional ao circuito.

</div>


---

<div class="cabecalho">

Transformação $Y \rightarrow \Delta$

</div>
<div class="conteudo normal">

Continuando as manipulações algébricas nas equações anteriores, que vocês deverão desenvolver, temos na transformação $Y \rightarrow \Delta$ as seguintes equivalências entre resistências:

$$
\begin{align}
R_{a} &= {{R_{1}R_{2} + R_{2}R_{3} + R_{3}R_{1}} \over {R_{1}}} \\
R_{b} &= {{R_{1}R_{2} + R_{2}R_{3} + R_{3}R_{1}} \over {R_{2}}} \\
R_{c} &= {{R_{1}R_{2} + R_{2}R_{3} + R_{3}R_{1}} \over {R_{3}}}
\end{align}
$$

E ao transformar $Y$ para $\Delta$, se remove um nó do circuito.

</div>
