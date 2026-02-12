     public class School {
    String schoolName = "Green Valley";

    void showSchool(){
        System.out.println("School: " +schoolName);
    }
    }
    class Teacher extends School{
    String teacherName = "Mr.Sharma";

    void showTeacherDetails(){
        showSchool();
        System.out.println("Teacher: " +teacherName);
    }

    static void main(String[] args) {
        Teacher t = new Teacher();

        t.showTeacherDetails();
    }
    }
