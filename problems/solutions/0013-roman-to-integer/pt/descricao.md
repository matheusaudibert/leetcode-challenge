# 13. Romano para Inteiro (Fácil)

Os números romanos são representados por sete símbolos diferentes: `I`, `V`, `X`, `L`,  
`C`, `D` e `M`.

    Símbolo       Valor
    I             1
    V             5
    X             10
    L             50
    C             100
    D             500
    M             1000

Por exemplo, o número `2` é escrito como `II` em algarismos romanos, ou seja, dois uns somados.  
O número `12` é escrito como `XII`, que é simplesmente `X + II`. O número `27` é escrito como `XXVII`, que é `XX + V + II`.

Os números romanos geralmente são escritos do maior para o menor valor, da esquerda para a direita.  
No entanto, o número quatro não é escrito como `IIII`. Em vez disso, ele é escrito como `IV`.  
Como o `I` vem antes do `V`, subtraímos 1 de 5, resultando em 4.  
O mesmo princípio se aplica ao número nove, que é escrito como `IX`.

Há seis situações em que a subtração é usada:

- `I` pode ser colocado antes de `V` (5) e `X` (10) para formar 4 e 9.
- `X` pode ser colocado antes de `L` (50) e `C` (100) para formar 40 e 90.
- `C` pode ser colocado antes de `D` (500) e `M` (1000) para formar 400 e 900.

Dado um número romano, converta-o para um número inteiro.

## Exemplo 1:

    Entrada: s = "III"
    Saída: 3
    Explicação: III = 3.

## Exemplo 2:

    Entrada: s = "LVIII"
    Saída: 58
    Explicação: L = 50, V = 5, III = 3.

## Exemplo 3:

    Entrada: s = "MCMXCIV"
    Saída: 1994
    Explicação: M = 1000, CM = 900, XC = 90 e IV = 4.

## Restrições

- `1 <= s.length <= 15`
- `s` contém apenas os caracteres `('I', 'V', 'X', 'L', 'C', 'D', 'M')`.
- É **garantido** que `s` é um número romano válido no intervalo `[1, 3999]`.
