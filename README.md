# 🤖 Comunicação de Incerteza em Localização de Robôs Móveis

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

### Interface B — Descrição do Ambiente *(em breve)*
Apresenta uma descrição textual dos arredores percebidos pelo robô. Abordagem **descritiva**.

### Interface C — Histórico de Movimento *(em breve)*
Apresenta o histórico recente de movimentos do robô como contexto temporal. Abordagem **temporal**.

---

## 📍 Cenários

Cada interface é aplicada aos mesmos 5 cenários, com complexidade e ambiguidade crescentes:

| Cenário | Situação |
|---------|----------|
| **1** | Corredor simples antes de uma curva |
| **2** | Corredor com duas direções possíveis |
| **3** | Corredor após curva, sem bifurcação |
| **4** | Corredor após curva com bifurcação à frente |
| **5** | Conflito de hipótese — robô em posição ambígua |

---

## 🧪 Design do Experimento

```
Participante → sorteio → Formulário A, B ou C
                              ↓
                     5 cenários sequenciais
                              ↓
                   4–5 perguntas por cenário
```

- **Tipo:** Between-subjects
- **Variável independente:** Tipo de interface (A, B ou C)
- **Variáveis dependentes:** Compreensão, confiança e tomada de decisão do operador

---

## 📁 Estrutura do Repositório

```
📦 Evaluating-UI-Strategies-for-Uncertainty-Communication-in-Robot-Localization/
├── 📄 README.md
├── 📄 interface_a.html     # Interface A — Sensor + Probabilidades
├── 📄 interface_b.html     # Interface B — Descrição textual
└── 📄 interface_c.html     # Interface C — Histórico de movimento
```

---

## 🔗 Links dos Formulários

> *(Serão adicionados após publicação no GitHub Pages)*

| Interface | Link |
|-----------|------|
| Interface A | `—` |
| Interface B | `—` |
| Interface C | `—` |

---

## 🛠️ Tecnologias

- HTML5 + CSS3 + JavaScript puro
- Imagens embarcadas em Base64 (sem dependências externas)
- Layout responsivo (desktop e mobile)
- Hospedado via **GitHub Pages**

---

## 📚 Referências

> *(A ser preenchido com as referências do artigo)*

---

<p align="center">
  Desenvolvido como parte de pesquisa de Mestrado em IHC<br>
  <sub>Interfaces geradas com apoio de prototipagem assistida por IA</sub>
</p>
