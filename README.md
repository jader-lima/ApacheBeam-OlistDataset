# ApacheBeam-OlistDataset
Combinando todos os datasets de vendas num arquivo de saida, utilizando Apache Beam para tratamento dos dados e junções.

Dados:
Os dados estão disponíveis em https://www.kaggle.com/olistbr/brazilian-ecommerce?select=olist_customers_dataset.csv

Criação do ambiente local, é possivel simplesmente instalar o apache beam no seu ambiente padrão python, com pip install apache-beam
Com o python 3.7 instalado 
pip install virtualenv
mkdir beam_python37
virtualenv.exe .\beam_python37\ 
cd beam_python37\Scripts\activate
pip install apache-beam

Rodar o ETL
python etl.py --input_itens  data/olist_order_items_dataset.csv --input_sellers data/olist_sellers_dataset.csv --input_products data/olist_products_dataset.csv --input_order data/olist_orders_dataset.csv --input_reviews data/olist_order_reviews_dataset.csv --input_payments data/olist_order_payments_dataset.csv --input_customer data/olist_customers_dataset.csv --output output/saida.txt
