abstract class Student {

    protected String name;
    protected int rollNo;

    Student(String name, int rollNo) {
        this.name = name;
        this.rollNo = rollNo;
    }

    abstract void generateReport();
}

class EngineeringStudent extends Student {

    private int marks;

    EngineeringStudent(String name, int rollNo, int marks) {
        super(name, rollNo);
        this.marks = marks;
    }

    void generateReport() {
        System.out.println("---- Engineering Student Report ----");
        System.out.println("Name: " + name);
        System.out.println("Roll No: " + rollNo);

        if (marks < 0 || marks > 100) {
            System.out.println("Invalid marks: " + marks);
            return;
        }

        System.out.println("Marks: " + marks);
        System.out.println("Result: " + (marks >= 40 ? "PASS" : "FAIL"));
    }
}

class MedicalStudent extends Student {

    private int marks;

    MedicalStudent(String name, int rollNo, int marks) {
        super(name, rollNo);
        this.marks = marks;
    }

    void generateReport() {
        System.out.println("---- Medical Student Report ----");
        System.out.println("Name: " + name);
        System.out.println("Roll No: " + rollNo);

        if (marks < 0 || marks > 100) {
            System.out.println("Invalid marks: " + marks);
            return;
        }

        System.out.println("Marks: " + marks);
        System.out.println("Result: " + (marks >= 40 ? "PASS" : "FAIL"));
    }
    public static void main(String[] args) {

        Student s1 = new EngineeringStudent("Rahul", 101, 75);
        Student s2 = new MedicalStudent("Anita", 202, 35);
        Student s3 = new EngineeringStudent("Amit", 303, 150);

        s1.generateReport();
        System.out.println();

        s2.generateReport();
        System.out.println();

        s3.generateReport();
    }
}
