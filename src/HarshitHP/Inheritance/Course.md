    class Course {
    String courseName;
    Course(String cn){
    courseName = cn;
    }

     void showCourse(){
         System.out.println("Course Name: " +courseName);
     }
    }

    class EnrolledStudent extends Course{
    String studentName;
    int rollNo;

     EnrolledStudent(String courseName, String sn, int rn){
         super(courseName);
         studentName = sn;
         rollNo = rn;
     }

     void showCourse(){
         System.out.println("Course Name: " +courseName);
         System.out.println("Student Name: " +studentName);
         System.out.println("Roll No: " +rollNo);
     }

    static void main(String[] args) {
        EnrolledStudent es = new EnrolledStudent("Java Programming","Harshit",10);
        es.showCourse();
    }
    }
