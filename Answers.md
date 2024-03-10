Que1. Explain the relationship between the "Product" and "Product_Category" entities from the above diagram.

ANS:The relationship between the "Product" and "Product_Category" entities is [ many-to-one ].
    This means that many products can belong to one product category. 
    In the "Product" table, the category_id field is a foreign key that references the id field in the "Product_Category" table.



Que2.How could you ensure that each product in the "Product" table has a valid category assigned to it?

ANS: To ensure that each product in the "Product" table has a valid category assigned to it, you can use a foreign key constraint. 
     This constraint will enforce that the category_id field in the "Product" table must correspond to an existing id in the "Product_Category" table.
     
     Ex: you can use with help of this sql query:
        ALTER TABLE Product
        ADD CONSTRAINT fk_product_category
        FOREIGN KEY (category_id)
        REFERENCES Product_Category(id);





    
