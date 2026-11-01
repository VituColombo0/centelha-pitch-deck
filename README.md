# Centelha — Localização Indoor via Wi-Fi Fingerprinting

Pitch deck interativo desenvolvido para apresentação executiva de projeto de inovação tecnológica submetido ao Programa Centelha, com foco em sistemas de posicionamento indoor de alta precisão baseados em redes neurais e infraestrutura Wi-Fi pré-existente.

[![Technology: Reveal.js](https://img.shields.io/badge/Framework-Reveal.js%204.3-crimson.svg)](https://revealjs.com/)
[![CSS: TailwindCSS](https://img.shields.io/badge/Styling-Tailwind%20CSS-38B2AC.svg)](https://tailwindcss.com/)
[![Reactivity: Alpine.js](https://img.shields.io/badge/Reactivity-Alpine.js-77C1D2.svg)](https://alpinejs.dev/)
[![Charts: Chart.js](https://img.shields.io/badge/Data%20Viz-Chart.js-FF6384.svg)](https://www.chartjs.org/)

---

## Contexto do Projeto

Em ambientes fechados — como hospitais, centros logísticos, plantas industriais e edifícios corporativos —, o sinal de GPS sofre severa atenuação por estruturas de concreto e distorções causadas por propagação multicaminho (*multipath effect*).

As abordagens tradicionais de localização interna exigem a instalação de balizas proprietárias (como Beacons Bluetooth Low Energy ou UWB), acarretando custos expressivos de aquisição inicial (*Capex*) e manutenção contínua com substituição de baterias (*Opex*).

Esta proposta aborda o problema por meio de **Wi-Fi Fingerprinting assistido por Inteligência Artificial**:
1. **Fase Offline (Mapeamento do Ambiente):** Amostragem das assinaturas de intensidade de sinal recebido (RSSI) dos pontos de acesso Wi-Fi já existentes no edifício.
2. **Fase Online (Inferência com Redes Neurais):** O dispositivo móvel capta os níveis de sinal circundantes e a rede neural realiza a triangulação não-linear em tempo real, determinando as coordenadas espaciais com precisão submétrica.

---

## Funcionalidades da Apresentação

- **Navegação Não-Linear:** Alternância entre slides sequenciais e aprofundamento sob demanda em tópicos específicos.
- **Painéis Interativos de Problema:** Hotspots clicáveis com modais de detalhamento técnico sobre atenuação eletromagnética, reflexão e viabilidade financeira.
- **Gráficos Dinâmicos:** Visualização comparativa de acurácia, latência e custos operacionais renderizados via Chart.js.
- **Interface com Design System Escuro:** Tipografia baseada em Outfit e Inter, elementos em *glassmorphism* e paleta de alto contraste para projeção em auditórios e reuniões executivas.

---

## Estrutura do Repositório

```text
centelha-pitch-deck/
├── index.html        # Estrutura completa da apresentação, lógica reativa e estilos
└── README.md         # Documentação técnica do projeto
```

---

## Como Executar Localmente

Como a aplicação é construída com arquitetura client-side pura (HTML5, JS e CSS via CDNs), não há dependências de build ou compiladores.

### Opção 1: Servidor Python local

```bash
# Clone o repositório
git clone https://github.com/VituColombo0/centelha-pitch-deck.git
cd centelha-pitch-deck

# Inicie um servidor HTTP local
python3 -m http.server 8000
```
Acesse `http://localhost:8000` em qualquer navegador moderno.

### Opção 2: Extensão Live Server (VS Code)

Basta abrir o diretório no VS Code e clicar em **"Go Live"** no arquivo `index.html`.

---

## Atalhos de Apresentação

| Tecla / Ação | Função |
| :--- | :--- |
| **Seta Direita / Espaço** | Avançar para o próximo slide |
| **Seta Esquerda** | Retornar ao slide anterior |
| **ESC** | Visão geral da grade de slides (Overview) |
| **F** | Modo Tela Cheia (Fullscreen) |
| **Clique nos Hotspots** | Abrir modais explicativos de arquitetura |

---

## Licença

Documento de apresentação desenvolvido no âmbito da proposta para o Programa Centelha. Todos os direitos reservados aos autores do projeto.
