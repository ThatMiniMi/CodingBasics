# C# Basics

This cheat sheet covers essential C# syntax, structure, and concepts used in .NET development. It focuses on the building blocks needed to write and understand simple programs.

---

## Program Structure

```csharp
using System; // Imports the System namespace which contains basic classes like Console.

namespace MyApp // Defines a namespace to organize code and avoid name conflicts.
{
    class Program // Defines a class named Program.
    {
         // The Main method is the entry point of the program.
        // 'static' means it belongs to the class, not an instance.
        // 'void' means this method does not return any value.
        static void Main(string[] args)
        {
            Console.WriteLine("Hello, world!"); // Prints text to the console.
        }
    }
}

## Variables and Data Types

int number = 5;             // Integer (whole number)
string name = "John";       // Text value
bool isActive = true;       // Boolean: true or false values (used for conditions)
double price = 9.99;        // Decimal number with double precision
char grade = 'A';           // Single character

//Use var to let the compiler infer the type.

var total = 100; // Compiler infers this as an int.

## Boolean Values

//Booleans are simple true or false values used to control logic.

bool isRaining = false;  // False means "no" or "off"
bool isSunny = true;     // True means "yes" or "on"

## Access Modifiers: public vs private

//public: Members (variables, methods) can be accessed from anywhere.

//private: Members can only be accessed inside the same class (hidden from outside).

class Person
{
    public string Name;        // Can be accessed anywhere
    private int Age;           // Only accessible inside the Person class

    public void SetAge(int age) // Public method to change private Age
    {
        Age = age;
    }

    private void SecretMethod() // Private method, only used inside the class
    {
        Console.WriteLine("This is private.");
    }
}

## Conditionals

if (age >= 18)           // If age is 18 or more
{
    Console.WriteLine("Adult");
}
else if (age >= 13)      // Else if age is 13 or more (but less than 18)
{
    Console.WriteLine("Teen");
}
else                     // Otherwise
{
    Console.WriteLine("Child");
}

## Loops

//For Loop: Repeats code a set number of times.
for (int i = 0; i < 5; i++)
{
    Console.WriteLine(i);
}

//While Loop: Repeats code while a condition is true.
int i = 0;
while (i < 5)
{
    Console.WriteLine(i);
    i++;
}

//Foreach Loop: Loops over each item in a collection.
string[] names = { "Anna", "Ben", "Chris" };

foreach (string n in names)
{
    Console.WriteLine(n);
}

## Methods //Functions

// Method that returns an int value.
static int Add(int a, int b)
{
    return a + b;
}

// 'void' means this method does not return any value.
public void PrintHello()
{
    Console.WriteLine("Hello!");
}

## Classes and Objects

class Person
{
    public string Name;   // Public field accessible outside the class
    public int Age;

    public void Greet()   // Public method
    {
        Console.WriteLine($"Hi, I'm {Name} and I'm {Age} years old.");
    }
}

// Using the class
Person p = new Person();
p.Name = "Alice";
p.Age = 30;
p.Greet(); // Output: Hi, I'm Alice and I'm 30 years old.

## Properties // Auto-Implemented

// Properties provide controlled access to fields and can include logic.

class Car
{
    public string Model { get; set; }  // Public property with get and set accessors
    public int Year { get; set; }
}

## Constructors

//Special methods that run when an object is created to initialize it.

class Book
{
    public string Title;
    public string Author;

    public Book(string title, string author) // Constructor with parameters
    {
        Title = title;
        Author = author;
    }
}

## Lists //A dynamic collection of items.

List<string> fruits = new List<string>(); // Create a new list of strings
fruits.Add("Apple");
fruits.Add("Banana");

foreach (string fruit in fruits)
{
    Console.WriteLine(fruit);
}

## Namespaces and Using Directives

//using lets you access built-in or custom libraries.
//using lets you access classes from other namespaces without typing the full path.

using System.Collections.Generic; // Needed to use List<T>

## Additional Concepts

| Concept   | Description                                |
|-----------|--------------------------------------------|
| static    | Belongs to the class itself, not instances |
| null      | Represents no value (empty or nothing)     |
| try/catch | Handles errors to prevent program crashes  |
| new       | Creates a new object or instance           |
| this      | Refers to the current object instance      |

## Notes
//All C# code must be inside a class or struct.

//The Main method is the entry point of a console app.

//C# is strongly typed and object-oriented.

//Use public to expose methods/variables; use private to hide them.

//void means a method does not return a value.