# geonamesjp_vs_dbpedia
[GeoNames.jp](http://geonames.jp/) と[DBpedia Japanese](http://ja.dbpedia.org/) のリンクセット


## What's this?
GeoNames.jp と DBpedia Japanese を [owl:sameAs](http://www.w3.org/2002/07/owl#sameAs) で結ぶリンクセットです。

このリンクセットのライセンスは  [CC-BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/) です。


## Example

	@prefix owl:   <http://www.w3.org/2002/07/owl#> .
	@prefix gnjp:  <http://geonames.jp/resource/> .
	@prefix dbpedia-ja: <http://ja.dbpedia.org/resource/> .

	gnjp:北海道  owl:sameAs  dbpedia-ja:北海道 .
	gnjp:北海道三笠市  owl:sameAs  dbpedia-ja:三笠市 .
	gnjp:北海道上川郡  owl:sameAs  dbpedia-ja:上川郡 .
	gnjp:北海道上川郡上川町  owl:sameAs  dbpedia-ja:上川町 .
	gnjp:北海道上川郡下川町  owl:sameAs  dbpedia-ja:下川町 .
	gnjp:北海道上川郡剣淵町  owl:sameAs  dbpedia-ja:剣淵町 .
	gnjp:北海道上川郡和寒町  owl:sameAs  dbpedia-ja:和寒町 .
	
## Note
* 2,332 Triples (2015/07/17時点)
* 現存の都道府県・郡・市区町村を対象としています

## Predicate
GeoNames と DBpedia のリンクセットは [w3c VoID](http://www.w3.org/TR/void/) でも例として挙げられている典型的な事例です。
VoID のサンプルでは以下のように owl:sameAs を用いた関係記述が行われています。
	
	<http://dbpedia.org/resource/Berlin> owl:sameAs <http://sws.geonames.org/2950159/>.
	
ここで owl:sameAs を使うことが適切かどうかは長年議論が行われており、確証が持てない状態ではあるのですが、
現在の本家 DBpedia では、GeoNames.org のリソースに対して owl:sameAs でリンクしているという事実があります。

<https://github.com/dbpedia/links/tree/master/links/dbpedia.org/www.geonames.org>


このリンクセットでは、 DBpedia と GeoNames.org の関係を踏襲して owl：sameAs を選択しています。


