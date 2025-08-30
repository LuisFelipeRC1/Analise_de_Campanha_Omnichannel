# 📊📱 Omnichannel Case + 🎮 Jogo de Palavras (Java)

Elegante e direto ao ponto: este repositório reúne **dois entregáveis** do meu portfólio — um **case analítico de marketing omnichannel** (Data/BI) e um **mini‑projeto em Java** (POO). O objetivo é mostrar pensamento analítico, clareza de comunicação e código organizado.

---

## 🧭 Sumário
- [Visão Geral](#-visão-geral)
- [Estrutura do Repositório](#-estrutura-do-repositório)
- [1) Case — Análise de Campanha Omnichannel](#-1-case--análise-de-campanha-omnichannel)
  - [Principais Insights](#principais-insights)
  - [Como Reproduzir](#como-reproduzir)
  - [Fontes & Referências](#fontes--referências)
- [2) Jogo de Palavras (Java)](#-2-jogo-de-palavras-java)
  - [Arquitetura & Classes](#arquitetura--classes)
  - [Como Executar](#como-executar)
  - [Possíveis Extensões](#possíveis-extensões)
- [Roadmap](#-roadmap)
- [Licença](#-licença)

---

## 🌟 Visão Geral

- **Case de Dados**: Explora oportunidades para uma **campanha omnichannel** com foco em **Sergipe**, utilizando dados públicos (ANATEL e estudos de mercado). Entregue em **notebook** (`.ipynb`) e **relatório PDF**.
- **Projeto Java**: Um **jogo de palavras** simples com foco em **POO**: separação de responsabilidades, mecânica do jogo e embaralhamento de palavras.

---

## 📁 Estrutura do Repositório

```
├── BancoDePalavras.class
├── Campanha Omnichannel Luis Felipe - estágio em dados.pdf
├── Case_–_Análise_de_Campanha_Omnichannel.ipynb
├── Embaralhador.class
├── EmbaralhadorAleatorio.class
├── MecanicaDoJogo.class
├── MecanicaSimples.class
├── Principal.class
```

> _Obs.: os arquivos `.class` são binários compilados do projeto Java; o notebook (`.ipynb`) contém o passo a passo analítico; o PDF consolida os achados em formato executivo._

---

## 1) Case — Análise de Campanha Omnichannel

**Objetivo**: Identificar **onde** e **como** uma operadora regional pode crescer com **5G FWA**, **combos fixo+móvel** e uma abordagem **mobile‑first** em Sergipe.

### Principais Insights
- **5G FWA em Sergipe**: Municípios com **alta cobertura 4G** e **baixa presença de fibra** sugerem **alto potencial** para FWA, com **payback** mais curto e **CAPEX** menor por domicílio.
- **Combos fixo+móvel**: Tendência de **crescimento do pós‑pago** e **queda do pré‑pago** indica espaço para **planos combinados**, aumento de **ARPU** e redução de **churn**.
- **Mobile‑First Marketing**: Cobertura 4G elevada + penetração de celular em domicílios → maior eficiência em **WhatsApp/SMS/push/redes sociais**.
- **Visualizações**: 
  - **Barras**: Municípios candidatos (cobertura 4G vs. fibra).
  - **Linhas**: Evolução da densidade móvel e da base pré vs. pós‑paga.
  - **Mapa de Calor**: Cobertura 4G por município em Sergipe.

### Como Reproduzir
1. **Abrir o notebook**: `Case_–_Análise_de_Campanha_Omnichannel.ipynb`.
2. Criar um ambiente (ex.: `conda` ou `venv`) e instalar dependências usuais para análise geográfica e de dados (ex.: `pandas`, `matplotlib`, `geopandas`/`shapely` quando aplicável).
3. Executar as células na ordem. As figuras e tabelas geradas correspondem ao PDF:  
   `Campanha Omnichannel Luis Felipe - estágio em dados.pdf`.

### Fontes & Referências
- **ANATEL** – Painéis “Meu Município” e “Telefonia Móvel” (indicadores de cobertura 4G e séries históricas).
- **J.D. Power (2024)** – Satisfação de clientes de internet residencial (comparativos FWA vs. cabo).
- **OpenSignal / GSMA / Ericsson Mobility / RCR Wireless** – Tendências de FWA e casos internacionais (T‑Mobile, Verizon, Xplore).

> _As referências completas e observações metodológicas constam no PDF._

---

## 2) Jogo de Palavras (Java)

Um jogo de console focado em **POO**. Pelo nome das classes, o design privilegia **baixo acoplamento** e **alta coesão**:

### Arquitetura & Classes
- `Principal.class` — ponto de entrada da aplicação (método `main`).
- `MecanicaDoJogo.class` / `MecanicaSimples.class` — regras e fluxo da partida (pontuação, tentativas, condições de vitória/derrota).
- `Embaralhador.class` / `EmbaralhadorAleatorio.class` — estratégia de **embaralhamento** das palavras (Strategy).
- `BancoDePalavras.class` — provê o **dicionário**/lista de termos do jogo.

> _O uso de interfaces/concretas (ex.: `Embaralhador` ↔ `EmbaralhadorAleatorio`) sugere um padrão **Strategy**, facilitando trocar a forma de embaralhar sem alterar a mecânica._

### Como Executar
> Pré‑requisitos: **Java 11+** instalado (JDK).

Se os `.class` estão no **pacote padrão** (sem `package` declarado) e foram compilados juntos:
```bash
# Na pasta onde estão os .class
java Principal
```

Caso exista **nome de pacote**, rode com o **classpath** adequado, por exemplo:
```bash
# Exemplo (ajuste para o seu package)
java -cp . br.com.seuprojeto.Principal
```

Para **recompilar** (se tiver os `.java`), use:
```bash
javac -Xlint:all -d out src/**/*.java
java -cp out Principal
```

### Possíveis Extensões
- Novos embaralhadores (ex.: reverso, vogais/consoantes, embaralhamento por níveis).
- Persistência de **ranking** (arquivo/SQLite).
- Internacionalização (PT‑BR/EN).
- Testes unitários (JUnit) e CI (GitHub Actions).

---

## 🗺️ Roadmap
- [ ] Publicar `environment.yml`/`requirements.txt` do notebook.
- [ ] Adicionar **screenshots** das visualizações (barras/linhas/heatmap).
- [ ] Documentar exemplos de entrada/saída do jogo Java e empacotar em **JAR** executável.
- [ ] Incluir testes automatizados e **badge** de CI.

---

## 📄 Licença
Distribuído sob **MIT License**. Sinta‑se à vontade para usar, adaptar e referenciar — atribuição é sempre bem‑vinda. 😉

---

> 💬 **Contato**: Abra uma _issue_ ou conecte‑se comigo no LinkedIn.