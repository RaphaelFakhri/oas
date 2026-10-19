---
'@readme/openapi-parser': patch
---

The parser is now compiled under TypeScript's `strict` mode. As part of this, spec validation no longer throws a `TypeError` for an OpenAPI parameter that has neither a `schema` nor a `content` object, and a failure while rendering code frames is reported with a readable message even when the thrown value is not an `Error`.
