# assignment-demo

1.How you loaded and separated featured vs non featured products -
I have created smart collection for featured and given condition where product tag contains featured! Before that I have added featured tag on those 15 products which needs to be separated! After that added condition in product grid to show featured collections product at first and then non-featured products! (Later added script to hide featured products, not to look like duplicate products!)

Note - I have mentioned featured in those product name as well for understanding!

2.How infinite scroll was implemented -
Removed old pagination of shopify from below product grid and added infinite scrolling snippet which had script to infinite scroll the products within collection! It is adapted from one source found while searching!

3.How duplicate products were prevented -
Point out products by productId to check and avoid duplication! Added script to hide it appearing in other pages while scroll down!

4.How solution scales for large collections -
We can use it for large solutions as featured separation working by product tag! Duplicate products also take care by script so only pagination part needs to fix only to show 20 products per each page!

5.How filtering & sorting were handled while maintaining proper logic -
As mentioned in requirements that when filters/sort applied then normal Shopify behaviour applies, I have added condition (if) where user apply for filter and sort then it should enter normal products loop without featured logic! And for else part added featured logic so when there will be o sort or filter then it show featured products at top as required!

6.Any limitations of Liquid and how you solved them -
Yes, shopify pagination is limiting as it doesn't load all collection products at start! It loads as per we scrolls/moves to other pages and applies condition for each page separately!

Currently it doesn't show 20 products at start due to shopify pagination! It shows 15 featured products first and then due to other loop 20 other products including featured and non featured! So due to duplication removal script, it removes featured products from it but count remains same per scroll! So if any featured products skips but it will be count in that loop of 20 products!

Now if you see when we scrolls down on collection page, it will not load 20 products for each page! Rest is working fine!