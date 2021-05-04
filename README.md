# Teste desenvolvedor Backend Rails.

Utilizando o framework Ruby on Rails, construa uma API onde o usuário deverá se autenticar para ter acesso aos demais endpoints da aplicação.

A aplicação consiste em um sistema de controle de denúncias onde os usuários cadastrados irão poder manipular essas denúncias.

O usuário deverá ter ao menos os atributos nome e e-mail.
 
A denúncia deverá ter ao menos os atributos descrição, status, latitude, longitude, usuario que criou a denuncia, medida adotada.

Caso seja necessário, fica a seu critério criar outros atributos ou modelos;

Endpoints:

O sistema deverá contar com o seguintes endpoints:

Público: 
- Endpoint para cadastro de usuário;
- Endpoint para login;
- Endpoint para recuperar senha;

Requer Autenticação:
- Editar apenas os dados do usuário logado;
- Atualizar a senha apenas do usuário logado;


- Listar todas as denúncias cadastradas, com suporte a paginação;
- Criar/Editar uma denúncia com os campos descrição, status, latitude, longitude, usuário que criou a denúncia; 
- Adicionar a medida adotada em uma denúncia e alterar o status;


## Considerações:

- Deverá utilizar a versão 2.7.3 do Ruby;
- Deverá utilizar o PostgreSQL
- Poderá utilizar o Devise e JWT para autenticação;

## Diferenciais
Os seguintes items serão considerados um diferencial:
- Lista das denúncias com suporte a busca pelo descrição;
- Utilização de Docker para rodar a aplicação localmente;
- Deploy da aplicação no Heroku;
- Implementar a validação da latitude e longitude armazenando no banco de dados as informações de endereço retornadas pela API Externa
  - O serviço de denúncia receberá a geolocalizacão a partir do request e deverá buscar os dados de endereço no seguinte serviço https://developer.mapquest.com/documentation/geocoding-api/;
  - Para saber como utilizar o referido serviço de geolocalização verifique https://developer.mapquest.com/documentation/ e https://developer.mapquest.com/documentation/geocoding-api/;
  - A API REST deverá retornar um erro caso o endereço não seja encontrado no serviço de geolocalização;

# Envio do teste

Ao finalizar, deverá ser enviado o link do repositório e do sistema em produção, no caso de ter feito o deploy, pelo seguinte formulário:
https://docs.google.com/forms/d/e/1FAIpQLSfRNR_ByyYpi1yJ5h6t6qoSCfE1dHCea5xrv3RvbpZMc3bUjw/viewform

# Avaliação

Irá ser avaliado: 
- Seu conhecimento técnico e criatividade;
- Sua habilidade para resolver problemas de forma simples e eficiente;
- Boas práticas de código.

# Design

Não haverá design, apenas os endpoints;

# Dúvidas

Caso tenha alguma dúvida, poderá enviar um email para alexandre@rogalabs.com e rafael@rogalabs.com.
