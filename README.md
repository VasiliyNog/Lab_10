# Lab_10
import java.util.ArrayList;
 
public class ListObjects {
    public static void main(String[] args) {
        ArrayList<Animal> house = new ArrayList<>();
        house.add(new Cat());
        house.add(new Dog());
        house.add(new Dog());
 
        for (Animal animal : house) {
            animal.voice();
        }
    }
}
 
abstract class Animal {
    abstract void voice();
}
 
class Cat extends Animal {
    void voice() {
        System.out.println("Meow");
    }
}
 
class Dog extends Animal {
    void voice() {
        System.out.println("Woof");
    }
}
