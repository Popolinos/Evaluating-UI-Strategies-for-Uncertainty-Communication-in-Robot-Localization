# Evaluating UI Strategies for Uncertainty Communication in Robot Localization

> Estudo de IHC — Mestrado  
> Avaliação de estratégias de interface para comunicar incerteza em sistemas de localização robótica

---

## 📋 Sobre o Projeto

Este repositório contém os protótipos de interface utilizados em um experimento de **Interação Humano-Computador (IHC)** que investiga como diferentes estratégias visuais impactam a compreensão de incerteza em sistemas de localização de robôs móveis.

O robô opera em ambientes internos e utiliza um algoritmo de localização probabilística que gera **múltiplas hipóteses de mapa**. O objetivo do estudo é comparar três abordagens distintas de comunicar essa incerteza ao operador humano.

---

## 🗺️ Mapas do Ambiente

O experimento utiliza três layouts de mapa com complexidade crescente:

| Mapa | Descrição | Característica |
|------|-----------|----------------|
| **A** | Corredor em L | Simples, sem bifurcação |
| **B** | Corredor em T | Bifurcação central simétrica |
| **C** | Corredor em L com bifurcação lateral | Ambíguo, estrutura assimétrica |

---

## 🖥️ Interfaces

O experimento adota um design **between-subjects**: cada participante avalia **uma única interface** aplicada aos **5 cenários**.

### Interface A — Visão do Sensor + Probabilidades
Apresenta a leitura do sensor LiDAR do robô junto com a probabilidade associada a cada hipótese de mapa. Abordagem **quantitativa**.

### Interface B — Descrição do Ambiente
Apresenta uma descrição textual dos arredores percebidos pelo robô, com efeito de digitação simulando transmissão em tempo real. Abordagem **descritiva**.

### Interface C — Histórico de Movimento
Apresenta o estado atual de movimento do robô simulando um log de sistema. Abordagem **temporal**.

---

## 📍 Cenários

Cada interface é aplicada aos mesmos 5 cenários, com complexidade e ambiguidade crescentes:

| Cenário | Complexidade |
|---------|----------|
| **1** | Baixa |
| **2** | Médias |
| **3** | Média |
| **4** | Alta |
| **5** | Alta |

---

## 🧪 Design do Experimento

```
Participante → triagem automática → Formulário A, B ou C
                                          ↓
                                 5 cenários sequenciais
                                          ↓
                               5–6 perguntas por cenário
```

- **Tipo:** Between-subjects
- **Variável independente:** Tipo de interface (A, B ou C)
- **Variáveis dependentes:** Compreensão, confiança e tomada de decisão do operador

---

## 📁 Estrutura do Repositório

```
📦 Evaluating-UI-Strategies-for-Uncertainty-Communication-in-Robot-Localization/
├── 📄 README.md
├── 📄 triagem.html         # Página de entrada — distribui participantes automaticamente
├── 📄 interface_a.html     # Interface A — Sensor LiDAR + Probabilidades
├── 📄 interface_b.html     # Interface B — Descrição textual do ambiente
└── 📄 interface_c.html     # Interface C — Histórico de movimento
```

---

## 🔗 Links

| Página | Link |
|--------|------|
| Triagem | [triagem](https://popolinos.github.io/Evaluating-UI-Strategies-for-Uncertainty-Communication-in-Robot-Localization/triagem.html) |
| Interface A | [interface_a](https://popolinos.github.io/Evaluating-UI-Strategies-for-Uncertainty-Communication-in-Robot-Localization/interface_a.html) |
| Interface B | [interface_b](https://popolinos.github.io/Evaluating-UI-Strategies-for-Uncertainty-Communication-in-Robot-Localization/interface_b.html) |
| Interface C | [interface_c](https://popolinos.github.io/Evaluating-UI-Strategies-for-Uncertainty-Communication-in-Robot-Localization/interface_c.html) |

---

## 🛠️ Tecnologias

- HTML5 + CSS3 + JavaScript puro
- Layout responsivo com `clamp()` — funciona em desktop, tablet e mobile
- Imagens embarcadas em Base64 (sem dependências externas)
- Hospedado via **GitHub Pages**

---

## 📚 Referências

> *(A ser preenchido com as referências do artigo)*

---

<p align="center">
  Desenvolvido como parte de pesquisa de Mestrado em IHC<br>
  <sub>Interfaces geradas com apoio de prototipagem assistida por IA</sub>
</p>
