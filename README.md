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
$$V_{2} = 25,4-2.0,7 = 24$$

### Capacitor
O capacitor atua como filtro, eliminando (ou minimizando) o ruído, chamado de ripple.
Considerando um ripple de 10%, temos:
$$R_{eq} = {V_{2} \over I} = {24 \over I} = 216\Omega$$
Onde a corrente I foi obtida usando o simulador Falstad.</br>
A capacitância será dada pela seguinte equação:
$$C = {V_{2} \over ripple.f.R_{eq}.2} = {24 \over 2,4.120.216.2} = 192μF$$

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

## Circuito no Falstad
![Falstad](https://github.com/renan823/fonte-ajustavel/blob/main/falstad.png)
Circuito experimental feito no Falstad. Utilizado para os cálculos e prototipação.</br>

## Placa no Eagle
![Esquema](https://github.com/renan823/fonte-ajustavel/blob/main/esquematico.jpeg)
Esquemático feito no Eagle.
</br></br>
![Placa](https://github.com/renan823/fonte-ajustavel/blob/main/placa.png)
Modelo gerado pelo Eagle após criação dos caminhos/rotas de conexão.
</br></br>

## Vídeo explicativo
[<img src="https://github.com/renan823/fonte-ajustavel/blob/main/thumbnail.png" width="100%">](https://youtu.be/DJt-_cFbtyc "Fonte de tensão ajustável")


