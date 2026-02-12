    class Vehicle {
 
    void displayInfo(){

    System.out.println("Generic Vehicle");
        
     } 

    } 

    class Car extends Vehicle{
    @Override

    void displayInfo(){
         System.out.println("Car: 4 Wheels");
     }

    }

    class Bike extends Vehicle{
     @Override

     void displayInfo(){
         System.out.println("Bike: 2 Wheels");
      }

     static void main(String[] args) {
         Vehicle v = new Vehicle();
         v.displayInfo();

         Vehicle c = new Car();
         c.displayInfo();

         Vehicle b = new Bike();
         b.displayInfo();
      }

    }
