Now lets try the function prototype in geometry elements. Monstly we give a function Shape which will have two variables (x,y)

```

function Shape(x,y){
    this.position = {x,y};

}
Shape.prototype.move = function (x,y){
    this.position.x += x;
    this.position.y += y;
    
```
(I dont understand +=x)

**Move** shape sum at the position initial, whereby, change the status
```
const figura1 = new Shape(5,10);
figura1.move(1,4);
console.log(figura1.position.x);
console.log(figura1.position.y);

```
The first element is a **Circle shape**: Remember the Circle have a parameters (x,y, radius) (x**2 + y**2 = 1)is the equation of the  Unitary circle in basic geometry. 
```
function Circle(x,y,radius){
    Shape.call(this,x,y);
    this.radius = radius; 
}
Circle.prototype = Object.create(Shape.prototype) /*Remember that  the function Object.create links the prototypes*/
const figura2 = new Circle(5,10,2);
console.log(figura2.position.x);
console.log(figura2.position.y);
console.log(figura2.radius);

```










