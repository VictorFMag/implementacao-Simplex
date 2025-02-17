# Formato da entrada
Um arquivo .txt com o seguinte padrão:<br><br>

- A primeira linha é um valor numérico que identifica se é um problema de minimização (-1) ou maximização (1)<br>
- A segunda linha é um valor numérico (x) que identifica quantas são as variáveis do problema.<br>
- A terceira linha é um valor numérico (y) que identifica quantas são as restrições do problema.<br>
- A quarta linha contém x valores numéricos que identificam os coeficientes das variáveis na função objetivo.<br>
- A demais linhas a partir da quarta contém x+1 valores numéricos que identificam os coeficientes das variáveis nas restrições do problema seguido do valor limitante de cada restrição (lado direito da equação).<br><br>
Exemplo:<br>
1<br>
2<br>
3<br>
3   5<br>
2   1    30<br>
3   -1   20<br>
1   4    15<br><br>
Essa entrada de dados representa o seguinte modelo:<br><br>
max 3x1 + 5x2<br>
s.a.:<br>
        2x1 + x2 <= 30<br>
        3x1 - x2 <= 20<br>
        x1 + 4x2 <= 15<br>
        x1, x2 >= 0
