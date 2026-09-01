# Painel de Campanhas CRM — Bet dá Sorte

Acompanhamento das campanhas de CRM por canal (Flow, Missão, E-mail, Telegram,
Pop-up, SMS, Inbox, Push, Banner). Substitui a planilha de acompanhamento.

- **Site:** publicado por GitHub Pages a partir da branch `main`.
- **Dados:** ficam no Supabase, não neste repositório.
- **Acesso:** restrito. Login por link enviado ao e-mail corporativo, e o banco
  só responde a quem está na tabela `perfis`.

## Sobre a chave que aparece no código

O `index.html` traz a URL do projeto e a chave *publishable* do Supabase. As duas
são públicas por natureza — ficam visíveis no navegador de qualquer visitante, como
em qualquer site. Elas não dão acesso a nada sozinhas: quem decide o que cada pessoa
pode ler e escrever são as regras de Row Level Security dentro do banco.

A chave `service_role` / secret **nunca** entra aqui.

## Como mexer

O painel é um arquivo só, `index.html`. Publicar = commit na `main`.
A estrutura do banco e as regras de segurança estão em `../supabase/`.
