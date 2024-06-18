# Fonte Ajustável
Alunos: Caio Petroncini, Caroline Akimi e Renan Trofino. 
Este projeto foi construído durante as aulas de eletrônica, e tem como objetivo ser uma **fonte regulável entre 3V e 12V com 100mA.**

## Processos

### Transformador
O transformador é responsável por reduzir a voltagem recebida, tornando-a útil neste dispositivo. Um transformador obedece a seguinte equação:
$$V_{e}.N_{s}=V_{s}.N_{e}$$
A entrada da tomada é de 127V, e a saída do transformador é de aproximadamente 25V.
Então, a razão entre as espiras é:
$${N_{1} \over N_{2}}={V_{max} \over V_{1}}={126,8 \over 25,4}=5$$

### Ponte de diodos
A ponte de diodos é composta por 4 diodos retificadores.
Sua função é tornar a senóide em outra onda, retificando-a.
A corrente alternada é então convertida em corrente contínua.
Para funcionar, os diodos precisam de uma tensão mínima, que, neste modelo,
é de 0.7V cada. Então, a tensão de entrada se torna:
$$25,4-2.0,7 = 24V$$

## Componentes usados
Os jumpers (fios) e transformadores foram reaproveitados de outros projetos.
| Qnt. usada | Componente | Valor |
|--------------|------------|-------|
| 04 | Diodo Retificador 1N 4007 (10 unid.) | 2,80 |
| 01 | Capacitor 470μF 63V | 3,46 |
| 01 | Diodo Zener 13V 1/2W (10 unid.) | 7,20 |
| 01 | Resistor 4K7 (50 unid.) | 4,00 |
| 01 | Resistor 680 (50 unid.) | 4,00 |
| 01 | Transistor NPN (5 unid.) | 3,10 |   
| 01 | Potenciômetro linear 10K | 4,50 |
|**Total:** | | **29,00** |




