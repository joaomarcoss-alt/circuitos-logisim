# Circuitos-logisim

## 4-bit-Adder:

## Entradas:
- A[3:0] - Vetor de 4 bits representando o primeiro operando da soma.  
  (A0 é o bit menos significativo e A3 o mais significativo).  
- B[3:0] - Vetor de 4 bits representando o segundo operando da soma.  
  (B0 é o bit menos significativo e B3 o mais significativo).  
- Cin - Carry In (vai-um de entrada). Usado quando o somador faz parte de um sistema maior de somadores.

### Saídas: 
- S[3:0] - Vetor de 4 bits representando o resultado da soma entre A e B, considerando o Carry In.  
- Cout - Carry Out (vai-um de saída). Indica se houve um resultado maior que 4 bits.

### Explicação:

O 4-bit Adder é um circuito combinacional composto por 4 somadores completos Full Adders conectados em série.  
Cada Full Adder realiza a soma de três bits: um bit de A, um bit de B e o Carry proveniente do somador anterior.

Funcionamento:

O primeiro Full Adder soma A0, B0 e Cin.  
Ele gera o bit S0 e o carry C1 , que é passado para o próximo estágio.  
O processo se repete para os demais bits propagando o Carry.  
O último somador gera S3 e o carry out Cout.


## Half subtractor:

# Entradas
- A: Minuendo
- B: Subtraendo de A

# Saidas
- Diff: Valor que vai resultar na subtração de A e de B
- Borrow: Valor que sera emprestado caso a cada de unidades do B seja maior que a do A