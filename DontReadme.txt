/*Наследование*/
public class Animal {
	//...
}
public class Dog extends Animal {
	//...
}

/*Инкапсуляция*/
public class Student {
	private String name;
	public String getName(){
	return name;
	}
	public void setName(String name){
	this.name = name;
	}
}
class Test {
	public static void main(String[] args) {
	Student student1 = new Student();
	student1.setName("John");
	System.out.println(student1.getName);
	}
}

/*Абстракция*/
public class Animals {
	private String type;
	private int weight;
	public Animals (String type, int weight){
	this.type = type;
	this.weight = weight;
	} 
	public void displayInfo() {
	System.out.println(type+" весит "+weight+" кг.");
	}
}
public class Main {
	public static void main(String[] args) {
		Animals cat = new Animals ("Кошка", 5);
		Animals dog = new Animals ("Собака", 10);
		cat.displayInfo();
		dog.displayInfo();
	}
}

/*Полиморфизм*/
class Animal {
	void sound() {
	System.out.println("...звук");
	}
}
class Dog extends Animal {
	void sound() {
	System.out.println("собака гавкает");
	}
}
class Cat extends Animal {
	void sound() {
	System.out.println("кошка мяукает");
	}
}
public class Main {
	public static main(String[] args) {
	Animal myDog = new Dog();
	Animal myCat = new Cat();
	myDog.sound();
	myCat.sound();
	}
}
