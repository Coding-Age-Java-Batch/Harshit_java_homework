    class Animal2 {
    void eat(){
     System.out.println("Animal is Eating");
     }
    }
    class Cat extends Animal{
    void eat(){
     System.out.println("Cat is Eating");
     }
    void sound(){
     System.out.println("Cat meows");
     }

    static void main(String[] args) {
        Cat c = new Cat();
        c.eat();
        c.sound();
     }
    }
