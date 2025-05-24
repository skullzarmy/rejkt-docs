[**REJKT.xyz Feed and Filter System Documentation v0.1.0**](../../../README.md)

***

[REJKT.xyz Feed and Filter System Documentation](../../../modules.md) / [lib/curatedFeed](../README.md) / fetchArtistFeed

# Function: fetchArtistFeed()

> **fetchArtistFeed**(`desiredCount`, `batchSize`, `initialLastId`, `filters`): `Promise`\<[`FilterResult`](../interfaces/FilterResult.md)\>

Fetches a feed of artist listings with additional filtering for aliases

## Parameters

### desiredCount

`number`

Number of listings to fetch

### batchSize

`number`

Size of each batch request

### initialLastId

`number`

ID to start fetching from

### filters

[`FiltersRecord`](../type-aliases/FiltersRecord.md)

Filter criteria to apply

## Returns

`Promise`\<[`FilterResult`](../interfaces/FilterResult.md)\>

A FilterResult object containing listings and error information
