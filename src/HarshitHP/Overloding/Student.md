  
    public class Student {
    void printDetails(String name, int age){
    System.out.println("Name: " + name + " Age: " + age);
     }
    void printDetails(String name, int age, String course){
    System.out.println("Name: " + name + " Age: " + age + " Course: " + course);
     }
    public static void main(String[] args){
    Student s = new Student();
    s.printDetails("Yash",22);
    s.printDetails("Harshit",21,"BCA");
     }
    }
