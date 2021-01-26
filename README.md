# WikiDataExo

## Liste peinture de Monet
````
SELECT ?Claude_Monet ?Claude_MonetLabel WHERE {
  SERVICE wikibase:label { bd:serviceParam wikibase:language "[AUTO_LANGUAGE],en". }
  ?Claude_Monet wdt:P170 wd:Q296.
  
  ?Claude_Monet wdt:P31 wd:Q3305213.
}
LIMIT 100
````

