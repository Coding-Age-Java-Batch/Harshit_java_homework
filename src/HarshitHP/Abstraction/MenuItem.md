abstract class MenuItem {

    protected String name;
    protected double price;

    MenuItem(String name, double price) {
        this.name = name;
        this.price = price;
    }
    
    abstract void prepare();
    
    void printPrice() {
        System.out.println(name + " Price: ₹" + price);
    }
}

class VegBurger extends MenuItem {

    VegBurger(double price) {
        super("Veg Burger", price);
    }

    void prepare() {
        System.out.println("Preparing Veg Burger:");
        System.out.println("- Grilling veg patty");
        System.out.println("- Adding lettuce and sauce");
        System.out.println("- Assembling bun");
    }
}

class ChickenBurger extends MenuItem {

    ChickenBurger(double price) {
        super("Chicken Burger", price);
    }

    void prepare() {
        System.out.println("Preparing Chicken Burger:");
        System.out.println("- Frying chicken patty");
        System.out.println("- Adding mayo and cheese");
        System.out.println("- Assembling bun");
    }
}

class ColdDrink extends MenuItem {

    ColdDrink(double price) {
        super("Cold Drink", price);
    }

    void prepare() {
        System.out.println("Preparing Cold Drink:");
        System.out.println("- Filling glass with ice");
        System.out.println("- Pouring chilled drink");
    }

    public static void main(String[] args) {

        MenuItem m1 = new VegBurger(120);
        MenuItem m2 = new ChickenBurger(180);
        MenuItem m3 = new ColdDrink(60);

        m1.prepare();
        m1.printPrice();
        System.out.println();

        m2.prepare();
        m2.printPrice();
        System.out.println();

        m3.prepare();
        m3.printPrice();
    }
}
