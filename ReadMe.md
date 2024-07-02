from neo4j import GraphDatabase

uri = "bolt://your_neo4j_host:7687"
username = "your_username"
password = "your_password"
# Specify encrypted connection
driver = GraphDatabase.driver(uri, auth=(username, password), encrypted=True)

# Use the driver...