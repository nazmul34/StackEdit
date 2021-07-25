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


<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE0ODE2Mjg4NzEsLTE0OTAyNTE1NTUsMT
YwMTY3NDA2NSwtMTA5ODk3ODg2MSwxMzE1NjE3MzcwXX0=
-->