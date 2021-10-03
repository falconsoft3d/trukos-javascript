```
npm install -g json-server
```

Create a db.json file with some data
```

  "posts": [
    { "id": 1, "title": "json-server", "author": "typicode" }
  ],
  "comments": [
    { "id": 1, "body": "some comment", "postId": 1 }
  ],
  "profile": { "name": "typicode" }
}
```

```
json-server --watch db.json
```

```
http://localhost:3000/posts/1
```

```
GET    /posts
GET    /posts/1
POST   /posts
PUT    /posts/1
PATCH  /posts/1
DELETE /posts/1
```

```
GET    /profile
POST   /profile
PUT    /profile
PATCH  /profile
```

