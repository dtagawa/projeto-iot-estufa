# Monitoramento Inteligente com IoT - Estufa Inteligente

## Descrição do Projeto

Este projeto tem como objetivo realizar o monitoramento inteligente de uma estufa utilizando conceitos de Internet das Coisas (IoT).

A solução utiliza um ESP32 conectado a sensores físicos para coleta de dados ambientais, transmitindo as informações via protocolo MQTT para o Node-RED, onde os dados são processados, exibidos em dashboard em tempo real e armazenados em banco de dados MySQL.

Além disso, o sistema realiza integração com API externa de clima para exibição de informações adicionais no dashboard.

---

# Arquitetura da Solução

ESP32 → MQTT (HiveMQ) → Node-RED → Dashboard → MySQL

---

# Tecnologias Utilizadas

- ESP32
- MQTT
- HiveMQ Cloud
- Node-RED
- Node-RED Dashboard
- MySQL
- phpMyAdmin
- Wokwi Simulator
- API Weather (wttr.in)

---

# Sensores Utilizados

## DHT22
Responsável pela leitura de:

- Temperatura
- Umidade

## LDR
Responsável pela leitura de:

- Luminosidade

---

# Funcionalidades

- Leitura periódica dos sensores
- Comunicação MQTT em tempo real
- Dashboard interativo no Node-RED
- Armazenamento de dados no MySQL
- Gráficos em tempo real
- Integração com API externa de clima
- Monitoramento remoto da estufa

---

# Estrutura MQTT

Tópico utilizado:

```txt
estufa1/dados
