Controle de Servo e LED RGB com Raspberry Pi Pico 🎮
Este projeto demonstra o controle de um servo motor e um LED RGB usando a Raspberry Pi Pico com PWM (Pulse Width Modulation). 
O código foi escrito em C e utiliza as bibliotecas pico/stdlib.h e hardware/pwm.h para controlar a movimentação do servo e a intensidade das cores do LED RGB.

🛒 Materiais Necessários
Raspberry Pi Pico 🖥️
Servo Motor 🤖
LED RGB (com 4 pinos ou 3 pinos de controle) 💡
Fonte de alimentação ⚡ (se necessário)
Fios de conexão 🔌
📏 Diagrama de Conexão
Servo Motor
Pino de controle do servo: GPIO 22 da Raspberry Pi Pico.
GND do servo: Conectar ao GND da Raspberry Pi Pico.
VCC do servo: Conectar à fonte de alimentação adequada.
LED RGB
Pino vermelho do LED: GPIO 12.
Pino verde do LED: GPIO 13.
Pino azul do LED: GPIO 14.
GND do LED: Conectar ao GND da Raspberry Pi Pico.
🎯 Objetivo
O código tem como objetivo:

Controlar o Servo Motor 🚗
Utiliza PWM para mover o servo entre as posições de 0°, 90° e 180°, além de realizar movimentos suaves entre esses valores.
Controlar o LED RGB 💡
Controla a cor do LED RGB, alternando entre as cores vermelho, verde, azul, amarelo, ciano e magenta.
⚙️ Instruções de Uso
1. Instalar a Raspberry Pi Pico
Conecte a Raspberry Pi Pico ao seu computador via USB.
Compile e carregue o código utilizando o ambiente de desenvolvimento adequado (ex: Visual Studio Code com o plugin para Raspberry Pi Pico ou o SDK do Raspberry Pi).
2. Compilação e Execução
Abra o terminal no diretório onde o código foi salvo.
Compile o código com o comando:
bash
Copiar
Editar
make
Carregue o arquivo compilado para a Raspberry Pi Pico.
3. Funcionamento
O servo motor começará a se mover para as posições de 0°, 90° e 180°.
O LED RGB começará a alternar entre as cores configuradas:
Vermelho 🔴
Verde 🟢
Azul 🔵
Amarelo 🟡
Ciano 🟣
Magenta 🟤
📝 Estrutura do Código
Funções Importantes
set_pwm_duty_cycle(uint slice, uint channel, uint16_t duty): Aplica o valor do duty cycle ao pino de controle do servo motor.
set_rgb_color(uint red, uint green, uint blue): Define a intensidade de cada cor (vermelho, verde e azul) do LED RGB.
Configuração PWM
Servo Motor: O PWM é configurado com uma frequência de 50Hz, o que é comum para servos.
LED RGB: O PWM é configurado com um wrap de 255, permitindo o controle da intensidade das cores.
🚀 Possíveis Melhorias
Controle de Velocidade do Servo: A movimentação do servo motor pode ser suavizada ainda mais, ajustando o tempo de transição entre as posições.
Controle de Cor Dinâmico: Implementar a possibilidade de controlar a cor do LED RGB dinamicamente (ex: com um potenciômetro ou sensor).
🎥 Vídeo Demonstrativo
Assista ao vídeo mostrando o funcionamento completo do projeto:
Vídeo Demonstrativo
https://drive.google.com/file/d/1HasKR0caR8ipp4cIm4ivL5UrO_1jCQD3/view?usp=drive_link
Autor e Contato
Brunna Barreto da Silva
20241bsifsa0027@ifba.edu.br
