---
title: "Range Tombstone Conversion: Faster Scans Over Long Runs of Deletes"
url: "http://rocksdb.org/blog/2026/06/22/range-tombstone-conversion.html"
date: "2026-06-22"
author: ""
feed_url: "https://rocksdb.org/feed.xml"
---
RocksDB has historically been known for poor performance when tombstones accumulate. This has become a common problem within Meta, and the community has raised it as well. Here, we introduce an optimization that attempts to convert contiguous tombstones into a range tombstone during scans. As a result, instead of skipping through N tombstones, we only need to skip through a single range tombstone.
