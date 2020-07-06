# read 07 API
API keys are a simple encrypted string that identifies an application without any principal


SuperAgent 

SuperAgent is light-weight progressive ajax API crafted for flexibility, readability, and a low learning curve after being frustrated with many of the existing request APIs. It also works with Node.js!

## Test documentation
The following test documentation was generated with Mocha's "doc" reporter, and directly reflects the test suite. This provides an additional source of documentation.

Request basics
A request can be initiated by invoking the appropriate method on the request object, then calling .then() (or .end() or await) to send the request. For example a simple GET request:
```
 request
   .get('/search')
   .then(res => {
      // res.body, res.headers, res.status
   })
   .catch(err => {
      // err.message, err.response
   });
   ```


   ## JSON / Urlencoded
   The property res.body is the parsed object, for example if a request responded with the JSON string '{"user":{"name":"tobi"}}', res.body.user.name would be "tobi". Likewise the x-www-form-urlencoded value of "user[name]=tobi" would yield the same result. Only one level of nesting is supported. If you need more complex data, send JSON instead.

   ## Response properties
   1. Response text : `res.text`
2. Response body : ` res.body`
3. Response header fields : ` res.header`
4. Response Content-Type : ` res.type`
5. Response status : ` res.status`

## Authentication


In both Node and browsers auth available via the .auth() method:
```
request
  .get('http://local')
  .auth('tobi', 'learnboost')
  .then(callback);
  ```

  # The End