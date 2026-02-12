    class LivingBeing {
    void breath(){
     System.out.println("Breathing...");
    }
    }
    class Animal1 extends LivingBeing{
    void eat(){
     System.out.println("Eating...");
    }
    }
    class Dog1 extends Animal1{
    void brak(){
    System.out.println("Barking...");
    }
    public static void main(String[] args){
     Dog1 d = new Dog1();
      d.breath();
      d.eat();
      d.brak();
     }
    }
