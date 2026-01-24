# HTTP Examples

This document explores HTTP requests and responses in detail, including their structure, methods, headers, status codes, and example payloads.

---

## HTTP Request Line

Every HTTP request begins with a **request line**.

### Format

<HTTP_METHOD> <RESOURCE_PATH> <HTTP_VERSION>

### Example

GET /home.html HTTP/1.1


| Component        | Description                                   |
|------------------|-----------------------------------------------|
| GET              | HTTP method                                   |
| /home.html       | Requested resource                            |
| HTTP/1.1         | HTTP protocol version                         |

---

## HTTP Methods

HTTP methods indicate the action the client wants to perform on a server resource.

| HTTP Method | Description                                                  |
|------------|--------------------------------------------------------------|
| GET        | Requests a resource from the server                          |
| POST       | Submits data to the server                                   |
| PUT        | Replaces an existing resource                                |
| DELETE     | Deletes a resource                                           |
| PATCH     | Partially updates an existing resource                       |

---

## HTTP Request Headers

After the request line, HTTP headers follow, separated from the body by a blank line.

Headers consist of a **case-insensitive name**, a colon (`:`), and a value.

### Common Request Headers

| Header Name        | Example Value                                                                 |
|-------------------|--------------------------------------------------------------------------------|
| Host              | example.com                                                                    |
| User-Agent        | Mozilla/5.0 (Macintosh; Intel Mac OS X 10.9; rv:50.0) Gecko/20100101 Firefox/50.0 |
| Accept            | */*                                                                            |
| Accept-Language   | en                                                                             |
| Content-Type      | text/json                                                                      |

### Header Descriptions

| Header Name      | Purpose                                                                 |
|------------------|-------------------------------------------------------------------------|
| Host             | Specifies the server where the resource is located                      |
| User-Agent       | Identifies the client application and operating system                  |
| Accept           | Specifies acceptable response media types                               |
| Accept-Language  | Indicates preferred language                                            |
| Content-Type     | Describes the format of the request body                                 |

---

## HTTP Request Body

An HTTP request may optionally include a **body**, commonly used with `POST` and `PUT` methods.

### POST Request Example

POST /users HTTP/1.1

Host: example.com

```json
{
  "key1": "value1",
  "key2": "value2",
  "array1": ["value3", "value4"]
}
```


### PUT Request Example

```http
PUT /users/1 HTTP/1.1
Host: example.com
Content-Type: text/json

{
  "key1": "value1"
}
```


---

## HTTP Responses

After processing a request, the server returns an **HTTP response**.

### Status Line Format

<HTTP_VERSION> <STATUS_CODE> <REASON_PHRASE>

### Example


| Component      | Description                                    |
|----------------|------------------------------------------------|
| HTTP/1.1       | Protocol version                               |
| 200            | Status code                                    |
| OK             | Reason phrase                                  |

---

## HTTP Status Codes

HTTP status codes indicate the result of a request.  
They are grouped by the **first digit**.

---

### 1XX – Informational

| Status Code | Reason Phrase        | Description                                                   |
|------------|----------------------|---------------------------------------------------------------|
| 100        | Continue             | Server received headers and expects request body              |
| 101        | Switching Protocols  | Server agrees to switch protocols                             |

---

### 2XX – Successful

| Status Code | Reason Phrase | Description                                                     |
|------------|---------------|-----------------------------------------------------------------|
| 200        | OK            | Request processed successfully                                  |
| 201        | Created       | Resource created successfully                                   |
| 202        | Accepted      | Request accepted but processing not completed                   |
| 204        | No Content    | Request successful, no response body                            |

---

### 3XX – Redirection

| Status Code | Reason Phrase        | Description                                                     |
|------------|----------------------|-----------------------------------------------------------------|
| 301        | Moved Permanently    | Resource moved permanently                                      |
| 302        | Found                | Resource temporarily moved                                      |

---

### 4XX – Client Error

| Status Code | Reason Phrase      | Description                                                     |
|------------|--------------------|-----------------------------------------------------------------|
| 400        | Bad Request        | Invalid request syntax or data                                  |
| 401        | Unauthorized       | Authentication required                                         |
| 403        | Forbidden          | Insufficient permissions                                        |
| 404        | Not Found          | Requested resource not found                                    |
| 405        | Method Not Allowed | HTTP method not supported                                       |

---

### 5XX – Server Error

| Status Code | Reason Phrase        | Description                                                     |
|------------|----------------------|-----------------------------------------------------------------|
| 500        | Internal Server Error| Unexpected server error                                         |
| 502        | Bad Gateway          | Invalid response from upstream server                           |
| 503        | Service Unavailable  | Server cannot process the request                               |

---

## HTTP Response Headers

Response headers follow the status line and provide metadata about the response.

### Common Response Headers

| Header Name       | Example Value                             |
|------------------|--------------------------------------------|
| Date             | Fri, 11 Feb 2022 15:00:00 GMT+2             |
| Server           | Apache/2.2.14 (Linux)                      |
| Content-Length   | 84                                         |
| Content-Type     | text/html                                  |

### Header Descriptions

| Header Name     | Purpose                                                         |
|-----------------|-----------------------------------------------------------------|
| Date            | Time the response was generated                                 |
| Server          | Web server software                                             |
| Content-Length  | Size of the response body                                       |
| Content-Type    | Media type of the returned resource                             |

---

## HTTP Response Body

The response body contains the actual content returned by the server.

### Example Response

HTTP/1.1 200 OK
Date: Fri, 11 Feb 2022 15:00:00 GMT+2
Server: Apache/2.2.14 (Linux)
Content-Length: 84
Content-Type: text/html

<html> <head><title>Test</title></head> <body>Test HTML page.</body> </html> ```

The response body may contain:
HTML documents
Images
Videos
Other media types

## Summary

HTTP requests begin with a request line
Methods define actions on resources
Headers provide metadata
Bodies carry request or response data
Status codes indicate request outcomes
Responses return content to the client
