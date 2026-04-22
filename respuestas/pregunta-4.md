MATCH (p:Persona)-[:AMIGO_DE]->(amigo)
WITH p, COUNT(amigo) AS num_amigos
WHERE num_amigos >= 2
RETURN p.nombre, num_amigos