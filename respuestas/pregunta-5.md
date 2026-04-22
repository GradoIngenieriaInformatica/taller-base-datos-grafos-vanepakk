MATCH (p:Persona)-[:GESTIONA]->(pr:Proyecto)
WHERE NOT (p)-[:PARTICIPA_EN]->(pr)
RETURN p.nombre, pr.nombre