
## Protocols Lab

## Instructions for lab submission

1. Fork the assignment repo
1. Clone your Fork to your machine
1. Complete the lab
1. Push your changes to your Fork
1. Submit a Pull Request back to the assignment repo
1. Paste a link of the pull request on Canvas and submit

## Question 1

a. Create a Human class with two properties: 
- name of type String
- age of type Int.

Then create an initializer for the class and create two Human instances.

b. Make the Human class adopt the CustomStringConvertible protocol. Then Print both of your previously initialized
Human objects.

c. Make the Human class adopt the Equatable protocol. Two instances of Human should be considered equal
if their names and ages are identical to one another. Print the result of a boolean expression
evaluating whether or not your two previously initialized Human objects are equal to eachother
(using ==). Then print the result of a boolean expression evaluating whether or not your two
previously initialized Human objects are not equal to eachother (using !=).

d. Make the Human class adopt the Comparable protocol. One Human is greater than another Human if its age is bigger. Create another
three instances of a Human, then create an array called people of type [Human] with all of the
Human objects that you have initialized.

Create a new array called sortedPeople of type [Human] that is the people array sorted by age.

</br> </br>


## Question 2.

a. Create a protocol called Vehicle with two requirements:
- a nonsettable numberOfWheels property of type Int,
- a function called drive().

b. Define a Car struct that implements the Vehicle protocol. numberOfWheels should return a value of 4,
and drive() should print "Vroom, vroom!" Create an instance of Car, print its number of wheels,
then call drive().

c. Define a Bike struct that implements the Vehicle protocol. numberOfWheels should return a value of 2,
and drive() should print "Begin pedaling!". Create an instance of Bike, print its number of wheels,
then call drive().

</br> </br>


## Question 3.
// Given the below two protocols, create a struct for penguin(a flightless bird) and an eagle.

Give your structs some properties and have them conform to the appropriate protocols.

```swift
protocol Bird {
 var name: String { get }
 var canFly: Bool { get }
}

protocol Flyable {
 var airspeedVelocity: Double { get }
}
```

</br> </br>

## Question 4.

a. Create a protocol called Transformation.  The protocol should specify a mutating method called transform

b. Make an enum called SuperHero that conforms to Transformation with cases `notHulk` and `hulk`

c. Create an instance of it named `bruceBanner`. Make it so that when the transform function is called that bruceBanner turns from
`.notHulk` to `.hulk.``

```swift
enum SuperHero: Transformation {
    // write code here.
}

// Example Output:
var bruceBanner = SuperHero.notHulk

bruceBanner.transform() . // hulk

bruceBanner.transform()  // notHulk
```

</br> </br>


## Question 5.

a. Create a protocol called Communication

b. Give it a property called `message`, of type String, and assign it an explicit getter.

c. Create three Classes. `Cow`, `Dog`, `Cat`.

d. Have your three classes conform to Communication

e. `message` should return a unique message for each animal when talk is called.

f. Put an instance of each of your Classes in an array.

g. Iterate over the array and have them print talk.
