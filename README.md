🛒 API de Pedidos - Microsserviço
📋 Descrição
Microsserviço responsável pelo gerenciamento de pedidos em um sistema de e-commerce. Realiza a criação e consulta de pedidos, integrando-se com o serviço de produtos para validação e cálculo de preços.

🚀 Funcionalidades
Criação de Pedidos - Registro de novos pedidos com múltiplos itens

Consulta de Pedidos - Listagem e busca de pedidos existentes

Integração em Tempo Real - Comunicação com serviço de produtos via OpenFeign

Validação de Estoque - Verificação automática de disponibilidade

Cálculo Automático - Soma de valores baseada nos preços dos produtos

Gestão de Status - Controle do fluxo do pedido (PENDENTE, PROCESSADO, etc.)

🏗️ Arquitetura
Java 17 + Spring Boot 3.2.0

Spring Cloud OpenFeign - Comunicação entre microsserviços

Spring Data JPA - Persistência de dados

H2 Database - Banco em memória

REST API - Comunicação HTTP/JSON

📊 Modelo de Dados
java
class Pedido {
    Long id;
    String cliente;
    LocalDateTime dataPedido;
    String status;
    List<ItemPedido> itens;
}

class ItemPedido {
    Long id;
    Long produtoId;
    Integer quantidade;
    Double precoUnitario;
}
🌐 Endpoints Principais
📋 Operações de Pedidos
Método	Endpoint	Descrição
GET	/api/pedidos	Lista todos os pedidos
GET	/api/pedidos/{id}	Busca pedido por ID
POST	/api/pedidos	Cria novo pedido
🔄 Integração com Produtos
Comunicação transparente com o microsserviço de produtos para:

✅ Validação de existência do produto

✅ Verificação de estoque disponível

✅ Obtenção de preços atualizados

✅ Cálculo automático de totais
