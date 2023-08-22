# Disparador de Mensagens via Whatsapp

## Informações gerais

Essa API possibilita o envio de mensagens via whatsapp para os clientes Citrus.  

As operações para o esta API corresponde a:

- Cadastro de clientes;
- Alterar produtos contratados;
- Pesquisas eNPS.

# Para quem é essa API?
Essa API é destinada para o público de negócios com o intuito de entrar em contato com os clientes por meio do aplicativo whatsapp. 

# Conhecimentos técnicos para usar essa API
* JSON
* Protocolo HTTP
* Especificação OpenAPI

# Tempo correspondente a integração dessa API
Tempo estimado para integração e uso dessa aplicação é de **aproximadamente 3 horas**, porém, depende do nível de conhecimento e senioridade da pessoa desenvolvedora. 

# Quais as necessidades que essa API atende?
Essa API proporciona: 

- Contato espontâneo e direto com o cliente;
- Interação mais próxima e ágil;
- Reduz a abertura de chamados.

# Endpoints

Observe abaixo as funcionalidades disponíveis para essa API.

|Ambiente| Endpoint|
|--------|---------|
|Desenvolvimento|http://api.dev.citrus.com.br/disparador-de-mensagens/v1|
|Produção|http://api.prd.citrus.com.br/disparador-de-mensagens/v1|
|Homologação|http://api.hml.citrus.com.br/disparador-de-mensagens/v1|

[GET]../disparos_de_mensagens
Dispara mensagens para os destinatários
Entrada
|Parâmtero| Tipo de Parâmetro| Tipo Dado|Obrigatório|Descrição|
|---------|------------------|----------|-----------|---------|
|x-citrus-apikey|header|string|sim|Chave da API para autorizar o consumo de uma aplicação requisitante|

[PUT]../alterar_produtos
Altera produtos cadastrados
Entrada
|Parâmtero| Tipo de Parâmetro| Tipo Dado|Obrigatório|Descrição|
|---------|------------------|----------|-----------|---------|
|x-citrus-apikey|header|string|sim|Chave da API para autorizar o consumo de uma aplicação requisitante|

[POST]../pesquisa_feedback
Dispara pesquisa de satisfação
Entrada
|Parâmtero| Tipo de Parâmetro| Tipo Dado|Obrigatório|Descrição|
|---------|------------------|----------|-----------|---------|
|x-citrus-apikey|header|string|sim|Chave da API para autorizar o consumo de uma aplicação requisitante|









