# Read09

## High-level HTTP
### The HTTP Request Lifecycle
- Step 1: Local Processing
- Step 2: Resolve an IP
- Step 3: Establish a TCP Connection
- Step 4: Send an HTTP Request
- Step 5: Tearing Down and Cleaning Up

## Java HTTP Request example

### HttpUrlConnection
- HttpURLConnection class is an abstract class directly extending from URLConnection class. It includes all the functionality of its parent class with additional HTTP specific features. HttpsURLConnection is another class which is used for the more secured HTTPS protocol

- It is one of the popular choices among the Java developers for interacting with web servers and android developing team has officially suggested to use it wherever possible.

#### Methods
- getResponseCode() : Used to retrieve the response status from server.
- setRequestMethod() : Used to set the request method. Default is GET.
- getRequestMethod() : Returns the request method.
- getResponseMessage() :Retrieves the response message.