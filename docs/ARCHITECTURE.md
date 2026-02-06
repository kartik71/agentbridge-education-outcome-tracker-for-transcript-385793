# Architecture Documentation

## Overview
This RAG implements Education Outcome Tracker for Transcript for Education use cases.

## Components
1. **Assessment Intake**: Collect, validate and normalize content metadata from SIS; attach a runId and timestamp for traceability.
2. **Retrieve**: Execute retrieve phase for the RAG pattern: persist interim state, enforce guardrails, and emit structured JSON results.
3. **Ground**: Execute ground phase for the RAG pattern: persist interim state, enforce guardrails, and emit structured JSON results.
4. **Readiness Check**: Readiness Check across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
5. **Practice Recommendation**: Practice Recommendation across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
6. **Progress Review**: Progress Review across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
7. **Parent/Student Notification**: Assemble final payload with status, artifacts, KPIs and audit trail; store to Identity/SSO; return response JSON for the client.

## Data Flow
- Input: Assessment Intake
- Processing: 7 sequential steps
- Output: Parent/Student Notification
