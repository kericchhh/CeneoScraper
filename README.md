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
|opinion |div.js_product-review |opninon |
|opinion ID |[data-entry-id] |opinion_id |
|author |user-post__author-name |author |
|reccommendation |span.user-post__author-recomendation > em |recommendation |
|number of stars |span.user-post__score-count |stars |
|content of opinion |div.user-post__text |content |
|list of advantages |div.review-feature__item--positive|pros |
|list of disadvantages |div.review-feature__item--negative |cons |
|for how many helpful |button.vote-yes[data-total-vote] |vote_yes |
|for how many unhelpful |button.vote-no[data-total-vote] |vote_no |
|publishing date |spam.user-post__published > time:nth-child(1)[datetime] |published |
|purchase date |spam.user-post__published > time:nth-child(2)[datetime] |purchased |
