# API Concepts Reference Sheet

[French Version](frenchVersion.md)

## Basic Concepts

### 1. API (Application Programming Interface)
- **Description**: Like a menu in a restaurant that tells you what you can order from a computer program.

### 2. Client-Server Architecture
- **Description**: The client (you) requests data or a service, and the server (a remote system) responds, like an interaction in a restaurant.

### 3. API Consumption
- **Description**: Using the API to request specific information or services, similar to ordering dishes through a restaurant menu.

## Interaction with Servers

### 4. HTTP Verbs
- **GET**: Requesting information, like viewing the menu.
- **POST**: Sending information to create something new, like ordering an unlisted dish.
- **PUT**: Updating existing information, like changing an entire order.
- **PATCH**: Partially updating, like modifying part of an order.
- **DELETE**: Removing something, like canceling an order.

### 5. Understanding What a Route is in an API

- **City (API)**: The city represents the entirety of the API, a complex system with various functions and services.
- **Address (Route)**: A route in an API is like a specific address in this city. Just as every address leads to a specific building or place, each route in an API leads to a specific function or resource.
- **Signage (API Documentation)**: Just as signs in a city help you find an address, the API's documentation guides developers to access the correct routes and understand what they do.
- **Modes of Transportation (HTTP Requests)**: The various modes of transportation (car, bike, on foot) can be seen as the different types of HTTP requests (GET, POST, etc.). Depending on the type of request, your "journey" to the address (route) will be different.
- **Destination (Resource or Service)**: Once you arrive at the address (route), you access the desired destination, which can be a specific piece of information, a service, or an interaction with the system, just like arriving at a restaurant, a library, or a park in a city.

## Other Concepts

### 6. Payload in HTTP Requests
- **Description**: The data sent in a request, similar to the contents of a letter.

### 7. MVC Model (Model-View-Controller)
- **Model**: Manages and processes data, like the kitchen in a restaurant.
- **View**: Presents data to the user, like the dining area of a restaurant.
- **Controller**: Manages interactions between the model and view, like the waiter in a restaurant.

### 8. REST Architecture
- **Description**: A set of rules for structuring requests and responses, like etiquette in a restaurant.

### 9. Stateful vs Stateless
- **Stateful**: The server remembers previous interactions.
- **Stateless**: Each request is treated independently, without memory of past interactions.

### 10. URL / URI / URN (Uniform Resource Locator / Uniform Resource Identifier / Uniform Resource Name)

- **URL (Uniform Resource Locator)**: An URL is a specific form of URI. It is primarily used to locate and access a resource on the Internet. An URL typically includes multiple components, such as the protocol (e.g., HTTP or HTTPS), the domain name (e.g., www.example.com), the path to the resource on the server (e.g., /page1), and optionally parameters (e.g., ?id=123) or anchors (#section1). URLs are commonly used to access websites, images, videos, and other online resources in a precise manner.

- **URI (Uniform Resource Identifier)**: A URI is a broader term that encompasses both URLs and URNs. A URI can be used to uniquely identify any resource, whether it is located on the Internet or not. URIs are used in various contexts, including hyperlinks, file identifiers on a local file system, database identifiers, and more. URIs primarily serve to designate and identify resources in a unique way.

- **URN (Uniform Resource Name)**: A URN is a subset of URIs specifically used to assign a unique name to a resource without specifying its location or access method. URNs are designed to be persistent and location-independent, meaning they should remain valid even if the resource changes location or access method. URNs are less common than URLs, but they are used in contexts such as file naming, name resolution, and assigning unique names to digital resources.

In summary, an URL is a specific type of URI that includes detailed information about the location of a resource on the Internet, a URN is another type of URI that assigns a unique name to a resource without specifying its location, and a URI is a broader term that encompasses both. All URLs are URIs, all URNs are URIs, but not all URIs are necessarily URLs or URNs.

### 11. Relative Path vs Absolute Path
- **Absolute Path**: A complete reference from the root of the file system.
- **Relative Path**: A reference based on the current location.

### 12. ORM (Object-Relational Mapping) vs ODM (Object-Document Mapping)
- **ORM**: Translates between data stored in tables and their use in objects.
- **ODM**: Translates for document-based databases (like JSON).

### 13. Middleware
- **Description**: Acts as an intermediary in a process, adding or modifying elements in a computer system.

## HTTP Status Codes

| Category | Description |
|----------|-------------|
| 2xx      | Success: The request has been received, understood, and accepted. |
| 3xx      | Redirection: Additional actions must be taken to complete the request. |
| 4xx      | Client Errors: The request contains errors or cannot be processed. |
| 5xx      | Server Errors: The server failed to process a valid request. |

### Specific Status Codes
- **418 I'm a teapot**: An April Fools' joke, indicating that the machine is a teapot, not a coffee maker.
- **420 Enhance Your Calm**: Used by Twitter to indicate that the client has been rate-limited for making too many requests.