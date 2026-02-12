    public class Greeter {
    void greet(){
    System.out.println("Hello");
     }
    void greet(String Name){
    System.out.println("Hello, " + Name);
     }
    void greet(String Name , String time){
    System.out.println("Good " + time + "," + Name);
     }

    static void main(String[] args) {
        Greeter g = new Greeter();
        g.greet();
        g.greet("Annu");
        g.greet("Annu","Morning");
     }
    }
