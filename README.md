# ![LOGO](logo.png) NSIDC Web Service Documentation Index **flow**ground Connector

## Description

A generated **flow**ground connector for the NSIDC Web Service Documentation Index API (version 1.0.0).

Generated from: https://api.apis.guru/v2/specs/nsidc.org/1.0.0/swagger.json<br/>
Generated at: 2019-05-07T17:43:18+03:00

## API Description

This API allows programmers to build National Snow and Ice Data Center data and metadata services into their applications.

## Authorization

This API does not require authorization.

## Actions

### View the facet information corresponding to a search

> In the NSIDC Search and Arctic Data Explorer interfaces, this endpoint is used in conjunction with /OpenSearch whenever a user submits a new search. Consequently, it has the same parameters as /OpenSearch.

*Tags:* `SwaggerDocs`

#### Input Parameters
* `searchTerms` - _optional_ - URL-encoded keyword or keywords desired by the client; OpenSearch 1.1
* `count` - _optional_ - The number of search results per page desired by the client; OpenSearch 1.1
* `startIndex` - _optional_ - First search result desired by the search client; OpenSearch 1.1
* `spatial` - _optional_ - 4 comma separated values - W, S, E, N; OpenSearch-Geo 1.0, "box" parameter
* `sortKeys` - _optional_ - Sort the results by most relevant (default), smallest or largest spatial area, shortest or longest temporal duration, or most recently updated; partial implementation of OpenSearch SRU 1.0
    Possible values: score,,desc, spatial_area,,asc, spatial_area,,desc, temporal_duration,,asc, temporal_duration,,desc, updated,,desc.
* `startDate` - _optional_ - The start date in yyyy-mm-dd format
* `endDate` - _optional_ - The end date in yyyy-mm-dd format
* `facetFilters` - _optional_ - Describes faceted restrictions on the search. A URL-encoded JSON object where the keys are the names of the facet, and the values are arrays of the selected facet values
* `source` - _optional_ - Custom parameter for selecting which source to use; the Arctic Data Explorer (ADE) uses data aggregated from many sources, including, but not limited to, NSIDC
    Possible values: NSIDC, ADE.

### Search documents using the OpenSearch 1.1 Specification

> This endpoint uses parameters from the OpenSearch 1.1 specification, as well as parameters from the OpenSearch Geo (1.0) and SRU (1.0) extensions.

*Tags:* `SwaggerDocs`

#### Input Parameters
* `searchTerms` - _optional_ - URL-encoded keyword or keywords desired by the client; OpenSearch 1.1
* `count` - _optional_ - The number of search results per page desired by the client; OpenSearch 1.1
* `startIndex` - _optional_ - First search result desired by the search client; OpenSearch 1.1
* `spatial` - _optional_ - 4 comma separated values - W, S, E, N; OpenSearch-Geo 1.0, "box" parameter
* `sortKeys` - _optional_ - Sort the results by most relevant (default), smallest or largest spatial area, shortest or longest temporal duration, or most recently updated; partial implementation of OpenSearch SRU 1.0
    Possible values: score,,desc, spatial_area,,asc, spatial_area,,desc, temporal_duration,,asc, temporal_duration,,desc, updated,,desc.
* `startDate` - _optional_ - The start date in yyyy-mm-dd format
* `endDate` - _optional_ - The end date in yyyy-mm-dd format
* `facetFilters` - _optional_ - Describes faceted restrictions on the search. A URL-encoded JSON object where the keys are the names of the facet, and the values are arrays of the selected facet values
* `source` - _optional_ - Custom parameter for selecting which source to use; the Arctic Data Explorer (ADE) uses data aggregated from many sources, including, but not limited to, NSIDC
    Possible values: NSIDC, ADE.

### Describes the web interface of NSIDC's data search engine

*Tags:* `SwaggerDocs`

### Suggest search terms based on a partial query

> In NSIDC Search and the Arctic Data Explorer, this endpoint is queried whenever the user types into the search terms box, and the returned suggestions are displayed in a dropdown beneath the search terms box. The q parameter and returned JSON follow the specifications of the OpenSearch Suggestions 1.0 extension.

*Tags:* `SwaggerDocs`

#### Input Parameters
* `q` - _required_ - Search terms typed into the interface (minimum two characters)
* `source` - _required_ - Custom parameter for selecting which source to use; the Arctic Data Explorer (ADE) uses data aggregated from many sources, including, but not limited to, NSIDC
    Possible values: NSIDC, ADE.

## License

**flow**ground :- Telekom iPaaS / nsidc-org-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
