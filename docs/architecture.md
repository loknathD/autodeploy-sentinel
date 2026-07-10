# AutoDeploy Sentinel Architecture

## High-Level Architecture

                    +----------------------+
                    |      Web Browser     |
                    +----------+-----------+
                               |
                               v
                    +----------------------+
                    |   React Frontend     |
                    +----------+-----------+
                               |
                          HTTPS / REST
                               |
                               v
                    +----------------------+
                    |    FastAPI Backend    |
                    +----------+-----------+
                               |
         +---------------------+---------------------+
         |                     |                     |
         v                     v                     v
+----------------+    +----------------+    +------------------+
| PostgreSQL     |    | Kubernetes     |    | AI Service       |
| Users & History|    | Python Client  |    | LLM Integration  |
+----------------+    +----------------+    +------------------+
                               |
                               v
                    +----------------------+
                    | Kubernetes Cluster   |
                    +----------------------+