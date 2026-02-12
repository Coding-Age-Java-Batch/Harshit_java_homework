public class Student {
String name;
int age;

    public Student(String n , int a){
        name = n;
        age = a;
        System.out.println("Name:" +name + " " + "Age:" +age);
    }
    public static void main(String[] args){

        Student s1 = new Student("Ankit", 22);
        Student s2 = new Student("Harshit", 23);

    }
}
