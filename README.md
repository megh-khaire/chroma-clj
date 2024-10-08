# chroma-clj

> A Clojure client for ChromaDB

<!-- [![Clojars Project](https://img.shields.io/clojars/v/org.clojars.megh/semantic-router-clj.svg)](https://clojars.org/org.clojars.megh/semantic-router-clj) -->

## ChromaDB Setup

### Running ChromaDB Locally

#### Step 1: [Install Docker on your system](https://docs.docker.com/engine/install/)

#### Step 2: Pull the ChromaDB Docker Image

```bash
docker pull chromadb/chromadb:latest
```

#### Step 3: Run the ChromaDB Container

```bash
docker run -p 8000:8000 chromadb/chromadb:latest
```

This command starts ChromaDB and maps port 8000 of the container to port 8000 on your host machine.

#### Step 4: Verify ChromaDB is Running

Send a GET request to the /api/v1/health endpoint:

```bash
curl <http://localhost:8000/api/v1/health>
```

You should receive a response indicating the server is healthy:

```json
{"status":"healthy"}
```

## License

This project is licensed under the terms of the MIT License.
