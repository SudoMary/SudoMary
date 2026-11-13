### Olá, eu sou a Maria Antonia

Desenvolvedora Python em formação e estudante de Análise e Desenvolvimento de Sistemas (conclusão em janeiro de 2029), em Teresina (PI). Gosto de backend, de dados e de usar IA dentro de sistemas de verdade, com teste e medição. Busco estágio.

## Projetos

### [consulta-cnpj](https://github.com/SudoMary/consulta-cnpj)

Consulta de CNPJ com histórico: guarda cada consulta e mostra quando a situação cadastral de uma empresa mudou, por exemplo de ATIVA para BAIXADA.

- Backend em FastAPI, com site (HTML montado no servidor, modo escuro) e linha de comando.
- SQLAlchemy com SQL escrito à mão; SQLite no desenvolvimento e PostgreSQL (Supabase) em produção; histórico append-only.
- Integração resiliente: timeout, novas tentativas com espera crescente e uma segunda API pública como reserva.
- Coleta diária das empresas acompanhadas, agendada no GitHub Actions e idempotente.
- Assistente com o Claude: perguntas em português respondidas por ferramentas que só leem o banco, com limite diário e registro de tokens.
- 407 testes no CI, com os testes de banco rodando nos dois bancos.

### [classificador-avaliacoes](https://github.com/SudoMary/classificador-avaliacoes)

Classifica avaliações de clientes em português (dataset público da Olist): o motivo da reclamação e se a loja precisa responder.

- Amostra estratificada por nota, com conjuntos separados de desenvolvimento e teste.
- Guia de rotulagem e ferramenta de rotulagem e revisão na linha de comando.
- Métricas implementadas do zero: precisão, revocação e F1 por categoria, F1 macro e matriz de confusão.
- Linha de base por regras: 78,7% de acerto no motivo e 91,3% em "precisa responder", contra 41,3% de "sempre a classe mais comum".
- Python só com a biblioteca padrão; 90 testes.

## Ferramentas

Python · FastAPI · SQLAlchemy · PostgreSQL · SQLite · pytest · Git · GitHub Actions · API do Claude

## Contato

[LinkedIn](https://www.linkedin.com/in/maria-antonia-rosa-a6598b43b/)
