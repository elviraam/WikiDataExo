# WikiDataExo

### Liste peinture de Monet
````
SELECT ?Claude_Monet ?Claude_MonetLabel WHERE {
  SERVICE wikibase:label { bd:serviceParam wikibase:language "[AUTO_LANGUAGE],en". }
  ?Claude_Monet wdt:P170 wd:Q296.
  
  ?Claude_Monet wdt:P31 wd:Q3305213.
}
LIMIT 100
````
````
SELECT ?Claude_Monet ?Claude_MonetLabel ?image WHERE {
  SERVICE wikibase:label { bd:serviceParam wikibase:language "[AUTO_LANGUAGE],en". }
  ?Claude_Monet wdt:P170 wd:Q296.
  
  ?Claude_Monet wdt:P31 wd:Q3305213.
  OPTIONAL { ?Claude_Monet wdt:P18 ?image. }
}
LIMIT 100
````
````
SELECT ?Claude_Monet ?Claude_MonetLabel ?collection ?collectionLabel WHERE {
  SERVICE wikibase:label { bd:serviceParam wikibase:language "[AUTO_LANGUAGE],en". }
  ?Claude_Monet wdt:P170 wd:Q296.
  ?Claude_Monet wdt:P31 wd:Q3305213.
  OPTIONAL { ?Claude_Monet wdt:P195 ?collection. }
}
LIMIT 100
````
