### 2.3.7 - 10/10/2016
- Ajustes no problema de comunicação com a API da Vindi.
- Alterando o tempo de cache dos métodos de pagamento para 1 hora.

### 2.3.6 - 02/02/2016
- Adicionando suporte para tls 1.2 e aumentando versão mínima do PHP para 5.5.19​

### 2.3.5 - 06/01/2016
- Correção do bug na página das Orders (call_user_func() 'WC_Vindi_BankSlip_Gateway').

### 2.3.4 - 10/11/2015
- Melhorias na validação da configuração da chave API.

### 2.3.3 - 22/10/2015
- Melhorias na comunicação com os webhooks.

### 2.3.2 - 30/07/2015
- Melhorias na comunicação com a API da Vindi.
- Arrumado erro com a constante `WC_VINDI_VERSION`

### 2.3.1 - 06/07/2015
- Adicionada opção para enviar informações para emissão de NFe's.

### 2.3.0 - 08/06/2015
- Adicionada validação tornando necessária a utilização de um certificado SSL para realização de cobranças em produção.
- Divisão dos métodos de pagamento Cartão de Crédito e Boleto Bancário em dois gateways distintos, podendo ser habilitados separadamente.
- Cobranças rejeitadas agora são informadas no pedido. Caso todas as tentativas de cobrança sejam rejeitadas, o status do pedido é atualizado para "Falhado".
- Adicionado token de segurança aos webhooks.
- Adicionada validação de quantidade ao atualizar itens do carrinho para evitar a compra de mais de uma assinatura ao mesmo tempo.
- Retrabalhada a validação do campo CVV em cartões.
- Removida a dependência CSS. As regras foram simplificadas e aplicadas de forma *inline*.
- Removido logo da Vindi das opções de pagamento. Com a divisão de gateways, tornou-se desnecessário.
- Algumas consultas a API foram adicionados ao cache do WordPress (*transients*) para ganho de performance.
- Adicionado o plugin [WooCommerce Extra Checkout Fields for Brazil](https://wordpress.org/extend/plugins/woocommerce-extra-checkout-fields-for-brazil/) à lista de dependências.
- Adicionada mensagem de alerta caso a conta Vindi esteja em modo Trial.
- Grande Refatoração do Código para manter o mesmo estilo de código do WordPress.
- Outras pequenas melhorias e validações.

### 2.2.0 - 08/05/2015
- Retrabalhada a forma como o status do pedido é definido quando a confirmação de pagamento é recebida.
- Informações de endereço e documento agora são enviados para a criação do usuário na Vindi, para permitir a emissão de notas fiscais.

### 2.1.0 - 26/04/2015
- Pedidos agora reduzem o estoque de produtos em assinaturas e vendas avulsas.

### 2.0.0 - 05/03/2015
- Nova versão do plugin, com suporte a nova API, aceitando assinaturas e vendas avulsas.
