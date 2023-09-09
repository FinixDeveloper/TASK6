var Circle = (function () {
    function Circle(radius, color) {
        this.radius = 1.0;
        this.color = "red";
        if (typeof (radius) !== "undefined") {
            this.radius = radius;
        }
        if (typeof (color) !== "undefined") {
            this.color = color;
        }
    }
    Circle.prototype.getRadius = function () {
        return this.radius;
    };
    Circle.prototype.setRadius = function (radius) {
        this.radius = radius;
    };
    Circle.prototype.getColor = function () {
        return this.color;
    };
    Circle.prototype.setColor = function (color) {
        this.color = color;
    };
    Circle.prototype.toString = function () {
        return "Radius: " + this.radius + " Color: " + this.color;
    };
    Circle.prototype.getArea = function () {
        return (2 * (Math.PI) * this.radius);
    };
    Circle.prototype.getCircumference = function () {
        return (2 * this.radius);
    };
    return Circle;
}());
var value1 = new Circle();
console.log("Constructor with no params: " + value1.toString());
var value2 = new Circle(3.5);
console.log("Constructor with one params: " + value2.toString());
var value3 = new Circle(2.2, 'Yellow');
console.log("getRadius: " + value3.getRadius());
value3.setRadius(3.3);
console.log("Radius value after setRadius: " + value3.getRadius());
console.log("getColor: " + value3.getColor());
value3.setColor("orange");
console.log("Color Value after setColor: " + value3.getColor());
console.log(value3.toString());
console.log("Area: " + value3.getArea());
console.log("Circumference: " + value3.getCircumference());
