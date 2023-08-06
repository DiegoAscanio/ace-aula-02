<style>
  section {
    background: #fff url(./img/background.png) no-repeat center center;
    background-size: cover;
  }

  .transparent {
    background-color: transparent!important;
  }

  .transparent-table-tr-td-th {
    background-color: rgba(0, 0, 0, 0.0) !important;
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

<!-- _class: lead -->
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


---

<div class="cabecalho large">

Resolução do Exemplo por $\Delta \rightarrow Y$

</div>
<div class="two-columns-50-50">
<div class="regular">

- Não existem resistores em série ou paralelo:

<center>
    <img class="transparent" src="https://cdn.kastatic.org/ka-perseus-images/5d6b711e0f765ad7e88a6d18b39bf20850ac8e18.svg">
</center>

</div>

<div class="regular">

- Redesenhando o circuito vemos que temos duas conexões $\Delta$ empilhadas uma sobre a outra:

<center>
    <img class="transparent" src="https://cdn.kastatic.org/ka-perseus-images/ed2ef2bdcfab1d6c66ae3bc17629a2c783d3ec64.svg">
</center>

- Ao fazermos uma transformação $\Delta \rightarrow Y$, adicionamos um nó ao circuito. Será que isso ordena os resistores de modo que seja possível determinar quem está em série e quem está em paralelo?

</div>

</div>


---

<div class="cabecalho large">

Resolução do Exemplo por $\Delta \rightarrow Y$

</div>
<div class="two-columns-50-50">
<div class="regular">

- Escolhemos arbitrariamente o $\Delta$ inferior:

<center>
    <img class="transparent" src="https://cdn.kastatic.org/ka-perseus-images/a656d249bff7a459daa9df0ebcb2c9b84f318f6d.svg">
</center>

</div>

<div class="regular">

- Ao fazer $\Delta \rightarrow Y$ no $\Delta$ inferior, os resistores pretos do $\Delta$ são substituídos pelos cinzas da configuração $Y$:

<table class="transparent-table-tr-td-th">
<tr class="transparent-table-tr-td-th">

<td class="transparent-table-tr-td-th">
<center>
    <img class="transparent" src="https://cdn.kastatic.org/ka-perseus-images/05cc24f20113bc6937dec9b8e85ee09e032d2a66.svg">
</center>
</td>
<td class="transparent-table-tr-td-th">
<center>
    <img class="transparent" src="https://cdn.kastatic.org/ka-perseus-images/b0c3af9ae2f46f3efa5620d14b6886971eeac777.svg">
</center>
</td>

</tr>
</table>

</div>

</div>


---

<div class="cabecalho large">

Resolução do Exemplo por $\Delta \rightarrow Y$

</div>
<div class="conteudo small" style="margin: auto;">
<table class="transparent-table-tr-td-th">
<tr class="transparent-table-tr-td-th">

<td class="transparent-table-tr-td-th">
<center>
    <img class="transparent" src="https://cdn.kastatic.org/ka-perseus-images/05cc24f20113bc6937dec9b8e85ee09e032d2a66.svg">
</center>
</td>
<td class="transparent-table-tr-td-th">
<center>
    <img class="transparent" src="https://cdn.kastatic.org/ka-perseus-images/b0c3af9ae2f46f3efa5620d14b6886971eeac777.svg">
</center>
</td>

</tr>
</table>


- Aplicando as equações de $\Delta \rightarrow Y$ temos:

$$
\begin{align}
R_{1} &= {{R_{b}R_{c}} \over {R_{a} + R_{b} + R_{c}}} = {{3 \times 5} \over {12}} = 1.25 \Omega \\
R_{2} &= {{R_{a}R_{c}} \over {R_{a} + R_{b} + R_{c}}} = {{4 \times 3} \over {12}} = 1 \Omega \\
R_{3} &= {{R_{a}R_{b}} \over {R_{a} + R_{b} + R_{c}}} = {{4 \times 5} \over {12}} = {5 \over 3} \Omega
\end{align}
$$


</div>


---

<div class="cabecalho large">

Resolução do Exemplo por $\Delta \rightarrow Y$

</div>
<div class="conteudo normal">

Substituindo o circuito $\Delta$ pelo seu $Y$ equivalente:

<center>
    <img class="transparent" src="https://cdn.kastatic.org/ka-perseus-images/f4a19d613dccddb714e8ca1e8ba002dccc7e628d.svg">
</center>

Agora que conseguimos distinguir quais resistores estão em paralelo e quais resistores estão em série, o circuito pode ser simplificado para calcular a resistência equivalente. 

</div>


---

<div class="cabecalho large">

Resolução do Exemplo por $\Delta \rightarrow Y$

</div>
<div class="conteudo regular" style="margin: auto;">

Somando os resistores do ramo esquerdo e do ramo direito temos:

<table class="transparent-table-tr-td-th">
<tr class="transparent-table-tr-td-th">

<td class="transparent-table-tr-td-th">
<center>
    <img class="transparent" src="https://cdn.kastatic.org/ka-perseus-images/f4a19d613dccddb714e8ca1e8ba002dccc7e628d.svg">
</center>
</td>
<td class="transparent-table-tr-td-th">
<center>
    <img class="transparent" src="https://cdn.kastatic.org/ka-perseus-images/17c405dba966e5cfeecb4c98cd4b5cfe7e4b1ee0.svg">
</center>
</td>

</tr>
</table>

Calculando a resistência equivalente dos resistores paralelos: ${{1} \over {{1 \over 4.375} + {1 \over 5}}} = {7 \over 3} \Omega$

Somando com a resistência de ${5 \over 3} \Omega$ em série: ${7 \over 3} + {5 \over 3} = {12 \over 3} = 4 \Omega$.

Portanto, a resistência equivalente do segmento de circuito é de $4 \Omega$.

</div>


---

<!-- _class: lead -->
# Divisão da Tensão


---

<div class="cabecalho">
    
Divisão da Tensão

</div>
<div class="conteudo" style="font-size: 20px;">

Tecnologias distintas de circuitos integrados (CIs) - TTL e CMOS - trabalham em níveis de tensão diferentes. Os circuitos construídos sobre a tecnologia TTL trabalham com níveis de tensão de 0V até +5V. Já os construídos com CMOS trabalham com níveis de tensão entre 0V e +3.3V.

Não obstante serem tecnologias distintas, frequentemente é necessário que CIs TTL e CMOS trabalhem juntos.

É conhecido que a presença de sobretensão (Tensões acima de +3.3V) em circuitos CMOS pode danificá-los.

Assim, considerando que em muitas situações circuitos TTL e CMOS precisam interagir, como mitigar a sobretensão causada pela tensão superior dos circuitos TTL?

Por meio da sua diminuição! Se houver uma forma de diminuir 5V para 3.3V os circuitos CMOS ficam protegidos contra eventuais danos de sobretensão.

Como diminuir esta tensão? Através da **Divisão da Tensão**!

</div>


---

<div class="cabecalho large">
Divisão da Tensão
</div>
<div class="conteudo small">

- Em resistores em série, a corrente $i$ é igual em todas as resistências. Porquê a carga elétrica não pode se acumular em um resistor, sempre fluindo do ponto de maior potencial elétrico para o ponto de menor potencial.

- Portanto, $V_{Rk} = R_{k} \cdot i$

<center>
    <img src="https://cdn.kastatic.org/ka-perseus-images/7c02d028f874842f69e5967b3972ab2e35ec21cf.svg" class="transparent" width="25%">
</center>

- Pela lei da conservação da energia, sabemos que: $V_{s} = V_{R1} + V_{R2} + V_{R3}$

- Se $V_{S} = 5V$ e $i = 0.25 A$, logo, $5V - 0.25 R_{1} = 3.3V \rightarrow R_{1} = 6.8\Omega$, uma resistência de $6.8 \Omega$ em um circuito com uma corrente de 0.25A provocaria um decaimento de tensão de $1.7V$ suficiente para abaixar a tensão de $5V$ para $3.3V$ após $R_{1}$.

- Porém, nem sempre conhecemos os valores de corrente, as fontes de tensão não necessariamente mantém valores estáveis para corrente, desta forma, precisamos de outros artifícios matemáticos para calcularmos de maneira independente da corrente as tensões $V_{k}$ existentes em cada resistor $R_{k}$.

</div>


---

<div class="cabecalho large">
Divisão da Tensão
</div>
<div class="conteudo small">

<center>
    <img src="https://cdn.kastatic.org/ka-perseus-images/7c02d028f874842f69e5967b3972ab2e35ec21cf.svg" class="transparent" width="25%">
</center>

- A corrente $i$ é igual em todo o circuito.
- Pela lei de Ohm, $V_{S} = R_{eq} i$ que implica dizer que:

$$ 
\begin{align}
V_{S} &= R_{1} i + R_{2} i + R_{3} i \rightarrow V_{S} = i (R_{1} + R_{2} + R_{3}) \\
i &= {{V_{S}} \over {R_{1} + R_{2} + R_{3}}}
\end{align}
$$

- Sabemos que a tensão $V_{k}$ em qualquer $R_{k}$ é dada por $V_{k} = R_{K} \cdot i$.
- Substituindo $i$ nessa equação temos:
    - $V_{k} = {R_{k} \over {R_{1} + R_{2} + R_{3}}} \cdot V_{S}$

- Assim, alcançamos a forma geral do princípio da divisão de tensão que elucida que em um circuito com $N$ resistências em série, a tensão $k$ entre os terminais de um resistor $k$ qualquer é dada por:

$$V_{k} = {R_{k} \over {R_{1} + R_{2} + \cdots + R_{N}}} \cdot V_{S}$$

</div>


---

<div class="cabecalho large">
Divisão da Tensão
</div>
<div class="conteudo small">

Retomando nosso exemplo para mitigar a sobretensão de +5V oriundas de CIs TTL na interação com CIs CMOS.

- Queremos criar uma configuração resistiva que em um resistor, preferencialmente o primeiro resistor do circuito $R_{1}$, a tensão diminua 1.7V, passando de +5V para +3.3V.
    - Pois, $5V = 1.7V + 3.3V$

<center>
    <img src="https://cdn.kastatic.org/ka-perseus-images/6b6e0b28312a3590640cf20b54fe950854299558.png" class="transparent" width="30%">
</center>

- O princípio da divisão da tensão é nosso melhor amigo na tarefa.
    - Pois, independentemente da corrente, com apenas dois resistores, conseguimos fazer com que a tensão $V_{1}$ nos terminais do resistor $R_{1}$ seja de 1.7V, abaixando assim, a tensão de +5V para +3.3V.
    - Com apenas dois resistores é possível fazer com que $V_{1}$ seja $+1.7V$.
    - Considerando que $V_{1} = {R_{1} \over {R_{1} + R_{2}}} \cdot 5V = 1.7V$ então, ${R_{1} \over {R_{1} + R_{2}}} = {1.7 \over 5}$

</div>


---

<div class="cabecalho large">
Divisão da Tensão
</div>
<div class="conteudo small">

<center>
    <img src="https://cdn.kastatic.org/ka-perseus-images/6b6e0b28312a3590640cf20b54fe950854299558.png" class="transparent" width="30%">
</center>

- Queremos criar uma configuração resistiva em que um resistor, preferencialmente o primeiro resistor do circuito $R_{1}$, a tensão diminua 1.7V, passando de +5V para +3.3V.
    - Pois, $5V = 1.7V + 3.3V$

- Considerando que $V_{1} = {R_{1} \over {R_{1} + R_{2}}} \cdot 5V = 1.7V$ então, ${R_{1} \over {R_{1} + R_{2}}} = {1.7 \over 5}$
- Definindo $R_{1} = 10 k\Omega$, logo:

$$
\begin{align}
5 \times 10 k\Omega &= 1.7 \times (10 k\Omega + R_{2}) \rightarrow \\
R_{2} &= {33 \over 1.7} k\Omega \rightarrow \\
R_{2} &\simeq 19.4 k\Omega
\end{align}
$$

</div>


---

<!-- _class: lead -->
# Aplicação do Divisor de Tensão


---

<div class="conteudo">
    <center>
        <img class="transparent" src="./img/aplicacao_divisao_de_tensao.png" width=75%>
    </center>
</div>
