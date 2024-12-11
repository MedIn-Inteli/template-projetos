# Template de Documentação para Hardware

## 🔠 Visão Geral

Esta seção descreve os componentes de hardware utilizados no projeto e como eles interagem entre si. Inclui detalhes sobre conexões, esquemas elétricos e requisitos de alimentação.

---

## 📋 Especificações Técnicas

| Componente        | Modelo/Referência  | Quantidade | Especificações          | Observações                 |
|--------------------|--------------------|------------|-------------------------|-----------------------------|
| Microcontrolador  | Arduino Uno R3     | 1          | 5V, 16MHz              | Principal unidade de controle. |
| Sensor EMG        | MyoWare            | 2          | 0-5V analógico         | Utilizado para leitura de sinais musculares. |
| LED Strip         | WS2812B            | 1          | 84 LEDs, alimentação 5V | Indica visualmente a força capturada. |
| Resistores        | 330Ω               | 2          | Resistência de carga.  | Conectados aos pinos de dados do LED. |

---

## 🛠️ Diagrama de Circuito

Adicione o diagrama elétrico completo mostrando as conexões entre os componentes. Utilize ferramentas como **Fritzing** ou **KiCad** para criar esquemas visuais.

![Diagrama do Circuito](../assets/circuit_diagram.png)

---

## 🔐 Conexões de Hardware

| Componente  | Pino no Microcontrolador | Conexão Física        |
|-------------|--------------------------|-----------------------|
| Sensor EMG  | A0                       | Via cabo jumper       |
| LED Strip   | D5                       | Via conector 3 pinos  |
| GND Geral   | GND                      | Barramento comum      |
| VCC Geral   | 5V                       | Fonte regulada 5V     |

---

## ⚙️ Instruções de Montagem

1. Conecte os sensores EMG aos pinos analógicos A0 e A1 do microcontrolador.
2. Conecte a fita de LED ao pino digital D5, e alimente-a com 5V estável.
3. Garanta que todos os componentes compartilhem o mesmo GND.
4. Utilize um multímetro para verificar continuidade antes de alimentar o circuito.

---

## 🔋 Requisitos de Alimentação

- Fonte de alimentação: 5V/2A.
- Consumo típico: 1.2A (dependente da intensidade dos LEDs).

---

## 🔂 Logs e Resultados

Documente aqui os resultados obtidos durante testes de hardware, como medições de tensão, correntes e sinais capturados pelos sensores.
