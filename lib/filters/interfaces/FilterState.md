[**REJKT.xyz Feed and Filter System Documentation v0.1.0**](../../../README.md)

***

[REJKT.xyz Feed and Filter System Documentation](../../../modules.md) / [lib/filters](../README.md) / FilterState

# Interface: FilterState

Base filter state interface for all filter types

## Extended by

- [`ToggleFilterState`](ToggleFilterState.md)
- [`RangeFilterState`](RangeFilterState.md)
- [`TagFilterState`](TagFilterState.md)
- [`SelectFilterState`](SelectFilterState.md)

## Properties

### isActive

> **isActive**: `boolean`

***

### lastModified?

> `optional` **lastModified**: `Date`

***

### range?

> `optional` **range**: \[`number`, `number`\]

***

### tags?

> `optional` **tags**: [`Tags`](../../tagData/type-aliases/Tags.md)

***

### type?

> `optional` **type**: [`FilterType`](../type-aliases/FilterType.md)
