# CeneoScraperCS12

https://www.ceneo.pl/136115744;48082-0v.htm#tab=reviews

## Algorithm for exctracting opinions about single product from Ceneo.pl

1. Send the request for accessing first webpage opinions about product
2. If response is OK, parse HTML content into DOM structure
3. Extract opinions and their components from DOM structure 
4. Assign opinions with their components to complex data structures
5. If there are more pages with opinions, repeat steps 1-5
6. Save data structures with opinions into database

## Structure of single opinion in Ceneo.pl
|Component|Variable|Selesctor|
|---------|--------|---------|
|opinion|opinion||
|opinion ID|opinion_id||
|opinion’s author|author||
|author’s recommendation|recomend||
|score expressed in number of stars|stars||
|opinion’s content|content||
|list of product advantages|pros||
|list of product disadvantages|cons||
|how many users think that opinion was helpful|up_votes||
|how many users think that opinion was unhelpful|down_votes||
|publishing date|published||
|purchase date|purchased||
