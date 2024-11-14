# Projeto de Monitoramento de Consumo de Energia com Arduino e MQTT

Este projeto simula um sistema de monitoramento e gestão de consumo de energia em um ambiente residencial. Usando o **Arduino Uno** no simulador **Wokwi**, o projeto monitora o consumo de diferentes circuitos, verifica a presença de luz natural e detecta movimento, com automação e alertas via **MQTT**.

## Funcionalidades

- **Monitoramento de Consumo de Energia**: Mede o consumo de energia de três circuitos (Iluminação, Eletrônicos e Eletrodomésticos) com potenciômetros simulando cada um.
- **Detecção de Luz Natural**: Usando um sensor de luz (LDR) para recomendar o desligamento das luzes quando há iluminação natural suficiente.
- **Detecção de Presença**: Um sensor de movimento (PIR) detecta presença, e o sistema desliga circuitos automaticamente em áreas desocupadas.
- **Alertas e Recomendações**: Envia alertas de consumo excessivo e recomendações de economia no **Node-RED**.
- **Controle Manual**: Um botão permite o controle manual de um circuito específico.

## Código do Arduino

O exemplo de código está em [codigo_arduino.ino](codigo_arduino.ino).

## Como Testar

1. **No Wokwi**:
   - Gire os potenciômetros para simular diferentes níveis de consumo.
   - Observe as mensagens de alerta e o comportamento dos LEDs no display.
   - Teste o sensor de luz e o PIR para simular as recomendações de economia.

2. **No Node-RED**:
   - Monitore os gráficos e gauges do consumo.
   - Verifique se os alertas e mensagens de recomendação aparecem corretamente.
