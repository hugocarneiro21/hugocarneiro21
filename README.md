# Hugo Carneiro

**Agentes de IA, hiperautomação e produtos SaaS.** Belo Horizonte, MG.

Construo agentes de IA e sistemas autônomos que eliminam processos manuais de ponta a ponta. Hoje faço isso na **Stellar Gaming (EstrelaBet)**, para as áreas de Facilities e Administrativo, e na **Evoliz**, minha marca de automação inteligente para empresas.

Sou formado em Automação Industrial, com pós-graduação em andamento. Comecei na automação predial. Foram 7 anos na Localiza&Co, onde saí do predial, passei pelo atendimento e cheguei à área de Processos, Qualidade e Melhoria Contínua, automatizando com RPA e dashboards. Hoje construo do banco ao deploy com Python, TypeScript e IA no fluxo de trabalho.

## O que eu sei fazer

- **Hiperautomação.** Processos inteiros de ponta a ponta, juntando RPA, IA, integrações e regras de negócio, com humano no circuito só onde a decisão pede.
- **Harness de engenharia com IA.** Desenvolvimento com Claude Code guiado por especificação, regras fixas, hooks que barram segredos, skills, memória e agentes revisores nos pedidos de maior risco.
- **Guardrails.** Saída de LLM validada antes de chegar ao banco, campo extraído só com o trecho literal da fonte, temperatura 0 e dry-run com aprovação humana antes de qualquer envio.
- **Boas práticas.** TDD, regra de negócio isolada de I/O, idempotência, RLS em todas as tabelas, segredos fora do código e ensaio transacional antes de mudança sensível no banco.
- **Agentes de IA.** LLM com ferramentas e MCP, extração estruturada de PDF com guardrail, RAG com busca vetorial (pgvector) e bots de Telegram e WhatsApp.
- **RPA e integração com ERP.** Robôs em Playwright em sistemas corporativos com login SSO/MFA e modo dry-run, integração com Oracle Fusion e OTBI, Jira Service Management, Pipefy e Microsoft Graph.
- **Automação orientada a eventos.** Workers que vigiam filas e chamados, com idempotência, retry, circuit breaker e watchdog para rodar sozinhos.
- **Backend e dados.** APIs em Python (FastAPI, Flask) e TypeScript, REST e GraphQL, Postgres e Supabase com RLS multi-tenant e edge functions.
- **Pagamentos.** Pix e cartão com confirmação por webhook idempotente, cobrança recorrente e split (Mercado Pago, Asaas).
- **Automação predial e IoT.** Controle de iluminação e climatização, integração com equipamentos locais e túnel zero-trust com Cloudflare.
- **Low-code quando faz sentido.** Lovable para front e Power Automate para fluxos do Microsoft 365.
- **Painéis e análise.** Dashboards em React, Flask com Chart.js e Power BI, e backtest quantitativo em Python.

## Na Stellar Gaming

**Plataforma de decisão de contratos.** Hiperautomação de ponta a ponta para a diretoria, no ar em 3 dias. Os contratos chegam por API GraphQL, um LLM lê os PDFs com saída estruturada e um guardrail só aceita o campo que vier com o trecho literal do contrato. Sem o trecho, o campo fica "Não identificado", nunca inventado. A diretoria decide contrato a contrato, e o envio pelo Microsoft Graph só sai depois de dry-run e aprovação humana. *Mais de 2.800 testes automatizados e nenhum envio duplicado.*

**Portal Gestão de Contratos.** Plataforma API-first de contratos e ordens de compra, a fonte única de verdade do Administrativo. Regras, KPIs e SLA são calculados no servidor, e os sistemas satélites só consomem o dado pronto. Assim nenhum painel mostra um número diferente do outro.

**Analisador de Contratos com IA.** Lê o PDF e gera a ficha contratual estruturada. A parte difícil foi governar o modelo: temperatura 0 para o mesmo contrato dar sempre o mesmo resultado e curadoria do corpus, que descarta propostas, catálogos e documentos societários antes da análise.

**Stellar Control System (BMS).** Sistema de controle predial do novo escritório, feito do zero. Ele faz o que plataformas comerciais (Siemens, Honeywell, Schneider) cobram de R$ 80 mil a R$ 300 mil só de licença. Controla iluminação e climatização em tempo real por zona e pavimento, com planta baixa interativa, integração por SSE e bridge com túnel zero-trust. O desligamento progressivo no fim do expediente corta o desperdício de energia.

**Agente Autônomo de Logística.** Orientado a eventos, monitora o Jira e executa o despacho nas plataformas dos parceiros: etiqueta de SEDEX no VIPP e cotação e pedido de motoboy. Tem idempotência para nunca duplicar frete, circuit breaker com retry e um painel em Flask.

**Locker System.** Ciclo completo dos escaninhos sem intervenção manual. Detecta o chamado, aloca o escaninho livre, gera o Termo de Uso em PDF, colhe a assinatura digital e fecha o chamado sozinho.

**Agente de políticas internas (RAG).** Responde dúvidas sobre as políticas do Administrativo com a resposta ancorada no documento real, por busca vetorial. *Next.js, Supabase, pgvector.*

## Produtos próprios

| Produto | O que faz | Stack |
|---|---|---|
| **[BarberJá](https://barberja.com.br)** | Agenda, clube de assinatura e caixa para barbearias. Cada barbearia ganha seu subdomínio, com cobrança recorrente, split automático de pagamento e lembrete por WhatsApp. | Next.js, FastAPI, Supabase, Asaas |
| **[AgendaDela](https://agendadela.com.br)** | O mesmo motor do BarberJá, desenhado para salões de beleza. | Next.js, Supabase |
| **[Tá Servido?](https://taservido.com.br)** | Delivery próprio para lanchonetes, sem taxa por pedido. Cardápio por loja, Pix confirmado por webhook e total sempre recalculado no servidor. | Next.js, Supabase, Mercado Pago |

## Stack

<img src="https://skillicons.dev/icons?i=py,ts,nextjs,react,tailwind,fastapi,flask,supabase,postgres,sqlite,cloudflare,vercel,git" alt="Python, TypeScript, Next.js, React, Tailwind, FastAPI, Flask, Supabase, Postgres, SQLite, Cloudflare, Vercel, Git" />

## Contato

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/hugocarneiro21/)
[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=flat-square&logo=instagram&logoColor=white)](https://instagram.com/hugocarneirofx)

<sub>Os sistemas da Stellar e os produtos têm código fechado. Os repositórios públicos abaixo são da fase de estudo, em Python, dados e C#.</sub>
