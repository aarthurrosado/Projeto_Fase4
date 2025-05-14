Sistema de Sensoriamento Agrícola com Controle de Irrigação – ESP32 + Wokwi

Descrição do Projeto

Este repositório apresenta um sistema de irrigação inteligente simulado na plataforma Wokwi, utilizando o microcontrolador ESP32. O sistema integra sensores de umidade, fósforo, potássio e pH, com controle automatizado de uma bomba de irrigação via relé, baseado nos valores lidos.

Componentes Utilizados

Componente

Função

ESP32 DevKit

Microcontrolador principal

Pushbutton (2x)

Simula sensores de Fósforo (P) e Potássio (K)

Sensor LDR

Simula medição de pH (analógico) pela luminosidade

Sensor DHT22

Mede a umidade do solo

Módulo Relé

Controla a bomba de irrigação (simulada por LED)

LED + Resistor (220Ω)

Indicador visual da ativação da bomba

Protoboard

Distribuição de alimentação (VCC e GND) para os componentes

Funcionalidades

Leitura digital de botões para detectar Fósforo e Potássio

Leitura analógica do pH via LDR

Leitura da umidade via DHT22

Acionamento automático do relé conforme condições definidas

Indicação com LED do status da irrigação

Totalmente funcional em simulação na Wokwi

Mapeamento de Pinos

Componente

Pino no ESP32

Botão Fósforo

GPIO 23

Botão Potássio

GPIO 4

LDR (AO)

GPIO 27

DHT22 (DATA)

GPIO 34

Relé (IN)

GPIO 12

LED (indicador)

Saída do relé (via terminal NO)

Plataforma

Simulação: Wokwi

Código: sketch.ino (Arduino/C++)

Lógica de Controle

A irrigação é ativada automaticamente se uma das seguintes condições for verdadeira:

Presença de fósforo ou potássio detectada via botões

Umidade abaixo do limiar configurado (via DHT22)

pH fora da faixa ideal (exemplo: < 5 ou > 8)
