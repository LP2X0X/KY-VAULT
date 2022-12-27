# Overview
![[Pasted image 20221227093921.png|center|1000]]
# Data sources and formats
![[Pasted image 20221227094058.png|center|700]]
## Physical storage layout models
![[Pasted image 20221227094747.png|center|700]]
## Different workloads
- OLTP:
	- Online transaction processing.
	- Lots of small operations involving *whole rows*.
- OLAP:
	- Online analytical processing.
	- Few large operations involving *subset of all columns*.
## Role-wise
- Great with OLTP workloads because:
	- With an insert operation you can just append it at the end.
	- With an update operation you can just find the location and updated the column values in place. The same goes with delete operation.
- [[Horizontal partitioning]].
## Columnar
- Great with OLAP workloads because:
	- OLAP only manipulate subset of all column so with Columnar, you only need to read column you are interested in.
- [[Vertical Partitioning]].
## Hybrid
![[Pasted image 20221227104830.png|center|700]]
- Horizontal and Vertical partitioning.
- **Used by Parquet**.
- Best of both world.