    class Persion {
    void showDetails(){
      System.out.println("Person details");
     }
    }

    class Student extends Persion{
    void showDetails(){
      System.out.println("Student Details");
    }

     public static void main(String[] args){
         Student s = new Student();
         s.showDetails();
      }
     }