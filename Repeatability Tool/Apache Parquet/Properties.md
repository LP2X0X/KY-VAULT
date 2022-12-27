1 - Column-oriented data file format: Items in the same column are stored next to each other. We do that so we can query columns quickly.
 Example: We have 3 column: Name, DOB, Job Tile. All the name will be stored next to each other, etc...
 
2 - Efficient data storage and retrieval:
- Within the column structure we're using encoding and the across the whole file we use compression.
- We can read from these files really quickly.