# **Projeto: E-commerce Olist**
<sub>Projeto desenvolvida por: **Natália Oliveira**</sub>

## Sobre o projeto:
O objetivo deste projeto é executar uma série de análises nos dados da plataforma brasileira de comércio eletrônico Olist. Essas análises serão divididas em etapas para uma melhor proposta de organização e análise.

## Sobre os dados:
Os dados disponíveis são de comércio eletrônico brasileiro feitos na loja Olist, contendo informações de 100 mil pedidos de 2016 a 2018, incluindo status do pedido, preço, pagamento, desempenho de frete, localização do cliente, atributos do produto e revisões escritas pelos clientes. Os dados são reais, mas foram anonimizados e as referências às empresas e parceiros foram substituídas por nomes de casas da série Game of Thrones. Também há um conjunto de dados de geolocalização que relaciona os códigos postais brasileiros às coordenadas LAT/LNG.

### Fonte dos Dados:

Brazilian E-Commerce Public Dataset by Olist: https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce/code?select=olist_geolocation_dataset.csv

### Esquema dos dados:
![](https://i.imgur.com/HRhd2Y0.png)

### Metadados:
**olist_orders_dataset.csv**
* **order_id:** identificador único do pedido;
* **customer_id:** identificador único do cliente;
* **order_status:** status do pedido;
* **order_purchase_timestamp:** data e hora do pedido;
* **order_approved_at:** data e hora da aprovação do pagamento;
* **order_delivered_carrier_date:** data e hora de quando o pedido foi entregue ao parceiro logístico;
* **order_delivered_customer_date:** data e hora real da entregua do pedido ao cliente;
* **order_estimated_delivery_date:** data estimada de entrega informada ao cliente.

**olist_customers_dataset.csv**
* **custumer_id:** chave para o conjunto de dados de pedidos. Cada pedido tem um customer_id único.
* **customer_unique_id:** identificador exclusivo de um cliente.
* **customer_zip_code_prefix:** primeiros cinco dígitos do CEP do cliente
* **customer_city:** nome da cidade do cliente
* **customer_state:** estado do cliente

**olist_geolocation_dataset.csv**
* **geolocation_zip_code_prefix:** primeiros 5 dígitos do CEP
* **geolocation_lat:** latitude
* **geolocation_lng:** longitude
* **geolocation_city:** nome da vidade
* **geolocation_state:** estado

**olist_order_items_dataset.csv**<
* **order_id:** identificador exclusivo do pedido
* **order_item_id:** número sequencial que identifica o número de itens incluídos na mesma ordem.
* **product_id:** identificador exclusivo do produto
* **seller_id:** identificador exclusivo do vendedor
* **shipping_limit_date:** Mostra a data limite de envio do vendedor para lidar com o pedido para o parceiro logístico.
* **price:** preço do item
* **freight_value:** item freight value item (se um pedido tiver mais de um item, o valor do frete será dividido entre itens)

**olist_order_payments_dataset.csv**<br>
**olist_order_reviews_dataset.csv**<br>
**olist_products_dataset.csv**<br>
**olist_sellers_dataset.csv**<br>
**product_category_name_translation.csv**<br>

---

## **Análise 01:  Análise de Comportamento de Compra de Consumidores do E-commerce Brasileiro**
**Objetivo:**<br>
A finalidade desta análise é examinar os dados dos consumidores do E-commerce brasileiro Olist, com o intuito de identificar os padrões de comportamento de compra e responder a diversas questões relacionadas ao negócio. Para alcançar esse objetivo, serão utilizadas diversas técnicas de análise de dados, incluindo a segmentação de clientes e análise de associação.

**Perguntas que serão respondidas:**
* Quais são os produtos mais vendidos?
* Quais são os produtos que são geralmente comprados juntos?
* Qual é o valor médio de cada compra?
* Quais são os clientes mais valiosos em termos de valor de vida útil (LTV) e padrões de compra?
* Qual é a taxa de recompra dos clientes?
* Quais são as preferências de compra dos clientes?
* Como as vendas variam ao longo do tempo?
* Como as vendas variam de acordo com a localização geográfica?
* Como o preço afeta o comportamento de compra dos clientes?
* Quais são as tendências de compra ao longo do tempo?

---
