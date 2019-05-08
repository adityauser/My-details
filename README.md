# Machine Learning Engineer Task
If any questions come up while working on the task, please don’t hesitate to ask us!

## Prerequisites

We recommend you to use Python 3 for solving the tasks. To get your environment ready, run
```
$ pip install -r requirements.txt
```
## Classification

Product enrichment at real is the process of identifying a product's category, color and many more features of a product. In this task, you are provided with a text dataset `data.zip` containing a list of products defined by the following fields:
* `id`: A unique product identifier
* `name`: The title of the product, as displayed on our website
* `description`: The description of the product
* `price`: The price of the product
* `shop`: The shop from which you can buy this product
* `brand`: The product brand
* `labels`: The category labels that apply to this product

The labels are arranged in a tree-like structure of depth that you can load from `label_info.csv` (example: level 3 "Leder Caps" belongs to lv.2 "Caps" which belongs to lv.1 "Accessoires").

Your goal is to build a classification model for this dataset and identify what is a good metric for the problem. To get you started, you can find `draft.py` which will train and score a multi-output model for level 2 labels only.
In addition to your code, please also send us a document where you describe what you did, and especially why you did it :-)

## Ranking

At real we evaluate the performance of millions of products and want to show the most relevant products to our users. To dip your toe into our daily work, please assign each product in the `product_scoring.csv` a “score” which you would suggest we should sort by. Here is an explanation of the fields:
* `product_id`: The id of the product
* `category_id`: Identifier of the category of the product
* `clicks`: The number of times this product was clicked
* `impressions`: The number of times this product was shown to users
* `cpc`: The amount of money we get per click

In addition to providing us with a score per product, please also provide us the code that you used and explain the algorithm that you used to calculate this score (this is the most important part of this task). Also, explain current shortcomings and ideas for possible future improvements!

Please note that the score calculation in this task does not require you to think about any sales conversion rates.

