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
