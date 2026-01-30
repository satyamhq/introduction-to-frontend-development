# Static and Dynamic Content

## Overview

Websites often show different content to different users. For example, online stores display personalized recommendations based on user profiles. This behavior is possible because websites use a combination of **static** and **dynamic** content.

Understanding the difference between static and dynamic content also helps clarify the roles of **web servers** and **application servers**.

---

## Web Servers and Content Delivery

* When a user opens a website, a **web server** sends content to the browser
* This content can be either **static** or **dynamic**

---

## Static Content

### Definition

Static content consists of files that are sent to the browser **exactly as they are stored** on the web server.

### Characteristics

* Does not change per user
* Served quickly
* No server-side processing required

### Examples

* Images
* Videos
* HTML files
* CSS files

---

## Dynamic Content

### Definition

Dynamic content is **generated at the time of the HTTP request**.

### Characteristics

* Can change based on user input, profile, or time
* Requires server-side processing
* Usually slower to generate than static content

### Examples

* Personalized recommendations
* News based on the current date
* User dashboards after login

---

## Role of Application Servers

* Web servers communicate with **application servers** (back-end servers)
* Application servers generate dynamic content

### Responsibilities of Application Servers

* Run application logic
* Communicate with databases
* Check permissions and authentication
* Customize content per user

---

## Static vs Dynamic Content Example

### Static Example

* Clicking **Play** on a video
* Web server sends the video file directly to the browser

### Dynamic Example

* Logging into a website
* Web server asks the application server to:

  * Verify enrollment or credentials
  * Decide what content to show

---

## Performance Considerations

* Dynamic content takes longer to generate
* Application servers have limited request capacity
* This can become a performance issue for large websites

---

## Caching

### What Is Caching?

Caching is a technique where the web server stores a **copy of dynamic content** after it is generated.

### How Caching Works

1. First request:

   * Web server checks cache
   * If content is missing, it requests it from the application server
   * Stores the result in the cache

2. Subsequent requests:

   * Web server serves content directly from the cache
   * No need to contact the application server

3. Cache Update:

   * Cache is refreshed after a time period or new user interaction

### Benefits

* Faster response times
* Reduced load on application servers
* Better scalability

---

## Key Takeaways

* **Static content** is pre-built and fast to deliver
* **Dynamic content** is generated per request and personalized
* **Web servers** deliver content and manage caching
* **Application servers** handle logic, databases, and personalization

Understanding these concepts helps identify whether website content is static or dynamic and how modern websites scale efficiently.
