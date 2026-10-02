# LAB-16.2

1. The Over-fetching Problem: In your own words, explain the concepts of “over-fetching” and “under-fetching” in the context of a REST API. How does GraphQL’s query language inherently solve this problem?

 - Answer: "Over-fetching" is when an endpoint delivers more data than needed to display a specific view or component. "Under-fetching" is the opposite and not enough data was provided causing sequential or parallel requests. GraphQl uses a query language that specifies the exact data and relationships required, returning a precise response in a single request.
   
2. Endpoint and Schema Philosophy: Compare the endpoint structure of a typical REST API with that of a GraphQL API. How does GraphQL’s strongly-typed schema benefit frontend developers?

 - Answer: GraphQl uses a predefined Schema Defininition Language that defines all available data types, fields, and relationships. This enables developers to use autocompletion and validation features in GraphQl. Frontend frameworks can automatically generate types and interfaces directly from the schema. Frontend teams can understand the accessible data structures without needing external documentation.
 
3. Caching and Complexity: Caching is often cited as a major advantage of REST. Explain why caching is simpler in REST compared to GraphQL. What is a use case where the flexibility of GraphQL might outweigh its caching complexity?

 - Answer: Caching in REST uses the native HTTP standards so browser caches, CDNs, and proxies can automatically cache responses using standard HTTP headers. GraphQl routes all operations through a single HTTP endpoint using POST requests making standard caching ineffective. GraphQl caching has to be handled on the application level which adds more architectural complexity. GraphQl is best used in complex and data rich apps with highly varied clients. The dynamic flexibility, smaller payload size, and reduction of network round trips in a single query outweigh the caching complexity.
