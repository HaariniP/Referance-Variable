# Referance-Variable
class Student {
    String name;
    void display() {
        System.out.println("Student Name: " + name);
    }
}

public class ReferenceVariableExample {
    public static void main(String[] args) {
        Student student1 = new Student();
        student1.name = "Alice";
        Student student2 = student1;
        System.out.println("Using student1 reference:");
        student1.display();
        System.out.println("Using student2 reference:");
        student2.display();
        student2.name = "Bob";
        System.out.println("\nAfter modifying through student2:");
        student1.display();
        student2.display();
    }
}
