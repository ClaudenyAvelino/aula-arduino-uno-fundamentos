# aula-arduino-uno-fundamentos
A aula tem como objetivo ensinar iniciantes a controlar um LED com Arduino. Os alunos aprenderão a montar um circuito simples e escrever um código básico em C++ para acender e apagar o LED. A atividade introduz conceitos de eletrônica, programação e interação com hardware, preparando para projetos mais avançados.

# Plano de Aula: Acender um LED com Arduino

## Objetivo:
Ensinar os alunos a configurar e controlar um LED usando a plataforma Arduino.

## Público-alvo:
Iniciantes em eletrônica e programação com Arduino.

## Duração:
1 hora

## Materiais Necessários:
- 1 Placa Arduino (Arduino Uno ou similar)
- 1 LED
- 1 Resistor de 220Ω
- Fios de conexão (jumpers)
- Protoboard
- Computador com o Arduino IDE instalado
- Cabo USB para conectar o Arduino ao computador

## Pré-requisitos:
Nenhum. Ideal para quem está começando com o Arduino.

## Estrutura da Aula:

### 1. Introdução (10 minutos)
- **O que é o Arduino?**
  - Explicar o que é o Arduino e como ele pode ser utilizado em projetos eletrônicos e de automação.
  - Breve introdução sobre programação em C/C++ no ambiente Arduino IDE.
  
### 2. Montagem do Circuito (20 minutos)
- **Explicar o esquema do circuito:**
  - Conectar o LED e o resistor à protoboard.
  - Explicar a pinagem do Arduino:
    - O pino positivo do LED (ânodo) vai ao pino digital 13 do Arduino.
    - O pino negativo do LED (cátodo) vai ao GND (terra) do Arduino, passando pelo resistor de 220Ω.
  
  **Diagrama do Circuito:**

  ```plaintext
        Arduino
      +-----------+
      |           |
      |           |
      |  Pin 13   |----->|---|<--- Resistor 220Ω ----> GND
      |           |
      +-----------+       |
                         LED

