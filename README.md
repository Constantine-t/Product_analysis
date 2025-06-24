# Marketplace Data Analysis

[Читать на русском](#аналитика-для-бразильского-маркетплейса)

## Analytics for a New Brazilian Goods Marketplace 

### Project Overview

The subject of the analysis is a Brazilian marketplace startup. A popular dataset for training.
**Goal:**
Identify growth barriers, improve retention and revenue, without negatively impacting the customer experience.

**Project Tasks**
1. Evaluate monthly order retention using cohort analysis.
2. Check if there is product/market fit for the marketplace.
3. Define 5 key metrics to maximize company profit.
4. Prioritize hypotheses using the ICE framework and select the most promising one.
5. Define the metrics that should be influenced by the chosen hypothesis.
6. Prepare conclusions and recommendations for the product manager.

### Dataset Description
Three tables are used in this project:

#### 1. `olist_customers_dataset.csv`
**Columns:**
- `customer_id` — user ID (per order)
- `customer_unique_id` — postal code
- `customer_city` — delivery city
- `customer_state` — delivery state
#### 2. `olist_orders_dataset.csv`
**Columns:**
- `order_id` — unique order ID (receipt number)
- `customer_id` — user ID (per order)
- `order_status` — order status
- `order_purchase_timestamp` — order creation time
- `order_approved_at` — payment approval time
- `order_delivered_carrier_date` — time the order was handed to logistics
- `order_delivered_customer_date` — delivery time to customer
- `order_estimated_delivery_date` — promised delivery date
**Order status values:**
- `created` — created
- `approved` — approved
- `invoiced` — invoice issued
- `processing` — being processed
- `shipped` — shipped
- `delivered` — delivered
- `unavailable` — canceled (item unavailable)
- `canceled` — canceled
#### 3. olist_order_items_dataset.csv
**Columns:**
- `order_id` — order number
- `order_item_id` — item ID within the order
- `product_id` — product ID
- `seller_id` — seller ID
- `shipping_limit_date` — latest shipping date by seller
- `price` — price per unit
- `freight_value` — delivery cost

**Example:**
Joining tables by order_id gives a complete view of any order.

**Example Analysis**
>This project covers cohort analysis, product/market fit assessment, identification of key business metrics, and data-driven recommendations.

How to Use
1. Download the dataset files (place them in the project root).
2. Open the notebook or analysis scripts.
3. Run the analysis blocks — use Pandas, SQL, or your favorite BI tools.

Useful Links
[Pandas Documentation](https://pandas.pydata.org/docs/)
[ICE Framework Overview](https://growthtools.com/ice-score-prioritization/)
[Cohort Analysis Example](https://towardsdatascience.com/a-cohort-analysis-in-python-3d13ad1e67b8)

---

# Аналитика для бразильского маркетплейса

## Описание проекта

Объект анализа — стартап бразильского маркетплейса. Используется популярный учебный датасет.  
**Цель:**  
Выявить барьеры роста, повысить удержание и выручку, не ухудшая клиентский опыт.

**Задачи проекта**
1. Оценить месячное удержание заказов с помощью когортного анализа.
2. Проверить, есть ли product/market fit у маркетплейса.
3. Определить 5 ключевых метрик для максимизации прибыли компании.
4. Приоритизировать гипотезы по ICE и выбрать самую перспективную.
5. Сформулировать метрики, на которые влияет выбранная гипотеза.
6. Подготовить выводы и рекомендации для продакта.

### Описание датасета

В проекте используются три таблицы:

#### 1. `olist_customers_dataset.csv`
**Поля:**
- `customer_id` — идентификатор пользователя (по заказу)
- `customer_unique_id` — уникальный идентификатор пользователя (аналог паспорта)
- `customer_city` — город доставки
- `customer_state` — штат доставки

#### 2. `olist_orders_dataset.csv`
**Поля:**
- `order_id` — уникальный идентификатор заказа (чек)
- `customer_id` — идентификатор пользователя (по заказу)
- `order_status` — статус заказа
- `order_purchase_timestamp` — время создания заказа
- `order_approved_at` — время подтверждения оплаты
- `order_delivered_carrier_date` — передан в логистику
- `order_delivered_customer_date` — доставлен покупателю
- `order_estimated_delivery_date` — обещанная дата доставки

**Статусы заказа:**
- `created` — создан  
- `approved` — подтверждён  
- `invoiced` — выставлен счёт  
- `processing` — в обработке  
- `shipped` — отправлен  
- `delivered` — доставлен  
- `unavailable` — отменён (товар недоступен)  
- `canceled` — отменён

#### 3. `olist_order_items_dataset.csv`
**Поля:**
- `order_id` — номер заказа
- `order_item_id` — номер товара в заказе
- `product_id` — идентификатор товара
- `seller_id` — идентификатор продавца
- `shipping_limit_date` — крайний срок отгрузки
- `price` — цена за единицу товара
- `freight_value` — стоимость доставки

**Пример:**  
Объединение таблиц по order_id даёт полную информацию по заказу.

**Пример анализа**
> В проекте проводится когортный анализ, оценка product/market fit, выявление ключевых бизнес-метрик и подготовка рекомендаций на основе данных.

**Как использовать**
1. Скачайте файлы датасета (разместите их в корне проекта).
2. Откройте ноутбук или скрипты с анализом.
3. Запустите блоки анализа — используйте Pandas, SQL или любимые BI-инструменты.

**Полезные ссылки**  
[Документация Pandas](https://pandas.pydata.org/docs/)  
[Обзор ICE-фреймворка](https://growthtools.com/ice-score-prioritization/)  
[Пример когортного анализа](https://towardsdatascience.com/a-cohort-analysis-in-python-3d13ad1e67b8)
