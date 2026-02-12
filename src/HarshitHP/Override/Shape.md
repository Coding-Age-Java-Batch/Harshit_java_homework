    class Shape {
    void draw(){
    System.out.println("Drawing Shape");
     }
    }
    class Circle extends Shape{
    @Override
    void draw(){
    System.out.println("Drawing Circle");
    }

    void draw(int radius){
        System.out.println("Drawing circle of radius: " +radius);
     }
    }
    class Rectangle extends Shape{
    @Override
    void draw(){
    System.out.println("Drawing rectangle");
    }

    static void main(String[] args) {
        Shape s = new Shape();
        s.draw();

        Circle c = new Circle();
        c.draw();
        c.draw(5);

        Rectangle r = new Rectangle();
        r.draw();
      }
    }
