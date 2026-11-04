# Avaliador de Importação ML

Calculadora para avaliar, na feira de importação, se um produto vindo da China compensa para vender no Mercado Livre — cenários otimista e pessimista, preço máximo a pagar ao fornecedor e ficha do fornecedor.

- App de arquivo único (`index.html`), sem build.
- Avaliações salvas no Supabase (projeto Seller.a, tabela `public.importacao_avaliacoes`, com RLS por usuário).
- Se a internet cair na feira, a avaliação fica guardada no aparelho e sobe sozinha quando a conexão voltar.
- A busca de produtos no Mercado Livre usa o conector JoomPulse e só funciona com a página aberta dentro do Claude. Fora dele, informe o preço de venda manualmente.
