# API Documentation

## Endpoints
### Assessment Intake
- **Description**: Collect, validate and normalize content metadata from SIS; attach a runId and timestamp for traceability.
- **Type**: Processing

### Retrieve
- **Description**: Execute retrieve phase for the RAG pattern: persist interim state, enforce guardrails, and emit structured JSON results.
- **Type**: Processing

### Ground
- **Description**: Execute ground phase for the RAG pattern: persist interim state, enforce guardrails, and emit structured JSON results.
- **Type**: Processing

### Readiness Check
- **Description**: Readiness Check across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Practice Recommendation
- **Description**: Practice Recommendation across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Progress Review
- **Description**: Progress Review across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Parent/Student Notification
- **Description**: Assemble final payload with status, artifacts, KPIs and audit trail; store to Identity/SSO; return response JSON for the client.
- **Type**: Processing
