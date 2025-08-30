# 📊 Campanha Omnichannel — Estágio em Dados

[![Made with Python](https://img.shields.io/badge/Made%20with-Python-3776AB.svg)](https://www.python.org/)
[![Jupyter Notebook](https://img.shields.io/badge/Notebook-Jupyter-F37626.svg)](https://jupyter.org/)
[![Status](https://img.shields.io/badge/status-completo-34D058.svg)](#)
[![License](https://img.shields.io/badge/license-MIT-black.svg)](#-licença)

Análises e protótipos para identificar **oportunidades de crescimento** em telecom a partir de dados públicos (ex.: Anatel) e benchmarks de mercado, com foco no estado de **Sergipe (BR)**. O trabalho se organiza em três frentes de insight: **(1)** potencial de **5G FWA**, **(2)** **combos fixo+móvel** e **(3)** estratégia **mobile-first** para aquisição e retenção.

---

## 🔎 Sumário

- [Destaques](#-destaques)
- [Estrutura do Repositório](#-estrutura-do-repositório)
- [Materiais](#-materiais)
- [Metodologia](#-metodologia)
- [Principais Resultados](#-principais-resultados)
- [Como Reproduzir](#️-como-reproduzir)
- [Dependências](#-dependências)
- [Como Navegar](#-como-navegar)
- [Próximos Passos](#-próximos-passos)
- [Licença](#-licença)
- [Autor](#-autor)

---

## ✨ Destaques

- **5G FWA em Sergipe:** priorização de municípios com **alta cobertura 4G** e **baixa presença de fibra**, maximizando viabilidade técnica e retorno sobre CAPEX.
- **Combos Fixo + Móvel:** tendências de **migração para pós-pago** e integração de ofertas elevando **ARPU** e reduzindo **churn**.
- **Aquisição Mobile-First:** cobertura 4G robusta viabiliza táticas de **WhatsApp, SMS e push**, acelerando ativações com CAC mais eficiente.

---

## 🗂 Estrutura do Repositório

├── README.md
└── Case_–_Análise_de_Campanha_Omnichannel.ipynb
└── Campanha Omnichannel Luis Felipe - estágio em dados.pdf
---

## 📁 Materiais

- **Notebook principal:** `notebooks/Case_–_Análise_de_Campanha_Omnichannel.ipynb`  
- **Relatório executivo (PDF):** `reports/Campanha Omnichannel Luis Felipe - estágio em dados.pdf`

---

## 🧪 Metodologia

1. **Coleta & Limpeza:** consolidação de indicadores de **cobertura 4G**, **presença de fibra/backhaul** e **perfil econômico** por município.
2. **Regras de Seleção (FWA):** filtros por **cobertura 4G elevada**, **baixa penetração de fibra** e **viabilidade econômica**.
3. **Visualização:**  
   - **Barras** (cobertura 4G vs. fibra) por município;  
   - **Séries temporais** (evolução pré x pós-pago);  
   - **Mapas/heatmaps** (intensidade de cobertura 4G).
4. **Leitura de Negócio:** priorização de praças com melhor **viabilidade técnica + econômica** e desenho de **ofertas** e **canais**.

---

## 📌 Principais Resultados

- **Praças indicadas para FWA:** municípios com combinação de **cobertura móvel alta** e **fibra limitada**, sugerindo implantação ágil e boa atratividade comercial.  
- **Tendências Comerciais:** **pós-pago em crescimento** e **queda do pré-pago** indicam espaço para **combos** e **upgrades**.  
- **Aquisição Digital:** **campanhas mobile-first** (WhatsApp/SMS/push) com segmentações por cobertura e propensão elevam eficiência e reduzem CAC.

> Os detalhes e evidências (gráficos e tabelas) estão no **notebook** e no **relatório em PDF**.

---

## ▶️️ Como Reproduzir

### Pré-requisitos
- **Python 3.10+**
- (Opcional) **conda** ou **venv** para isolar o ambiente
- **Jupyter Lab** ou **Jupyter Notebook**

### Instalação
```bash
git clone https://github.com/<seu-usuario>/<seu-repo>.git
cd <seu-repo>

# Ambiente virtual (venv)
python -m venv .venv
# Windows:
# .venv\Scripts\activate
# macOS/Linux:
source .venv/bin/activate

# Dependências
pip install -r requirements.txt

jupyter lab
# ou:
jupyter notebook
# Abra: notebooks/Case_–_Análise_de_Campanha_Omnichannel.ipynb


🧭 Como Navegar

FWA: células que filtram por cobertura 4G e fibra + gráficos comparativos por município.

Combos fixo+móvel: análise de pré vs. pós-pago e impactos em ARPU/churn.

Mobile-first: mapas/heatmaps de cobertura 4G e recomendações de canais e segmentação.

📄 Licença

Este projeto está licenciado sob a MIT License. Consulte o arquivo LICENSE para mais detalhes.

🙋‍♂️ Autor

Luis Felipe Ramalho Carvalho
luisfeliperamalhoc@gmail.com



