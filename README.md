# 🌞 IoT para Monitoramento de Energia Solar em Datacenters 🌐

## 📜 Descrição do Projeto
Este projeto simula um sistema IoT que monitora a geração e o armazenamento de energia solar para datacenters. A solução foi desenvolvida com foco em **eficiência energética e sustentabilidade**, enfrentando os desafios do crescimento exponencial das Inteligências Artificiais (IAs) e o consequente aumento do consumo energético.

O sistema utiliza sensores para medir variáveis ambientais, como temperatura e umidade, e calcula a energia gerada por painéis solares simulados. Ele também monitora o nível de uma bateria virtual enquanto publica todos os dados em um broker MQTT para acompanhamento em **tempo real**.

## 🚀 Tecnologias Utilizadas
- **Wokwi**: Simulador de IoT para desenvolvimento do protótipo.
- **ESP32**: Microcontrolador para leitura de sensores e integração MQTT.
- **MQTT**: Para enviar os dados monitorados em tempo real.
- **DHT22**: Sensor para medir temperatura e umidade.
- **LDR**: Sensor para simular a intensidade da luz solar.
- **LEDs**: Indicadores para o estado do sistema:
  - Carregamento da bateria
  - Bateria cheia
  - Alerta de alta temperatura

## ⚙️ Funcionalidades
- **Monitora**:
  - Temperatura e umidade do ambiente.
  - Intensidade da luz solar (via LDR), usada para calcular a energia gerada.
  - Nível da bateria virtual (de 0Ah a 500Ah).
- **Alertas de Temperatura**:
  - Acende um LED e envia alertas via MQTT quando a temperatura ultrapassa 25°C.
  - Reduz 0,5% da eficiência dos painéis solares para cada grau acima de 25°C.
- **Publica os dados em tempo real para um broker MQTT**:
  - Temperatura (°C), Umidade (%), Energia Gerada (W), Perda de Eficiência (%) e Nível da Bateria (Ah).

## 📊 Dashboard
Um Dashboard visual foi desenvolvido para exibir os dados monitorados, incluindo:

- **Temperatura (°C)**
- **Umidade (%)**
- **Energia gerada (W)**
- **Perda de eficiência (%)**
- **Nível da bateria (Ah)**

O nível da bateria é atualizado em tempo real, mostrando o carregamento de 0Ah até 500Ah com base na energia gerada.

## 🎥 Demonstração
- **Projeto no Wokwi**: [Clique aqui](#)
- **Vídeo no YouTube**: [Clique aqui](#)

## 🛠️ Como Testar o Projeto
Acesse o link do projeto no Wokwi: [Clique aqui](#).

Inicie a simulação no Wokwi e acompanhe os seguintes comportamentos:
- **LEDs** indicando os estados de carregamento, bateria cheia e alerta de temperatura.
- **Publicações MQTT em tempo real** com os dados monitorados.
- **Opcional**: Use um cliente MQTT como o MQTTX para assinar os tópicos e visualizar os dados.

## 🌟 Impacto e Benefícios
- **Sustentabilidade**: Reduz o consumo de energia não renovável.
- **Eficiência**: Monitora em tempo real as condições ambientais e o uso da energia solar.
- **Inovação**: Integração com IoT e MQTT para controle remoto e monitoramento contínuo.

## 🧩 Contribuições
- RM556275 - Daniel Vieira Novais
- RM559124 - Bento Rangel
- RM559067 - Werbeth Nunes
	
