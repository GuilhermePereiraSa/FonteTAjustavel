# Fonte Ajustável

## Descrição
Este é o primeiro trabalho de Eletrônica Digital, que envolve o projeto de uma Fonte de Tensão ajustável entre 3V a 12V com capacidade de 100mA.

## Componentes Utilizados

| Nº Componente | Componente          | Especificação        | Link para explicação detalhada                                    |
|---------------|---------------------|----------------------|-----------------------------------------------------------------|
| 5             | Diodo 1N4004/1N4001 | -                    | [Explicação do Diodo 1N4004/1N4001](link_para_explicação)    |
| 2             | Capacitor           | 470uF a 680uF         | [Explicação do Capacitor](link_para_explicação)                |
| 2             | Diodo Zener -12     | 12,7V/13V             | [Explicação do Diodo Zener](link_para_explicação)              |
| 1             | Potenciômetro       | 5k - 10k              | [Explicação do Potenciômetro](link_para_explicação)            |
| 4             | Resistores          | 4                    | [Explicação dos Resistores](link_para_explicação)              |
| 3             | LED Vermelho        | 5mm                  | [Explicação do LED Vermelho](link_para_explicação)             |
| 2             | Transistor NPN      | -                    | [Explicação do Transistor NPN](link_para_explicação)           |
| 1             | Fusível             | -                    | [Explicação do Fusível](#explicacao_fusivel)                   |
| 1             | Varistor            | -                    | [Explicação do Varistor](#explicacao_varistor)                 |

## Notas Adicionais

- **Transistor NPN**: Resolve o problema do Diodo Zener, ainda passando a tensão necessária para o Diodo iniciar e deixar a carga passar.

- **Ideia de Fusível e Varistor**: Oferece segurança contra correntes altas e proteção contra incêndios.

---

## Explicações do uso dos componentes:

<a name="explicacao_fusivel"></a>

### Fusível
- O fusível é um dispositivo de segurança projetado para proteger um circuito elétrico contra correntes excessivas. Quando a corrente elétrica no circuito excede um certo limite seguro o fusível se rompe, interrompendo assim, o fluxo de corrente.

<a name="explicacao_varistor"></a>

### Varistor
- O varistor é um dispositivo também de segurança com intuito principal de proteger "outros dispositivos" conectados ao circuito contra picos de tensão, pois ele possui uma resistência elétrica variável dependente da tensão aplicada. Quando ocorre, por exemplo, um aumento repentino na tensão, o varistor conduz a corrente elétrica excessiva para o solo.
