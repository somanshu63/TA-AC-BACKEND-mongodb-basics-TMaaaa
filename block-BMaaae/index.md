writeCode

Write code to:-

- create a database named `sports`.
  //use sports

- list all databases present in local mongod server.
  //show dbs

- create 3 collections named `cricket`, `football`, `TT` in sports databse.
  //db.createCollection("cricket")
  //db.createCollection("football")
  //db.createCollection("TT")

- add multiple players in those collections which should have fields like `name`, `age` and `email` and `bid_price`.
  //db.TT.insertMany([{name: "keran bell", age: 24, email: "keran@gmail.com", bid_price: 1500 }, {name: "john", age: 23, email: "john@gmail.com", bid_price: 1200 }])
  //db.football.insertMany([{name: "keran bell", age: 24, email: "keran@gmail.com", bid_price: 900 }, {name: "john", age: 23, email: "john@gmail.com", bid_price: 800 }])
  //db.cricket.insertMany([{name: "keran bell", age: 24, email: "keran@gmail.com", bid_price: 500 }, {name: "john", age: 23, email: "john@gmail.com", bid_price: 600 }])

- list all collections in sports database.
  //show collections

- rename `TT` collection to `tennis`.
  //db.TT.renameCollection("tennis")

- create a capped collection called `khokho` which should have max 3 documents.
  //db.createCollection("khokho", {capped: true, size:10000, max:3})

  Try inserting more than 3 and see what happens?

- check whether a collection is capped or not?
  //db.khokho.isCapped()

- drop all documents from `football` collection.
  //db.football.remove({})

- delete cricket collection completely.
  //db.cricket.drop()

- delete sports database.
  //db.dropDatabase()

- check which database you are connected to ?
  //db

- connect to test database
  //use test
