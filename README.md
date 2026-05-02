# RocksDB

RocksDB is an embeddable persistent key-value store for fast storage, developed at Facebook (Meta) based on LevelDB. It uses a Log-Structured Merge (LSM) tree design optimized for fast, low-latency storage on flash and RAM. RocksDB provides a C++ library with language bindings for Java, Python, Ruby, Rust, and other languages, and is widely used as the storage engine inside databases, data streaming systems, and distributed key-value stores.

**Website:** [https://rocksdb.org/](https://rocksdb.org/)

**GitHub:** [https://github.com/facebook/rocksdb](https://github.com/facebook/rocksdb)

**Documentation:** [https://github.com/facebook/rocksdb/wiki](https://github.com/facebook/rocksdb/wiki)

## APIs

### RocksDB Embedded API
The RocksDB C++ library API providing key-value storage operations including Get, Put, Delete, Merge, iterators, snapshots, column families, transactions, compaction, and backup.

- **Documentation:** [https://rocksdb.org/docs/getting-started.html](https://rocksdb.org/docs/getting-started.html)
- **GitHub:** [https://github.com/facebook/rocksdb](https://github.com/facebook/rocksdb)

### RocksJava API
Official Java bindings for RocksDB used in Apache Kafka Streams, Flink, and Cassandra.

- **Documentation:** [https://github.com/facebook/rocksdb/wiki/RocksJava-Basics](https://github.com/facebook/rocksdb/wiki/RocksJava-Basics)
- **Maven:** [https://mvnrepository.com/artifact/org.rocksdb/rocksdbjni](https://mvnrepository.com/artifact/org.rocksdb/rocksdbjni)

## Artifacts

### JSON Schema
| File | Description |
|------|-------------|
| [json-schema/rocksdb-options-schema.json](json-schema/rocksdb-options-schema.json) | RocksDB database configuration options schema |
| [json-schema/rocksdb-key-value-schema.json](json-schema/rocksdb-key-value-schema.json) | RocksDB key-value entry schema |

### JSON Structure
| File | Description |
|------|-------------|
| [json-structure/rocksdb-options-structure.json](json-structure/rocksdb-options-structure.json) | RocksDB configuration options hierarchy |

### JSON-LD
| File | Description |
|------|-------------|
| [json-ld/rocksdb-context.jsonld](json-ld/rocksdb-context.jsonld) | JSON-LD context for RocksDB data semantics |

### Examples
| File | Description |
|------|-------------|
| [examples/rocksdb-get-example.json](examples/rocksdb-get-example.json) | RocksDB Get operation example |
| [examples/rocksdb-put-example.json](examples/rocksdb-put-example.json) | RocksDB Put operation example |

### Vocabulary
| File | Description |
|------|-------------|
| [vocabulary/rocksdb-vocabulary.yml](vocabulary/rocksdb-vocabulary.yml) | RocksDB domain vocabulary and terminology |

## Key Features

- **Core Operations:** Get, Put, Delete, Merge, Multi-Get
- **Column Families:** Logical data separation within one DB instance
- **Transactions:** ACID properties with TransactionDB / OptimisticTransactionDB
- **Snapshots and Iterators:** Consistent point-in-time reads
- **Compaction Styles:** Leveled, Universal, FIFO
- **Compression:** Snappy, zlib, LZ4, ZSTD
- **BlobDB:** Optimized large-value storage
- **TTL:** Automatic key expiration
- **Backup and Restore:** Incremental backup support

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
