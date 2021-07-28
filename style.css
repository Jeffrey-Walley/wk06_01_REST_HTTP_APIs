/* 
 07/26/21  RESTful API

            REpresentational State Transfer (REST) is the architecture 

            -- resource - the object which is acted upon, commonly mapped in a single table (but not always)
                
            -- create, read, update, delete (CRUD)

            -- a 'collection' is a set of resources (ex: a company resource contains department resources, which contains additional resources)

            -- URL (Uniform Resource Locator) part of a USI and helped to locate a resource and perform actions on it

            ** REST defines a set of 6 constraints
                    -uniform interface - each Resource must map to exactly 1 resource name and URL (HATEOAS - Hypermedia as the engine of the app state)
                                            data format should be consistent. JSON is very common for passing data into and returning from an API
                                **JSON - JavaScript Object Notation. compact & serialize-able with parsers, simple text to pass through proxies and firewalls
                                        denoted with {}, objects are name:value pairs, value can be standard name, or nested array / object   
                    
                    -client-server serperation -   clients and servers are independent of one another. the client is not concerned with server implementation and vice-versa
                                                        -allows for portability for clients and adaptability for servers

                    -stateless -  Server should treat request as independent and brand new - essentialy SERVER does not hold any client state.
                                           *** every request must contain all the information needed for the server to understand and process it.

                    -cacheable - improves client-side performance and reduces server-side load
                                    ** Example: An API has a resource for all the employees in a company. Every night, a process runs to update the resource so that newly
                                           hired employees are added. That means that during each work day, the resource will not change.

                    -layered system - 

                    - Code-on-demand -  optional 

            
            // Endpoints, HTTP methods, and response codes //
                
                    -Endpoints - are the entry point for the API and take the form of the URL

                    -HTTP Methods - comprise the various methods that can be carried out on resources
                                
                            * GET: get method is used to retrieve a resource from a server. GET request are read-only operations and don't change a resource.

                            * POST: the Post method is used to send data to the server (actually creates and entity in a particular resource).

                            * PUT: updates an entity at a resource - replaces an existing entity

                            * PATCH: used to update an entity, but ONLY SENDS the UPDATED parts to the server

                            * DELETE: will delete a particular entity in a resource.

                            * HEAD: read-only (like GET) but ONLY returns response of headers and status line

                            * CONNECT: establish a tunnel to a server (used to set up a secure connection before transmitting data)
                            
                            * OPTIONS: will determine the supported operations in communication 
                                        (some resources may only support GET or POST, so OPTIONS will return which are supported)

                            * TRACE: used for network diagnostics and performs a loop-back test on a resource by returning what was sent 
                                    *used for testing, but normally not supported in production server*            


                    -HTTP response codes -
                      
                            * 1xx - INFORMATIONAL RESPONSE
                                    100 Continue: response indicates everything is ok so far
                            
                            * 2xx -  SUCCESSFUL RESPONSE
                                    200 OK: request succeeded
                                    
                                    201 Created: request has succeeded and a resource has been created - typical response for a POST

                                    202 Accepted: request received but no action has been taken, the request will be processed later

                            * 3xx -  REDIRECTIONAL response
                                    301 Moved Permanently: URL of the requested resource has changed
                                    
                            * 4xx - RESPONSE CODES 
                                    400 Bad Request: server could not process because not formatted properly
                                    
                                    401 Unauthorized: client needs to authenticate before access

                                    403 Forbidden: client has authenticated, but does NOT have access

                                    404 Not Found: endpoint does not exist, Server cannot be found
                            
                                    405 Method Not Allowed: method used is not supported   
                            
                            * 5xx - SERVER ERROR
                                    500 Internal Server Error: server has encounteded an error and cannot process request     
                                    
             
            // Designing API Endpoints

                        endpoints should contain Plural Nouns (NEVER Verbs)

                    a good ex: for a car website would be
                            /dealerships/{dealershipId}
                            /dealerships/{dealershipId}/cars        // this would be a 'cars' endpoint

                -If I want to create a new dealership, I make a POST request to /dealerships.
                -If I want to update the dealership with id 84, I make a PUT request to /dealerships/84.
                -If I want to get all cars at the dealership with id 27, I make a GET request to /dealerships/27/cars.
                -If I want to delete car with id 119 at dealership with id 6, I make a DELETE request to /dealerships/6/cars/119.            

            // Path vs Query Parameters
            
                    -Path Parameters are used to IDENTIFY resources
                    -Query Parameters are used to FILTER resourcers
                      ex: /dealerships/27/cars?color=red    // the '?color=red' is a query parameter
                      ex2: /dealerships/27/cars?sort=msrp   // sorting by '?sort=msrp'
                      ex3: /dealerships/27/cars?color=red&sort=msrp  // filter both color and msrp

                      */