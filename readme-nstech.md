# 🚂 Performance nos Trilhos — Dashboard Operacional NST 2.0

> **GBM Tech & Control by NSTECH** · Porto de Santos · Jan–Jun 2026

![Badge](https://img.shields.io/badge/Versão-NST%202.0-FF4500?style=for-the-badge)
![Badge](https://img.shields.io/badge/Período-Jan–Jun%202026-374151?style=for-the-badge)
![Badge](https://img.shields.io/badge/Terminais-4-FF4500?style=for-the-badge)
![Badge](https://img.shields.io/badge/GitHub%20Pages-Online-16A34A?style=for-the-badge&logo=github)

---

## 📊 Sobre o Projeto

Dashboard operacional interativo desenvolvido para análise consolidada das operações ferroviárias e portuárias dos terminais de granéis do Porto de Santos. Cobre os terminais **TGRÃO**, **TEC**, **COPERSUCAR** e **CLI**, com dados de **Janeiro a Junho de 2026**.

Construído inteiramente em **HTML5 + CSS3 + JavaScript puro**, sem dependência de servidor ou banco de dados — basta abrir o arquivo `index.html` no navegador.

---

## ✨ Funcionalidades

### 📈 Análises Disponíveis
| Seção | Descrição |
|-------|-----------|
| **Dashboard Consolidado** | Visão geral com KPIs, vagões, toneladas e paradas |
| **Volume Operacional** | Vagões por terminal e mês com evolução temporal |
| **Vol. Movimentado (t)** | ⭐ Novo — Toneladas por terminal, moega e mês |
| **Taxa Vagão/Hora** | Produtividade operacional por terminal |
| **Tendência** | Série temporal Jan–Jun com vagões e toneladas |
| **Impacto Paradas** | Ferrovia × Terminal × Operação em % |
| **Janeiro × Junho** | Comparativo de crescimento entre períodos |
| **Por Terminal** | Análise individual: TGRÃO, TEC, COP, CLI |
| **Análise por Moegas** | Ranking de produtividade das 13 moegas |
| **Produtos & Operadores** | Açúcar · Soja · Milho · RUMO · MRS · VLI |
| **Planejado × Realizado** | Meta vs execução por terminal e mês |
| **Riscos & Ações** | Matriz de riscos e plano de ação |

### 🎛 Filtros Funcionais
- **Terminal** — TGRÃO, TEC, COPERSUCAR, CLI ou Todos
- **Mês** — Janeiro a Junho (01-27) ou período completo
- Filtros **combinados** — ex: CLI + Maio
- Botão **Limpar** restaura visão consolidada

### 📺 Ticker Breaking News
- Dados do mês atual rolando em tempo real
- Taxa Vgs/Hr, vagões, toneladas e ferrovia % por terminal
- Pausa ao passar o mouse

### 🔊 Voz (Web Speech API)
- Passe o mouse sobre qualquer gráfico ou KPI
- O navegador **lê os dados em português** automaticamente
- Análises detalhadas com números reais para cada seção
- Funciona sem internet adicional (voz nativa do navegador)
- Compatível com **Chrome** e **Edge** (recomendado)

### 📤 Exportação
- **Excel (.xlsx)** — 3 abas: Volume, Toneladas, Moegas
- **PDF** — via impressão do navegador (Ctrl+P)

---

## 🏭 Terminais Cobertos

| Terminal | Moegas | Produto | Operador |
|----------|--------|---------|----------|
| **TGRÃO** | Moegão-Terra | Soja / Milho | RUMO |
| **TEC** | L12A · Moegão 1 · 2 · 3 | Açúcar / Soja | RUMO · MRS |
| **COPERSUCAR** | Moegão · Linha 5 · Linha 6 | Açúcar | MRS · RUMO |
| **CLI** | CL-Mar · CL-Terra · Moegão-Mar · Moegão-Terra · T23 | Açúcar · Soja · Milho | RUMO · MRS · VLI |

---

## 📦 Dados Consolidados (Jan–Jun 2026)

| Terminal | Vagões | Toneladas (t) | Taxa Máx (Vgs/Hr) |
|----------|--------|--------------|-------------------|
| TGRÃO | 11.014 | 985.039 | 5,60 (Mai) |
| TEC | 21.981 | 1.268.036 | 18,03 (Mai) ⭐ |
| COPERSUCAR | 19.202 | 1.638.603 | 10,14 (Abr) |
| CLI | 36.342 | 2.853.263 | 16,97 (Fev) |
| **TOTAL** | **88.539** | **6.744.941** | — |

---

## 🛠 Tecnologias Utilizadas

```
HTML5          → Estrutura e semântica
CSS3           → Design System NST 2.0 (fundo branco + laranja #FF4500)
JavaScript ES6 → Lógica, filtros, voz e exportação
Chart.js 4.4.1 → Gráficos interativos (CDN Cloudflare)
XLSX.js 0.18.5 → Exportação Excel (CDN Cloudflare)
Web Speech API → Leitura de dados em voz alta (nativo do navegador)
GitHub Pages   → Hospedagem gratuita com HTTPS
```

---

## 🚀 Como Usar

### Opção 1 — Direto no Navegador
```bash
# Baixe o arquivo index.html e abra no Chrome ou Edge
# Não precisa de instalação ou servidor
```

### Opção 2 — GitHub Pages (este repositório)
Acesse: **https://SEU-USUARIO.github.io/nstech-dashboard/**

### Opção 3 — Clonar o repositório
```bash
git clone https://github.com/SEU-USUARIO/nstech-dashboard.git
cd nstech-dashboard
# Abra o index.html no navegador
```

---

## 📁 Estrutura do Projeto

```
nstech-dashboard/
│
├── index.html        ← Dashboard completo (arquivo único)
└── README.md         ← Esta documentação
```

> O dashboard é **100% self-contained** — todos os estilos, scripts e dados
> estão embutidos no `index.html`. Não há dependências locais.

---

## 🔊 Sobre a Funcionalidade de Voz

O dashboard utiliza a **Web Speech API** nativa dos navegadores modernos para leitura dos dados em português brasileiro.

**Como ativar:**
1. Passe o mouse sobre qualquer gráfico, KPI ou card
2. A voz inicia automaticamente lendo a análise do elemento
3. Use o botão **⏹ Parar** no canto inferior esquerdo para interromper

**Navegadores suportados:**
| Navegador | Suporte | Qualidade da Voz |
|-----------|---------|-----------------|
| Google Chrome | ✅ Total | ⭐⭐⭐⭐⭐ |
| Microsoft Edge | ✅ Total | ⭐⭐⭐⭐⭐ |
| Firefox | ⚠️ Parcial | ⭐⭐⭐ |
| Safari | ✅ Total | ⭐⭐⭐⭐ |

> ⚠️ A Web Speech API requer **HTTPS** — o GitHub Pages fornece isso automaticamente.

---

## 👥 Equipe

| Papel | Nome |
|-------|------|
| Analista de Dados | Luiz C. Oliveira |
| Analista de Dados | Gabriela Vasconcelos |
| Coordenador Operacional | Marcel de Souza Silva |
| Gerente Operacional | Diego Brazão |

---

## 🤖 Desenvolvimento

Este dashboard foi desenvolvido com auxílio de **Inteligência Artificial Claude (Anthropic)** via [claude.ai](https://claude.ai), com desenvolvimento iterativo e refinamento contínuo baseado nos dados operacionais reais da NSTECH.

---

## 📄 Licença

© 2026 **GBM Tech & Control by NSTECH** · Todos os direitos reservados.  
Uso interno — Porto de Santos · Operações Ferroviárias e Portuárias.

---

<div align="center">
  <strong>🚂 Performance nos Trilhos · NST 2.0 · Porto de Santos · 2026</strong><br>
  <sub>Criado com auxílio de Claude IA (Anthropic) · GBM Tech & Control by NSTECH</sub>
</div>
