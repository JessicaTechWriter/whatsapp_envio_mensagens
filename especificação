openapi: 3.0.1
info:
  title: Disparador de Mensagens via Whatsapp
  description: API para disparar mensagens instantâneas aos clientes 
  version: 0.0.1
  termsOfService: https://mockapi.io
  contact:
    name: Suporte a Devs
    email: contato@example.com
    url: https://mockapi.io
  license:
    name: "Lincença: GPLv3"
    url: https://www.gnu.org/licenses/gpl-3.0.html
externalDocs:
  description: Documentação burocrática
  url: https://mockapi.io
servers:
- url: Content-type
  description: Disparo de mensagens via whatsapp
paths:
  /clientes/cadastro:
    get:
      summary: Buscar cadastro de clientes
      responses:
        200:
          description: Sucesso
          content:
            application/json:
              schema:
                $ref: "#/components/schemas/cliente"
  /alterar/produtos:           
    put:
      summary: Alterar produtos contratados
      requestBody:
        content:
          application/json:
            schema:
              type: object
              properties:
                descricao:
                  type: string
      responses:
        400:
          description: "Parâmetros Inválidos"
          content:
            application/json:
              schema:
                $ref: "#/components/schemas/cliente"
  /pesquisa/feedback:
    post:
      summary: Criar pesquisa de satisfação
      requestBody:
        content:
           application/json:
            schema:
              type: object
              properties:
                descricao:
                  type: string
      responses:
        401:
          description: Autenticação falhou
          content:
            application/json:
              schema:
                $ref: "#/components/schemas/cliente"
        500:
          description: Erro de servidor interno
          content:
            application/json:
              example: "Not Found"
security: 
- auth: []
components:
  schemas:
    cliente:
      type: object
      properties:
        id:
          type: integer
        descricao:
          type: string
    alterar:
      type: array
      items:
        $ref: "#/components/schemas/cliente"
  securitySchemes:
    auth:
      type: http
      scheme: bearer
      bearerFormat: JWT
