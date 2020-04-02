# All start from use cases

## What is differences between Class and Object?
   - ....
## Final
   - Not be changed
   - Must be init when instantiate a object
## Static
  - It belongs to class not object
  
## Encapsulation
  - access label
  
| Modifier | class | package | subclass | world |  
|----------|-------|---------|----------|-------|
|  Public  |  Y    |   Y     |   Y      |  Y    |
| Potected |  Y    |   Y     |   Y      |  N    |
| Modifier |  Y    |   Y     |   N      |  N    |
| Private  |  Y    |   N     |   N      |  N    |

## Signature
   - make the apporpriate name to avoid change later
   
## API:
   - define to public
## Internal implementation(helper function): 
   - define private
## 'default' in Java
   - private
## Inheritance
   - one drived class(subclass) only can inherit one base class
## Interface vs. Abstract class
   - They are cannot be new
   - Interface no have implementation, just include method definition
   - Abstract class has implementations, and data fields
   
         interface <interface_name>{  

          // declare constant fields  
          // declare methods that abstract   
          // by default.  
         }  
   
## Extend
   - only can extend one class
   - class extends class
   - interface extends class
## Implement
   - could implement multiple interface
   - class implements interface
## Polymorphism
   - Although same use class, each can find itself implementation
   - hashtable to implement this function
## Overloading and Overriding
   - Overloading occurs when two or more methods in one class have the same method name but different parameters.
   - Overriding means having two methods with the same method name and parameters.
   
  Example: Overriding
   
      class Dog{
          public void bark(){
              System.out.println("woof ");
          }
      }
      class Hound extends Dog{
          public void sniff(){
              System.out.println("sniff ");
          }

          public void bark(){
              System.out.println("bowl");
          }
      }

  Example: Overloading
    
      class Dog{
          public void bark(){
              System.out.println("woof ");
          }

          //overloading method
          public void bark(int num){
            for(int i=0; i<num; i++)
              System.out.println("woof ");
          }
      }
