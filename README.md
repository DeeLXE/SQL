--Create a cafe order menu database

CREATE TABLE vietdeelight (id INTEGER, name TEXT, rating INTEGER, category TEXT, price TEXT);

INSERT INTO vietdeelight VALUES (1, "Bo bun", 5, "main", "£6.99");
INSERT INTO vietdeelight VALUES (2,"Ga bun", 4, "main", "£6.99");
INSERT INTO vietdeelight VALUES (3, "Pho", 4, "main", "£11.50");
INSERT INTO vietdeelight VALUES (4, "Pho Veggie", 5, "main", "£11.50");
INSERT INTO vietdeelight VALUES (5, "Pork Cha gio", 5, "starter", "£4.99");
INSERT INTO vietdeelight VALUES (6, "Veggie Cha Gio", 4, "starter", "£4.99");
INSERT INTO vietdeelight VALUES (7, "Spring rolls - Shrimp", 5, "starter", "£5.99");
INSERT INTO vietdeelight VALUES (8, "Spring rolls - Tofu", 5, "starter", "£5.99");
INSERT INTO vietdeelight VALUES (9, "Banh mi - Beef", 5, "main", "£6.99");
INSERT INTO vietdeelight VALUES (10, "Che chua", 3, "desert", "£4.99");
INSERT INTO vietdeelight VALUES (11, "VN Ice coffee", 5, "drink", "£6.99");
INSERT INTO vietdeelight VALUES (12, "Banh mi - Chicken", 4, "main", "£6.99");
INSERT INTO vietdeelight VALUES (13, "Banh bo", 2, "desert", "£4.99");
INSERT INTO vietdeelight VALUES (14, "VN Fried chicken", 5, "starter", "£4.99");
INSERT INTO vietdeelight VALUES (1, "Sinh to", 1, "drink", "£4.99");


--display the database ordered by price. 
SELECT * FROM vietdeelight
ORDER BY price DESC;

--what is the avg price of items in the main category?
SELECT * FROM vietdeelight
WHERE category="main";

--what are the most 5 popular items? 
SELECT name, price, rating
FROM vietdeelight
ORDER BY rating desc
LIMIT 5; 


