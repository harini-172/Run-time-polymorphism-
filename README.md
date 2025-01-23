# Run-time-polymorphism-
package vehicletest;
class Vehicle {
    public void start() {
        System.out.println("Vehicle is starting");
    }
}
class Car extends Vehicle {
    @Override
    public void start() {
        System.out.println("Car is starting with key");
    }
}
class Motorcycle extends Vehicle {
    @Override
    public void start() {
        System.out.println("Motorcylce is starting with a kick");
        
    }
}

/**
 *
 * @author 1BSCCSA35
 */
public class VehicleTest {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
        Vehicle v1 = new Vehicle();
        Vehicle v2 = new Car();
        Vehicle v3 = new Motorcycle ();
        
        v1.start();
        v2.start();
        v3.start();
    }
    
}
output:
Vehicle is starting
Car is starting with key
Motorcylce is starting with a kick
