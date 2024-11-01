=== Vindi WooCommerce Assinaturas ===
Contributors: erico.pedroso, tales.galvao.vindi, wnarde
Website Link: https://www.vindi.com.br
Tags: vindi, subscription, membership, pagamento-recorrente, cobranca-recorrente, cobrança-recorrente, recurring, site-de-assinatura, assinaturas, faturamento-recorrente, recorrencia, assinatura, subscription-billing, cielo, elavon, rede, redecard, boleto, boleto-bancario, cartao-de-credito, bank-slip, credit-card, woocommerce
Requires at least: 4.0
Tested up to: 4.2
Stable Tag: 2.3.7
License: GPLv3
License URI: http://www.gnu.org/licenses/gpl-3.0.html

Este plugin foi descontinuado. Já está disponível o Vindi WooCommerce Subscriptions, acesse o link na descrição.

== Description ==
**Este plugin foi descontinuado. Já está disponível o [Vindi WooCommerce Subscriptions](http://www.github.com/vindi/vindi-woocommerce-subscriptions) para uma gestão mais completa de assinaturas e compras únicas.**

O **Vindi WooCommerce** oferece uma solução simples para pagamentos únicos e assinaturas com cartão de crédito e boleto utilizando o [WooCommerce](https://wordpress.org/plugins/woocommerce/). Basta ter [uma conta habilitada na Vindi](https://app.vindi.com.br/prospects/new), para começar a cobrar seus clientes.

A [Vindi](http://www.vindi.com.br/) é líder em cobrança recorrente no Brasil. Com centenas de clientes usando soluções como pagamento online, soluções de notas fiscais integradas, emissão de boletos por email e PDF, integrações com ERPs e diversos relatórios, a Vindi possibilita um sistema online completo para negócios de venda recorrente. Além disso, empresas podem usar o gateway de pagamento integrado ao billing recorrente ou para faturas avulsas.

== Installation ==

1. Envie os arquivos do plugin para a pasta `wp-content/plugins` ou utilize o instalador de plugins do WordPress.
1. Ative o plugin.

= Requisitos =
- PHP versão **5.5.19** ou superior.
- Um site com o WordPress instalado.
- Plugin [WooCommerce](https://wordpress.org/plugins/woocommerce/) instalado e habilitado.
- Plugin [WooCommerce Extra Checkout Fields for Brazil](https://wordpress.org/extend/plugins/woocommerce-extra-checkout-fields-for-brazil/) instalado e habilitado.
- Certificado Digital (é recomendado um de 2048 bits).
- [Possuir uma conta habilitada na Vindi](https://app.vindi.com.br/prospects/new).

= Configuração =

1. Configure o plugin na página de administração do WordPress em:
    - *WooCommerce -> Configurações -> Finalizar Compra -> Vindi - Cartão de Crédito* e
    - *WooCommerce -> Configurações -> Finalizar Compra -> Vindi - Boleto Bancário*.
1. Em *WooCommerce -> Campos do Checkout*, ative Tipo de Pessoa Física e Jurídica, RG e Inscrição estadual.
1. Em *WooCommerce -> Configurações -> Produtos -> Inventário*, coloque um zero na opção "Manter estoque (minutos)".

Para mais detalhes sobre a instalação de plugins no WordPress leia o tutorial [WordPress - Gerenciando Plugins] (http://codex.wordpress.org/pt-br:Gerenciando_Plugins#Instalando_Plugins).

== Frequently Asked Questions ==

Para suporte ou dúvidas relacionadas ao Plugin você pode seguir pelos canais:
- [Github](https://github.com/vindi/vindi-woocommerce/issues)
- [Fórum do Plugin](https://wordpress.org/plugins/vindi-woocommerce-assinaturas) (apenas em inglês)

Caso necessite de informações sobre a plataforma ou API por favor siga através do canal
- [Atendimento Vindi](http://atendimento.vindi.com.br/hc/pt-br)[Atendimento Vindi](http://atendimento.vindi.com.br/hc/pt-br)

== Screenshots ==

1. Configurações do plugin para cartão de crédito.
2. Configurações do plugin para boleto bancário.
3. Método de pagamento na página de finalizar o pedido para cartão de crédito.
4. Método de pagamento na página de finalizar o pedido para boleto bancário.
5. Botão de download do boleto ao concluir o pedido via boleto bancário.

== Changelog ==

= 2.3.7 - 10/10/2016 =
- Ajustes no problema de comunicação com a API da Vindi.
- Alterando o tempo de cache dos métodos de pagamento para 1 hora.

= 2.3.6 - 02/02/2016 =
- Adicionando suporte para tls 1.2 e aumentando versão mínima do PHP para 5.5.19​

= 2.3.5 - 04/01/2016 =
- Correção do bug na página das Orders (call_user_func() 'WC_Vindi_BankSlip_Gateway').

= 2.3.4 - 10/11/2015 =
- Melhorias na validação da configuração da chave API.

= 2.3.3 - 22/10/2015 =
- Melhorias na comunicação com os webhooks.

= 2.3.2 - 30/07/2015 =
- Melhorias na comunicação com a API da Vindi.
- Arrumado erro com a constante 'WC_VINDI_VERSION'

= 2.3.1 - 06/07/2015 =
- Adicionada opção para enviar informações para emissão de NFe's.

= 2.3.0 - 08/06/2015 =
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

= 2.2.0 - 08/05/2015 =
- Retrabalhada a forma como o status do pedido é definido quando a confirmação de pagamento é recebida.
- Informações de endereço e documento agora são enviados para a criação do usuário na Vindi, para permitir a emissão de notas fiscais.

= 2.1.0 - 26/04/2015 =
- Pedidos agora reduzem o estoque de produtos em assinaturas e vendas avulsas.

= 2.0.0 - 05/03/2015 =
- Nova versão do plugin, com suporte a nova API, aceitando assinaturas e vendas avulsas.

== License ==

Vindi WooCommerce Assinaturas is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

Vindi WooCommerce Assinaturas is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with Vindi WooCommerce Assinaturas. If not, see http://www.gnu.org/licenses/.
