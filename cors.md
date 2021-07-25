## Cors
1. Using app.use(cors()); removes cors error.
2. **Example:** Access to XMLHttpRequest at 'http://localhost:8000/posts' from origin 'http://localhost:3000' has been blocked by CORS policy: No 'Access-Control-Allow-Origin' header is present on the requested resource.

## Access-Control-Allow-Origin
1. **Setup** : app.use(cors({origin: 'http://localhost:3000'}))
2. **Or** res.header('Access-Control-Allow-Origin', 'http://localhost:3000');
3. use 



<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE5MTQxNjA4MjgsLTEwOTg5Nzg4NjEsMT
MxNTYxNzM3MF19
-->