# Fonte Ajustável

## Descrição
Este é o primeiro trabalho de Eletrônica Digital, que envolve o projeto de uma Fonte de Tensão ajustável entre 3V a 12V com capacidade de 100mA.

## Componentes Utilizados

| Nº Componente | Componente          | Especificação        | Link para explicação detalhada                                    |
|---------------|---------------------|----------------------|-----------------------------------------------------------------|
| 5             | Diodo 1N4004/1N4001 | -                    | [Explicação do Diodo](#explicacao_diodo)                        |
| 2             | Capacitor           | 470uF a 680uF         | [Explicação do Capacitor](#explicacao_capacitor)                |
| 2             | Diodo Zener -12     | 12,7V/13V             | [Explicação do Diodo Zener](#explicacao_diodo_zener)            |
| 1             | Potenciômetro       | 5k - 10k              | [Explicação do Potenciômetro](#explicacao_potenciometro)        |
| 4             | Resistores          | 4                    | [Explicação dos Resistores](#explicacao_resistores)              |
| 3             | LED Vermelho        | 5mm                  | [Explicação do LED Vermelho](#explicacao_led)                   |
| 2             | Transistor NPN      | -                    | [Explicação do Transistor NPN](#explicacao_transistor_npn)      |
| 1             | Fusível             | -                    | [Explicação do Fusível](#explicacao_fusivel)                    |
| 1             | Varistor            | -                    | [Explicação do Varistor](#explicacao_varistor)                  |

## Notas Adicionais

- **Transistor NPN**: Resolve o problema do Diodo Zener, ainda passando a tensão necessária para o Diodo iniciar e deixar a carga passar.

- **Ideia de Fusível e Varistor**: Oferece segurança contra correntes altas e proteção contra incêndios.

---

## Explicações do uso dos componentes:

##### Diodo

<a name="explicacao_diodo"></a>

- O diodo é um dispositivo que aqui será usado em conjunto, atuando 4 de uma vez na mesma área, porém, afetando todo o circuito. Esse conjunto é chamado de ponte de diodo, quando, claro, colocado em um circuito daquela forma. No circuito em si, é configurado como uma ponte retificadora, que converte corrente alternada em corrente contínua.

### Capacitor

<a name="explicacao_capacitor"></a>

- O capacitor é utilizado para armazenar cargas elétricas e fornecer energia ao circuito quando necessário. No caso da fonte ajustável, ele ajuda a suavizar as flutuações de tensão e a estabilizar a saída.

### Diodo Zener

<a name="explicacao_diodo_zener"></a>

- O diodo Zener é usado para regular a tensão no circuito. Ele permite que uma tensão específica seja mantida através dele, protegendo os componentes do circuito contra picos de tensão.

### Potenciômetro

<a name="explicacao_potenciometro"></a>

- O potenciômetro é um resistor variável que permite ajustar a tensão de saída da fonte conforme necessário. Ele é essencial para garantir que a fonte seja ajustável entre 3V a 12V.

### Resistores

<a name="explicacao_resistores"></a>

- Os resistores são usados para limitar a corrente e dividir a tensão em diferentes partes do circuito, garantindo o funcionamento correto dos componentes.

### LED Vermelho

<a name="explicacao_led"></a>

- Os LEDs vermelhos são usados para indicar visualmente o funcionamento do circuito. Eles acendem quando a fonte de alimentação está ligada e funcionando corretamente.

### Fusível

<a name="explicacao_fusivel"></a>

- O fusível é um dispositivo de segurança projetado para proteger o circuito elétrico contra correntes excessivas. Quando a corrente elétrica no circuito excede um certo limite seguro, o fusível se rompe, interrompendo assim o fluxo de corrente.

### Varistor

<a name="explicacao_varistor"></a>

- O varistor é um dispositivo de segurança projetado para proteger outros componentes do circuito contra picos de tensão. Ele possui uma resistência elétrica variável que diminui quando a tensão aplicada aumenta, permitindo que ele desvie a corrente excessiva para o solo e proteja o circuito contra danos causados por sobretensão.
