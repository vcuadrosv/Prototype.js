What is a Prototype in JavaScritp? 

In my opinion the prototype evidence a JSON or a  Object, which are colection not ordered of (name):(value)
The function prototype is necesary for call object in Javascrip, that is to say a JSON, in all shap. A example that is watching in internet is: 

function Person(name,age){
    this.name = name;
    this.age =age; 
}
Person.prototype.interests = ["newspaper","games"];
Person.prototype.getAge = function(){
    return this.age;
}
const juan = new Person ("Juan Ortiz", 25);
const valery = new Person("valery cuadros", 25);

console.log(juan,valery);
  
