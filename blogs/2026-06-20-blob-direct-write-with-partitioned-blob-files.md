---
title: "Blob Direct Write With Partitioned Blob Files"
url: "http://rocksdb.org/blog/2026/06/20/blob-direct-write-partitioned-blob-files.html"
date: "2026-06-20"
feed_url: "https://rocksdb.org/feed.xml"
---
TL;DR Blob Direct Write moves large-value separation earlier in RocksDB’s write path. When enable_blob_files and enable_blob_direct_write are enabled, values at or above min_blob_size can be written directly to blob files during a write, while the WAL and memtable store a compact BlobIndex reference instead of the full value. The companion partitioning support makes this more than a write-path optimization.
