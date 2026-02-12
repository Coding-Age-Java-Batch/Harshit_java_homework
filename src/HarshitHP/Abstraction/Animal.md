    abstract class Animal {
    abstract void makeSound();

    void describe(){
        System.out.println("This animal makes sound: ");
    
    }
    }
    class Dog extends Animal{
    void makeSound(){
    System.out.println("Dogs Barks..");
    }
    }
    class Cat extends Animal{
    void makeSound(){
    System.out.println("Cat meows..");
    }
    }
    class Cow extends Animal{
    void makeSound(){
    System.out.println("Cow Moos..");
    }

    static void main(String[] args) {
        Animal dg = new Dog();
        Animal ct = new Cat();
        Animal cw = new Cow();

        dg.describe();
        dg.makeSound();

        ct.describe();
        ct.makeSound();

        cw.describe();
        cw.makeSound();
    }
    }