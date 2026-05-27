### Parte 1 – Análise do Sistema Real

* **1.1 Objetivo:** Sistema de pedidos para otimizar o atendimento em estabelecimento comercial, reduzindo a necessidade de atendimento humano direto e mitigando gargalos operacionais na recepção.
* **1.2 Escopo Funcional (Cliente):** * Visualização de cardápio (itens, combos e promoções).
    * Customização de itens com validação de campos obrigatórios antes da inserção no carrinho (ex: seleção de sabores e bordas).
    * Persistência de dados cadastrais (endereço e telefone) via *local storage*.
    * Cálculo automatizado de taxas de entrega com base na modalidade (Delivery ou Retirada).
    * Registro do método de pagamento (PIX, Crédito, Débito ou Dinheiro com cálculo de troco); o processamento do pagamento é estritamente presencial (checkout offline).
    * Bloqueio de requisições fora do horário de funcionamento com redirecionamento de rota.
* **1.3 Fluxo de Navegação:** Cardápio (Categorias/Promoções/Descontos) -> Customização e Observações do Item -> Carrinho de Compras -> Checkout (Definição de entrega e pagamento) -> Envio do pedido.
* **1.4 Estrutura do Cardápio:** * *Categorias:* Produtos individuais tratados de forma isolada (ex: tamanhos de pizza gerenciados como SKUs distintos).
    * *Combos:* Produtos base acoplados a extras com acréscimos de valor fixo (R$10 ou R$12).
    * *Promoções:* Seção destinada a itens com desconto aplicado.

---

