## Cors
1. Using app.use(cors()); removes cors error.
2. **Example:** Access to XMLHttpRequest at 'http://localhost:8000/posts' from origin 'http://localhost:3000' has been blocked by CORS policy: No 'Access-Control-Allow-Origin' header is present on the requested resource.

## Access-Control-Allow-Origin
1. **Setup** : app.use(cors({origin: 'http://localhost:3000'}))
2. **Or** res.header('Access-Control-Allow-Origin', 'http://localhost:3000');
3. Replace  'http://localhost:3000' with '*' to allow all website. 



<!--stackedit_data:
eyJoaXN0b3J5IjpbMTYwMTY3NDA2NSwtMTA5ODk3ODg2MSwxMz
E1NjE3MzcwXX0=
-->