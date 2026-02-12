public class Circle {

    private double radius;

    public Circle(double radius) {
        setRadius(radius);
    }

    public void setRadius(double radius) {
        if (radius > 0) {
            this.radius = radius;
        } else {
            System.out.println("Invalid radius! Radius must be positive.");
        }
    }

    public double getRadius() {
        return radius;
    }

    // Calculate Area (π × r²)
    public double getArea() {
        return Math.PI * radius * radius;
    }

    // Calculate Circumference (2 × π × r)
    public double getCircumference() {
        return 2 * Math.PI * radius;
    }

    // Calculate Diameter (2 × r)
    public double getDiameter() {
        return 2 * radius;
    }

    public static void main(String[] args) {

        Circle c = new Circle(5);

        System.out.println("Radius: " + c.getRadius());
        System.out.println("Area: " + c.getArea());
        System.out.println("Circumference: " + c.getCircumference());
        System.out.println("Diameter: " + c.getDiameter());

        c.setRadius(10);
        
        System.out.println("\nAfter changing radius to 10:");
        System.out.println("Radius: " + c.getRadius());
        System.out.println("Area: " + c.getArea());
        System.out.println("Circumference: " + c.getCircumference());
        System.out.println("Diameter: " + c.getDiameter());
    }
}