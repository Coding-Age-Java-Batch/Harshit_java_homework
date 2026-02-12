    public class Employee {
    String Name;
    void display(){
      System.out.println("Employee Name: " +Name);
     }
    }
    class Manager extends Employee{
    String department;
    void display(){
      System.out.println("Employee Name: " +Name);
      System.out.println("Department Name: " +department);
    }
    public static void main(String[] args){
    Manager m = new Manager();
    m.Name = "Rakesh"; 
    m.department = "IT";

     m.display();
    }
    }
