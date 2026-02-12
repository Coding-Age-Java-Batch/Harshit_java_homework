    public class College {
    String CollegeName = "Techno insitute";

    }
    class Admission extends College{
    String StudentName = "Harshit";
    String CourseName = "B.Tech";

    void showDetails(){
        System.out.println("College Name: " +CollegeName);
        System.out.println("Student Name: " +StudentName);
        System.out.println("Course Name: " +CourseName);
    }

    static void main(String[] args) {
        Admission ad = new Admission();
        ad.showDetails();
    }
}
