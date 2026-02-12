    public class Parent { 
    Parent(){
      System.out.println("Parent constructor called");
    }
    }

    class Child extends Parent{
    Child(){
    System.out.println("Child constructor called");
    }
    public static void main(String[] args){
     Child c = new Child();
     }
    }