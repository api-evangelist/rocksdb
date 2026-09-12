---
title: "Native Async/Coroutine Reads in RocksDB"
url: "http://rocksdb.org/blog/2026/08/24/native-coroutine-reads.html"
date: "2026-08-24"
feed_url: "https://rocksdb.org/feed.xml"
---
A point lookup that misses RocksDB’s block cache can spend most of its time waiting for storage. The traditional way to keep more reads in flight is to add threads. That works, but each outstanding read parks a thread, carries a stack, and adds context-switching overhead.
