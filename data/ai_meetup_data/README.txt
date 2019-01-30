The three files contained are:

1) wikidata_companies.csv: data for entities from wikidata database which may be companies. Columns are:
	1) wikidata_id: unique identifier for each entity
	2) item_title: name of the page for this unique identifier
	3) country: country this entity is associated with, if available

2) ishares_companies.csv: data for entities from ishares constituency lists, which may be companies. Columns are:
	1) ishares_id: unique identifier for each entity
	2) Name: name of this entity
	3) Country: country of this entity, as determined by what ETF they were in
	4) Sector: business sector of this entity, as provided by iShares
	5) Ticker: trading ticker for local exchange, as provided by iShares
	6) Market Value: market value of entity, as provided by iShares

3) labeled_data.csv: ~150 hand annotated links. Columns are:
	1) ishares_id: unique identifier for ishares entity
	2) wikidata_id: unique identifier for wikidata entity. May be null. If null, signifies that there is no corresponding match in the wikidata db.