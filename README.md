## Guilherme Caliari

Ciência da Computação na UVV, 2º período. Desenvolvo sistemas web com **Python** e
**PostgreSQL**, construindo com agentes de IA de código (Claude Code e Codex): eu especifico a
tarefa, reviso o que é gerado, rodo os testes e coloco no ar.

---

### Em destaque: sistema de gestão da Comercinox *(repositório privado)*

Sistema interno de consulta e gestão de uma distribuidora B2B de aço inox, em uso desde
outubro de 2026, construído com agentes de IA sob minha condução.

- **Back-end** em Python com SQLAlchemy e banco PostgreSQL
- **Interface web** com 11 telas, entre catálogo, clientes, ficha do produto com histórico de
  vendas, vendas do dia, Mercado Livre e alerta de saldo negativo de estoque
- **Integração sem abrir o ERP para fora:** um coletor na loja lê o banco do ERP só para
  leitura, valida os dados e envia uma cópia compactada para um armazenamento privado na
  nuvem. Um worker agendado importa essa cópia no PostgreSQL em uma única transação
- **Testes:** 130 em Python (pytest) e 24 de ponta a ponta no navegador (Playwright)
- **Processo:** dois agentes de código trabalhando em paralelo, cada um na sua branch e
  worktree, com reserva de arquivos antes de editar, revisão antes de integrar e decisões de
  arquitetura registradas

---

### Projetos

**[Retain](https://github.com/guzazo/RetainByBolt)** · [app no ar](https://retainbybolt.streamlit.app) — hackathon InovaApps (UVV, setembro de 2026).
Painel para empresas de contrato recorrente que ordena os clientes por risco de cancelamento
vezes a mensalidade, com pesos explicáveis tirados do histórico, projeção de 3 meses e ajuste
dos pesos pelo gestor com recálculo na hora. Equipe de 4; desenvolvi o protótipo com mais um
integrante. Python, Streamlit, pandas, NumPy e Altair.

**[Vennperio](https://github.com/UVV-CC1N-26-P3/Vennperio)** — jogo multiplayer em JavaScript nos moldes do paper.io, em que a mecânica é teoria dos conjuntos.
Extensão universitária ligada à ODS 4 (Educação de Qualidade). A parte de rastro e dominação
de território ficou com duas pessoas, cada uma com sua versão. A
[minha](https://github.com/UVV-CC1N-26-P3/Vennperio/tree/dominacao-guzazo) faz a geometria de
polígonos sem biblioteca (ponto em polígono, interseção de segmentos, fusão do rastro com a
base e diferença entre polígonos), sincroniza a captura de área entre jogadores via socket.io,
detecta colisão com rastro usando grade espacial e desenha um minimapa. Node.js, Express e
socket.io.

**[Projeto ARCA](https://github.com/Projeto-arca/PROJETO-ARCA---Grupo-4)** — sistema web de gestão de adoção e cuidado de animais, para o Programa de Proteção Animal da Prefeitura da Serra.
Fiquei com a interface: telas de login e dashboard para quatro perfis de usuário (tutor,
candidato à adoção, ONG e prefeitura). Node.js, Express, PostgreSQL e front em HTML, CSS e
JavaScript puro. De oito grupos da turma, o nosso foi um dos três escolhidos para apresentar o
projeto à Prefeitura da Serra; a apresentação está sendo organizada e ainda não tem data.

**[atendimento-ia](https://github.com/guzazo/atendimento-ia)** — integração da API do Mercado Livre com a API da Anthropic, orquestrada em n8n, para responder perguntas de pós-venda.
Funcionou, mas desliguei depois de medir que o custo por pergunta não compensava no volume
do canal.

---

### Stack

- **Linguagens** — Python, JavaScript, SQL
- **Back-end** — SQLAlchemy, Node.js, Express, socket.io
- **Front-end** — HTML, CSS, Streamlit
- **Dados** — PostgreSQL, SQL Server; modelagem, DDL, DML e consultas analíticas
- **Testes e entrega** — pytest, Playwright, GitHub Actions, Git
- **IA** — agentes de código (Claude Code, Codex), API da Anthropic, n8n

---

Inglês B2. Uma regra que eu sigo, em relatório e em código: separo o que foi medido, o que é
leitura minha em cima disso e o que ainda não dá para afirmar. Nunca misturo os três.
