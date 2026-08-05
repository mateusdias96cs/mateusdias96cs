<div align="center">

```
╔══════════════════════════════════════════════════════════╗
║           MATEUS CAMARA DIAS // mateusdias96cs           ║
║      Security Engineering & AI Applied to Cybersecurity  ║
╚══════════════════════════════════════════════════════════╝
```

</div>

<div align="center">

[![TryHackMe](https://img.shields.io/badge/TryHackMe-mateus96cs-212C42?style=for-the-badge&logo=tryhackme&logoColor=red)](https://tryhackme.com/p/mateus96cs)
[![GitHub](https://img.shields.io/badge/GitHub-mateusdias96cs-0d1117?style=for-the-badge&logo=github&logoColor=white)](https://github.com/mateusdias96cs)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Mateus_Dias-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/mateusdiascs/)

</div>

---

## `> whoami`

```bash
$ cat perfil.txt

Nome      : Mateus Camara Dias
Curso     : Tecnologia em Cibersegurança — SENAC (2° Semestre)
Programa  : Hackers do Bem — SENAI (Fundamental ✅ | Blue Team Especializado ✅)
Foco      : Threat Intelligence Automation | Detection Engineering | Agentes de IA aplicados à segurança
Status    : [ CONSTRUINDO ] Automação de segurança e IA aplicada a triagem, detecção e resposta a incidentes
País/Estado: Brasil - Santa Catarina 🇧🇷
```

> *"Security is not a product, but a process."* — Bruce Schneier

---

## `> ./interesses.sh`

```
┌─────────────────────────────────────────────────┐
│  🤖  Agentes de IA aplicados à segurança         │
│  🔵  Threat Intelligence & Detection Engineering │
│  🛡️  Automação de resposta a incidentes          │
│  📊  Correlação de dados e arquitetura de pipeline│
│  🟢  Redes & Protocolos                          │
└─────────────────────────────────────────────────┘
```

---

## `> ls skills/`

**Linguagens & ferramentas em uso:**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![DuckDB](https://img.shields.io/badge/DuckDB-FFF000?style=for-the-badge&logo=duckdb&logoColor=black)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnu-bash&logoColor=white)
![Wireshark](https://img.shields.io/badge/Wireshark-1679A7?style=for-the-badge&logo=wireshark&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

**IA & Agentes:**

![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white)
![Gemini](https://img.shields.io/badge/Gemini_API-8E75B2?style=for-the-badge&logo=googlegemini&logoColor=white)
![Groq](https://img.shields.io/badge/Groq-F55036?style=for-the-badge&logo=groq&logoColor=white)
![Pydantic](https://img.shields.io/badge/Pydantic-E92063?style=for-the-badge&logo=pydantic&logoColor=white)
![ChromaDB](https://img.shields.io/badge/ChromaDB-4B0082?style=for-the-badge)

**Dados:**

![dbt](https://img.shields.io/badge/dbt-FF694B?style=for-the-badge&logo=dbt&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white)

---

## `> ls repos/`

### 🎯 Projetos em destaque

| Repositório | Descrição | Stack |
|---|---|---|
| 🔗 [attack-chain-verdict](https://github.com/mateusdias96cs/attack-chain-verdict) | **Pipeline de 4 agentes** que transforma telemetria bruta do Windows (Sysmon, Security, PowerShell) em veredito de segurança estruturado, com técnica MITRE ATT&CK atribuída, confiança e justificativa. Trava de grounding: o veredito nunca cita técnica que a busca não recuperou. Avaliado contra golden set rotulado manualmente — 93% recall na recuperação, 87% acurácia estrita na atribuição final, 0 violações de grounding em 15 casos. Construído sobre o dataset de avaliação APT29 do MITRE (783 mil eventos reais). | Python · LangGraph · Groq · Gemini · DuckDB · ChromaDB · Pydantic |
| 🛡️ [aegis-threat-intelligence](https://github.com/mateusdias96cs/aegis-threat-intelligence) | **AEGIS CTI Platform** — plataforma open source de Cyber Threat Intelligence com pipeline automatizado de coleta, normalização e scoring auditável de IOCs (~29.000 ativos em produção). Correlation graph com detecção de comunidades, MITRE ATT&CK Explorer, camada de analytics própria (dbt, bronze/silver/gold) com busca semântica via embeddings. | Python · FastAPI · PostgreSQL · dbt · pgvector |
| 🎣 [aegis-antiphishing-pipeline](https://github.com/mateusdias96cs/aegis-antiphishing-pipeline) | Detecção de domínios de phishing em tempo real via Certificate Transparency Logs, com arquitetura de dupla costimulação (heurística + confirmação factual via VirusTotal/RDAP) e análise por IA antes de qualquer alerta. Detectou domínios reais em produção, alertas automáticos via Telegram. | Python · n8n · Docker · Gemini API |

### 🧠 Fundamentos de agentes de IA

| Repositório | Descrição | Stack |
|---|---|---|
| 🔍 [cve-triage-agent](https://github.com/mateusdias96cs/cve-triage-agent) | Agente de triagem de CVEs implementado em três camadas progressivas (loop ReAct manual → saída estruturada Pydantic → framework smolagents), para entender o que cada abstração esconde antes de depender dela. | Python · Gemini · Pydantic · smolagents |
| 🔢 [nutriquery](https://github.com/mateusdias96cs/nutriquery) | Agente Text-to-SQL em LangGraph sobre base nutricional (star schema em DuckDB via dbt), com harness de avaliação em três níveis (exact match → subconjunto numérico → overlap de nomes). | Python · LangGraph · DuckDB · dbt |

### 🔵 Detecção & infraestrutura de segurança

| Repositório | Descrição | Stack |
|---|---|---|
| 📐 [Sigma](https://github.com/mateusdias96cs/Sigma) *(sentinel-as-code)* | Detection-as-Code para Blue Team: regras Sigma versionadas com teste TP/FP automatizado offline, cobertura MITRE ATT&CK medida como percentual, pipeline CI/CD completo até deploy no Elastic. | Python · Sigma · Elastic · GitHub Actions |
| 🍯 [honeypot-ssh](https://github.com/mateusdias96cs/honeypot-ssh) *(APATE)* | Honeypot SSH que simula servidor Linux real. Detecta brute force, escalada de privilégios, reconhecimento e movimento lateral, com relatório automático de sessão. | Python · Paramiko · bcrypt |
| 🛡️ [cybersentry](https://github.com/mateusdias96cs/cybersentry) | Scanner de vulnerabilidades web para PMEs — detecta falhas em headers, cookies, CORS, SSL, DNS, SQLi e XSS via API REST. | Python · FastAPI · SQLite |
| ⚙️ [aegis-lakehouse](https://github.com/mateusdias96cs/aegis-lakehouse) | Camada de analytics medalhão (bronze/silver/gold) para o AEGIS, rodando diariamente via GitHub Actions, com orçamento de armazenamento monitorado automaticamente antes de cada execução. | dbt · PostgreSQL · GitHub Actions |
| 📰 [security-news-aggregator](https://github.com/mateusdias96cs/security-news-aggregator) | Agregador de notícias de cibersegurança com 10+ fontes, deploy público com atualização diária via GitHub Actions. | Python · GitHub Actions |

### 🧬 Engenharia de sistemas

| Repositório | Descrição | Stack |
|---|---|---|
| ⚖️ [Homeostatic-Load-controller](https://github.com/mateusdias96cs/Homeostatic-Load-controller) | Controlador de admissão inspirado em fisiologia humana (barorreceptor, AIMD, disjuntor com período refratário), prevenindo falhas metaestáveis sob tempestade de retentativas. Comparação A/B mensurável contra versão ingênua. | Go · Docker · Prometheus · Grafana |

> 🔨 *Portfólio em construção ativa — novos projetos sendo adicionados regularmente.*

---

## `> cat certificados.txt`

### 🏆 TryHackMe

| Path | Status |
|------|--------|
| 🛡️ Pre Security | ✅ Concluído |
| 🔐 Cyber Security 101 | ✅ Concluído |
| 🤖 AI Security | ✅ Concluído |

### 📜 Cisco Networking Academy

Certificados concluídos: Introdução à Cibersegurança, Conceitos Básicos de Rede, Fundamentos do Python 1, Fundamentos do Hardware do Computador, Introdução à IoT e à Transformação Digital, Começando com o Cisco Packet Tracer.

> 🏆 Selecionado entre mais de 70.000 alunos para a 12ª Edição do Programa CiberEducação Cisco Brasil.

### 🇧🇷 Hackers do Bem — SENAI (Programa Federal)

| Nível | Status |
|---|---|
| 🟢 Fundamental | ✅ Concluído (12/12 módulos + avaliação final) |
| 🟢 Especializado — Blue Team | ✅ Concluído |

### 🎓 Programas

- **Santander Bootcamp 2026 — 1° Semestre** (Santander + DIO): aprovado e selecionado
- **triggo.ai AI Engineering Bootcamp**: selecionado entre ~1.000 candidatos via exame técnico

---

## `> top -stats github`

[![trophy](https://github-profile-trophy.vercel.app/?username=mateusdias96cs&theme=dark&no-frame=true&row=1&column=6)](https://github.com/mateusdias96cs)

<div align="center">

[![GitHub Stats](https://github-readme-stats.vercel.app/api?username=mateusdias96cs&show_icons=true&theme=dark&hide_border=true&bg_color=0d1117&title_color=00ff41&icon_color=00ff41&text_color=ffffff)](https://github.com/mateusdias96cs)

[![GitHub Streak](https://streak-stats.demolab.com?user=mateusdias96cs&theme=dark&hide_border=true&background=0d1117&ring=00ff41&fire=00ff41&currStreakLabel=00ff41)](https://github.com/mateusdias96cs)

</div>

---

<div align="center">

```
╔══════════════════════════════════════════════╗
║   Aberto para networking, dicas e conexões   ║
║         Vamos crescer juntos na área!        ║
╚══════════════════════════════════════════════╝
```

![Visitor Count](https://komarev.com/ghpvc/?username=mateusdias96cs&color=00ff41&style=flat-square&label=VISITAS)

</div>
