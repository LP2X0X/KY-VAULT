![[Pasted image 20221227111005.png|center|700]]
![[1578403454001.jpg|center|700]]
![[Pasted image 20221229113737.png|center|700]]
# File Root
- File Root, is just a directory that holds everything.
# Parquet Files
- Inside the root we have many individual .parquet files, each containing a partition of our data.
# Row Groups
- A single parquet file is composed of many **row groups**. A logical horizontal partitioning of the data into rows. There is no physical structure that is guaranteed for a row group. A row group consists of a column chunk for each column in the dataset.
![[1 3g4RfWdSWKcGs56cNDtJjA.webp|center]]
# Columns
- A single row group contains many **columns**.
# Data Page
- Finally, within our columns are **data pages**, which actually hold the raw data and some relevant metadata. A page is conceptually an indivisible unit (in terms of compression and encoding). There can be multiple page types which is interleaved in a column chunk.
![[1 bsjh1Stj8xK-jKHXjU3NQg.webp|center]]
# Footer
![[1578403507285 1.jpg|center|700]]