    public class Food {
    String FoodName = "Gulab Jamun";

    void display(){
        System.out.println("Food Name: " +FoodName);
    }
    }
    class Dessert extends Food {
    String SweetnessLevel = "High";

    void display(){
        System.out.println("Food Name: " +FoodName);
        System.out.println("SweetnessLevel: " +SweetnessLevel);
    }

    static void main(String[] args) {
        Dessert d = new Dessert();
        d.display();
     }
    }
