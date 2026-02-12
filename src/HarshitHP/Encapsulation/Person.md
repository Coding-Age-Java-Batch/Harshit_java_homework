public class Person {

        private String name;
        private int age;
        private String email;

        public Person(String name, int age, String email) {
            this.name = name;
            setAge(age);
            setEmail(email);
        }

        public String getName() {
            return name;
        }

        public int getAge() {
            return age;
        }

        public String getEmail() {
            return email;
        }

        public void setName(String name) {
            this.name = name;
        }

        public void setAge(int age) {
            if (age >= 0 && age <= 120) {
                this.age = age;
            } else {
                System.out.println("Invalid age! Age must be between 0 and 120.");
            }
        }

        public void setEmail(String email) {
            if (email.contains("@")) {
                this.email = email;
            } else {
                System.out.println("Invalid email! Email must contain '@'.");
            }
        }

        @Override
        public String toString() {
            return "Name: " + name +
                    ", Age: " + age +
                    ", Email: " + email;
        }

    public static void main(String[] args) {

        Person p1 = new Person("Harshit", 20, "harshit@gmail.com");

        p1.setAge(25);
        p1.setAge(-5);

        p1.setEmail("newharshit@gmail.com");

        System.out.println(p1);
    }
}