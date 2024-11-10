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

Passos para montagem:
Insira o LED na protoboard.
Conecte o terminal positivo (ânodo) do LED ao pino digital 13 do Arduino.
Conecte o terminal negativo (cátodo) do LED ao resistor.
O outro terminal do resistor deve ser conectado ao pino GND do Arduino.
3. Programação (20 minutos)
Explicar o código:

Vamos escrever um código simples que acende e apaga o LED no Arduino.

// Definir o pino digital 13 como saída
int ledPin = 13;

void setup() {
  // Inicializa o pino 13 como saída
  pinMode(ledPin, OUTPUT);
}

void loop() {
  // Acende o LED
  digitalWrite(ledPin, HIGH);
  delay(1000); // Espera 1 segundo

  // Apaga o LED
  digitalWrite(ledPin, LOW);
  delay(1000); // Espera 1 segundo
}

Explicação do código:

A função setup() é executada uma vez, configurando o pino 13 como saída com o comando pinMode().
A função loop() é executada repetidamente. Dentro dela, o comando digitalWrite(ledPin, HIGH) acende o LED e digitalWrite(ledPin, LOW) apaga o LED.
O delay(1000) faz uma pausa de 1 segundo (1000 milissegundos) entre as ações de acender e apagar o LED.
4. Teste e Verificação (10 minutos)
Subir o código para o Arduino:
Conectar o Arduino ao computador via cabo USB.
No Arduino IDE, selecionar a placa e a porta corretas.
Clicar em "Upload" para enviar o código para o Arduino.
Verificar o funcionamento:
O LED deve começar a piscar a cada 1 segundo.
Se o LED não acender, revisar as conexões e o código.
5. Conclusão e Discussão (10 minutos)
Revisar o conteúdo aprendido:
O que é um circuito simples com LED.
Como acender e apagar um LED usando programação no Arduino.
Possíveis variações:
Trocar o pino do LED.
Usar outros tipos de LEDs (como LEDs RGB).
Fazer o LED piscar de forma diferente (com intervalos variados).
6. Tarefas para casa (Opcional)
Modificar o código para fazer o LED piscar mais rápido (reduzir o valor de delay).
Criar um código onde o LED acende quando o botão é pressionado.
Avaliação:
Durante a aula, verificar se os alunos estão conseguindo montar o circuito e entender o código.
Perguntar sobre o funcionamento do código e pedir para modificar pequenas partes, como o tempo de delay.




