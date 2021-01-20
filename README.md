# Test



 select DISTINCT ?peinture ?peintureLabel ?lieux ?lieuxLabel
where {
 ?peinture wdt:P170 wd:Q296.
 ?peinture wdt:P195 ?lieux.
SERVICE wikibase:label { #pour récuéprer les labels
bd:serviceParam wikibase:language "fr,en"}
}
