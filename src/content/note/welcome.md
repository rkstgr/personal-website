---
title: Microsoft SQL Server's Bizarre UUID Implementation
description: A deep dive into Microsoft SQL Server's unusual UUID byte ordering, where they uniquely combine little and mixed endian formats—creating unnecessary complexity for developers.
publishDate: "2024-08-09T11:23:00Z"
---

Microsofts SQL server is a incomprehensible mess of inconsistencies.

Couldn't figure out why the parsing of UUID was not working, turns out they decided to use little endian for the first half, and big endian for the second half.

exactly like no one ever...
