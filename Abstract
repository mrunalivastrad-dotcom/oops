abstract class Animal {
    abstract void sound();

    void sleep() {
        System.out.println("This animal is sleeping...");
    }
}

class Dog extends Animal {
    
    @Override
    void sound() {
        System.out.println("Dog barks: Woof! Woof!");
    }

    // The entry point of the program
    public static void main(String[] args) {
        // Create an instance of the concrete subclass
        Dog myDog = new Dog();

        // Call the implemented abstract method
        myDog.sound();

        // Call the inherited regular method
        myDog.sleep();
    }
}
