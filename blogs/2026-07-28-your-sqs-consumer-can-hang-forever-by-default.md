---
title: "Your SQS consumer can hang forever by default"
url: "https://encore.dev/blog/message-queue-hangs"
date: "2026-07-28"
feed_url: "https://encore.dev/rss/feed.xml"
---
The AWS Rust SDK ships no request timeout by default, so one SQS receive on a dead connection can hang a whole consumer with nothing in the logs.
