# Módulo MercadoPago para WHMCS

Este módulo integra o gateway de pagamento MercadoPago ao WHMCS, permitindo que você ofereça opções de pagamento contínuas para seus clientes.

## Funcionalidades
- Suporte a pagamentos via MercadoPago em diversos países, incluindo Argentina, Brasil, Colômbia, México e Venezuela.
- Estilos de botão de pagamento personalizáveis.
- Taxas configuráveis (percentual e taxa fixa auxiliar).
- Múltiplas opções de janela para exibir o processo de pagamento.
- Suporte a pagamentos recorrentes.
- Abertura automática da janela de pagamento.

## Requisitos
- WHMCS (última versão recomendada).
- PHP 7.4 ou superior.
- Credenciais da API do MercadoPago (`client_id` e `client_secret`).

## Instalação
1. Baixe o módulo e extraia os arquivos.
2. Envie os arquivos para o diretório `modules/gateways/` da sua instalação do WHMCS.
3. Envie o arquivo de callback para o diretório `modules/gateways/callback/`.
4. Navegue até `Configurações > Pagamentos > Gateways de Pagamento` na área administrativa do WHMCS.
5. Selecione "MercadoPago" da lista de gateways disponíveis.
6. Configure as configurações do módulo usando suas credenciais do MercadoPago.

## Configuração
### Configurações Necessárias
- **Client ID**: Pode ser obtido no portal do desenvolvedor do MercadoPago para o seu país.
- **Client Secret**: Pode ser obtido no portal do desenvolvedor do MercadoPago para o seu país.
- **Modo de Janela de Pagamento**: Escolha o modo desejado para exibir o processo de pagamento:
  - Mesma Janela
  - Nova Janela
  - Lightbox
  - Pop-up

### Configurações Opcionais
- **Abrir Janela de Pagamento Automaticamente**: Ative esta opção para abrir a janela de pagamento automaticamente ao acessar a fatura.
- **Texto do Botão de Pagamento**: Personalize o texto que aparece no botão de pagamento.
- **Taxa Percentual**: Defina uma taxa percentual adicional a ser adicionada ao valor da fatura.
- **Taxa Fixa**: Defina uma taxa fixa adicional a ser adicionada ao valor da fatura.
- **Classe CSS do Botão de Pagamento**: Personalize a classe CSS para o botão de pagamento.
- **CSS Personalizado**: Adicione CSS personalizado para mais estilização.

## Notas de Uso
- A URL de notificação para o MercadoPago deve ser configurada na sua conta do MercadoPago. Use o seguinte formato:
  - `<WHMCS_URL>/modules/gateways/callback/mercadopago.php`
- Substitua `<WHMCS_URL>` pela URL do sistema WHMCS.

## Informações Importantes
- Este módulo é destinado apenas para uso pessoal. **Revenda é estritamente proibida**.
- Desenvolvido por Lucas Farias, LF Developer. Visite [lf.dev.br](http://lf.dev.br) ou entre em contato pelo e-mail [lucas@lf.dev.br](mailto:lucas@lf.dev.br) para suporte.

## Personalização
O botão de pagamento e os estilos adicionais podem ser personalizados nas configurações do módulo no WHMCS. Você pode definir seus próprios estilos CSS para combinar com o tema do seu site.

## Solução de Problemas
- **Credenciais Inválidas**: Certifique-se de que o `client_id` e o `client_secret` estão corretos.
- **Problemas de Callback**: Verifique se a URL de callback está corretamente configurada nas configurações da sua conta MercadoPago.
- **Janela de Pagamento Não Abre**: Verifique a opção "Abrir Janela de Pagamento Automaticamente" nas configurações do módulo.

## Licença
Este módulo é licenciado apenas para uso pessoal. Redistribuição ou revenda são estritamente proibidas.

## Autor
- Lucas Farias, LF Developer
- Website: [lf.dev.br](http://lf.dev.br)
- Email: [lucas@lf.dev.br](mailto:lucas@lf.dev.br)

