A regra de ruffini é uma técnica para facilmente dividir [[Polinómios]] por binómios (polinómios de 2 [[monómios]])

Começa por fazer uma tabela e escreve o coeficiente de todos os graus da equação do maior grau ao menor grau.

Vamos usar $\frac{x^5+1}{x+3}$ como exemplo, é preciso escrever: 1 | 0 | 0 | 0 | 0 | 1
porque tem que ter todos os graus, mesmo os que não estão no polinómio, os que foram pulados tem coeficiente 0 e monómios só com a parte literal ou só com a parte numérica tem coeficiente 1 implicitamente.

|     | 1   | 0   | 0   | 0   | 0   | 1   |
| --- | --- | --- | --- | --- | --- | --- |
| ` ` |     |     |     |     |     |     |
| ` ` |     |     |     |     |     |     |

Depois pegamos o número do monómio do binómio que estamos a dividir e invertemos o sinal e colocamos na tabela:

|     | 1   | 0   | 0   | 0   | 0   | 1   |
| --- | --- | --- | --- | --- | --- | --- |
| -3  |     |     |     |     |     |     |
| ` ` |     |     |     |     |     |     |

Primeiro descemos o primeiro número:

|     | 1   | 0   | 0   | 0   | 0   | 1   |
| --- | --- | --- | --- | --- | --- | --- |
| -3  |     |     |     |     |     |     |
|     | 1   |     |     |     |     |     |

Depois multiplicamos pelo -3 e colocamos do lado:

|     | 1   | 0   | 0   | 0   | 0   | 1   |
| --- | --- | --- | --- | --- | --- | --- |
| -3  |     | -3  |     |     |     |     |
|     | 1   |     |     |     |     |     |

Somamos com o número de cima e colocamos o resulado em baixo:

|     | 1   | 0   | 0   | 0   | 0   | 1   |
| --- | --- | --- | --- | --- | --- | --- |
| -3  |     | -3  |     |     |     |     |
|     | 1   | -3  |     |     |     |     |

E repetir até chegar no final:

|     | 1   | 0   | 0   | 0   | 0   | 1        |
| --- | --- | --- | --- | --- | --- | -------- |
| -3  |     | -3  | 9   | -27 | 81  | -243     |
|     | 1   | -3  | 9   | -27 | 81  | **-242** |

O ultimo número é o **resto da divisão** e os outros números são os coeficientes para cada grau desde o grau mais alto até o mais baixo:

$1x^5-3x^4+9x^3-27x^2+81x^1-243x^0$
ou

$1x^5-3x^4+9x^3-27x^2+81x-243$
