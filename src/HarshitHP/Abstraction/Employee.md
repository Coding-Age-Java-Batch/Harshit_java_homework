    abstract class Employee {
    String name;

    Employee(String n){
        name = n;
    }
    abstract  double calculateSalary();

    }
    class FullTimeEmployee extends Employee{
    FullTimeEmployee(String name){
    super(name);
    }
    double calculateSalary(){
    return 50000;
    }
    }
     class PArtTimeEmployee extends Employee{
    int hoursWorked;

    PArtTimeEmployee(String name, int hw){
        super(name);
        hoursWorked = hw;
    }
    double calculateSalary(){
        return hoursWorked * 500;
    }

    static void main(String[] args) {
        Employee e1 = new FullTimeEmployee("Rahul");
        Employee e2 = new PArtTimeEmployee("Aman",40);

        System.out.println("Employee: " + e1.name + ",Salary: " + e1.calculateSalary());
        System.out.println("Employee: " +e2.name + ", Salary: " +e2.calculateSalary());

    }
    }
