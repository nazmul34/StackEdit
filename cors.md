## Cors
1. Using app.use(cors()); removes cors error.
2. **Example:** Access to XMLHttpRequest at 'http://localhost:8000/posts' from origin 'http://localhost:3000' has been blocked by CORS policy: No 'Access-Control-Allow-Origin' header is present on the requested resource.

## Access-Control-Allow-Origin
1. **Setup** : app.use(cors({origin: 'http://localhost:3000'}))
2. **Or** res.header('Access-Control-Allow-Origin', 'http://localhost:3000');
3. Replace  'http://localhost:3000' with '*' to allow all website. 

## Access-Control-Allow-Headers
The  **`Access-Control-Allow-Headers`**  response header is used in response to a  [preflight request](https://developer.mozilla.org/en-US/docs/Glossary/Preflight_request)  which includes the  [`Access-Control-Request-Headers`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Access-Control-Request-Headers)  to indicate which HTTP headers can be used during the actual request.

This header is required if the request has an  [`Access-Control-Request-Headers`](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Access-Control-Request-Headers)  header.

## Access-Control-Allow-Credentials
1. By default it is false, usually this header is used for sending cookie token to the browser.
2. The  **`Access-Control-Allow-Credentials`**  response header tells browsers whether to expose the response to frontend JavaScript code when the request's credentials mode ([`Request.credentials`](https://developer.mozilla.org/en-US/docs/Web/API/Request/credentials)) is  `include`.
When a request's credentials mode ([`Request.credentials`](https://developer.mozilla.org/en-US/docs/Web/API/Request/credentials)) is  `include`, browsers will only expose the response to frontend JavaScript code if the  `Access-Control-Allow-Credentials`  value is  `true`.
Credentials are cookies, authorization headers or TLS client certificates.
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE2ODE0ODI1NywtMTQ5MDI1MTU1NSwxNj
AxNjc0MDY1LC0xMDk4OTc4ODYxLDEzMTU2MTczNzBdfQ==
-->