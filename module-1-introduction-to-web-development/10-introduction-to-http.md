# Introduction to HTTP

## Introduction

Have you ever noticed the lock icon beside a website’s URL in your web browser?  
This indicates that **HTTPS**, the secure version of HTTP, is being used.

**HTTP (Hypertext Transfer Protocol)** is a core protocol of the World Wide Web.  
It enables communication between a web browser (client) and a web server that hosts a website.

Whenever you browse the internet, HTTP or HTTPS is working behind the scenes.

---

## What Is HTTP?

HTTP is a protocol used for transferring web resources such as:
- HTML documents
- Images
- Stylesheets
- Other files required to display a webpage

HTTP follows a **request–response model**, where:
- The client sends a request
- The server returns a response

---

## HTTP Requests

An **HTTP request** contains several components:

- **Method**
- **Path**
- **Version**
- **Headers**
- **Body** (optional)

### HTTP Methods

The most commonly used HTTP methods are:

- **GET**  
  Retrieves data from the server

- **POST**  
  Sends data to the server

- **PUT**  
  Updates an existing resource on the server

- **DELETE**  
  Removes a resource from the server

---

### Path

The **path** specifies the location of a resource on the server.

Example: example.com/images/image.jpg

---


This path tells the server exactly which file is being requested.

---

### HTTP Versions

There are multiple versions of HTTP.  
The most widely used versions today are:
- HTTP/1.1
- HTTP/2

---

### Headers and Body

- **Headers** contain additional information about the request and the client
- Some request methods include a **body**, which contains data sent to the server

---

## HTTP Responses

HTTP responses follow a structure similar to requests.

A response includes:
- Status line
- Headers
- Optional message body containing the requested content

The response body may include:
- HTML pages
- Images
- Other requested resources

---

## HTTP Status Codes

HTTP status codes indicate whether a request was successful.

Status codes range from **100 to 599** and are grouped by their first digit.

### Status Code Groups

- **100–199**: Informational responses  
- **200–299**: Successful responses  
- **300–399**: Redirection messages  
- **400–499**: Client error responses  
- **500–599**: Server error responses  

---

### Common Status Codes

#### Informational
- **100 Continue**  
  Indicates that the client should continue sending the request

#### Success
- **200 OK**  
  The request was successfully processed

The meaning of success depends on the method:
- GET: Resource returned
- POST: Data successfully sent
- PUT: Resource updated
- DELETE: Resource removed

---

#### Redirection
- **301 Moved Permanently**
- **302 Found** (temporary redirection)

Browsers automatically request the resource from the new location.

---

#### Client Errors
- **400 Bad Request** – Invalid request data  
- **401 Unauthorized** – Authentication required  
- **403 Forbidden** – Request refused due to insufficient permissions  
- **404 Not Found** – Resource does not exist  

---

#### Server Errors
- **500 Internal Server Error**  
  Indicates a failure on the server while processing the request

---

## What Is HTTPS?

**HTTPS** is the secure version of HTTP.

It provides:
- Encrypted communication
- Protection of sensitive data
- Secure transfer of information

Before data is sent, it is encrypted into a secure format that only the intended recipient can decrypt.

The lock icon in the browser address bar indicates HTTPS is active.

---

## Summary

In summary:
- HTTP is the foundation of communication on the web
- It enables browsers and servers to exchange data
- Requests and responses follow a defined structure
- HTTP methods define actions performed on resources
- Status codes indicate the outcome of requests
- HTTPS secures communication using encryption

Understanding HTTP is essential to understanding how the web works.


