# Feira Livre Virtual

## Descrição do Projeto
O Sistema Feira Livre é uma aplicação em Haskell desenvolvida para simular uma feira comunitária virtual, onde produtores locais podem cadastrar e divulgar seus produtos, e consumidores podem consultar os itens disponíveis e realizar pedidos. O sistema é orientado a dados, com menus interativos e persistência em arquivos, garantindo que todas as informações cadastradas sejam mantidas entre execuções.

## Perfis de Usuário

### Perfil Produtor
 
Produtor é o responsável por ofertar produtos na feira. Cada produtor tem um ID, nome e meio de contato.


#### Funcionalidades do Produtor:

- Cadastrar-se no sistema

- Cadastrar novos produtos (nome, preço, quantidade)

- Visualizar seus próprios produtos cadastrados

- Atualizar ou remover produtos cadastrados

### Perfil Consumidor
 
Consumidor é quem visita a feira para visualizar produtos e realizar pedidos. 
- Cada consumidor tem um ID, nome e endereço.
- Funcionalidades do Consumidor:

- Cadastrar-se no sistema

- Consultar produtos disponíveis na feira

	- Buscar por nome do produto
  
	- Filtrar por produtor
  
	- Filtrar por faixa de preço
  
- Realizar pedidos (selecionar produtos e quantidades)
- Visualizar pedidos feitos anteriormente


## Entidades

### Entidade Produtor
Atributos:
- produtorID --> Type ProdutorID --> int
- nomeProdutor --> String
- contatoProdutor --> String

### Entidade Produto
Atributos:
- produtoID --> type ProdutoID --> int
- nomeProduto --> String
- preco --> Float
- quantidade --> int
- produtorRef --> Type ProdutorID --> int

### Entidade Consumidor
Atributos:
- consumidorID --> Type ConsumidorID
- nomeConsumidor --> String
- endereco --> String

### Entidade Pedido
Atributos:
- pedidoID --> int
- consumidorREF --> Type ConsumidorID --> int
- produtosPedido --> Tupla(Type ProdutoID --> int, int)

## Funcionalidades Principais
- Cadastro e gerenciamento de produtores com nome e dados de contato.

- Cadastro de produtos agrícolas (frutas, legumes, laticínios, etc.) vinculados aos respectivos produtores.

- Registro de consumidores, com informações básicas como nome e endereço.

- Realização de pedidos, onde consumidores selecionam produtos e quantidades desejadas.

- Consulta de pedidos por consumidor, por produto ou por produtor.

- Busca de produtos por nome, produtor ou faixa de preço.

- Persistência de dados em arquivos .txt, garantindo que o sistema mantenha o estado das entidades entre sessões.

- Menus interativos por módulo (produtores, produtos, consumidores, pedidos) para facilitar a navegação e a organização do sistema.




