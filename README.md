![alt text align:center](https://www.vindi.com.br/image/vindi-logo-transparente.png "Vindi")

# Vindi - WooCommerce

[![Última Versão no WordPress][ico-version]][link-version]
[![Licença do Software][ico-license]](license.txt)
[![Avaliação do Plugin][ico-rates]][link-rates]
[![Downloads no Total][ico-downloads]][link-downloads]

## Descrição
O **Vindi WooCommerce** oferece uma solução simples para pagamentos únicos e assinaturas com cartão de crédito e boleto utilizando o [WooCommerce](https://wordpress.org/plugins/woocommerce/). Basta ter [uma conta habilitada na Vindi](https://app.vindi.com.br/prospects/new), para começar a cobrar seus clientes.

>Veja também nosso plugin [Vindi WooCommerce Subscriptions](http://www.github.com/vindi/vindi-woocommerce-subscriptions) que oferece uma gestão mais completa e leia [nosso artigo](http://atendimento.vindi.com.br/hc/pt-br/articles/217612217) com um comparativo de recursos entre os dois plugins.

A [Vindi](http://www.vindi.com.br/) é líder em cobrança recorrente no Brasil. Com centenas de clientes usando soluções como pagamento online, soluções de notas fiscais integradas, emissão de boletos por email e PDF, integrações com ERPs e diversos relatórios, a Vindi possibilita um sistema online completo para negócios de venda recorrente. Além disso, empresas podem usar o gateway de pagamento integrado ao billing recorrente ou para faturas avulsas.

## Requisitos
- PHP versão **5.5.19** ou superior.
- Um site com o WordPress instalado.
- Plugin [WooCommerce](https://wordpress.org/plugins/woocommerce/) instalado e habilitado.
- Plugin [WooCommerce Extra Checkout Fields for Brazil](https://wordpress.org/extend/plugins/woocommerce-extra-checkout-fields-for-brazil/) instalado e habilitado.
- Certificado Digital.
- Conta ativa na [Vindi](https://www.vindi.com.br "Vindi").

## Instalação
1. Envie os arquivos do plugin para a pasta `wp-content/plugins`, ou utilize o instalador de plugins do WordPress.
1. Ative o plugin.

## Configuração
1. Configure o plugin na página de administração do WordPress em:
    1. *WooCommerce -> Configurações -> Finalizar Compra -> Vindi - Cartão de Crédito* e
    1. *WooCommerce -> Configurações -> Finalizar Compra -> Vindi - Boleto Bancário*.
1. Em *WooCommerce -> Campos do Checkout*, ative Tipo de Pessoa Física e Jurídica, RG e Inscrição estadual.
1. Em *WooCommerce -> Configurações -> Produtos -> Inventário*, coloque um zero na opção "Manter estoque (minutos)".

>Para mais detalhes sobre a instalação de plugins no WordPress leia o tutorial [WordPress - Gerenciando Plugins](http://codex.wordpress.org/pt-br:Gerenciando_Plugins#Instalando_Plugins).

## Dúvidas
Para suporte ou dúvidas relacionadas ao Plugin você pode seguir pelos canais:
- [Github](https://github.com/vindi/vindi-woocommerce/issues)
- [Fórum do Plugin](https://wordpress.org/plugins/vindi-woocommerce-assinaturas) (apenas em inglês)

Caso necessite de informações sobre a plataforma ou API por favor siga através do canal
- [Atendimento Vindi](http://atendimento.vindi.com.br/hc/pt-br)[Atendimento Vindi](http://atendimento.vindi.com.br/hc/pt-br)

## Contribuindo
Por favor, leia o arquivo [CONTRIBUTING.md](CONTRIBUTING.md).

Caso tenha alguma sugestão ou bug para reportar por favor nos comunique através das [issues](./issues).

## Changelog
Todas as informações sobre cada release pode ser  [CHANGELOG.md](CHANGELOG.md).

## Créditos
- [Vindi](https://github.com/vindi)
- [Todos os Contribuidores](https://github.com/vindi/vindi-woocommerce/contributors)

## Licença
GNU GPLv3. Por favor, veja o [Arquivo de Licença](LICENSE) para mais informações.

[ico-version]: https://img.shields.io/wordpress/plugin/v/vindi-assinaturas-e-cobranca-recorrente.svg?style=flat-square
[ico-license]: https://img.shields.io/badge/license-GPLv3-brightgreen.svg?style=flat-square
[ico-rates]: https://img.shields.io/wordpress/plugin/r/vindi-assinaturas-e-cobranca-recorrente.svg?style=flat-square
[ico-downloads]: https://img.shields.io/wordpress/plugin/dt/vindi-assinaturas-e-cobranca-recorrente.svg?style=flat-square

[link-version]: https://wordpress.org/plugins/vindi-assinaturas-e-cobranca-recorrente/
[link-rates]: https://wordpress.org/support/view/plugin-reviews/vindi-assinaturas-e-cobranca-recorrente
[link-downloads]: https://wordpress.org/plugins/vindi-assinaturas-e-cobranca-recorrente/stats/
