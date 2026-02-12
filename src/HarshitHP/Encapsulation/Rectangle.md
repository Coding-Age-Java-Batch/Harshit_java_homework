public class Rectangle {

    private double length;
    private double width;

    public Rectangle(double length, double width) {
        setLength(length);   // validation ke liye setter use kiya
        setWidth(width);
    }

    public double getLength() {
        return length;
    }

    public void setLength(double length) {
        if (length > 0) {
            this.length = length;
        } else {
            System.out.println("Invalid length! Must be positive.");
        }
    }

    public double getWidth() {
        return width;
    }

    public void setWidth(double width) {
        if (width > 0) {
            this.width = width;
        } else {
            System.out.println("Invalid width! Must be positive.");
        }
    }

    public double getArea() {
        return length * width;
    }

    public double getPerimeter() {
        return 2 * (length + width);
    }

    public boolean isSquare() {
        return length == width;
    }

    public static void main(String[] args) {

        Rectangle r = new Rectangle(4, 6);

        System.out.println("Length: " + r.getLength());
        System.out.println("Width: " + r.getWidth());
        System.out.println("Area: " + r.getArea());
        System.out.println("Perimeter: " + r.getPerimeter());
        System.out.println("Is Square? " + r.isSquare());

        r.setWidth(4);

        System.out.println("After making it square:");
        System.out.println("Length: " + r.getLength());
        System.out.println("Width: " + r.getWidth());
        System.out.println("Is Square? " + r.isSquare());
    }
}
