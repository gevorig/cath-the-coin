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