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
