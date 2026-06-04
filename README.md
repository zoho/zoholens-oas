# Zoho Lens OpenAPI Specification (OAS)

Welcome to the **Zoho Lens OpenAPI Specification (OAS)** repository. This repository provides the OpenAPI Specification files for Zoho Lens APIs, enabling developers to seamlessly integrate Zoho Lens with their applications using standardized API definitions.

---

## **Overview**

The OpenAPI Specification (OAS) is a standardized format for documenting RESTful APIs. It provides details about API structure, endpoints, request/response formats, and authentication methods in JSON or YAML formats. This repository hosts the OAS files for Zoho Lens APIs to help developers:

- Understand Zoho Lens API endpoints and their usage.
- Generate SDKs in various programming languages.

---

## **Repository Structure**

The repository is organized into the following sections:

- **`ZohoLens/`**: Contains the OAS files for Zoho Lens APIs.

### Session Management

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

### Session Files & Downloads

| File | Description |
|------|-------------|
| `downloadSessionChats.yaml` | Download chat transcripts from a session |
| `downloadSessionNotes.yaml` | Download notes from a session |
| `downloadSessionRecordings.yaml` | Download session recordings |
| `downloadSessionScreenshots.yaml` | Download session screenshots |
| `fetchAllSessionsFilesMetadata.yaml` | Fetch file metadata for all sessions |
| `fetchSpecificSessionFilesMetadata.yaml` | Fetch file metadata for a specific session |
| `downloadSpecificSessionAllFiles.yaml` | Download all files from a specific session |

### Organization & Department

| File | Description |
|------|-------------|
| `fetchOrganizationsList.yaml` | List all organizations |
| `setDefaultOrganization.yaml` | Set the default organization |
| `fetchDepartmentsList.yaml` | List all departments |
| `setPreferredDepartment.yaml` | Set the preferred department |
| `fetchOrgMembersList.yaml` | List organization members |

### User & Work Instructions

| File | Description |
|------|-------------|
| `fetchUserDetails.yaml` | Fetch authenticated user details |
| `fetchWorkInstructionsList.yaml` | List all work instructions |
| `fetchWorkInstructionDetails.yaml` | Fetch details of a work instruction |

---

## **Getting Started**

### **1. Explore OAS Files**
1. Navigate to the `ZohoLens/` folder in this repository.
2. Select the OAS file relevant to your use case (e.g., `sessionSchedule.yaml` for scheduling sessions).
3. Use tools like Swagger's API Hub or Postman to import and explore these files.

### **2. Generate SDKs**
Zoho Lens's OAS files can be used to generate SDKs in various programming languages such as Python, Java, and Node.js.

#### Steps:
1. Import the OAS file into Swagger's API Hub:
   - Go to **Swagger API Hub > Design > Import API**.
   - Paste the raw link of the selected OAS file from this repository.
2. Navigate to **Codegen > Client SDK** in Swagger's API Hub.
3. Select your preferred language and download the generated SDK.

---

## **Authentication**

Zoho Lens APIs use OAuth 2.0 for secure authentication via Zoho IAM. All scopes are prefixed by `ZohoLens.*`.

To authenticate your requests:
1. Obtain your `Client ID`, `Client Secret`, and `Refresh Token` from Zoho's [Developer Console](https://api-console.zoho.com).
2. Configure these credentials in your SDK or application.

---

## **Support**

For any questions or assistance, refer to [Zoho Lens Documentation](https://www.zoho.com/lens/) or contact our support team.

---

Start building powerful integrations with Zoho Lens today!
