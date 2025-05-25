
##### Neo4J - Graph RAG 

- https://neo4j.com/blog/developer/microsoft-graphrag-neo4j/

##### Initial Code Credits --  
- Initial Source Code - https://github.com/tomasonjo/blogs/blob/master/msft_graphrag/ms_graphrag_import.ipynb

#
```bash
(base) dhankar@dhankar-1:~/.../artifacts$ pwd
graph_rag/neo4j/data_dir/artifacts
(base) dhankar@dhankar-1:~/.../artifacts$ tree
.
├── create_base_documents.parquet
├── create_base_entity_graph.parquet
├── create_base_extracted_entities.parquet
├── create_base_text_units.parquet
├── create_final_communities.parquet
├── create_final_community_reports.parquet
├── create_final_documents.parquet
├── create_final_entities.parquet
├── create_final_nodes.parquet
├── create_final_relationships.parquet
├── create_final_text_units.parquet
├── create_summarized_entities.parquet
├── join_text_units_to_entity_ids.parquet
├── join_text_units_to_relationship_ids.parquet
└── stats.json

0 directories, 15 files

#
base) dhankar@dhankar-1:~/.../artifacts$ ls -lahtr
total 4.7M
-rw-r--r-- 1 dhankar dhankar 152K Jul  3  2024 create_base_text_units.parquet
-rw-r--r-- 1 dhankar dhankar 129K Jul  3  2024 create_base_extracted_entities.parquet
-rw-r--r-- 1 dhankar dhankar 149K Jul  3  2024 create_summarized_entities.parquet
-rw-r--r-- 1 dhankar dhankar 540K Jul  3  2024 create_base_entity_graph.parquet
-rw-r--r-- 1 dhankar dhankar 2.8M Jul  3  2024 create_final_entities.parquet
-rw-r--r-- 1 dhankar dhankar  29K Jul  3  2024 join_text_units_to_entity_ids.parquet
-rw-r--r-- 1 dhankar dhankar 117K Jul  3  2024 create_final_nodes.parquet
-rw-r--r-- 1 dhankar dhankar  26K Jul  3  2024 create_final_communities.parquet
-rw-r--r-- 1 dhankar dhankar  22K Jul  3  2024 join_text_units_to_relationship_ids.parquet
-rw-r--r-- 1 dhankar dhankar  81K Jul  3  2024 create_final_relationships.parquet
-rw-r--r-- 1 dhankar dhankar 5.6K Jul  3  2024 stats.json
-rw-r--r-- 1 dhankar dhankar 172K Jul  3  2024 create_final_text_units.parquet
-rw-r--r-- 1 dhankar dhankar 125K Jul  3  2024 create_final_documents.parquet
-rw-r--r-- 1 dhankar dhankar 241K Jul  3  2024 create_final_community_reports.parquet
-rw-r--r-- 1 dhankar dhankar 125K Jul  3  2024 create_base_documents.parquet
drwxr-xr-x 2 dhankar dhankar 4.0K Jul  3  2024 .
drwxrwxr-x 3 dhankar dhankar 4.0K May 25 14:58 ..

```