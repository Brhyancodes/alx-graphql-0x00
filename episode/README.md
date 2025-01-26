# GraphQL Episode Query

This repository contains a GraphQL query to retrieve details of an episode from a GraphQL API. The query uses the `episode(id: ID!)` field to fetch specific details about an episode.

## Query Details

The GraphQL query retrieves the following fields for a specified episode:

- `id`: The unique identifier of the episode.
- `name`: The name of the episode.
- `air_date`: The date the episode aired.
- `episode`: The episode code.

### GraphQL Query

The query is defined in the `episode-page-1.graphql` file:

```graphql
query GetEpisodeDetails($id: ID!) {
  episode(id: $id) {
    id
    name
    air_date
    episode
  }
}