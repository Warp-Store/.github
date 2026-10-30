<div align="center">

# 🚀 Warp Store

**Crie sua loja e monetize seu servidor de forma automática.**

Plataforma de lojas virtuais com **entrega instantânea** de produtos para servidores de jogos.
Configure sua loja, conecte ao seu servidor e comece a vender — sem entrega manual.

[🌐 Site](https://warpstore.app) · [📚 Documentação](https://wiki.warpstore.app/introduction) · [❓ F.A.Q](https://wiki.warpstore.app/faq)

</div>

---

## O que é a Warp Store?

A Warp Store é uma solução de ponta a ponta para **donos de servidores de FiveM e MTA:SA** que
querem monetizar seus projetos. Você cria a loja, cadastra os produtos e conecta ao seu servidor —
a partir daí, cada compra é **entregue automaticamente ao jogador assim que o pagamento é aprovado**.

> Usada por mais de 250 servidores. 💜

### ✨ Principais recursos

- ⚡ **Entrega automática** — o produto chega ao jogador logo após a confirmação do pagamento.
- 🛠️ **Solução completa** — criação da loja, cadastro de produtos e conexão com o servidor.
- 🎨 **Personalização** — ajuste a aparência e o funcionamento da sua loja.
- 📊 **Painel de ganhos** — gráficos de vendas em tempo real e gestão dos meios de pagamento.
- 💳 **Múltiplos pagamentos** — Mercado Pago & Pix e PayPal.
- 🔒 **Segurança e desempenho** — stack moderna com foco em performance e proteção.
- 🔌 **Integrações** — redes sociais, chat online e API para layouts customizados.

---

## 📦 Conteúdo deste repositório

Este repositório reúne os componentes de integração da Warp Store:

| Pasta | Descrição | Stack |
|---|---|---|
| [`warp-delivery-game-mta/`](warp-delivery-game-mta) | Plugin de integração para **MTA:SA** (`warpstore_integration` v3.0) que recebe a fila de comandos da plataforma e entrega os produtos no servidor. | Lua (MTA:SA) |

---

## 🎮 Plugin MTA:SA (`warp-delivery-game-mta`)

Resource que conecta seu servidor MTA:SA à plataforma e executa as entregas.

**Requisitos:** MTA:SA `1.5.9` ou superior (cliente e servidor).

### Instalação

1. Copie a pasta `warp-delivery-game-mta` para o diretório `resources/` do seu servidor.
2. Configure o [`config.lua`](warp-delivery-game-mta/config.lua):
   - `['token']` — token da sua loja (em **warpstore.app**).
   - `['data:id']` — element data usada para identificar o ID do jogador.
   - `['color:hex']` — cor padrão das mensagens.
   - Ajuste os formatos de notificação de entrega: **balões**, **chatbox** e **infobox**.
3. Personalize os comandos de entrega em [`commands.lua`](warp-delivery-game-mta/commands.lua)
   conforme os produtos da sua loja.
4. Inicie o resource:
   ```
   start warpstore_integration
   ```

> 💡 As notificações de entrega e os comandos de produto são totalmente editáveis.

---

## 💳 Meios de pagamento

- [Mercado Pago & Pix](https://wiki.warpstore.app/gateways/mercado-pago)
- [PayPal](https://wiki.warpstore.app/gateways/paypal)

## 🔗 Links úteis

- **Site:** https://warpstore.app
- **Documentação:** https://wiki.warpstore.app/introduction
- **F.A.Q:** https://wiki.warpstore.app/faq
- **Termos & Condições:** https://wiki.warpstore.app/terms
- **API para desenvolvedores:** https://wiki.warpstore.app/developers/layout/introduction
- **Demo:** https://demo.wrpstore.app
- **Demo Esmerald:** https://esmerald.wrpstore.app

---

## 🏁 Começando em 4 passos

1. **Crie sua conta** em [warpstore.app](https://warpstore.app).
2. **Crie sua loja** e cadastre seus produtos.
3. **Configure o plugin** no seu servidor (veja a seção do MTA:SA acima).
4. **Divulgue o link** da sua loja para seus clientes e comece a vender. 🎉

---

<div align="center">

**[warpstore.app](https://warpstore.app)** — transformando o mundo com a melhor automatização do mercado.

</div>
