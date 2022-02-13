
Node.js/Express Customer CRUD using GraphQL and JSON-Server

- install dependencies
- run (npm run json)
- run (npm run dev)
-Visit Graphiql IDE at  http://localhost:4000/graphql and try these functions.

 get all customers
 {
   customers {
     id,name
   }
 }

 get customer by id
 {
   customer(id:"1") {
     id,name
   }
 }

 add new customer
 mutation{
   addCustomer(
     name:"khizram saeed khan",
     email:"khizram@decotechs.com",
     age:22
   ){
     name,email,id
   }
 }


 delete a customer by id
 mutation{
   deleteCustomer(id: "5"){
     name,email,id
   }
 }

 edit customer info by id
 mutation{
   editCustomer(id: "4" , name:"Jen Thompson Updated"){
     name,email,id
   }
 }