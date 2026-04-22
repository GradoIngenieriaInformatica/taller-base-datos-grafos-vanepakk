MATCH (p:Persona)-[:VIVE_EN]->(c:Ciudad)
RETURN p.nombre, c.nombre