Projeto de Monitoramento de Cheias e Chuvas com Arduino
Este projeto utiliza um Arduino UNO para simular o monitoramento do nível de um rio e da quantidade de chuva acumulada. Ele utiliza sensores ultrassônicos, buzzer, LEDs e um display LCD para informar os dados em tempo real e emitir alertas em caso de risco de cheia ou excesso de chuva.

- Componentes Utilizados
Arduino UNO

2 sensores ultrassônicos (HC-SR04)

Display LCD 20x4 com I2C

Módulo RTC DS3231 (Relógio de tempo real)

LEDs (Verde, Amarelo e Vermelho)

Buzzer (alarme sonoro)

Breadboard e jumpers

- Funcionamento
Um sensor mede a altura do nível do rio.

O outro sensor simula um pluviômetro, medindo a altura da água acumulada em um recipiente.

O sistema compara os valores com limiares pré-definidos:

• Chuva intensa: acima de 20 mm

• Cheia do rio: acima de 250 cm

Com base nisso, o sistema ativa os LEDs e o buzzer:

🟢 Verde: tudo normal

🟡 Amarelo: chuva intensa

🔴 Vermelho: risco de cheia ou cheia em andamento

O display LCD exibe:

Altura atual do rio

Volume de chuva acumulado

Relógio em tempo real

O Serial Monitor imprime informações detalhadas, incluindo duração da chuva e das cheias com base no RTC.

- Exemplo de Saída no Display

Alt.Rio:  265.0 cm
Chuva:     24.8 mm
Hora:     14:32:05
Diagrama de Montagem

- Possíveis Expansões
Enviar os dados via Wi-Fi para a internet

Enviar dados via satelite para celulares e aparelhos móveis dos produtores rurais 

Armazenar registros em cartão SD

Incluir gráfico em display OLED ou dashboard online

- Aplicações Reais
Esse projeto simula situações reais de monitoramento ambiental e pode ser aplicado em:

Defesa Civil

Áreas de risco de enchente

Projetos escolares e educacionais de ciência e tecnologia
