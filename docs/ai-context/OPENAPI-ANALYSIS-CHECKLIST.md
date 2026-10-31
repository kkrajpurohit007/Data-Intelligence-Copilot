# Swagger / OpenAPI analysis checklist

- Spec file and OpenAPI/Swagger version
- Servers and base URL assumptions
- Path + HTTP method + operationId
- Parameters: path/query/header/cookie, required, type, constraints
- Request body and content types
- Responses: status codes, schemas, headers, error shapes
- Authentication/security schemes and scopes
- Components, references, enums, nullable/required fields
- Pagination, filtering, sorting, idempotency where documented
- Contract gaps, inconsistencies, compatibility impact
- Exact source references
- Distinguish documented contract from runtime implementation
