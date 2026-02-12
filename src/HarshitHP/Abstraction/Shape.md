    abstract class Shape {
    String name;

    Shape(String n){
        name = n;
    }
    abstract double area() ;

        public String toString () {
            return "Shape: " + name + ", Area: " + area();
        }

    }

    class Circle extends Shape{
    double radius;

    Circle(double rd){
        super("Circle");
        radius = rd;
    }

    double area(){
        return Math.PI * radius * radius;
    }
    }

    class Rectangle extends Shape{
    double width, height;

    Rectangle(double wd, double ht){
        super("Rectangle");
        width = wd;
        height = ht;
    }
    double area(){
        return width * height;
    }


    static void main(String[] args) {
        Shape c = new Circle(3);
        Shape r = new Rectangle(4,5);

        System.out.println(c);
        System.out.println(r);
    }
    }
