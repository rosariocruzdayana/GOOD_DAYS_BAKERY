# GOOD_DAYS_BAKERY

CREATE TABLE good_days_bakery (id INTEGER PRIMARY KEY, cake TEXT, price INTEGER, baked_daily INTEGER, closing_sale INTEGER);

INSERT INTO good_days_bakery VALUES (1, "vanilla" 12, 15, 8);
INSERT INTO good_days_bakery VALUES (2, "white" 10, 5, 7);
INSERT INTO good_days_bakery VALUES (3, "chocolate" 12, 15, 10);
INSERT INTO good_days_bakery VALUES (4, "almond" 15, 5, 12);
INSERT INTO good_days_bakery VALUES (5, "cherry" 12, 5, 8);
INSERT INTO good_days_bakery VALUES (6, "lemon" 15, 10, 10);
INSERT INTO good_days_bakery VALUES (7, "rasberry" 18, 6, 15);
INSERT INTO good_days_bakery VALUES (8, "strawberry" 15, 8, 12);
INSERT INTO good_days_bakery VALUES (9, "blueberry" 15, 5, 12);
INSERT INTO good_days_bakery VALUES (10, "brandy" 20, 5, 18);
INSERT INTO good_days_bakery VALUES (11, "banana" 10, 12, 8);
INSERT INTO good_days_bakery VALUES (12, "carrot" 12, 6, 10);
INSERT INTO good_days_bakery VALUES (13, "red_velvet" 15, 10, 12);
INSERT INTO good_days_bakery VALUES (14, "pumkin" 10, 4, 8);
INSERT INTO good_days_bakery VALUES (15, "lavendar" 20, 8, 18);

SELECT * FROM good_days_bakery ORDER BY price 

/* How much cake is baked daily? */
INSERT SUM(baked_daily) FROM good_days_bakery;

/* What is the highest discounted cake? */
SELECT MAX(closing_sale) as most_discounted_cake FROM good_days_bakery;

/* What is the average cake baked at good_days_bakery? */
SELECT AVG(cake) FROM good_days_bakery;

