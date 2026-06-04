# MCP OAS – Zoho Lens

OpenAPI 3.0 specifications for [Zoho Lens](https://www.zoho.com/lens/) APIs, designed for use with the **Model Context Protocol (MCP)**.

## Overview

This repository contains individual OpenAPI spec files that describe the Zoho Lens REST API endpoints. These specs can be consumed by MCP-compatible tools to enable AI-powered remote assistance workflows.

## API Specifications

| File | Description |
|------|-------------|
| `sessionSchedule.yaml` | Schedule a new remote assistance session |
| `sessionReschedule.yaml` | Reschedule an existing session |
| `sessionStart.yaml` | Start a remote assistance session |
| `fetchScheduledSessionDetail.yaml` | Fetch details of a scheduled session |
| `fetchOngoingSessionsList.yaml` | List all ongoing sessions |
| `fetchCompletedSessions.yaml` | List all completed sessions |
| `fetchSessionReports.yaml` | Fetch session reports |
| `getSysIdForSessionId.yaml` | Get system ID for a given session ID |
| `downloadSessionChats.yaml` | Download chat logs from a session |
| `downloadSessionNotes.yaml` | Download notes from a session |
| `downloadSessionRecordings.yaml` | Download session recordings |
| `downloadSessionScreenshots.yaml` | Download session screenshots |
| `fetchAllSessionsFilesMetadata.yaml` | Fetch file metadata for all sessions |
| `fetchSpecificSessionFilesMetadata.yaml` | Fetch file metadata for a specific session |
| `downloadSpecificSessionAllFiles.yaml` | Download all files from a specific session |
| `fetchUserDetails.yaml` | Fetch authenticated user details |
| `fetchOrganizationsList.yaml` | List all organizations |
| `setDefaultOrganization.yaml` | Set the default organization |
| `fetchDepartmentsList.yaml` | List all departments |
| `setPreferredDepartment.yaml` | Set the preferred department |
| `fetchOrgMembersList.yaml` | List organization members |
| `fetchWorkInstructionsList.yaml` | List all work instructions |
| `fetchWorkInstructionDetails.yaml` | Fetch details of a work instruction |

## Usage

Each YAML file is a standalone OpenAPI 3.0 specification. Import them into any OpenAPI-compatible tool or MCP server to interact with the Zoho Lens API.

### Authentication

All endpoints use OAuth 2.0 via Zoho IAM with scopes prefixed by `ZohoLens.*`.

### Base URL

```
https://lens.zoho.com
```

## License

See [LICENSE](LICENSE) for details.
