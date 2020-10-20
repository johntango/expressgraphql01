# expressgraphql01

# GraphQL

## here are the query and mutation structures

query getContacts{
contacts{
name
email
}
query getContact($iid: Int = 1){
    contact(id:$id){
name
email
}
}

mutation setContacts{
setContact(input: {
name: "john williams",
email: "jrw@mit.edu",
age:50
}){
name
email
age
}
}

query getContacts{
contacts{
name
email
}
}
mutation deleteContacts($idd: Int = 1){
  deleteContact(id: $idd){
ok
}
}

mutation editContacts($idd: Int = 1, $age: Int = 35){
editContact(id: $idd, age: $age){
name
age
}
}
