# CREATE TABLE ... Example (Slide 27)

---

## 1.
Q: Create the `Product_Offers` table in your own environment

A: 
```
CREATE TABLE "sequel-mart-schema"."Product_Offers" (
	offer_id INT NOT NULL GENERATED BY DEFAULT AS IDENTITY PRIMARY KEY,
	offer_name VARCHAR(50) NOT NULL,
	product_id INT NOT NULL DEFAULT 0,
	offer_discount_percentage NUMERIC(4,2),
	offer_start_date DATE,
	offer_end_date DATE
);
```