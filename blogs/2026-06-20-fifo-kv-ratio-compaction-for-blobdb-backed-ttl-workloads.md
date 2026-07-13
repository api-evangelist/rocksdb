---
title: "FIFO KV-Ratio Compaction for BlobDB-Backed TTL Workloads"
url: "http://rocksdb.org/blog/2026/06/20/fifo-kv-ratio-compaction.html"
date: "2026-06-20"
author: ""
feed_url: "https://rocksdb.org/feed.xml"
---
RocksDB 11.0 added CompactionOptionsFIFO::max_data_files_size and CompactionOptionsFIFO::use_kv_ratio_compaction for a specific but important shape of workload: FIFO compaction, integrated BlobDB, large values, point lookups, and data that naturally expires by TTL or by a bounded data-size budget. The implementation was added in pull request #14326 . The goal is to keep FIFO’s low write amplificat
