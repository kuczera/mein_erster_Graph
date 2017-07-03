# mein_erster_Graph
Erste Schritte in Graphdatenbanken

In diesem GraphGist sollen die grundlegenden Eigenschaften von Graphen erläutert werden.
Dabei wird die Graphdatenbank https://www.neo4j.com[neo4j] genutzt.

[source,cypher]
----
CREATE (p1:Person {name:'Karl der Große'});
CREATE (p2:Person {name:'Karl der Große'});
CREATE (b1:Buch {Titel:'Vita Karoli Magni'});
CREATE (p1)-[:KENNT]->(p2);
CREATE (p1)-[:KOMMT_VOR_IN]->(b1);
CREATE (p2)-[:SCHRIEB_CA_828-830]->(b1);

----
