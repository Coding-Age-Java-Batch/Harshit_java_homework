    public class PtShape {
    void printShape(){
    System.out.println("This is a Shape");
     }
    }
    class square extends PtShape{
    void printShape(){
    System.out.println("This is a square");
     }
    }
    class Triangle extends PtShape{
    void printShape(){
    System.out.println("This is a Triangle");
    }

    static void main(String[] args) {
        PtShape ps = new PtShape();
        ps.printShape();

        square s = new square();
        s.printShape();

        Triangle t = new Triangle();
        t.printShape();
     }
    }