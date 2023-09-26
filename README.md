# Designing a RESTful API

## Good API Design
  - CLear Naming
  - Clear Directions
  - Knowledge of use cases
  - Adoptability
  - Versoning
  - Backwards Compability

## Verbs
**GET**
- Retrieve a resource or collection of resources

**DELETE**
  - Deletes a resouce

**PUT**
  - Updates a single resource that already exists by replacing it

**POST**
  - Catch-all for HTTP resources
  - used to change the status or state of  aresoucre
  - used for anything else that does'nt clearly fit the other verbs

**PATCH**
  - Updates a single resource that already exists by patching the column that is being modified

**OPTIONS**
  - Returns info about API (methods/content type)
  - Does not return an entity body, just metadata in the form of HTTP headers.

**HEAD**
  - Returns info about resource (version/length/type)
  - Does not return an entity body, just metadata in the form of HTTP headers.

## REST and HTML

HTTP - Protocol  
XML - Markup Language, can add structure to HTTP.  
JSON - Notation, can add contxt to HTTP.

**REST** is a set of principles and constraints.

**SOAP**
- A fixed process
- Lots of documentations up front
- Detailed scenarios
- Complex error handeling

**REST**
- Few arguments
- Docs discovered as you go
- Flexible, based on needs
- Flexible, based on Patterns

## HTTP Codes
| Codes   | Meaning       |
| ------- |:-------------:|
| 100s    | Informational | 
| 200s    | Success       |
| 300s    | Redirect      |
| 400s    | Client Error  |
| 500s    | Server Error  |

## REST API Constrains

### 1. Client-Server Architecture
### 2. Stateless Architecture
  - Stability
  - Scalability
  - Reliability
  - flexibility
### 3. Cacheable

| HTTP Method | Idempotent | Safe |
|-------------|------------|------|
| OPTIONS     | yes        | yes  |
| GET         | yes        | yes  |
| HEAD        | yes        | yes  |
| PUT         | yes        | no   |
| POST        | no         | no   |
| DELETE      | yes        | no   |
| PATCH       | no         | no   |  

- **Idempotence** means the result will never be changed, you can keep calling the method, but the response you get back will always be the same.
- **Safety** is where the resource on the server is not changed in any way. Things might happen on the server, but the resource itself is not modified.
