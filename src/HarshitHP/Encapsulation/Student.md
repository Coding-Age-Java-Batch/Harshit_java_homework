public class Student {

    private String name;
    private int rollNumber;
    private double mathGrade;
    private double scienceGrade;
    private double englishGrade;

    public Student(String name, int rollNumber) {
        this.name = name;
        this.rollNumber = rollNumber;
    }

    public String getName() {
        return name;
    }

    public int getRollNumber() {
        return rollNumber;
    }

    public double getMathGrade() {
        return mathGrade;
    }

    public double getScienceGrade() {
        return scienceGrade;
    }

    public double getEnglishGrade() {
        return englishGrade;
    }

    public void setMathGrade(double grade) {
        if (grade >= 0 && grade <= 100) {
            this.mathGrade = grade;
        } else {
            System.out.println("Invalid Math grade! Must be between 0-100.");
        }
    }

    public void setScienceGrade(double grade) {
        if (grade >= 0 && grade <= 100) {
            this.scienceGrade = grade;
        } else {
            System.out.println("Invalid Science grade! Must be between 0-100.");
        }
    }

    public void setEnglishGrade(double grade) {
        if (grade >= 0 && grade <= 100) {
            this.englishGrade = grade;
        } else {
            System.out.println("Invalid English grade! Must be between 0-100.");
        }
    }

    public double getAverageGrade() {
        return (mathGrade + scienceGrade + englishGrade) / 3;
    }

    public char getLetterGrade() {
        double avg = getAverageGrade();

        if (avg >= 90) {
            return 'A';
        } else if (avg >= 80) {
            return 'B';
        } else if (avg >= 70) {
            return 'C';
        } else if (avg >= 60) {
            return 'D';
        } else {
            return 'F';
        }
    }

    public static void main(String[] args) {

        Student s = new Student("Harshit", 10);

        s.setMathGrade(96);
        s.setScienceGrade(92);
        s.setEnglishGrade(87);

        System.out.println("Name: " + s.getName());
        System.out.println("Roll No: " + s.getRollNumber());
        System.out.println("Average Grade: " + s.getAverageGrade());
        System.out.println("Letter Grade: " + s.getLetterGrade());
    }
}
