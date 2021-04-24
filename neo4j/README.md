# Create db, logs, plugins, import directories

mkdir db logs plugins import

# data directory to stores the system information and graph data.

# logs directory, Outputting the Neo4j logs to a place outside the container ensures we can troubleshoot any errors in Neo4j, even if the container crashes.

# The import directory, so we can copy CSV or other flat files into that directory for importing into Neo4j. Load scripts for importing that data can also be placed in this folder for us to execute.

# Plugins directory, If we want to include any custom extensions or add the Neo4j APOC or graph algorithms library.

# Minimal Jupyter LAB at http://localhost:8888

# Neo4j browser: http://localhost:7474/browser/

docker-compose up
