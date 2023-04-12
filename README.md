# CeneoScraper
## Selektory składowych opinii w Ceneo.pl

| składowa | nazwa | sektor |
| --- | --- | --- |
| identyfikator opinii | opinion\_id | [data-entry-id] |
| autora | author | span.user.post\_\_author-name |
| rekomendację | recommendation | span.user-post\_\_author-recomendation\>em |
| liczbę gwiazdek | rating | user-post\_\_score-count |
| czy opinia jest potwierdzona zakupem | verified | div.review-pz |
| data wystawienia opinii | post\_data | span.user-post\_\_published\>time:nth-child(1)[datatime] |
| data zakupu produktu | purchase\_date | span.user-post\_\_published\>time:nth-child(2)[[datatime] |
| ile osób uznało opinię za przydatną | vote\_up | buton.vote-yes[data-total-vote]buton.vote-yes\>span |
| ile osób uznało opinię za nieprzydatną | vote\_down | buton.vote-no[data-total-vote]buton.vote-no\>span |
| treść opinii | content | div.user-post\_\_text |
| listę wad | pons | div.review-feature\_\_title—negatives~div.review-feature\_\_item |
| listę zalet | pros | div.review-feature\_\_title—positives~div.review-feature\_\_item |

## Wykorzystane bibloteki
- BeautifulSoup4
- Requirements