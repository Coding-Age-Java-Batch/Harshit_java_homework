    public class Student {

    String name;
    int RollNo;
    float marks;

    void SetDetails(String n, int rn, float m){
        name = n;
        RollNo = rn;
        marks = m;
    }

    void displayInfo(){
        System.out.println("Student name is : " +name);
        System.out.println("Student RollNo is : " +RollNo);
        System.out.println("Student name is : " +marks);
    }

    void haspassed(){
        if(marks>=40){
            System.out.println("True");
        }
        else{
            System.out.println("False");
        }
    }
    public static void main(String[] args){
        Student s = new Student();

        s.SetDetails("Harshit",01,84.65f);
        s.displayInfo();
        s.haspassed();
    }
}
