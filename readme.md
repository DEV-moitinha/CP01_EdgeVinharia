# 🍷 Vinheria Agnello - Sistema de Monitoramento de Luminosidade

## 📌 Descrição do Projeto

Este projeto foi desenvolvido para a Vinheria Agnello com o objetivo de monitorar a luminosidade do ambiente de armazenamento de vinhos utilizando Arduino Uno e sensor LDR (Light Dependent Resistor).

A luminosidade influencia diretamente na conservação da qualidade dos vinhos, portanto o sistema realiza leitura contínua do ambiente e sinaliza o estado por meio de LEDs e buzzer.

---

## 🎯 Objetivo

Capturar os níveis de luminosidade do ambiente e classificar em três estados:

- 🟢 LED Verde: ambiente adequado  
- 🟡 LED Amarelo: nível de alerta  
- 🔴 LED Vermelho: condição crítica + acionamento do buzzer  

---

## ⚙️ Componentes Utilizados

- Arduino Uno  
- Protoboard  
- Sensor LDR  
- 3 LEDs (verde, amarelo e vermelho)  
- 4 resistores  
- 1 buzzer  
- Jumpers  

---

## 🔌 Ligações do Circuito

### Arduino → Componentes

- LED Verde → pino digital 5  
- LED Amarelo → pino digital 2  
- LED Vermelho → pino digital 3  
- Buzzer → pino digital 4  
- LDR → A0  

### Alimentação

- 5V → trilha positiva da protoboard  
- GND → trilha negativa da protoboard  

---

## 📈 Faixas de Luminosidade Definidas

- 0 a 100 → Verde (ambiente ideal)  
- 101 a 400 → Amarelo (alerta)  
- 401 a 679+ → Vermelho (problema crítico)  

---

## 🚨 Funcionamento

### Verde
- LED verde pisca 3 vezes  
- Sem buzzer  

### Amarelo
- LED amarelo pisca 3 vezes  
- Sem buzzer  

### Vermelho
- LED vermelho pisca 3 vezes  
- Buzzer toca junto durante o alerta  

---

## 💻 Código Implementado

O código realiza:

- leitura analógica do LDR com analogRead(A0)
- comparação por limites definidos
- acionamento visual e sonoro conforme estado

---

## ▶️ Como Reproduzir no Tinkercad

1. Abrir Arduino Uno no Tinkercad  
2. Montar o circuito com os componentes informados  
3. Inserir o código no editor  
4. Iniciar simulação  
5. Alterar luminosidade do LDR para observar os estados  

---

## 📦 Dependências

Nenhuma biblioteca externa foi necessária.

Utilizado apenas:

- Arduino IDE padrão / Tinkercad  

---

## 🎥 Vídeo de Apresentação:
https://youtu.be/5iWHtU4yrp4

No vídeo deve ser apresentado:

- funcionamento do circuito  
- explicação dos componentes  
- lógica do código  
- dificuldades encontradas  
- solução aplicada  

Tempo máximo: 3 minutos

---

## 📚 Contexto Acadêmico

Projeto desenvolvido para disciplina de Edge Computing aplicado ao desafio proposto para a Vinheria Agnello.

Integrante:

Gustavo Romero - 571271
Gustavo Moita - 569180
Bruno Carreiro - 569423
Daniel Graciano - 568886