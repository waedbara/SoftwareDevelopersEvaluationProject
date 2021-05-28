# Running the application

`mkdir db logs plugins import`

> Data directory, to stores the system information and graph data.

> Logs directory, Outputting the Neo4j logs to a place outside the container ensures we can troubleshoot any errors in Neo4j, even if the container crashes.

> Import directory, we can copy CSV or other flat files into that directory for importing into Neo4j.

> Plugins directory, If we want to include any custom extensions or add the Neo4j APOC or graph algorithms library.

`docker-compose up`

> Minimal Jupyter LAB at http://localhost:8888

> Neo4j browser: http://localhost:7474/browser/