# CeneoScraper
https://www.ceneo.pl/84514582#tab=click
## Ceneo scraping algorithm 
1. Analysis of the structure of the webpage
2. Sending http request to access first page with opinions 
3. Checking  the code of https responce
4. Parse the html code of the first page with opinions 
5. Extract required data from parsed code
6. If there are more pages, move to the next page and repeat steps 2-6 for it
7. Save extracted data

## Analysis of the structure of the webpage
|Component|Selector|Variable|
|---------|--------|--------|
|opinion ID |#opinion-id | |
|author |.author | |
|reccommendation |.recommendation | |
|number of stars |.stars .rating | |
|content of opinion |.opinion-content | |
|list of advantages |.advantages li | |
|list of disadvantages |.disadvantages li | |
|for how many helpful |.helpful-count | |
|for how many unhelpful |.unhelpful-count | |
|publishing date |.publish-date | |
|purchase date |.purchase-date | |
