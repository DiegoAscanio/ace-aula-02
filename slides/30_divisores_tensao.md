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
