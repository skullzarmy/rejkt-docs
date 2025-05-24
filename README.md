**REJKT.xyz Feed and Filter System Documentation v0.1.0**

***

# REJKT.xyz Feed and Filter System Documentation

This documentation provides a comprehensive overview of the feed and filter systems in REJKT.xyz.

## System Overview

REJKT.xyz implements multiple feed types with different approaches to displaying NFT content:

### Feed Types

| Feature                    | Main Feed                | Artist Feed                | Gallery Feed                | Single Artist Feed   |
| -------------------------- | ------------------------ | -------------------------- | --------------------------- | -------------------- |
| **Data Focus**             | Listings                 | Artist profiles            | Tokens                      | Artist portfolio     |
| **Filter Support**         | Full                     | Full                       | None                        | Limited              |
| **Pagination**             | ID-based                 | ID-based                   | Offset-based                | Offset-based         |
| **Data Model**             | `BaseListing`            | `BaseListing`              | `GalleryToken`              | Artist tokens        |
| **UI Component**           | `MediaModal`             | `ArtistModal`              | `MediaModal`                | `MediaModal`         |
| **Caching Strategy (TTL)** | Short-term (5 min)       | Medium-term (10 min)       | Long-term (15 min)          | Medium-term (10 min) |
| **Persistence Hook**       | `useMainFeedPersistence` | `useArtistFeedPersistence` | `useGalleryFeedPersistence` | N/A                  |

### Core Architectural Patterns

1. **Component-Based UI**: React components isolate UI concerns
2. **Custom React Hooks**: Encapsulate complex business logic
3. **Provider Pattern**: Global state management
4. **Repository Pattern**: Data access abstraction
5. **Optimistic UI Updates**: Update UI before persistence completes
6. **Lazy Loading**: Defer loading of non-critical components
7. **Progressive Enhancement**: Graceful degradation when features are unavailable

## Documentation Structure

This documentation is organized into the following sections:

-   **Feed Systems**: Implementation of various feed types
-   **Filter Systems**: Filter implementation and management
-   **Persistence**: Feed state persistence and caching
-   **Hooks**: React hooks for feed state management
-   **Utilities**: Support utilities for the feed system

## Integration Diagram

```
┌─────────────────┐     ┌─────────────────┐     ┌─────────────────┐
│  User Interaction│────▶│    Filter UI    │────▶│  Filter State   │
└─────────────────┘     └─────────────────┘     └────────┬────────┘
                                                        │
┌─────────────────┐                                     ▼
│  Render Results  │◀───┐                      ┌─────────────────┐
└─────────────────┘    │                       │ Feed Component  │
                      │                       └────────┬────────┘
┌─────────────────┐    │    ┌─────────────────┐        │
│ Persistence Layer│◀───┴────│Filter Application│◀───────┴────────┐
└───────┬─────────┘         └─────────────────┘                  │
        │                                                        │
        ▼                                                        │
┌─────────────────┐                              ┌───────────────┴─┐
│ IndexedDB Store │                              │   API Query     │
└─────────────────┘                              └─────────────────┘
```
