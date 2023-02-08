# Dropshipping-Store-Demo
I created a dropshipping store webpage for a class project.

How it works: 
1.) A bash script downloads 50 store webpages (25 from each Target and RiteAid) from url files every 6 hours. The script then converts those html webpages to xhtml files using tagsoup and passes them into a python program.
2.) A python program scrapes product data (name, price, and description) from the .xhtml files using the DOM API. The program then inserts/updates this information in a MYSQL database.
3.) PHP scripts retrieve product data from the database and display it on a dropshipping style webpage. After a customer selects a product from one store, they will be taken to a second page that presents them with a side-by-side comparison of the item they chose and a similar item from the other store, with the cheaper product highlighted. After selecting an item, the customer is taken to a final checkout page that takes their information and stores it in a database.

Note:
If the store webpage templates have changed, then the python web scraper might not work. For example purposes, I have downloaded 25 product webpages from each store that can be used with the web scraper.

As this is a demo dropshipping webpage for a class project, the php scripts do not have any security features built in. 
