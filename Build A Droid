public class Droid {
// instance fields
  String name;
  int batteryLevel;
  String performTask;
  
// constructor method
  public Droid(String droidName){
    name = droidName;
    batteryLevel = 100;
  }
  
// methods
  public String performTask(String task){
    performTask = task;
    batteryLevel -= 10;
    return name + " is performing task: " + task;   
  }

// method  
  public void energyReport(){
    System.out.println( name + "'s battery level is now " + batteryLevel);
  }
// method
  public static String energyTransfer(Droid droidA, Droid droidB){
    int a = droidA.batteryLevel;
    int b = droidB.batteryLevel;
    droidB.batteryLevel = b;
    droidA.batteryLevel = a;
    return droidA + " is now " + a + " and " + droidB + " is now " + b + ".";
  }
// main method
  public static void main(String[] args){
    Droid firstDroid = new Droid("Codey");
    // Before performing task 
    System.out.println(firstDroid);
    System.out.println("The battery level before " + firstDroid.name + " performing task: " + firstDroid.batteryLevel + ".");
    // Ａfter performing task
    System.out.println(firstDroid.performTask("dancing"));
    System.out.println("The battery level after " + firstDroid.name + " performing task: " + firstDroid.batteryLevel + ".");

    Droid secondDroid = new Droid("Ray");
    //System.out.println(secondDroid.performTask("jumping"));
    System.out.println("The battery level after " + secondDroid.name + " performing task: " + secondDroid.batteryLevel + ".");

System.out.println("After energy transfering...");
    // tranfering energy ***
    energyTransfer(firstDroid, secondDroid);
    
    // reporting energy ***
    firstDroid.energyReport();
    secondDroid.energyReport();
  }

  public String toString(){
    return "Hello, I'm the droid: " + name;
  }

}
