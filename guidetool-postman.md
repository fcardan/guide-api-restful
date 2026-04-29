# 📖 Guide: Postman Integration

## 🔹 Introduction
Postman is a vital tool for developers, QA engineers, and integration teams working with RESTful APIs. It provides an intuitive interface to test, document, and mock endpoints, streamlining development and fostering cross-team collaboration.

---

## Navigating the Postman Interface

The Postman UI brings all your workflow tools together:

- **New (+)**: create requests, collections, or environments.  
- **Import**: upload collections, environments, or paste cURL commands.  
- **Collections**: group related requests for better organization.  
- **Environments**: manage variables per context (dev, staging, prod).  
- **Monitor**: schedule automated runs of collections for health checks.  
- **Mock Servers**: serve predefined API responses.  
- **Flow**: build visual automation flows without code.

---

## Parameters

Parameters help make calls dynamic and reusable:

| Type            | Location                         | Purpose                                  |
|-----------------|----------------------------------|------------------------------------------|
| Path Params     | In the URL path (`/users/:id`)   | Identify specific resources.             |
| Query Params    | After `?` in the URL             | Filter or modify returned data.          |
| Header Params   | In the HTTP headers              | Send metadata (auth, formatting, etc.).  |
| Body Params     | In the request body (JSON, form) | Provide the data to be processed.        |

---
## Creating and Sending Requests

1. Click **New (+)** ▶ **Request**.  
2. Pick an HTTP method (GET, POST, PUT, DELETE, etc.).  
3. Enter the endpoint URL.  
4. Add headers, parameters, or a request body as needed.  
5. Hit **Send** to execute and view the response.

---

## Authorization

The **Authorization** tab automates the `Authorization` header:

| Type           | Common Use                     | Example                          |
|----------------|--------------------------------|----------------------------------|
| No Auth        | Public APIs                    | —                                |
| API Key        | Static key                     | Header or query string           |
| Bearer Token   | JWT / OAuth2                   | `Authorization: Bearer …`        |
| Basic Auth     | Encoded user and password      | Legacy internal systems          |
| OAuth 1.0 / 2.0| Secure token flows             | Social networks, banking APIs    |
| Hawk / AWS Sig.| Specialized signatures         | AWS services, niche scenarios    |

---
