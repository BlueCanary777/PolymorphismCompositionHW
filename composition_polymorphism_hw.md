```# Polymorphism & Composition Homework - Quiz

# Polymorphism

1. What does the ___word___ 'polymorphism' mean?

Polymorphism is the ability to utilise objects such that functions originally
associated with a different class objects can be performed upon them, resulting in objects
which can be combined in a single array list.

2. What does it mean when we apply polymorphism to OO design? Give a simple Java example.

public class Network {
    private String name;
    private ArrayList<Desktop> devicesDesktop;
    private ArrayList<Printer> devicesPrinter;


3. What can we use to implement polymorphism in Java?

An interface.

4. How many 'forms' can an object take when using polymorphism?

Theoretically unlimited.

5. Give an example of when you could use polymorphism.

A factory producing 20 different gadgets requiring a status data
(applying same Java method) from each at switch on and during testing.



# Composition

6. What do we mean by 'composition' in reference to object-oriented programming?

An object's ability to reference a group of behaviours
available to other objects.

7. When would you use composition? Provide a simple example in Java.

To enable individual objects to access the method/s they need from
one common interface while minimising the code necessary to achieve that.

package device_management;
import behaviours.IOutput;
public class Printer extends PrintingDevice implements IOutput

package device_management;
import behaviours.IOutput;
public class Monitor extends VideoDevice implements IOutput


8. What is/are the advantage(s) of using composition?

DRY coding and flexibility.

9. What happens to the behaviours when the object composed of them is destroyed?

They too are destroyed.
