
    public class Shape2 {
    void perimeter(){
    System.out.println("Calculating Perimeter");
    }
    }
    class square extends Shape2{
    int side;
    square(int s){
    side = s;
    }
    void permitere(){
    int p = 4*side;
    System.out.println("Perimeter of square: " +p);
    }

    static void main(String[] args) {
        square s = new square(20);
        s.permitere();
    }
    }