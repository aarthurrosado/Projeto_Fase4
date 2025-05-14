#FIAP - Faculdade de Informática e Administração Paulista



Enterprise Challenge - Sprint 1 - Reply

Nome do Grupo

Arthur Luiz Rosado Alves -> RM562061

Sumário

1. Justificativa do Problema

2. Descrição da Solução Proposta

3. Tecnologias Propostas

4. Pipeline de Dados

5. Plano Inicial de Desenvolvimento

6. Diagrama do Circuito

1. Justificativa do Problema

As atividades agrícolas dependem de condições ambientais ideais e controle eficiente de recursos. O excesso ou a deficiência de nutrientes, umidade e pH do solo podem prejudicar drasticamente a produtividade. Nesse contexto, propomos um sistema automatizado de sensoriamento e irrigação que otimize o uso da água e monitore a presença de nutrientes essenciais, como fósforo e potássio.

2. Descrição da Solução Proposta

Desenvolvemos uma solução baseada no microcontrolador ESP32, integrada à plataforma de simulação Wokwi. O sistema realiza a leitura de sensores que simulam as variáveis de umidade do solo (DHT22), pH (LDR) e presença de fósforo e potássio (push buttons). A bomba de irrigação é acionada automaticamente por um relé, e um LED indica visualmente o status da irrigação.

Funcionalidades

Leitura em tempo real dos sensores

Acionamento da bomba de irrigação

Indicação luminosa do estado da irrigação

Simulação completa e testável via ambiente Wokwi

3. Tecnologias Propostas/Planejadas

Camada

Tecnologias

Microcontrolador

ESP32 DevKit

Simulação de Sensores

Wokwi.com

Código e Lógica

Arduino C++ (sketch.ino)

Indicação visual

LED com resistor

Controle de atuadores

Módulo relé

4. Pipeline de Dados

Leitura dos Sensores:

Botões digitais para fósforo e potássio

Sensor DHT22 para umidade

Sensor LDR para simular o pH do solo

Processamento local no ESP32:

As leituras são convertidas em decisões lógicas

Ação automatizada:

Se qualquer sensor indicar necessidade, o relé é acionado

LED acende indicando bomba ativa

Simulação na Wokwi:

Permite testes visuais e ajustes lógicos em tempo real

5. Plano Inicial de Desenvolvimento

Etapa

Atividade

1

Montagem do circuito no Wokwi

2

Definição dos sensores simulados

3

Implementação da lógica no código

4

Testes com diferentes condições

5

Ajustes e documentação

6. Diagrama do Circuito



Autor

Arthur Luiz Rosado AlvesRM562061Curso: Inteligência Artificial – FIAPProjeto: Enterprise Challenge – Sprint 1

