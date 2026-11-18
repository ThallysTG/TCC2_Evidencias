# Evidências dos testes de segurança

Arquivos de apoio do Trabalho de Conclusão de Curso "Análise de vulnerabilidades em APIs de aplicações SaaS geradas por assistentes de IA (Lovable, Gemini, Claude) com base no OWASP API Security Top 10 (2023)", Bacharelado em Sistemas de Informação, UNITINS, Câmpus Palmas, 2026.

- Autor: Thallys Antonio Barbosa Silva
- Orientadora: Profa. Dra. Márcia Maria Savoine

O repositório reúne os registros das 174 execuções (29 casos de teste em 6 aplicações) e as capturas de tela feitas durante os testes.

## Aplicações

| Código | Assistente | Condição do *prompt* |
|---|---|---|
| A1 | Lovable | A: apenas a especificação funcional |
| B1 | Lovable | B: especificação funcional e requisitos de segurança |
| A2 | Gemini (Google Antigravity) | A |
| B2 | Gemini (Google Antigravity) | B |
| A3 | Claude (Claude Code) | A |
| B3 | Claude (Claude Code) | B |

## Estrutura

| Pasta ou arquivo | Conteúdo |
|---|---|
| `evidencias/<aplicação>/<caso>.txt` | Requisições e respostas HTTP de cada execução. O nome do arquivo é o código do caso (Quadro 7 e Apêndice B do trabalho). |
| `evidencias/<aplicação>/ACEITACAO.txt` | Teste de aceitação funcional das aplicações executadas localmente (A2, B2, A3 e B3). |
| `capturas/<aplicação>/` | Capturas de tela do Postman, do Burp Suite, do OWASP ZAP e do Visual Studio Code. As figuras do Apêndice E do trabalho são recortes destas capturas. |
| `capturas/aceitacao/` | Telas de login, de tarefas e de administração de cada aplicação no teste de aceitação. |
| `zap/` | Relatórios da varredura passiva do OWASP ZAP, em HTML e em Markdown. |
| `postman/` | Coleções e ambientes do Postman usados nos testes. |

## Dados ocultados

Para a publicação, foram ocultados:

- as senhas das contas de teste, que aparecem como `****`;
- os *tokens* JWT, que aparecem truncados (início…fim [tamanho]);
- as chaves de API do Supabase, que aparecem como `sb_publishable_[chave removida]`;
- o e-mail pessoal do pesquisador, trocado por `pesquisador@email.removido` nos textos e coberto por tarja cinza nas capturas.

As senhas padrão encontradas nos arquivos `docker-compose.yml` (caso T8.5) foram mantidas, porque são a própria falha registrada. Os *tokens* que aparecem nas capturas das aplicações locais (A2, B2, A3 e B3) não dão acesso a nenhum serviço publicado.
