# 🌱 FarmTech Solutions – Sistema de Irrigação Inteligente (Fase 2)

## 📌 Descrição do Projeto

Este projeto tem como objetivo o desenvolvimento de um sistema de irrigação automatizado utilizando conceitos de IoT (Internet das Coisas), simulado na plataforma Wokwi com o microcontrolador ESP32.

A solução proposta monitora condições do solo e nutrientes essenciais, tomando decisões inteligentes para ativar ou desativar a irrigação, visando economia de água e aumento da produtividade agrícola.

---

## 🎯 Objetivos

* Monitorar a umidade do solo em tempo real
* Simular níveis de nutrientes (NPK)
* Simular o pH do solo
* Automatizar a irrigação com base em regras definidas
* Reduzir desperdício de água

---

## 🧪 Sensores e Componentes Utilizados

| Componente | Função no Projeto           |
| ---------- | --------------------------- |
| ESP32      | Microcontrolador principal  |
| DHT22      | Simula a umidade do solo    |
| LDR        | Simula o pH do solo         |
| Botão N    | Representa Nitrogênio       |
| Botão P    | Representa Fósforo          |
| Botão K    | Representa Potássio         |
| Relé       | Aciona a bomba de irrigação |

---

## ⚙️ Funcionamento do Sistema

O sistema realiza leituras contínuas dos sensores e aplica uma lógica de decisão para controlar a irrigação.

### 🌧️ Umidade do solo:

* Abaixo de 60% → Irrigação ligada
* Entre 60% e 80% → Irrigação desligada
* Acima de 80% → Irrigação desligada

### 🧪 pH do solo (via LDR):

* Convertido para escala de 0 a 14
* Ideal: entre 5.5 e 7.0
* Fora do ideal → Irrigação pode ser reduzida ou bloqueada

### 🌿 Nutrientes (NPK):

* Representados por botões (ligado/desligado)
* Se algum nutriente estiver ausente → Irrigação reduzida

---

## 🧠 Lógica de Decisão

A irrigação será ativada apenas quando todas as condições ideais forem atendidas:

* Umidade abaixo do nível mínimo
* N, P e K ativos
* pH dentro da faixa ideal

Caso contrário, o sistema mantém a irrigação desligada para evitar desperdício.

---

## 🔌 Estrutura do Projeto

```
farmtech-irrigacao-inteligente-fase2
│
├── codigo-esp32/
├── imagens-circuito/
├── python-api/ (opcional)
├── analise-r/ (opcional)
├── README.md
```

---

## 🖼️ Circuito

Imagens do circuito desenvolvido no Wokwi estão disponíveis na pasta:

📁 `/imagens-circuito`

---

## 💻 Código

O código desenvolvido para o ESP32 está disponível em:

📁 `/codigo-esp32`

---

## 🎥 Demonstração do Projeto

🔗 Link do vídeo no YouTube (não listado):

(INSIRA AQUI O LINK DO SEU VÍDEO)

---

## 🚀 Funcionalidades Extras (Opcional)

### 🌐 Integração com API

Possível integração com API meteorológica para prever chuvas e evitar irrigação desnecessária.

### 📊 Análise em R

Utilização de dados históricos para apoiar decisões de irrigação com base estatística.

---

## 👥 Integrantes do Grupo

* Nome 1
* Nome 2
* Nome 3
* Nome 4

---

## 📈 Conclusão

Este projeto demonstra como tecnologias de IoT podem ser aplicadas no agronegócio para otimizar recursos naturais, reduzir desperdícios e melhorar a eficiência produtiva.

A solução proposta contribui para o conceito de agricultura inteligente, alinhada com práticas sustentáveis e inovação tecnológica.

---
