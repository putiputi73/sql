# sql
/*
  @author: Bonface Mogiso
  Problem Description:
    Create your own store! Your store should sell one type of things, like clothing or bikes, whatever you want your store to specialize in. 
    You should have a table for all the items in your store, and at least 5 columns for the kind of data you think you'd need to store.
    You should sell at least 15 items, and use select statements to order your items by price and show at least one statistic about the items.
*/
CREATE TABLE library_store (id INTEGER PRIMARY KEY, name TEXT, price INTEGER, aisle INTEGER, discount INTEGER );

INSERT INTO library_store VALUES (0, "chemistry book", 10, 1, 0);
INSERT INTO library_store VALUES (1, "maths book", 100, 1, 0);
INSERT INTO library_store VALUES (2, "biology book", 10, 2, 0);
INSERT INTO library_store VALUES (3, "geography book", 90, 2, 0);
INSERT INTO library_store VALUES (4, "home science", 10, 3, 0);
INSERT INTO library_store VALUES (5, "english book", 85, 3, 0);
INSERT INTO library_store VALUES (6, "kiswahili book", 50, 3, 0);
INSERT INTO library_store VALUES (7, "french book", 15, 4, 0);

INSERT INTO library_store VALUES (8, "chinese book", 30, 4, 0);
INSERT INTO library_store VALUES (9, "CRE book", 15, 5, 0);
INSERT INTO library_store VALUES (10, "Quran book", 150, 5, 0);
INSERT INTO library_store VALUES (11, "Excel fundamental", 20, 2, 0);
INSERT INTO library_store VALUES (12, "Business book", 20, 2, 0);
INSERT INTO library_store VALUES (13, "agriculture book", 50, 2, 0);
INSERT INTO library_store VALUES (14, "physics", 60, 2, 0);
INSERT INTO library_store VALUES (15, "course manual", 110, 2, 0);


SELECT * FROM library_store ORDER BY price;
SELECT aisle, MAX(price) from library_store GROUP BY aisle;
