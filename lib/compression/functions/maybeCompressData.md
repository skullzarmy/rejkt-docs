[**REJKT.xyz Feed and Filter System Documentation v0.1.0**](../../../README.md)

***

[REJKT.xyz Feed and Filter System Documentation](../../../modules.md) / [lib/compression](../README.md) / maybeCompressData

# Function: maybeCompressData()

> **maybeCompressData**\<`T`\>(`data`, `sizeThreshold`, `forceCompress`): [`CompressionResult`](../interfaces/CompressionResult.md)\<`T`\>

Compresses data if it exceeds the size threshold

## Type Parameters

### T

`T`

## Parameters

### data

`T`

The data to potentially compress

### sizeThreshold

`number` = `102400`

Size threshold in bytes (default: 100KB)

### forceCompress

`boolean` = `false`

Forces compression regardless of thresholds (for testing)

## Returns

[`CompressionResult`](../interfaces/CompressionResult.md)\<`T`\>

Compression result with metadata
