<div class="cabecalho large">
Exemplo - Divisão de Correntes
</div>
<div class="two-columns-50-50" style="top: 20%;">
<div class="regular" >

Começamos a resolver o exemplo a partir do exercício 2 e desenhamos inicialmente o diagrama do circuito para viabilizar nossa resolução:

<center>
    <img src='img/circuito-exemplo-divisao-correntes.png' class='transparent' >
</center>

Sabemos que todos os equipamentos trabalham na tensão de $110V$ e por estarem em paralelo, possuem esta mesma tensão em suas entradas.

</div>
<div class="regular" style="margin-left: 5%;">

Agora, sabemos a corrente do monitor $i_{3} = 1.5A$, devemos calcular as correntes do computador e do som.

Começando pelo som, pela lei de Ohm, temos que $I = {V \over R}$. Considerando que a tensão é de $110V$ e a resistência do aparelho de som é de $220 \Omega$, logo, $i_{2} = {110 \over 220} = 0.5 A$. Conseguimos também calcular sua potência $P = 110 \times 0.5 = 55W$.

Avançando para o computador, sabemos da potência elétrica que $P = VI$. Considerando que $V = 110V$ e $P = 440W$, logo, $i_{1} = {440 \over 110} = 4A$.

Sabemos pela LKC que $I = i_{1} + i_{2} + i_{3}$. Então, $I = 4 + 0.5 + 1.5 = 6A$.

Considerando que mais um monitor em paralelo acrescentaria uma carga de $+1.5A$, que a carga total com este monitor seria de $7.5 < 10A$, logo, é possível adicionar mais um monitor a esta configuração.

</div>
</div>
