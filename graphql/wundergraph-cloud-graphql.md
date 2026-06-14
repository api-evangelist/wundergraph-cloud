# WunderGraph Cloud GraphQL API

WunderGraph Cosmo is the full lifecycle GraphQL API management platform for building, managing, and scaling federated supergraphs. The control plane exposes a Platform API (used by the Cosmo CLI and Studio) via Connect RPC (protobuf over HTTP) at `https://cosmo-cp.wundergraph.com`. The GraphQL SDL below represents the canonical type surface derived from the official protobuf service definition (`proto/wg/cosmo/platform/v1/platform.proto`) in the open-source Cosmo repository.

The Platform API covers federated graph lifecycle management (create/update/delete subgraphs and federated graphs), schema registry operations (publish, check, fix schemas), analytics and metrics queries, organization and member management, API key management, feature flags, schema proposals, cache warmer configuration, persisted operations, webhook and integration management, and billing.

Authentication is performed via a Bearer API key issued through Cosmo Studio or the `wgc` CLI. Requests must include `Authorization: Bearer <api-key>`.

**Endpoint:** https://cosmo-cp.wundergraph.com

**Documentation:** https://cosmo-docs.wundergraph.com/

**References:**

- Documentation: https://cosmo-docs.wundergraph.com/
- GettingStarted: https://cosmo-docs.wundergraph.com/getting-started/cosmo-cloud-onboarding
- GitHub: https://github.com/wundergraph/cosmo
- Proto Source: https://github.com/wundergraph/cosmo/blob/main/proto/wg/cosmo/platform/v1/platform.proto
