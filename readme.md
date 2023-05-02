I made this assignment to check on the number of requests allowed and if the  count exceeds the number it can take, then the rate limiter blocks all the extra requests.
A fixed capacity bucket into which tokens are added at a fixed rate called the the TOKEN BUCKET ALGORITHM. Here, The bucket is checked to determine if it contains at least a single token before allowing the API to continue. 
If one token is pulled out of the bucket, and the API can continue else if no tokens, then the API returns a message'Limit Reached'

-> Spring Boot dependencies with Bucket4j is used which is a Java rate-limiting library based on the same token-bucket algorithm which was used. 
-> Testing can be performed using Playwright or Selenium for browser headed tests.
User bucket preference and information is stored in a HASH MAP.
Request limit and window time happens via an API calling API, and without using any database to fetch data. Microservices have prior knowledge of rate limiting and request limit is 10/minute.



