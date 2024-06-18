# Fonte Ajustável

## Descrição

Este é o primeiro trabalho de Eletrônica Digital, que envolve o projeto de uma Fonte de Tensão ajustável entre 3V a 12V com capacidade de 100mA. É burro friendly, então seja bem-vindo 🤓.

## Componentes Utilizados

| Nº Componente | Componente      | Especificação                  | Link para explicação detalhada                             |
| ------------- | --------------- | ------------------------------ | ---------------------------------------------------------- |
| 1             | Fonte           | Corrente Alternada 2 Terminais | [Explicação da Fonte CA](#explicacao_fonte)                |
| 1             | Transformador   | Razão: 6.979                   | [Explicação do Transformador](#explicacao_trans)           |
| 4             | Diodo           | 1N4004/1N4001                  | [Explicação do Diodo](#explicacao_diodo)                   |
| 1             | Capacitor       | 680uF com ≈ 24.2V              | [Explicação do Capacitor](#explicacao_capacitor)           |
| 1             | Diodo Zener -12 | 12,7V/13V                      | [Explicação do Diodo Zener](#explicacao_diodo_zener)       |
| 1             | Potenciômetro   | 10k                            | [Explicação do Potenciômetro](#explicacao_potenciometro)   |
| 4             | Resistores      | De 8.2KΩ à 120Ω                | [Explicação dos Resistores](#explicacao_resistores)        |
| 1             | LED Vermelho    | 5mm                            | [Explicação do LED Vermelho](#explicacao_led)              |
| 1             | Transistor      | NPN - bc337 uso geral - até 0,8A| [Explicação do Transistor NPN](#explicacao_transistor_npn) |


## Explicações Básicas:
Algumas questões básicas que serão feitas pelo professor de Eletrônica para Computadores da USP, Eduardo Simões.
[Explicações aqui!](#explicacao_bas)

### Resistores

| Resistores Ω | Especificação |
| ------------ | ------------- |
| 8.2KΩ        | LED           |
| 2.7KΩ        | Diodo Zenner  |
| 5.3KΩ        | Potenciômetro |

## Explicação de algumas questões básicas: 

<a name="explicacao_bas"></a>

### 1ª - Se cada "quarto"/"cômodo", sendo 3 cômodos, tem sua própria fase, portanto é um sistema trifásico (modo de distribuição mais comum de energia elétrica), como podemos justificar a economia (redução do que seria gasto no total) de fios para este número de cômodos?
- Na úsina, usa-se o sistema trifásico, incorporando três ondas senoidais, defasadas entre si, de forma a tanto "estabilizar" o sistema quanto de torná-lo mais eficiente e (quando chega a casa) é possível de distribuir entre os dois níveis de tensão, já que é um sistema só. Chegando na casa, normalmente tem-se um fio só para a fase para a casa toda. Agora, por termos cada fase para cada cômodo, ou uma fase apenas para o cômodo específico, logo a resistência, para "segurar" as fases, se for apenas uma para toda a casa, o fio seria maior, ou vários fios menores para cada quarto com sua própria fase.

### 2ª - Explique a relação entre a "grossura" do fio com a resistência:
- De acordo com a 2ª lei de Ohm: R = (φ * C)/A, sendo a Área, justamente essa "grossura", assim, a Resistência é proporcionalmente inversa à Área.

### 3ª - Por que o Diodo não queima na Ponte de [Diodos](#explicacao_diodo)?           
- Por conta do RMS, Root Mean Square, que seria a raiz quadrada do quadrado dos valores dos sinais de voltagem ao quadrado num certo ponto, tendo valores instantâneos, logo, estamos falando de derivada ou integral. Aqui calculamos a raiz quadrada da integral derivando o Ox, como o tempo que o certo valor f(x), que seria a voltagem, teria. Logo, por ser a integral, não importa se dentro de uma raiz quadrada, é a média de f(x), voltagem, assim, temos os picos e vales, já que estamos falando de corrente alternada. E para o diodo este RMS é crucial para sabermos se, caso o pico seja muito alto o tempo de "esfriar" também o será, logo o que importa é o tempo que a voltagem ficará no pico, não sendo igual portanto o tempo que ficará esfriando, assim o queimando.


## Explicações do uso dos componentes:

<a name="explicacao_fonte"></a>

#### Fonte

<img src="img/battery9V.png" width="80px" alt="Itaipu2.0">

- A fonte aqui faz simulação de tomada, direto de Itaipu, que ao passar pelo transformador, como tem em alguns postes de luz (só que maior), "reduz" a tensão máxima antes de passar por ele, que é de 180V, para uma nova, mais aceitável e que usamos no resto do circuito.

<a name="explicacao_trans"></a>


#### Transformador

<img src="img/transformador.jpg" width="80px">

- O transformador aqui faria com que a corrente alternada advinda da fonte alternada, fazendo com que com a tensão máxima de 180V, "vinda da tomada", se "transforme" pela relação de espiras, na diferença de potencial que o nosso transformador na vida real tem, para o resto do circuito.

<a name="explicacao_diodo"></a>

#### Diodo 

<img src="img/diode.png" width="80px">

- O diodo é um dispositivo que aqui será usado em conjunto, atuando 4 de uma vez na mesma área, porém, afetando todo o circuito. Esse conjunto é chamado de ponte de diodo, quando, claro, colocado em um circuito daquela forma. No circuito em si, é configurado como uma ponte retificadora, que converte corrente alternada em corrente contínua.

<a name="explicacao_capacitor"></a>

#### Capacitor

<img src="img/capacitorPolarized.png" width="80px">

- O capacitor é utilizado para armazenar cargas elétricas e fornecer energia ao circuito quando necessário. No caso da fonte ajustável, ele ajuda a suavizar as flutuações de tensão e a estabilizar a saída.

<a name="explicacao_diodo_zener"></a>

#### Diodo Zener

<img src="img/diode.png" width="80px" alt="Diodo com Z em simulação">

- O diodo Zener é usado para regular a tensão no circuito. Ele permite que uma tensão específica seja mantida através dele, protegendo os componentes do circuito contra picos de tensão.

<a name="explicacao_potenciometro"></a>

#### Potenciômetro

<img src="img/potentiometer.png" width="80px">

- O potenciômetro é um resistor variável que permite ajustar a tensão de saída da fonte conforme necessário. Ele é essencial para garantir que a fonte seja ajustável entre 3V a 12V.

<a name="explicacao_resistores"></a>

#### Resistores

<img src="img/resistor.png" width="80px">

- O primeiro será para o LED, fazendo com que não passe uma potência tão grande;
  - O segundo será para o Diodo Zenner, já que para este, a tensão não deve ser tão alta, nem tão baixa também por causa da corrente mínima que o Zenner-12 requer;
    - O terceiro será para o final, fazendo com que, passado pelo Coletor do Transistor NPN, a tensão "original" com 100mA e 24V passe por este resistor de 120, chegando no final com 12V e 100mA;
      - E o quarto, e último, seria para limitarmos a queda de tensão no potenciômetro, indo de 12V para o mínimo de 3V, ao invés de 3mV.

<a name="explicacao_led"></a>

#### LED Vermelho

<img src="img/led.png" width="80px">

- Os LEDs vermelhos são usados para indicar visualmente o funcionamento do circuito. Eles acendem quando a fonte de alimentação está ligada e funcionando corretamente.

<a name="explicacao_transistor_npn"></a>

#### Transistor NPN

<img src="img/transistorNPN.png" width="80px">

- O transistor NPN aqui serve para a resolução do resistor do Zenner, já que queremos que ao final tenhamos 100mA e conservemos a voltagem "original", porém com 12V no final, sem ter o problema do Zenner-12 se alimentar um pouco desses 12V e não ter a tensão mínima requerida no final, enquanto mantém também esses 100mA. Ele está ali então para regular a corrente, como um duto desta.

### Imagem do Circuito no Falstad

<img src="photosEscreens/Falstadscreenshot.png">

### Imagens de Cálculos:

<img src="photosEscreens/calculo1.png">
<img src="photosEscreens/calculo2.png">

### Transformadores

<img src="img/transformadores.png">
