
## graphdb (private only)persistence strategy


## GraphDB stores all of its data (statements, indexes, entity pool, etc.) in files in the configured storage directory, usually called storage. The content and names of these files is not defined and is subject to change between versions.

### There are several types of indexes available, all of which apply to all triples, whether explicit or implicit. These indexes are maintained automatically.

- In general, the index structures used in GraphDB are chosen and optimized to allow for efficient:

- handling of billions of statements under reasonable RAM constraints;

- query optimization;

- transaction management.

### GraphDB maintains two main indexes on statements for use in inference and query evaluation: the predicate-object-subject (POS) index and the predicate-subject-object (PSO) index. There are many other additional data structures that are used to enable the efficient manipulation of RDF data, but these are not listed, since these internal mechanisms cannot be configured.
