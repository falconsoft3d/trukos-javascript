
# HTTP response status codes
```
Informational responses (100–199)
Successful responses (200–299)
Redirects (300–399)
Client errors (400–499)
Server errors (500–599)
```

# 200
```
res.status(200).json(product);
```

# 500
```
res.status(500).json(err);
```

# 400
```
res.status(401).json("Wrong credentials!");
res.status(403).json("Token is not valid!");
res.status(401).json("You are not authenticated!");
```

# Sample
```
router.post("/register", async (req, res) => {
  const newUser = new User({
    username: req.body.username,
    email: req.body.email,
    password: CryptoJS.AES.encrypt(
      req.body.password,
      process.env.PASS_SEC
    ).toString(),
  });

  try {
    const savedUser = await newUser.save();
    res.status(201).json(savedUser);
  } catch (err) {
    res.status(500).json(err);
  }
});
```
