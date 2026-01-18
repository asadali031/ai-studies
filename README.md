# AI Studies - Roadmap Completo de Estudos em IA

Repositório de estudos de Inteligência Artificial aplicada, focado em construir sistemas RAG (Retrieval-Augmented Generation) profissionais do zero.

---

## Table of Contents

- [Objetivo](#objetivo)
- [FASE 1 (0-2 meses) - Base Sólida de IA Aplicada](#fase-1-0-2-meses---base-sólida-de-ia-aplicada)
  - [001 - Python, APIs LLM e Prompt Engineering](#001---python-apis-llm-e-prompt-engineering)
  - [002 - Embeddings e Vector Databases](#002---embeddings-e-vector-databases)
  - [003 - RAG Chatbot Completo](#003---rag-chatbot-completo)
- [FASE 2 (3-5 meses) - RAG Profissional & Automações](#fase-2-3-5-meses---rag-profissional--automações)
  - [004 - RAG Avançado](#004---rag-avançado)
  - [005 - RAG em Produção](#005---rag-em-produção)
  - [006 - Sistema RAG Corporativo](#006---sistema-rag-corporativo)
- [FASE 3 (6-8 meses) - Agents & Automações](#fase-3-6-8-meses---agents--automações)
  - [Conceitos Principais](#conceitos-principais)
  - [Tool Calling](#tool-calling)
  - [ReAct Pattern](#react-pattern)
  - [LangGraph](#langgraph)
  - [Orquestração de Agentes](#orquestração-de-agentes)
  - [Agents + APIs Externas](#agents--apis-externas)
  - [Agents com Memória](#agents-com-memória)
  - [Projeto 3: Agent de Automação](#projeto-3-agent-de-automação)
- [FASE 4 (9-12 meses) - Produto + Mercado](#fase-4-9-12-meses---produto--mercado)
  - [Conceitos Principais](#conceitos-principais-1)
  - [Fine-tuning](#fine-tuning)
  - [Avaliação de LLMs](#avaliação-de-llms)
  - [Custos e Escalabilidade](#custos-e-escalabilidade)
  - [Segurança em IA](#segurança-em-ia)
  - [Padrões de Arquitetura](#padrões-de-arquitetura)
  - [Projeto Final: Mini SaaS com IA](#projeto-final-mini-saas-com-ia)
- [Tecnologias e Ferramentas](#tecnologias-e-ferramentas)
- [Estrutura do Repositório](#estrutura-do-repositório)
- [Projetos Principais](#projetos-principais)
- [Como Usar Este Repositório](#como-usar-este-repositório)
- [O que Você Vai Aprender](#o-que-você-vai-aprender)
- [Requisitos Iniciais](#requisitos-iniciais)
- [Recursos e Documentação](#recursos-e-documentação)
- [Notas](#notas)

---

## Objetivo

Parar de "testar" IA e começar a construir direito. Este repositório cobre as **FASES 1 e 2** de um roadmap completo de 12 meses para se tornar um desenvolvedor sênior em IA aplicada.

---

## FASE 1 (0-2 meses) - Base Sólida de IA Aplicada

**Objetivo:** Construir base sólida para trabalhar com IA aplicada

### Módulos:

#### 001 - Python, APIs LLM e Prompt Engineering
- Python essencial para devs JS (sintaxe, tipos, estruturas de dados)
- Integração com APIs de LLM (OpenAI, Anthropic)
- Autenticação e configuração de APIs
- Prompt Engineering: tipos de prompts, few-shot learning, chain-of-thought
- Tratamento de erros e variáveis de ambiente

#### 002 - Embeddings e Vector Databases
- O que são embeddings e como funcionam
- Similarity search (busca por similaridade semântica)
- Qdrant: setup, collections, upsert, query
- Armazenamento de embeddings com metadados
- Filtros por metadata para busca mais eficiente
- Integração embeddings + LLM

#### 003 - RAG Chatbot Completo
- Arquitetura RAG completa (retriever + generator)
- Fluxo: upload → chunk → embed → store → query → retrieve → generate
- Upload e processamento de PDFs
- Chunking de documentos longos
- Chat com histórico de conversa
- Backend Node.js + Python integrados
- **Projeto 1:** Chatbot RAG com documentos PDFs

---

## FASE 2 (3-5 meses) - RAG Profissional & Automações

**Objetivo:** Sair do "hello world" de IA e construir sistema profissional

### Módulos:

#### 004 - RAG Avançado
- Chunking strategies: tamanho fixo, hierárquico, semântico
- Metadata filtering: filtrar por tipo, data, fonte
- Re-ranking: ordenar resultados por relevância mais precisa
- Cross-Encoders e LLM-based re-ranking
- Otimização de precisão vs performance

#### 005 - RAG em Produção
- Cache de respostas (memória, Redis)
- Performance: latência, throughput, otimização
- Custos: token usage, otimização de gastos
- Avaliação de RAG: métricas, testes automatizados
- Monitoramento de qualidade e performance

#### 006 - Sistema RAG Corporativo
- Multi-usuário: autenticação, isolamento de dados
- Controle de acesso: permissões por usuário/grupo
- Logs e observabilidade: rastreamento de atividades
- Métricas e auditoria
- Deploy real: considerações de produção
- **Projeto 2:** Sistema RAG corporativo completo

---

## Tecnologias e Ferramentas

### Principais:
- **Python 3.8+**: Linguagem principal para IA
- **Node.js**: Backend para APIs e integração
- **OpenAI API**: LLMs e embeddings
- **Qdrant**: Vector database para embeddings
- **Redis**: Cache distribuído (opcional)

### Bibliotecas Python:
- `openai`: Cliente OpenAI API
- `qdrant-client`: Cliente Qdrant
- `PyPDF2`: Processamento de PDFs
- `python-dotenv`: Variáveis de ambiente
- `sentence-transformers`: Re-ranking (opcional)

### Backend:
- `express`: Framework Node.js
- `multer`: Upload de arquivos
- `axios`: Cliente HTTP

---

## Estrutura do Repositório

```
ai-studies/
├── README.md                          # Este arquivo - visão geral
├── 001_Python_APIs_LLM/
│   ├── README.md                       # Conceitos e teoria
│   └── DESAFIO.md                      # Prática e exercícios
├── 002_Embeddings_Vector_DB/
│   ├── README.md
│   └── DESAFIO.md
├── 003_RAG_Chatbot/
│   ├── README.md
│   └── DESAFIO.md                      # Projeto 1: Chatbot RAG
├── 004_RAG_Avancado/
│   ├── README.md
│   └── DESAFIO.md
├── 005_RAG_Producao/
│   ├── README.md
│   └── DESAFIO.md
└── 006_Sistema_RAG_Corporativo/
    ├── README.md
    └── DESAFIO.md                      # Projeto 2: Sistema Corporativo
```

---

## Projetos Principais

### Projeto 1: Chatbot RAG com Documentos (Módulo 003)
- Backend Node.js + Python
- Upload de PDFs
- Processamento e chunking
- Embeddings + Qdrant
- Chat com histórico
- Interface básica (opcional)

**Status:** Prático - Construir sistema completo do zero

### Projeto 2: Sistema RAG Corporativo (Módulo 006)
- Multi-usuário com autenticação
- Controle de acesso a documentos
- Logs e observabilidade
- Dashboard básico de métricas
- Deploy real (local ou cloud)

**Status:** Prático - Sistema completo para produção

---

## Como Usar Este Repositório

1. **Sequencial:** Os módulos são progressivos - comece pelo 001
2. **Teoria + Prática:** Cada módulo tem README.md (conceitos) e DESAFIO.md (prática)
3. **Projetos:** Complete os desafios para construir portfólio
4. **Referência:** Use READMEs como documentação de conceitos

---

## O que Você Vai Aprender

### Técnico:
- Python para trabalhar com IA
- Integração com APIs LLM (OpenAI, Anthropic)
- Prompt Engineering avançado
- Embeddings e similarity search
- Arquitetura RAG completa
- Vector databases (Qdrant)
- Otimização de sistemas RAG
- Produção: cache, performance, custos
- Multi-usuário e controle de acesso

### Projetos:
- **Chatbot RAG** funcional e completo
- **Sistema RAG corporativo** para produção
- Habilidades acima de 70% dos devs no mercado

---

## Requisitos Iniciais

- Conhecimento de JavaScript/TypeScript
- Familiaridade com APIs REST
- Noções básicas de terminal/linha de comando
- Conta OpenAI (para APIs)
- Python 3.8+ instalado
- Node.js 18+ instalado

---

## FASE 3 (6-8 meses) - Agents & Automações

**Objetivo:** Entrar no território mais valorizado - construir agentes autônomos que executam tarefas complexas

### Conceitos Principais

Agentes são sistemas de IA que podem:
- Tomar decisões autonomamente
- Usar ferramentas (tools) para executar ações
- Persistir memória entre interações
- Planejar e executar tarefas complexas
- Integrar com APIs externas

### Tool Calling

Agentes usam "tools" (ferramentas) para executar ações do mundo real:

**Conceitos:**
- Tools são funções que o agente pode chamar
- Schema de tools define input/output esperado
- LLM decide quando e como usar cada tool
- Tools podem ser: APIs, banco de dados, funções Python, etc.

**Exemplos de Tools:**
- Buscar informações (web search, APIs)
- Manipular dados (banco de dados, arquivos)
- Executar ações (enviar email, criar tarefa)
- Consultar sistemas externos

**Implementação:**
- Function calling da OpenAI
- Tools como parâmetro na chamada do LLM
- Parsing de respostas do modelo
- Execução de tools e retorno de resultados

### ReAct Pattern

ReAct (Reasoning + Acting) é um padrão que combina raciocínio e ação:

**Fluxo:**
1. **Thought**: Agente pensa sobre a tarefa
2. **Action**: Decide qual tool usar
3. **Observation**: Observa resultado da ação
4. **Thought**: Reavalia baseado na observação
5. **Repete** até completar tarefa

**Benefícios:**
- Raciocínio transparente (pode ver pensamentos do agente)
- Ações justificadas (cada ação tem motivo)
- Recuperação de erros (pode ajustar estratégia)
- Melhor para tarefas complexas e multi-passos

### LangGraph

LangGraph é uma biblioteca para construir agentes com grafos de estado:

**Conceitos:**
- Agente como grafo de estados
- Nós do grafo = decisões/ações
- Arestas = transições condicionais
- Estado persiste entre nós
- Fluxo de controle complexo

**Casos de Uso:**
- Agentes multi-passos
- Workflows complexos
- Loops e condições
- Memória e contexto entre etapas
- Orquestração de múltiplos agentes

**Vantagens:**
- Visualizar fluxo do agente
- Debug facilitado
- Reutilização de componentes
- Escalabilidade para sistemas complexos

### Orquestração de Agentes

Coordenar múltiplos agentes trabalhando juntos:

**Arquiteturas:**
- **Hierárquica**: Agente supervisor coordena agentes especializados
- **Paralela**: Múltiplos agentes trabalham simultaneamente
- **Sequencial**: Agentes executam em pipeline
- **Colaborativa**: Agentes trocam informações

**Desafios:**
- Comunicação entre agentes
- Resolução de conflitos
- Coordenação de tarefas
- Compartilhamento de contexto
- Performance e latência

### Agents + APIs Externas

Integrar agentes com sistemas externos via APIs:

**Integrações Comuns:**
- APIs REST/SOAP
- Banco de dados (SQL, NoSQL)
- Serviços cloud (AWS, GCP, Azure)
- Sistemas de terceiros (Slack, GitHub, etc.)
- Web scraping e pesquisa

**Padrões:**
- Wrapper de APIs como tools
- Autenticação e autorização
- Tratamento de erros e rate limits
- Cache de respostas
- Validação de inputs/outputs

**Segurança:**
- Validação de inputs antes de chamar APIs
- Sandbox para execução de tools
- Rate limiting e quotas
- Logs de todas as ações
- Controle de permissões

### Agents com Memória

Persistir memória entre interações para contexto continuado:

**Tipos de Memória:**
- **Curto prazo**: Contexto da conversa atual
- **Longo prazo**: Histórico de conversas anteriores
- **Semântica**: Embeddings de conversas passadas
- **Estruturada**: Informações específicas (perfil, preferências)

**Implementação:**
- Conversational memory (histórico)
- Vector store para busca semântica
- Banco de dados para persistência
- Summarization para memória longa
- Retrieval de contexto relevante

**Casos de Uso:**
- Chatbots com contexto
- Assistentes pessoais
- Sistemas de recomendação
- Aprendizado contínuo
- Personalização baseada em histórico

### Projeto 3: Agent de Automação

**Objetivo:** Construir agente que executa tarefas complexas autonomamente

**Funcionalidades:**
- Executa tarefas baseadas em descrição natural
- Consulta APIs externas para informações
- Atualiza banco de dados automaticamente
- Gera relatórios baseados em dados
- Interface web para interação
- Histórico de execuções e logs

**Stack:**
- Backend Python (LangChain/LangGraph)
- APIs para tools externas
- Banco de dados para persistência
- Interface web (React/HTML)
- Sistema de logs e observabilidade

**Exemplo de Tarefa:**
"Busque produtos com estoque baixo na API de inventário, atualize planilha com resultados e envie email para equipe de compras"

---

## FASE 4 (9-12 meses) - Produto + Mercado

**Objetivo:** Parecer um dev sênior com IA - construir produto completo e deploy em produção

### Conceitos Principais

Fase focada em levar sistema de IA para mercado real:
- Fine-tuning para casos específicos
- Avaliação rigorosa de qualidade
- Otimização de custos e escalabilidade
- Segurança e compliance
- Arquitetura de produção
- Produto SaaS completo

### Fine-tuning

Treinar modelo de base em dados específicos para melhor performance:

**Quando Usar:**
- Casos de uso específicos e repetitivos
- Vocabulário técnico/domínio específico
- Consistência em formato de saída
- Redução de custos (modelos menores)
- Melhor performance que prompts

**Processo:**
1. Coletar dataset de treinamento
2. Preparar dados no formato correto
3. Treinar modelo usando API de fine-tuning
4. Avaliar modelo fine-tuned
5. Deploy e monitoramento

**Datasets:**
- Conversas exemplo (input/output)
- Padrões de respostas esperadas
- Casos de borda e edge cases
- Validação e test sets

**Ferramentas:**
- OpenAI Fine-tuning API
- Hugging Face Transformers
- Google Vertex AI
- Local fine-tuning (LLaMA, Mistral)

### Avaliação de LLMs

Avaliar qualidade e performance de modelos de forma sistemática:

**Métricas Principais:**
- **Precisão**: Respostas corretas / total de respostas
- **Relevância**: Quanto resposta atende ao contexto
- **Consistência**: Respostas consistentes para inputs similares
- **Latência**: Tempo de resposta
- **Custo**: Tokens/custo por resposta

**Avaliação de RAG:**
- Precisão de retrieval (documentos relevantes)
- Relevância de resposta ao contexto
- Factualidade (respostas corretas)
- Coerência e fluidez
- Evitação de alucinações

**Ferramentas:**
- LLM-as-judge (GPT-4 avalia respostas)
- Testes unitários automatizados
- Métricas humanas (avaliação manual)
- Benchmarks públicos (MMLU, HellaSwag)
- Ragas (RAG-specific evaluation)

**Melhores Práticas:**
- Dataset de teste representativo
- Avaliação contínua em produção
- A/B testing entre modelos
- Monitoramento de qualidade em tempo real
- Feedback loop com usuários

### Custos e Escalabilidade

Otimizar custos e garantir escalabilidade para produção:

**Custos Principais:**
- **API Calls**: Preço por token (input/output)
- **Embeddings**: Criação e armazenamento
- **Vector DB**: Armazenamento e queries
- **Infraestrutura**: Servers, storage, bandwidth

**Otimização de Custos:**
- Cache de respostas frequentes
- Modelos menores quando possível (fine-tuned)
- Batch processing quando apropriado
- Compressão de embeddings
- Storage classes econômicas

**Escalabilidade:**
- **Horizontal**: Múltiplos servidores/instâncias
- **Vertical**: Servidores maiores
- **Load Balancing**: Distribuir carga
- **Caching**: Reduzir chamadas à API
- **Async Processing**: Processar em background

**Monitoramento:**
- Custos por usuário/feature
- Métricas de uso (queries, tokens)
- Alerts para custos elevados
- Otimizações baseadas em dados
- Budget limits e quotas

### Segurança em IA

Implementar segurança robusta em sistemas de IA:

**Principais Preocupações:**
- **Prompt Injection**: Ataques via input malicioso
- **Data Leakage**: Vazamento de dados de treinamento
- **Bias**: Vieses nos modelos
- **Privacy**: Dados sensíveis dos usuários
- **Adversarial Attacks**: Inputs manipulados

**Medidas de Segurança:**
- Validação rigorosa de inputs
- Sanitização de prompts
- Rate limiting e throttling
- Autenticação e autorização robustas
- Criptografia em trânsito e repouso
- Logs de auditoria

**Compliance:**
- LGPD/GDPR (proteção de dados)
- LGPD para dados pessoais em IA
- Transparência em uso de IA
- Direito de explicação
- Consentimento do usuário

### Padrões de Arquitetura

Padrões de arquitetura para sistemas de IA em produção:

**Arquiteturas Comuns:**
- **Microservices**: Serviços separados (RAG, LLM, Vector DB)
- **Serverless**: Funções serverless para escalabilidade
- **Event-Driven**: Eventos para comunicação assíncrona
- **Pipeline**: Processamento em etapas
- **Hybrid**: Combinação de padrões

**Componentes Típicos:**
- **API Gateway**: Roteamento e autenticação
- **Orquestrador**: Coordena fluxo (LangGraph, Airflow)
- **Vector DB**: Armazenamento de embeddings
- **Cache Layer**: Redis/Memcached
- **Message Queue**: RabbitMQ, SQS
- **Monitoring**: Logs, métricas, tracing

**Deploy:**
- **Docker**: Containers para consistência
- **Kubernetes**: Orquestração de containers
- **CI/CD**: Deploy automatizado
- **Blue-Green**: Deploy sem downtime
- **Canary**: Rollout gradual

### Projeto Final: Mini SaaS com IA

**Objetivo:** Construir produto SaaS completo de ponta a ponta

**Funcionalidades:**
- **Chat + RAG**: Chatbot com documentos próprios
- **Agents**: Automações inteligentes
- **Multi-tenant**: Múltiplos clientes isolados
- **Pagamentos**: Integração com Stripe/PagSeguro (fake ou real)
- **Dashboard**: Métricas, logs, configurações
- **Landing Page**: Página de apresentação do produto
- **Documentação**: Docs completas para usuários

**Stack:**
- **Frontend**: React/Next.js + Tailwind CSS
- **Backend**: Node.js/Express ou Python/FastAPI
- **Database**: PostgreSQL (dados) + Qdrant (embeddings)
- **Cache**: Redis
- **Auth**: JWT + OAuth2
- **Payments**: Stripe API
- **Deploy**: Vercel/Railway/AWS/GCP
- **Monitoring**: Sentry, DataDog

**Componentes:**
- Landing page responsiva
- Sistema de autenticação (signup/login)
- Dashboard de administração
- Interface de chat com RAG
- Configuração de agentes
- Planos e pagamentos
- Analytics e métricas
- Documentação interativa

**Deploy Real:**
- Deploy em cloud (AWS/GCP/Azure)
- Domínio customizado
- SSL/TLS certificates
- CDN para assets estáticos
- Backup automático
- Monitoring em produção

**Valor no Mercado:**
- Este tipo de projeto aparece muito em vagas PJ no Brasil
- Demonstra habilidades completas de IA aplicada
- Portfólio que destaca no mercado
- Base para produto real ou startup

---

## Recursos e Documentação

### Links Úteis:
- [OpenAI Platform](https://platform.openai.com/)
- [Qdrant Documentation](https://qdrant.tech/documentation/)
- [LangChain Documentation](https://python.langchain.com/)
- [Python Documentation](https://docs.python.org/3/)

### Cada Módulo Contém:
- Links para documentação oficial
- Exemplos de código práticos
- Dicas de troubleshooting
- Próximos passos sugeridos

---

## Notas

- Este repositório cobre **FASES 1 e 2** do roadmap completo
- Foco em prática: teoria + código em cada módulo
- Projetos reais para portfólio
- Padrão similar a `aws-cloud-basics` para consistência

---

**Comece pelo módulo 001 e siga em sequência. Boa jornada!** 🚀
