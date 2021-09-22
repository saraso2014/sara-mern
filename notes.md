# MongoDB Driver Connection .js
```
const { MongoClient } = require('mongodb');
const uri = "mongodb+srv://mern:<password>@cluster0.whaax.mongodb.net/myFirstDatabase?retryWrites=true&w=majority";
const client = new MongoClient(uri, { useNewUrlParser: true, useUnifiedTopology: true });
client.connect(err => {
  const collection = client.db("test").collection("devices");
  // perform actions on the collection object
  client.close();
});

# MongoDB Connection Driver String
```mongodb+srv://mern:<password>@cluster0.whaax.mongodb.net/myFirstDatabase?retryWrites=true&w=majority