### Olá, eu sou a Maria Antonia

Desenvolvedora Python em formação e estudante de Análise e Desenvolvimento de Sistemas (conclusão em janeiro de 2029), em Teresina (PI). Gosto de backend, de dados e de usar IA dentro de sistemas de verdade, com teste e medição. Busco estágio.

## Projetos

### [consulta-cnpj](https://github.com/SudoMary/consulta-cnpj)

Consulta de CNPJ com histórico: guarda cada consulta e mostra quando a situação cadastral de uma empresa mudou, por exemplo de ATIVA para BAIXADA.

**No ar:** [consulta-cnpj-pfpj.onrender.com](https://consulta-cnpj-pfpj.onrender.com) (plano grátis: o primeiro acesso depois de um tempo parado leva cerca de 1 minuto).

- Backend em FastAPI, com site (HTML montado no servidor, modo escuro) e linha de comando.
- SQLAlchemy com SQL escrito à mão; SQLite no desenvolvimento e PostgreSQL (Supabase) em produção; histórico append-only.
- Integração resiliente: timeout, novas tentativas com espera crescente e uma segunda API pública como reserva.
- Coleta diária das empresas acompanhadas, agendada no GitHub Actions e idempotente.
- Assistente com LLM, no site e na linha de comando: perguntas em português respondidas por ferramentas que só leem o banco, com o Claude ou com um modelo grátis do OpenRouter; limite diário e registro de tokens por pergunta.
- 445 testes no CI, com os testes de banco rodando nos dois bancos.

### [classificador-avaliacoes](https://github.com/SudoMary/classificador-avaliacoes)

Classifica avaliações de clientes em português (dataset público da Olist): o motivo da reclamação e se a loja precisa responder.

**No ar:** [classificador-avaliacoes.onrender.com](https://classificador-avaliacoes.onrender.com): cole uma avaliação e veja as regras e o LLM lado a lado.

- Amostra estratificada por nota, com conjuntos separados de desenvolvimento e teste.
- Guia de rotulagem e ferramenta de rotulagem e revisão na linha de comando.
- Métricas implementadas do zero: precisão, revocação e F1 por categoria, F1 macro e matriz de confusão.
- Linha de base por regras: 78,7% de acerto no motivo, contra 41,3% de "sempre a classe mais comum".
- Classificador com LLM grátis (Nemotron 3.5 Super, via OpenRouter): 96,0% de acerto no motivo, custo zero, 15 avaliações por requisição e cache das respostas.
- Classificador e medição só com a biblioteca padrão; site em FastAPI; 126 testes, nenhum chama a rede.

## Ferramentas

Python · FastAPI · SQLAlchemy · PostgreSQL · SQLite · pytest · Git · GitHub Actions · API do Claude · OpenRouter

## Contato

[LinkedIn](https://www.linkedin.com/in/maria-antonia-rosa-a6598b43b/)
