# Assignment-15.1

1.Write a simple program to show inheritance in scala.

class Employee{  
    var salary:Float = 10000  
}  
  
class Programmer extends Employee{  
    var bonus:Int = 5000  
    println("Salary = "+salary)  
    println("Bonus = "+bonus)  
}  
  
object MainObject{  
    def main(args:Array[String]){  
        new Programmer()  
    }  
}  

Output:

Salary = 10000.0
Bonus = 5000


2.Write a simple program to show multiple inheritance in scala.

class A{  
    var salary1 = 10000  
}  
  
class B extends A{  
    var salary2 = 20000  
}  
  
class C extends B{  
    def show(){  
        println("salary1 = "+salary1)  
        println("salary2 = "+salary2)  
    }  
}  
  
object MainObject{  
    def main(args:Array[String]){{    
        var c = new C()  
        c.show()  
      
    }  
}  
Output:

salary1 = 10000
salary2 = 20000
