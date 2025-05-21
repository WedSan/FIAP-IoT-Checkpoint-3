# Checkpoint 3 Projeto IoT ESP32: Monitoramento de Temperatura, Umidade, Pressão, Altitude com protocolo MQTT

## 🚀 Sobre o Projeto

Este projeto utiliza um ESP32 para monitorar e enviar, via MQTT, informações de temperatura, umidade, pressão e altitude. Os dados são enviados de forma periódica para um broker MQTT e podem ser visualizados em qualquer cliente compatível (no caso o Node-RED).

---

## 🛠️ Funcionalidades

- 📡 Conexão automática à rede Wi-Fi.
- 🔄 Conexão, reconexão e publicação de dados em um broker MQTT.
- 🌡️ Leitura de temperatura e umidade com sensor DHT22.
- 🌬️ Geração simulada de valores de pressão e altitude (aleatórios).
- 🔔 Envio dos dados somente quando houver alteração.
- 📝 Mensagens e logs enviados pela porta serial para debug.

---

## ⚙️ Componentes Utilizados

- ESP32 DevKit
- Sensor DHT22 (Temperatura e Umidade)
- LED e resistor
- Broker MQTT

---

## 📦 Como Funciona

1. O ESP32 conecta ao Wi-Fi e ao broker MQTT.
2. O sensor DHT22 faz a leitura da temperatura e umidade.
3. Os valores de pressão e altitude são gerados aleatoriamente (simulação).
4. Os dados são publicados via MQTT em um tópico específico.
5. Todas as ações são registradas no monitor serial para acompanhamento.

---

## 🖥️ Exemplo de Mensagem Publicada

```json
{
  "temperatura": 25.5,
  "umidade": 60.0,
  "status_led": "on",
  "pressao": 1012,
  "altitude": 123.45
}
```
