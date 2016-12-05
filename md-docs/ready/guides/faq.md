---
id: faq
title: FAQ
permalink: ready/guides/faq/index.html
---

### Paginating content from Sync Gateway

<img src="img/pagination.png" width="25%" />

Paginating a list view is a good pattern when the data source is fairly large and is retrieved over the Sync Gateway REST API. If you wish to display the documents in a channel for example, it's recommended to use the `/{db}/_changes` endpoint with the `limit` and `since` querystring parameters. If you wish to display the documents in a logical order by key then you can use the `/{db}/_all_docs` endpoint with the `startkey` and `limit` querystring parameters.