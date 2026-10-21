# GL Estoque

Sistema de gestão para depósito de material de construção. Projeto de portfólio da GL Solutions: HTML, CSS e JavaScript puro, sem build. Os dados são fictícios e ficam salvos no `localStorage` do navegador.

## Como abrir
Abra `index.html` no navegador ou sirva a pasta:

```bash
python -m http.server 5173
```

## O que a demonstração mostra
- **Balcão:** venda rápida por busca ou categoria, carrinho com quantidades (sacos, m³, milheiros), desconto, entrega com frete, pagamento em dinheiro (com troco), PIX, cartão ou fiado, com limite de crédito do cliente. Cupom para imprimir ou enviar por WhatsApp.
- **Orçamentos:** salvar do carrinho, enviar ao cliente, aprovar ou recusar e converter em venda com um clique.
- **Estoque:** 61 produtos, alerta de estoque mínimo, entrada de mercadoria, ajuste de contagem, margem por produto, reposição agrupada por fornecedor (pedido por WhatsApp) e histórico de movimentações.
- **Clientes e a receber:** ficha com saldo devedor e limite, recebimento total ou parcial, cobrança por WhatsApp.
- **Entregas:** quadro de separando, em rota e entregue, com motorista e aviso ao cliente.
- **Caixa:** abertura, suprimento, sangria, despesas e fechamento com conferência.
- **Painel e relatórios:** vendas, lucro bruto, ticket médio, curva ABC, categorias e exportação em CSV.
- Responsivo, com foco no celular, e tema claro/escuro.

## Estrutura
```
index.html
css/styles.css, css/estoque.css
js/util.js    ícones, datas, gráficos SVG
js/data.js    catálogo e gerador de dados de demonstração
js/core.js    regras de negócio (estoque, vendas, fiado) e interface
js/pdv.js     balcão, carrinho, orçamentos e documentos
js/pages.js   painel, vendas, estoque, clientes, entregas, caixa, relatórios
js/app.js     rotas e layout
```
