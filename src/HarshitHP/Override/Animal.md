    class Animal {
     void makeSound(){
      System.out.println("Animal Makes Sound");
     }
    }
    class Dog extends Animal{
    void makeSound(){
      System.out.println("Dog Barks...");
     }
    }
    class Cat extends Animal{
    void makeSound(){
      System.out.println("Cat Meows..."); 
    }

    static void main(String[] args) {
        Animal a = new Animal();
        a.makeSound();

        Animal d = new  Dog();
        d.makeSound();

        Animal c = new Cat();
        c.makeSound();


     }
    }
