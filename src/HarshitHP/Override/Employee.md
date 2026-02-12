    public class Employee {
    int getBonus(){
    return 1000;
     }
    }
    class Manager extends Employee{
    int getBonus(){
    return 2000;
     }
    }
    class Developer extends Employee{
    int getBonus(){
    return 3000;
    }

    static void main(String[] args) {
        Employee e = new Employee();
        Manager m = new Manager();
        Developer d = new Developer();

        System.out.println("Employee Bonus: " +e.getBonus());
        System.out.println("Manager Bouns: " +m.getBonus());
        System.out.println("Developer Bonus: " +d.getBonus());
     }
    }
