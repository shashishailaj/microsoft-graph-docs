---
title: "Overview of the Microsoft Search API in Microsoft Graph (preview)"
description: "Use the Microsoft Search API to index content and add search across your Office and indexed content to your apps."
localization_priority: Priority
ms.prod: "search"
author: "snlraju-msft"
scenarios: "getting-started"
---

# Overview of the Microsoft Search API in Microsoft Graph (preview)

Microsoft Search is an enterprise search engine that delivers productivity gains and relevant search results for your organization. It harnesses the collective knowledge and productivity of an organization, and surfaces relevant content to keep end users up to date. Microsoft Search is available in various experiences including Office, SharePoint, Delve, Windows, and Bing. You can use the Microsoft Search API in Microsoft Graph to extend Microsoft Search to your apps.

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

<!-- markdownlint-disable MD026 -->
## Why use the Microsoft Search API?

### One unified search endpoint for Microsoft cloud data

The Microsoft Search API provides one unified search endpoint that you can use to [query](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) data in the Microsoft cloud - messages and events in Outlook mailboxes, and files on OneDrive and SharePoint - that Microsoft Search already indexes.

### Include custom external data in search experience

Customers who want to include data outside of the Microsoft cloud in their search experience can use [connectors](/microsoftsearch/connectors-overview) to connect to a specific data source such as an organization's human resources database or product catalog, and use the Microsoft Search API to seamlessly [query](/graph/api/search-query?view=graph-rest-beta&preserve-view=true) the external data source. The [Microsoft Graph connectors gallery](/microsoftsearch/connectors-gallery) lists a number of ready-to-use connectors. Alternatively, customers can [build connectors](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true#common-use-cases), index external custom items, and query specific external data sources as well.

### Consistent, up-to-date search experience

When you use the Microsoft Search API, your customers benefit from more personalized, relevant search results powered by Microsoft Graph. The search experience in your apps will return results that are consistent with search in Office applications.

## What data can I add or access by using the Microsoft Search API?

The Microsoft Search API supports searching the following content in the Microsoft cloud:

- Outlook email [messages](/graph/api/resources/message?view=graph-rest-beta&preserve-view=true) and calendar [events](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true) objects
- SharePoint and OneDrive files and folders ([driveItem](/graph/api/resources/driveitem?view=graph-rest-beta&preserve-view=true)), [lists](/graph/api/resources/list?view=graph-rest-beta&preserve-view=true), [listItems](/graph/api/resources/listitem?view=graph-rest-beta&preserve-view=true), [sites](/graph/api/resources/site?view=graph-rest-beta&preserve-view=true) and [drives](/graph/api/resources/drive?view=graph-rest-beta&preserve-view=true)
- Content ingested throught the Graph Connectors platform : [externalItems](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true)

## API reference

Looking for the API reference for this service?

- [Use the Microsoft Search API to query data](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true)
- [Use the Microsoft Search API to index data](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true)

## Next steps

- Learn more about [Microsoft Search](/microsoftsearch/).
- Learn more about a few key use cases:
  - [Manage connections to index external content](search-index-manage-connections.md)
  - [Index external content](search-index-manage-items.md)
  - [Search Outlook messages](search-concept-messages.md)
  - [Search calendar events](search-concept-events.md)
  - [Search content in Sharepoint and OneDrive](search-concept-files.md)
  - [Search external content](search-concept-custom-types.md)
  - [Sort search results](search-concept-sort.md)
  - [Refine search results](search-concept-aggregation.md)
  
- Explore the search APIs in  [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).
- Download the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub.

## See also

- Engage with the community on [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoft-graph-search) or on GitHub
