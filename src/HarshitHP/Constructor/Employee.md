public class Employee {
int id;
String name;
String Department;

    public Employee(int i,String n, String dpt){
        id = i;
        name = n;
        Department = dpt;
    }
    Employee(int i, String n){
        id = i;
        name = n;
        Department = "General";
    }
    void displayDetails(){
        System.out.println("Id: " +id);
        System.out.println("Name: " +name);
        System.out.println("Department: " +Department);
        System.out.println("       ");
    }

    static void main(String[] args) {
        Employee e1 = new Employee(101,"Aman","IT");
        Employee e2 = new Employee(102,"Rahul");

        e1.displayDetails();
        e2.displayDetails();
    }
}
