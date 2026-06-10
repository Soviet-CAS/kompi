# 1. Introduction to C#

C# (អានថា "C Sharp") គឺជាភាសាសរសេរកម្មវិធីទំនើបដែលមានលក្ខណៈវត្ថុនិយមបង្កើតឡើងដោយ Microsoft។ វាត្រូវបានប្រើយ៉ាងទូលំទូលាយសម្រាប់ការបង្កើតកម្មវិធី Windows, កម្មវិធីវេប, ហ្គេម (តាមរយៈ Unity), និងកម្មវិធីទូរស័ព្ទ។ C# គឺជាផ្នែកមួយនៃប្រព័ន្ធ .NET ដែលផ្តល់នូវក្របខ័ណ្ឌដ៏រឹងមាំសម្រាប់ការអភិវឌ្ឍកម្មវិធីដែលមានស្ថេរភាពនិងសុវត្ថិភាព។

## 1.1 What is C#?

C# គឺជាភាសាសរសេរកម្មវិធីដែលបង្កើតឡើងដោយ Microsoft ក្នុងឆ្នាំ 2000។ វាត្រូវបានរចនាឡើងសម្រាប់ការអភិវឌ្ឍន៍កម្មវិធីនៅលើវេទិកា .NET។ C# គឺជាភាសាដែលងាយស្រួលរៀននិងមានលក្ខណៈពិសេសដូចជា OOP (Object-Oriented Programming), type safety, និងការគ្រប់គ្រងកំហុស។

លក្ខណៈពិសេសរបស់ C#៖

- គាំទ្រការសរសេរកម្មវិធីបែបវត្ថុ (OOP)។

- មានប្រព័ន្ធប្រមូលសំរាមដោយស្វ័យប្រវត្តិ (Garbage Collection)។

- អាចដំណើរការបានលើវេទិកាផ្សេងៗ (Windows, macOS, Linux)។

- មានបណ្ណាល័យស្តង់ដារដែលធំទូលាយសម្រាប់ការអភិវឌ្ឍ។

ឧទាហរណ៍នៃ OOP ក្នុង C#៖

```csharp
using System;

class Animal {
    public string Name { get; set; }

    public void Speak() {
        Console.WriteLine(Name + " makes a sound.");
    }
}

class Dog : Animal {
    public Dog(string name) {
        Name = name;
    }

    public void Bark() {
        Console.WriteLine(Name + " barks.");
    }
}

class Program {
    static void Main() {
        Dog dog = new Dog("Buddy");
        dog.Speak(); // Output: Buddy makes a sound.
        dog.Bark();  // Output: Buddy barks.
    }
}
```

**លទ្ធផល៖**

```text
Buddy makes a sound.
Buddy barks.
```

## 1.2 Setting Up the Environment (Installing .NET SDK & Visual Studio)

ដើម្បីចាប់ផ្តើមសរសេរកម្មវិធី C# អ្នកត្រូវការដំឡើង .NET SDK និង IDE ដូចជា Visual Studio។

ជំហានដើម្បីរៀបចំបរិស្ថាន៖

1. ទាញយក .NET SDK ពីគេហទំព័រផ្លូវការរបស់ Microsoft។

2. ដំឡើង Visual Studio ឬ Visual Studio Code។

3. ធានាថា .NET SDK ត្រូវបានភ្ជាប់ជាមួយ IDE របស់អ្នក។

ឧទាហរណ៍នៃការដំឡើង .NET SDK លើ Windows៖

```bash
dotnet --version
```

**លទ្ធផល៖**

```text
7.0.100
```

ឧទាហរណ៍នៃការបង្កើត Project ថ្មី៖

```bash
dotnet new console -o MyFirstApp
cd MyFirstApp
dotnet run
```

**លទ្ធផល៖**

```text
Hello, World!
```

## 1.3 Writing and Running Your First C# Program

កម្មវិធី C# ដំបូងរបស់អ្នកអាចត្រូវបានសរសេរនៅក្នុងឯកសារ .cs ហើយដំណើរការដោយប្រើ .NET CLI។

ឧទាហរណ៍កម្មវិធី "Hello, World!"៖

```csharp
using System;

class Program {
    static void Main() {
        Console.WriteLine("Hello, World!");
    }
}
```

ជំហានដើម្បីចងក្រង និងដំណើរការ៖

1. រក្សាទុកកូដនៅក្នុងឯកសារ Program.cs។

2. បើក terminal ហើយចងក្រងដោយប្រើពាក្យបញ្ជា៖

```bash
dotnet run
```

**លទ្ធផល៖**

```text
Hello, World!
```

## 1.4 Understanding the .NET Framework

.NET គឺជាក្របខ័ណ្ឌដែលផ្តល់នូវបណ្ណាល័យនិងឧបករណ៍សម្រាប់ការអភិវឌ្ឍកម្មវិធី។ វារួមបញ្ចូល CLR (Common Language Runtime) និង FCL (Framework Class Library)។

សមាសធាតុសំខាន់ៗនៃ .NET៖

- CLR: គ្រប់គ្រងការអនុវត្តកូដនិងការគ្រប់គ្រងអង្គចងចាំ។

- FCL: បណ្ណាល័យស្តង់ដារសម្រាប់ការអភិវឌ្ឍ។

- គាំទ្រភាសាចម្រុះ (C#, F#, VB.NET)។

ឧទាហរណ៍នៃការប្រើបណ្ណាល័យ .NET៖

```csharp
using System;

class Program {
    static void Main() {
        DateTime now = DateTime.Now;
        Console.WriteLine("Current date and time: " + now);
    }
}
```

**លទ្ធផល៖**

```text
Current date and time: 10/25/2023 12:34:56 PM
```

# 2. C# Basics

ផ្នែកនេះគ្របដណ្តប់អំពីគោលគំនិតជាមូលដ្ឋាននៃការសរសេរកម្មវិធី C# រួមទាំង syntax, អថេរ, ប្រភេទទិន្នន័យ, ប្រតិបត្តិករ, និងការបំលែងប្រភេទទិន្នន័យ។ គោលគំនិតទាំងនេះគឺជាការចាំបាច់សម្រាប់ការបង្កើតគ្រឹះរឹងមាំក្នុងការអភិវឌ្ឍ C#។

## 2.1 Syntax and Structure

C# syntax គឺស្រដៀងនឹងភាសា C-style ផ្សេងទៀតដូចជាមួយនឹងការប្រើប្រាស់វគ្គដែលមានចំណុចចាប់ផ្តើមជាមួយនឹងអនុគមន៍ Main()។

គន្លឹះ Syntax របស់ C#៖

- រាល់កម្មវិធី C# ត្រូវតែមានអនុគមន៍ Main() ជាចំណុចចាប់ផ្តើម។

- ប្រើ using ដើម្បីភ្ជាប់ namespace។

- ប្រើ ; ដើម្បីបញ្ចប់សេចក្តីថ្លែងការណ៍។

- ប្រើ ដើម្បីកំណត់ប្លុកកូដ។

ឧទាហរណ៍នៃកម្មវិធី C# សាមញ្ញ៖

```csharp
using System;

class Program {
    static void Main() {
        Console.WriteLine("Hello, C#!");
    }
}
```

**លទ្ធផល៖**

```text
Hello, C#!
```

## 2.2 Variables and Data Types

អថេរគឺជាកន្លែងសម្រាប់ផ្ទុកទិន្នន័យនិងត្រូវបានកំណត់ដោយប្រភេទទិន្នន័យ។ C# គាំទ្រប្រភេទទិន្នន័យជាច្រើន ដូចជា int, double, string, bool, និងផ្សេងៗទៀត។

ការប្រកាសនិងកំណត់តម្លៃអថេរ

អថេរត្រូវបានប្រកាសដោយប្រើប្រភេទទិន្នន័យ និងឈ្មោះអថេរ។ អ្នកអាចកំណត់តម្លៃអថេរនៅពេលប្រកាស ឬក្រោយមក។

```csharp
// ប្រកាសអថេរ
int age;
double salary;
string name;
bool isActive;

// កំណត់តម្លៃអថេរ
age = 25;
salary = 1000.50;
name = "John";
isActive = true;

// ប្រកាសនិងកំណត់តម្លៃក្នុងពេលតែមួយ
int score = 100;
double pi = 3.14159;
string greeting = "Hello, World!";
bool isCompleted = false;
```

ប្រភេទទិន្នន័យនៅក្នុង C#

C# គាំទ្រប្រភេទទិន្នន័យជាច្រើន។ ខាងក្រោមនេះគឺជាប្រភេទទិន្នន័យដែលគេប្រើញឹកញាប់៖

1. ប្រភេទចំនួនគត់ (Integer Types)

ប្រភេទទិន្នន័យចំនួនគត់រួមមាន int, long, short, និង byte។
```csharp
int age = 25; // ចំនួនគត់ (32-bit)

long population = 7800000000; // ចំនួនគត់ធំ (64-bit)

short temperature = -10; // ចំនួនគត់តូច (16-bit)

byte flags = 0b1010; // ចំនួនគត់តូច (8-bit)
```
2. ប្រភេទចំនួនទសភាគ (Floating-Point Types)

ប្រភេទទិន្នន័យចំនួនទសភាគរួមមាន float, double, និង decimal។
```csharp
float piFloat = 3.14f; // ចំនួនទសភាគ (32-bit)

double piDouble = 3.14159; // ចំនួនទសភាគ (64-bit)

decimal price = 19.99m; // ចំនួនទសភាគសម្រាប់តម្លៃហិរញ្ញវត្ថុ (128-bit)
```
3. ប្រភេទអក្សរ និងឃ្លា (Character and String Types)

ប្រភេទទិន្នន័យអក្សររួមមាន char និង string។
```csharp
char grade = 'A'; // អក្សរតែមួយ

string name = "John Doe"; // ឃ្លាអក្សរ
```
4. ប្រភេទតម្លៃពិត (Boolean Type)

ប្រភេទទិន្នន័យ bool ផ្ទុកតម្លៃពិត (true) ឬមិនពិត (false)។

```csharp
bool isActive = true;
bool isCompleted = false;
```

5. ប្រភេទទិន្នន័យផ្សេងៗ (Other Data Types)

C# ក៏គាំទ្រប្រភេទទិន្នន័យផ្សេងៗទៀត ដូចជា object, dynamic, និង var។
```csharp
object obj = 10; // អាចផ្ទុកតម្លៃណាមួយ

dynamic dynamicValue = "Hello"; // ប្រភេទទិន្នន័យត្រូវបានកំណត់នៅពេលដំណើរការ

var message = "Hello, World!"; // ប្រភេទទិន្នន័យត្រូវបានកំណត់ដោយស្វ័យប្រវត្តិ
```
អថេរថេរ (Constants)

អថេរថេរគឺជាអថេរដែលមិនអាចផ្លាស់ប្តូរតម្លៃបាន។ វាត្រូវបានប្រកាសដោយប្រើ const។

```csharp
const double PI = 3.14159;
const string GREETING = "Hello, World!";
```

## 2.3 Constants and Readonly Fields

Constants និង readonly fields គឺជាអថេរដែលមិនអាចផ្លាស់ប្តូរតម្លៃបានបន្ទាប់ពីការចាប់ផ្តើម។ Constants ត្រូវបានកំណត់ដោយប្រើ const ខណៈពេលដែល readonly fields ត្រូវបានកំណត់ដោយប្រើ readonly។

ឧទាហរណ៍៖

```csharp
const double PI = 3.14159; // Constant value
readonly int maxAttempts = 5; // Readonly field (can be set in constructor)
```

**លទ្ធផល៖**

```text
PI = 3.14159
maxAttempts = 5
```

ភាពខុសគ្នារវាង const និង readonly៖

- const: តម្លៃត្រូវតែកំណត់នៅពេលប្រកាស និងមិនអាចផ្លាស់ប្តូរបាន។

- readonly: តម្លៃអាចត្រូវបានកំណត់នៅពេលប្រកាស ឬនៅក្នុង constructor នៃ class។

## 2.4 Operators (Arithmetic, Logical, Comparison)

Operators គឺជានិមិត្តសញ្ញាសម្រាប់ធ្វើប្រតិបត្តិការលើតម្លៃនិងអថេរ។ C# គាំទ្រប្រតិបត្តិករប្រភេទផ្សេងៗដូចជា arithmetic, logical, និង comparison។

### Arithmetic Operators

Arithmetic operators ត្រូវបានប្រើសម្រាប់ធ្វើប្រតិបត្តិការគណិតវិទ្យាមូលដ្ឋានដូចជា បូក, ដក, គុណ, និងចែក។

```csharp
int a = 10;
int b = 5;

int sum = a + b;       // Addition, sum = 15
int difference = a - b; // Subtraction, difference = 5
int product = a * b;    // Multiplication, product = 50
int quotient = a / b;   // Division, quotient = 2
int remainder = a % b;  // Modulus, remainder = 0
```

**លទ្ធផល៖**

```text
sum = 15
difference = 5
product = 50
quotient = 2
remainder = 0
Comparison Operators
```

Comparison operators ត្រូវបានប្រើសម្រាប់ប្រៀបធៀបតម្លៃពីរ។ លទ្ធផលគឺជាតម្លៃ boolean (`true` ឬ `false`)។

```csharp
int x = 10;
int y = 5;

bool isEqual = (x == y);      // Equal to, isEqual = false
bool isNotEqual = (x != y);   // Not equal to, isNotEqual = true
bool isGreater = (x > y);     // Greater than, isGreater = true
bool isLess = (x < y);        // Less than, isLess = false
bool isGreaterOrEqual = (x >= y); // Greater than or equal to, isGreaterOrEqual = true
bool isLessOrEqual = (x <= y);    // Less than or equal to, isLessOrEqual = false
```

**លទ្ធផល៖**

```text
isEqual = False
isNotEqual = True
isGreater = True
isLess = False
isGreaterOrEqual = True
isLessOrEqual = False
Logical Operators
```

Logical operators ត្រូវបានប្រើសម្រាប់បញ្ចូលគ្នានូវលក្ខខណ្ឌច្រើន។ ពួកវាត្រូវបានប្រើជាទូទៅនៅក្នុងសេចក្តីថ្លែងការណ៍ត្រួតពិនិត្យ (if, else, while, etc.)។

```csharp
bool condition1 = true;
bool condition2 = false;

bool andResult = condition1 && condition2; // Logical AND, andResult = false
bool orResult = condition1 || condition2;  // Logical OR, orResult = true
bool notResult = !condition1;              // Logical NOT, notResult = false
```

**លទ្ធផល៖**

```text
andResult = False
orResult = True
notResult = False
Ternary Operator
```

Ternary operator (`? :`) គឺជាប្រតិបត្តិករសន្សំសំចៃសម្រាប់ការសរសេរ `if-else` សាមញ្ញ។

```csharp
int age = 20;
string status = (age >= 18) ? "Adult" : "Minor"; // status = "Adult"
```

**លទ្ធផល៖**

```text
status = Adult
```

## 2.5 Type Casting and Conversions

Type casting គឺជាការបំលែងប្រភេទទិន្នន័យពីប្រភេទមួយទៅប្រភេទមួយទៀត។ C# គាំទ្រការបំលែង implicit (ស្វ័យប្រវត្តិ) និង explicit (ដោយចេញពីអ្នកប្រើប្រាស់)។

ឧទាហរណ៍នៃ type casting៖

```csharp
double num1 = 10.5;
int num2 = (int)num1; // Explicit casting (double to int)

int num3 = 10;
double num4 = num3; // Implicit casting (int to double)
```

**លទ្ធផល៖**

```text
num2 = 10
num4 = 10.0
```

ការប្រើប្រាស់ Convert class សម្រាប់ការបំលែង៖

```csharp
string str = "123";
int num = Convert.ToInt32(str); // Convert string to int
```

**លទ្ធផល៖**

```text
num = 123
```

# 3. Control Flow

Control flow statements នៅក្នុង C# អនុញ្ញាតឱ្យអ្នកគ្រប់គ្រប់គ្រងការប្រតិបត្តិកម្មវិធីរបស់អ្នកដោយផ្អែកលើលក្ខខណ្ឌរង្វិលជុំនិងការលោត។ ផ្នែកនេះគ្របដណ្តប់អំពី conditional statements, loops, និង jump statements។

## 3.1 Conditional Statements (if, else, switch)

Conditional statements ត្រូវបានប្រើដើម្បីប្រតិបត្តិកូដផ្សេងៗដោយផ្អែកលើលក្ខខណ្ឌជាក់លក្ខណះ។ C# គាំទ្រសេចក្តី if, else, else if, និង switch statements។

```csharp
if Statement
```

if statement ត្រូវបានប្រើដើម្បីប្រតិបត្តិកូដនៅពេលលក្ខខណ្ឌមួយគឺពិត (`true`)។ ប្រសិនបើលក្ខខណ្ឌមិនពិត (`false`), កូដនៅក្នុង if block នឹងមិនត្រូវបានអនុវត្តទេ។

```csharp
int number = 10;
if (number > 5) {
    Console.WriteLine("The number is greater than 5.");
}
```

**លទ្ធផល៖**

```text
The number is greater than 5.
```

```csharp
if-else Statement
```

if-else statement ត្រូវបានប្រើដើម្បីប្រតិបត្តិកូដផ្សេងៗដោយផ្អែកលើលក្ខខណ្ឌ។ ប្រសិនបើលក្ខខណ្ឌគឺពិត (`true`), កូដនៅក្នុង if block នឹងត្រូវបានអនុវត្ត។ បើមិនដូច្នេះទេ, កូដនៅក្នុង else block នឹងត្រូវបានអនុវត្ត។

```csharp
int age = 18;
if (age >= 18) {
    Console.WriteLine("You are an adult.");
} else {
    Console.WriteLine("You are a minor.");
}
```

**លទ្ធផល៖**

```text
You are an adult.
```

```csharp
if-else if-else Statement
```

if-else if-else statement ត្រូវបានប្រើដើម្បីពិនិត្យលក្ខខណ្ឌច្រើន។ ប្រសិនបើលក្ខខណ្ឌទីមួយមិនពិត (`false`), លក្ខខណ្ឌបន្ទាប់នឹងត្រូវបានពិនិត្យ។ ប្រសិនបើគ្មានលក្ខខណ្ឌណាមួយពិតទេ, កូដនៅក្នុង else block នឹងត្រូវបានអនុវត្ត។

```csharp
int score = 85;
if (score >= 90) {
    Console.WriteLine("Grade: A");
} else if (score >= 80) {
    Console.WriteLine("Grade: B");
} else if (score >= 70) {
    Console.WriteLine("Grade: C");
} else {
    Console.WriteLine("Grade: F");
}
```

**លទ្ធផល៖**

```text
Grade: B
Nested if Statement
```

Nested if statement ត្រូវបានប្រើនៅពេលអ្នកត្រូវការពិនិត្យលក្ខខណ្ឌជាច្រើនដែលស្ថិតនៅក្នុងលក្ខខណ្ឌមួយផ្សេងទៀត។

```csharp
int age = 20;
bool hasLicense = true;

if (age >= 18) {
    if (hasLicense) {
        Console.WriteLine("You can drive.");
    } else {
        Console.WriteLine("You need a license to drive.");
    }
} else {
    Console.WriteLine("You are too young to drive.");
}
```

**លទ្ធផល៖**

```text
You can drive.
```

```csharp
switch Statement
```

switch statement ត្រូវបានប្រើដើម្បីជ្រើសរើសកូដមួយក្នុងចំណោមកូដច្រើនដែលត្រូវបានអនុវត្ត។ វាសមរម្យសម្រាប់ការពិនិត្យតម្លៃនៃអថេរមួយប្រឆាំងនឹងតម្លៃជាច្រើន។

```csharp
int day = 3;
switch (day) {
    case 1:
        Console.WriteLine("Monday");
        break;
    case 2:
        Console.WriteLine("Tuesday");
        break;
    case 3:
        Console.WriteLine("Wednesday");
        break;
    default:
        Console.WriteLine("Invalid day");
        break;
}
```

**លទ្ធផល៖**

```text
Wednesday
Ternary Operator
```

Ternary operator (`? :`) គឺជាប្រតិបត្តិករសន្សំសំចៃសម្រាប់ការសរសេរ if-else សាមញ្ញ។

```csharp
int age = 20;
string status = (age >= 18) ? "Adult" : "Minor"; // status = "Adult"
```

**លទ្ធផល៖**

```text
Adult
```

## 3.2 Loops (for, while, do-while, foreach)

Loops ត្រូវបានប្រើដើម្បីអនុវត្តកូដដដែលៗដោយផ្អែកលើលក្ខខណ្ឌជាក់លាក់។ C# គាំទ្ររង្វិលជុំដូចជា for, while, do-while, និង foreach។

```csharp
for Loop
```

for loop ត្រូវបានប្រើនៅពេលអ្នកដឹងចំនួនដងដែលអ្នកចង់អនុវត្តកូដ។

```csharp
for (int i = 0; i < 5; i++) {
    Console.WriteLine("Iteration: " + i);
}
```

**លទ្ធផល៖**

```text
Iteration: 0
Iteration: 1
Iteration: 2
Iteration: 3
Iteration: 4
```

```csharp
while Loop
```

while loop ត្រូវបានប្រើនៅពេលអ្នកមិនដឹងចំនួនដងដែលអ្នកចង់អនុវត្តកូដ ប៉ុន្តែអ្នកដឹងលក្ខខណ្ឌដែលត្រូវបំពេញ។

```csharp
int i = 0;
while (i < 5) {
    Console.WriteLine("Iteration: " + i);
    i++;
}
```

**លទ្ធផល៖**

```text
Iteration: 0
Iteration: 1
Iteration: 2
Iteration: 3
Iteration: 4
```

```csharp
do-while Loop
```

do-while loop ស្រដៀងនឹង while loop ប៉ុន្តែវាធានាថាកូដនឹងត្រូវបានអនុវត្តយ៉ាងហោចណាស់ម្តង។

```csharp
int i = 0;
do {
    Console.WriteLine("Iteration: " + i);
    i++;
} while (i < 5);
```

**លទ្ធផល៖**

```text
Iteration: 0
Iteration: 1
Iteration: 2
Iteration: 3
Iteration: 4
```

```csharp
foreach Loop
```

foreach loop ត្រូវបានប្រើដើម្បីធ្វើវាងាយស្រួលក្នុងការប្រើប្រាស់ collections ដូចជា arrays ឬ lists។

```csharp
string[] fruits = { "Apple", "Banana", "Cherry" };
foreach (string fruit in fruits) {
    Console.WriteLine(fruit);
}
```

**លទ្ធផល៖**

```text
Apple
Banana
Cherry
```

## 3.3 Jump Statements (break, continue, return, goto)

Jump statements ត្រូវបានប្រើដើម្បីគ្រប់គ្រងលំហូរនៃកម្មវិធីដោយប្រើ break, continue, return, និង goto។

```csharp
break Statement
```

break statement ត្រូវបានប្រើដើម្បីចាកចេញពី loop ឬ switch statement។

```csharp
for (int i = 0; i < 10; i++) {
    if (i == 5) {
        break; // Exit the loop when i is 5
    }
    Console.WriteLine("Iteration: " + i);
}
```

**លទ្ធផល៖**

```text
Iteration: 0
Iteration: 1
Iteration: 2
Iteration: 3
Iteration: 4
```

```csharp
continue Statement
```

continue statement ត្រូវបានប្រើដើម្បីរំលងការប្រតិបត្តិកូដនៅក្នុង loop និងបន្តទៅការប្រតិបត្តិបន្ទាប់។

```csharp
for (int i = 0; i < 5; i++) {
    if (i == 2) {
        continue; // Skip iteration when i is 2
    }
    Console.WriteLine("Iteration: " + i);
}
```

**លទ្ធផល៖**

```text
Iteration: 0
Iteration: 1
Iteration: 3
Iteration: 4
```

```csharp
return Statement
```

return statement ត្រូវបានប្រើដើម្បីបញ្ចប់ការប្រតិបត្តិនៃអនុគមន៍ និងត្រឡប់តម្លៃទៅកាន់ caller។

```csharp
int Add(int a, int b) {
    return a + b;
}

int result = Add(5, 10);
Console.WriteLine("Result: " + result);
```

**លទ្ធផល៖**

```text
Result: 15
```

```csharp
goto Statement
```

goto statement ត្រូវបានប្រើដើម្បីលោតទៅកាន់ label ជាក់លាក់នៅក្នុងកូដ។

```csharp
int i = 0;
start:
if (i < 5) {
    Console.WriteLine("Iteration: " + i);
    i++;
    goto start;
}
```

**លទ្ធផល៖**

```text
Iteration: 0
Iteration: 1
Iteration: 2
Iteration: 3
Iteration: 4
```

# 4. Methods and Functions

Methods និង functions គឺជាប្លុកកូដដែលអាចហៅដើម្បីអនុវត្តកិច្ចការជាក់លាក់។ ផ្នែកនេះគ្របដណ្តប់អំពីការកំណត់ហៅ methods, parameters, overloading, និង recursion។

## 4.1 Defining and Calling Methods

Methods គឺជាកូដដែលត្រូវបានកំណត់ដោយប្រើ keyword void (ប្រសិនបើមិនត្រឡប់តម្លៃ) ឬប្រភេទទិន្នន័យជាក់លាក់ (ប្រសិនបើត្រឡប់តម្លៃ)។

ឧទាហរណ៍នៃការកំណត់និងហៅ method៖

```csharp
// Define a method
void Greet() {
    Console.WriteLine("Hello, World!");
}

// Call the method
Greet();
```

**លទ្ធផល៖**

```text
Hello, World!
```

ឧទាហរណ៍នៃ method ដែលត្រឡប់តម្លៃ៖

```csharp
// Define a method that returns a value
int Add(int a, int b) {
    return a + b;
}

// Call the method
int result = Add(5, 10);
Console.WriteLine("Result: " + result);
```

**លទ្ធផល៖**

```text
Result: 15
```

## 4.2 Method Parameters (ref, out, params)

Parameters អនុញ្ញាតឱ្យអ្នកបញ្ជូនទិន្នន័យទៅកាន់ method។ C# គាំទ្រប្រភេទ parameters ដូចជា ref, out, និង params។

### ref Parameter

ref parameter អនុញ្ញាតឱ្យអ្នកបញ្ជូនតម្លៃដោយ reference ដូច្នេះការផ្លាស់ប្តូរនៅក្នុង method នឹងប៉ះពាល់ដល់តម្លៃដើម។

```csharp
void Increment(ref int num) {
    num++;
}

int x = 5;
Increment(ref x);
Console.WriteLine(x);
```

**លទ្ធផល៖**

```text
6
out Parameter
```

out parameter ស្រដៀងនឹង ref ប៉ុន្តែវាមិនតម្រូវឱ្យតម្លៃដើមត្រូវបានចាប់ផ្តើមទេ។

```csharp
void GetValues(out int a, out int b) {
    a = 10;
    b = 20;
}

int y, z;
GetValues(out y, out z);
Console.WriteLine(y + ", " + z);
```

**លទ្ធផល៖**

```text
10, 20
params Parameter
```

params parameter អនុញ្ញាតឱ្យអ្នកបញ្ជូនចំនួនអថេរនៃ arguments ទៅកាន់ method។

```csharp
int Sum(params int[] numbers) {
    int sum = 0;
    foreach (int num in numbers) {
        sum += num;
    }
    return sum;
}

int result = Sum(1, 2, 3, 4);
Console.WriteLine(result);
```

**លទ្ធផល៖**

```text
10
```

## 4.3 Method Overloading

Method overloading អនុញ្ញាតឱ្យអ្នកកំណត់ច្រើន methods ដែលមានឈ្មោះដូចគ្នាប៉ុន្តែមាន parameters ខុសគ្នា។

ឧទាហរណ៍នៃ method overloading៖

```csharp
void Print(int num) {
    Console.WriteLine("Number: " + num);
}

void Print(string text) {
    Console.WriteLine("Text: " + text);
}

Print(10); // Output: Number: 10
Print("Hello"); // Output: Text: Hello
```

**លទ្ធផល៖**

```text
Number: 10
Text: Hello
```

## 4.4 Recursion

Recursion គឺជាការហៅ method ដោយខ្លួនឯង។ វាមានប្រយោជន៍សម្រាប់ការដោះស្រាយបញ្ហាដូចជា factorial ឬ Fibonacci។

ឧទាហរណ៍នៃ recursion៖

```csharp
int Factorial(int n) {
    if (n == 0) {
        return 1;
    }
    return n * Factorial(n - 1);
}

int result = Factorial(5);
Console.WriteLine(result);
```

**លទ្ធផល៖**

```text
120
```

ឧទាហរណ៍នៃ Fibonacci sequence៖

```csharp
int Fibonacci(int n) {
    if (n <= 1) {
        return n;
    }
    return Fibonacci(n - 1) + Fibonacci(n - 2);
}

int result = Fibonacci(6);
Console.WriteLine(result);
```

**លទ្ធផល៖**

```text
8
```

# 5. Object-Oriented Programming (OOP) in C#

Object-Oriented Programming (OOP) គឺជារបៀបសរសេរកម្មវិធីដែលប្រើ objects និង classes ដើម្បីរៀបចំកម្មវិធី។ C# គឺជាភាសាដែលគាំទ្រយ៉ាងពេញលេញនូវគោលគំនិត OOP ដូចជា encapsulation, inheritance, និង polymorphism។ ផ្នែកនេះគ្របដណ្តប់អំពីគោលគំនិតមូលដ្ឋាននៃ OOP ក្នុង C#។

## 5.1 Classes and Objects

Class គឺជាគ្រោងការណ៍សម្រាប់បង្កើត objects ខណៈពេល object គឺជា instance នៃ class។ Class មាន fields (ទិន្នន័យ) និង methods (អនុគមន៍)។

ឧទាហរណ៍នៃ class និង object៖

```csharp
class Car {
    public string Model; // Field
    public void Drive() { // Method
        Console.WriteLine("Driving " + Model);
    }
}

Car myCar = new Car(); // Create an object
myCar.Model = "Toyota";
myCar.Drive();
```

**លទ្ធផល៖**

```text
Driving Toyota
```

## 5.2 Constructors and Destructors

Constructor គឺជាអនុគមន៍ពិសេសដែលត្រូវបានហៅដោយស្វ័យប្រវត្តិនៅពេលបង្កើត object។ Destructor ត្រូវបានហៅនៅពេល object ត្រូវបានបំផ្លាញ។

ឧទាហរណ៍នៃ constructor និង destructor៖

```csharp
class Car {
    public string Model;

    // Constructor
    public Car(string model) {
        Model = model;
        Console.WriteLine("Car created: " + Model);
    }

    // Destructor
    ~Car() {
        Console.WriteLine("Car destroyed: " + Model);
    }
}

Car myCar = new Car("Toyota");
```

**លទ្ធផល៖**

```text
Car created: Toyota
```

Note: Destructor នឹងត្រូវបានហៅនៅពេល object ត្រូវបានបំផ្លាញ (e.g., នៅពេលចប់កម្មវិធី)។

## 5.3 Encapsulation (Access Modifiers)

Encapsulation គឺជាការលាក់ទិន្នន័យនិងអនុគមន៍ពីការចូលប្រើពីខាងក្រៅ។ C# ប្រើ access modifiers ដូចជា public, private, protected, និង internal។

ឧទាហរណ៍នៃ encapsulation៖

```csharp
class Car {
    private string Model; // Private field

    public void SetModel(string model) { // Public method
        Model = model;
    }

    public string GetModel() { // Public method
        return Model;
    }
}

Car myCar = new Car();
myCar.SetModel("Toyota");
Console.WriteLine(myCar.GetModel());
```

**លទ្ធផល៖**

```text
Toyota
```

## 5.4 Properties and Auto-Properties

Properties គឺជាវិធីដើម្បីចូលប្រើ fields ដោយប្រើ getter និង setter។ Auto-properties ធ្វើឱ្យការកំណត់ properties កាន់តែងាយស្រួល។

ឧទាហរណ៍នៃ properties និង auto-properties៖

```csharp
class Car {
    // Auto-property
    public string Model { get; set; }

    // Property with custom logic
    private int _year;
    public int Year {
        get { return _year; }
        set { _year = value > 2000 ? value : 2000; }
    }
}

Car myCar = new Car();
myCar.Model = "Toyota";
myCar.Year = 1995;
Console.WriteLine(myCar.Year);
```

**លទ្ធផល៖**

```text
2000
```

## 5.5 Static Members

Static members ជាកម្មសិទ្ធិរបស់ class ជាជាង instance។ ពួកវាអាចត្រូវបានចូលប្រើដោយផ្ទាល់តាមរយៈ class។

ឧទាហរណ៍នៃ static members៖

```csharp
class Car {
    public static int TotalCars = 0;

    public Car() {
        TotalCars++;
    }
}

Car myCar1 = new Car();
Car myCar2 = new Car();
Console.WriteLine(Car.TotalCars);
```

**លទ្ធផល៖**

```text
2
```

## 5.6 Inheritance (base and derived classes)

Inheritance អនុញ្ញាតឱ្យ class មួយទទួលយក fields និង methods ពី class ផ្សេង។ Class ដែលទទួលយកគេហៅថា derived class ហើយ class ដែលត្រូវបានទទួលយកគេហៅថា base class។

ឧទាហរណ៍នៃ inheritance៖

```csharp
class Vehicle { // Base class
    public string Brand = "Toyota";
}

class Car : Vehicle { // Derived class
    public void Drive() {
        Console.WriteLine("Driving " + Brand);
    }
}

Car myCar = new Car();
myCar.Drive();
```

**លទ្ធផល៖**

```text
Driving Toyota
```

## 5.7 Polymorphism (method overriding, abstract classes, virtual methods)

Polymorphism អនុញ្ញាតឱ្យ methods មានឥរិយាបទខុសៗគ្នានៅក្នុង derived classes។ វាអាចសម្រេចបានតាមរយៈ method overriding, abstract classes, និង virtual methods។

ឧទាហរណ៍នៃ polymorphism៖

```csharp
class Animal { // Base class
    public virtual void Sound() {
        Console.WriteLine("Animal sound");
    }
}

class Dog : Animal { // Derived class
    public override void Sound() {
        Console.WriteLine("Bark");
    }
}

Animal myDog = new Dog();
myDog.Sound();
```

**លទ្ធផល៖**

```text
Bark
```

## 5.8 Interfaces

Interface គឺជាកិច្ចសន្យាដែលកំណត់អំពីអ្វីដែល class ត្រូវអនុវត្ត។ វាមិនមាន implementation នោះទេ។

ឧទាហរណ៍នៃ interface៖

```csharp
interface IDriveable {
    void Drive();
}

class Car : IDriveable {
    public void Drive() {
        Console.WriteLine("Driving car");
    }
}

IDriveable myCar = new Car();
myCar.Drive();
```

**លទ្ធផល៖**

```text
Driving car
```

## 5.9 Sealed and Partial Classes

Sealed class គឺជា class ដែលមិនអាចទទួលយកបាន។ Partial class អនុញ្ញាតឱ្យអ្នកបែងចែកការកំណត់ class ទៅជាឯកសារច្រើន។

ឧទាហរណ៍នៃ sealed និង partial classes៖

```csharp
// Sealed class
sealed class Animal {
    public void Sound() {
        Console.WriteLine("Animal sound");
    }
}

// Partial class
partial class Car {
    public void Drive() {
        Console.WriteLine("Driving");
    }
}

partial class Car {
    public void Stop() {
        Console.WriteLine("Stopping");
    }
}

Car myCar = new Car();
myCar.Drive();
myCar.Stop();
```

**លទ្ធផល៖**

```text
Driving
Stopping
```

# 6. Exception Handling

Exception handling គឺជាបច្ចេកទេសដែលអនុញ្ញាតឱ្យអ្នកគ្រប់គ្រងកំហុសដែលកើតឡើងក្នុងកម្មវិធីដោយមិនធ្វើឱ្យកម្មវិធីរត់ប៉ះ។ C# ផ្តល់នូវឧបករណ៍ដូចជា try-catch-finally និងការបង្កើត exceptions ផ្ទាល់ខ្លួន។

## 6.1 Try-Catch-Finally Blocks

try-catch-finally គឺជារចនាសម្ព័ន្ធសម្រាប់ចាប់យក exceptions។ កូដនៅក្នុង try block ត្រូវបានអនុវត្ត ហើយប្រសិនបើមាន exception វានឹងត្រូវបានចាប់យកដោយ catch block។finally block ត្រូវបានអនុវត្តរៀងរាល់ពេល។

ឧទាហរណ៍នៃ try-catch-finally៖

```csharp
try {
    int result = 10 / 0; // This will throw an exception
} catch (DivideByZeroException ex) {
    Console.WriteLine("Error: " + ex.Message);
} finally {
    Console.WriteLine("This will always execute.");
}
```

**លទ្ធផល៖**

```text
Error: Attempted to divide by zero.
This will always execute.
```

## 6.2 Throwing Exceptions

អ្នកអាចបង្កើតនិងបោះ exceptions ដោយប្រើ keyword throw។ វាមានប្រយោជន៍នៅពេលអ្នកចង់រាយការណ៍អំពីកំហុសផ្ទាល់ខ្លួន។

ឧទាហរណ៍នៃការបោះ exception៖

```csharp
int age = -5;
if (age < 0) {
    throw new ArgumentException("Age cannot be negative.");
}
```

**លទ្ធផល៖**

```text
Unhandled exception: System.ArgumentException: Age cannot be negative.
```

ឧទាហរណ៍នៃការបោះ exception ជាមួយ try-catch៖

```csharp
try {
    int age = -5;
    if (age < 0) {
        throw new ArgumentException("Age cannot be negative.");
    }
} catch (ArgumentException ex) {
    Console.WriteLine("Error: " + ex.Message);
}
```

**លទ្ធផល៖**

```text
Error: Age cannot be negative.
```

## 6.3 Custom Exceptions

អ្នកអាចបង្កើត exceptions ផ្ទាល់ខ្លួនដោយសរសេរ class ថ្មីដែលទាញយកពី Exception class។

ឧទាហរណ៍នៃ custom exception៖

```csharp
class NegativeAgeException : Exception {
    public NegativeAgeException(string message) : base(message) {}
}

try {
    int age = -5;
    if (age < 0) {
        throw new NegativeAgeException("Age cannot be negative.");
    }
} catch (NegativeAgeException ex) {
    Console.WriteLine("Error: " + ex.Message);
}
```

**លទ្ធផល៖**

```text
Error: Age cannot be negative.
```

## 6.4 Multiple Catch Blocks

អ្នកអាចប្រើច្រើន catch blocks ដើម្បីចាប់យក exceptions ប្រភេទផ្សេងៗ។

ឧទាហរណ៍នៃ multiple catch blocks៖

```csharp
try {
    int[] numbers = { 1, 2, 3 };
    Console.WriteLine(numbers[5]); // This will throw an IndexOutOfRangeException
} catch (IndexOutOfRangeException ex) {
    Console.WriteLine("Index error: " + ex.Message);
} catch (Exception ex) {
    Console.WriteLine("General error: " + ex.Message);
}
```

**លទ្ធផល៖**

```text
Index error: Index was outside the bounds of the array.
```

## 6.5 Nested Try-Catch Blocks

អ្នកអាចប្រើ try-catch blocks ដែលជាន់គ្នាដើម្បីគ្រប់គ្រង exceptions នៅក្នុងស្ថានភាពស្មុគស្មាញ។

ឧទាហរណ៍នៃ nested try-catch blocks៖

```csharp
try {
    try {
        int result = 10 / 0; // This will throw a DivideByZeroException
    } catch (DivideByZeroException ex) {
        Console.WriteLine("Inner error: " + ex.Message);
        throw; // Re-throw the exception
    }
} catch (Exception ex) {
    Console.WriteLine("Outer error: " + ex.Message);
}
```

**លទ្ធផល៖**

```text
Inner error: Attempted to divide by zero.
Outer error: Attempted to divide by zero.
```

# 7. Collections and Data Structures

Collections និង data structures គឺជាផ្នែកសំខាន់នៃការសរសេរកម្មវិធី C#។ ពួកវាផ្តល់នូវវិធីដើម្បីរៀបចំនិងគ្រប់គ្រងទិន្នន័យយ៉ាងមានប្រសិទ្ធភាព។ ផ្នែកនេះគ្របដណ្តប់អំពី arrays, lists, dictionaries, queues, stacks, និង sets។

## 7.1 Arrays (one-dimensional, multi-dimensional, jagged)

Arrays គឺជាបណ្តុំនៃធាតុដែលមានប្រភេទដូចគ្នា។ C# គាំទ្រការប្រើ arrays មួយវិមាត្រ, ពហុវិមាត្រ, និង jagged arrays។

ឧទាហរណ៍នៃ arrays៖

```csharp
// One-dimensional array
int[] numbers = { 1, 2, 3, 4, 5 };
Console.WriteLine("One-dimensional array:");
foreach (int num in numbers) {
    Console.Write(num + " ");
}

// Multi-dimensional array
int[,] matrix = { { 1, 2 }, { 3, 4 } };
Console.WriteLine("\nMulti-dimensional array:");
for (int i = 0; i < 2; i++) {
    for (int j = 0; j < 2; j++) {
        Console.Write(matrix[i, j] + " ");
    }
    Console.WriteLine();
}

// Jagged array
int[][] jaggedArray = {
    new int[] { 1, 2 },
    new int[] { 3, 4, 5 }
};
Console.WriteLine("\nJagged array:");
foreach (int[] arr in jaggedArray) {
    foreach (int num in arr) {
        Console.Write(num + " ");
    }
    Console.WriteLine();
}
```

**លទ្ធផល៖**

```text
One-dimensional array:
1 2 3 4 5

Multi-dimensional array:
1 2
3 4

Jagged array:
1 2
3 4 5
```

## 7.2 Lists (List<T>)

Lists គឺជា collections ដែលអាចផ្លាស់ប្តូរទំហំបាន។ ពួកវាផ្តល់នូវភាពងាយស្រួលក្នុងការបន្ថែមយកចេញនិងចូលប្រើធាតុ។

ឧទាហរណ៍នៃ List៖

```csharp
List<int> numbers = new List<int> { 1, 2, 3 };
numbers.Add(4); // Add an element
numbers.Remove(2); // Remove an element
Console.WriteLine("List elements:");
foreach (int num in numbers) {
    Console.Write(num + " ");
}
```

**លទ្ធផល៖**

```text
List elements:
1 3 4
```

## 7.3 Dictionaries (Dictionary<TKey, TValue>)

Dictionaries គឺជា collections ដែលផ្ទុក key-value pairs។ ពួកវាអនុញ្ញាតឱ្យអ្នកចូលប្រើតម្លៃដោយប្រើ key។

ឧទាហរណ៍នៃ Dictionary៖

```csharp
Dictionary<string, int> ages = new Dictionary<string, int>();
ages["John"] = 25; // Add a key-value pair
ages["Jane"] = 30;
Console.WriteLine("Dictionary elements:");
foreach (var kvp in ages) {
    Console.WriteLine(kvp.Key + ": " + kvp.Value);
}
```

**លទ្ធផល៖**

```text
Dictionary elements:
John: 25
Jane: 30
```

## 7.4 Queues and Stacks

Queues និង stacks គឺជា collections ដែលធ្វើការតាមគោលការណ៍ FIFO (First-In-First-Out) និង LIFO (Last-In-First-Out)។

ឧទាហរណ៍នៃ Queue និង Stack៖

```csharp
// Queue
Queue<int> queue = new Queue<int>();
queue.Enqueue(1); // Add to the queue
queue.Enqueue(2);
Console.WriteLine("Queue elements:");
while (queue.Count > 0) {
    Console.Write(queue.Dequeue() + " "); // Remove from the queue
}

// Stack
Stack<int> stack = new Stack<int>();
stack.Push(1); // Add to the stack
stack.Push(2);
Console.WriteLine("\nStack elements:");
while (stack.Count > 0) {
    Console.Write(stack.Pop() + " "); // Remove from the stack
}
```

**លទ្ធផល៖**

```text
Queue elements:
1 2
Stack elements:
2 1
```

## 7.5 HashSet and SortedSet

HashSet និង SortedSet គឺជា collections ដែលមិនអនុញ្ញាតឱ្យមានធាតុស្ទួន។ SortedSet រក្សាធាតុតាមលំដាប់។

ឧទាហរណ៍នៃ HashSet និង SortedSet៖

```csharp
// HashSet
HashSet<int> hashSet = new HashSet<int> { 1, 2, 3 };
hashSet.Add(2); // Duplicate, will not be added
Console.WriteLine("HashSet elements:");
foreach (int num in hashSet) {
    Console.Write(num + " ");
}

// SortedSet
SortedSet<int> sortedSet = new SortedSet<int> { 3, 1, 2 };
Console.WriteLine("\nSortedSet elements:");
foreach (int num in sortedSet) {
    Console.Write(num + " ");
}
```

**លទ្ធផល៖**

```text
HashSet elements:
1 2 3
SortedSet elements:
1 2 3
```

# 8. File Handling and Streams

File handling និង streams គឺជាផ្នែកសំខាន់នៃការសរសេរកម្មវិធី C#។ ពួកវាអនុញ្ញាតឱ្យអ្នកអាននិងសរសេរទិន្នន័យទៅកាន់ឯកសារ JSON និង CSV។ ផ្នែកនេះគ្របដណ្តប់អំពីការប្រើ File, StreamReader, StreamWriter, និង System.Text.Json។

## 8.1 Reading and Writing Files (File, StreamReader, StreamWriter)

C# ផ្តល់នូវវិធីជាច្រើនដើម្បីអាននិងសរសេរទិន្នន័យទៅកាន់ឯកសារ។ អ្នកអាចប្រើ File class សម្រាប់ប្រតិបត្តិការសាមញ្ញ ឬ StreamReader និង StreamWriter សម្រាប់ការគ្រប់គ្រងលម្អិតបន្ថែម។

ឧទាហរណ៍នៃការសរសេរនិងអានឯកសារ៖

```csharp
using System;
using System.IO;

class Program
{
    static void Main()
    {
        string filePath = "example.txt";

        // Writing to a file using File.WriteAllText
        File.WriteAllText(filePath, "Hello, World!");
        Console.WriteLine("File written using File.WriteAllText.");

        // Reading from a file using File.ReadAllText
        string content = File.ReadAllText(filePath);
        Console.WriteLine("Content read using File.ReadAllText:");
        Console.WriteLine(content); // Output: Hello, World!

        // Appending to a file using File.AppendAllText
        File.AppendAllText(filePath, "\nThis is an appended line.");
        Console.WriteLine("Line appended using File.AppendAllText.");

        // Reading all lines from a file using File.ReadAllLines
        string[] lines = File.ReadAllLines(filePath);
        Console.WriteLine("Content read using File.ReadAllLines:");
        foreach (string line in lines)
        {
            Console.WriteLine(line);
        }
        // Output:
        // Hello, World!
        // This is an appended line.

        // Using StreamWriter to write to a file
        using (StreamWriter writer = new StreamWriter(filePath))
        {
            writer.WriteLine("This is a new line written using StreamWriter.");
            writer.WriteLine("Another line added.");
        }
        Console.WriteLine("File written using StreamWriter.");

        // Using StreamReader to read from a file line by line
        using (StreamReader reader = new StreamReader(filePath))
        {
            Console.WriteLine("Content read using StreamReader:");
            string line;
            while ((line = reader.ReadLine()) != null)
            {
                Console.WriteLine(line);
            }
        }
        // Output:
        // This is a new line written using StreamWriter.
        // Another line added.

        // Handling exceptions when working with files
        try
        {
            string nonExistentFilePath = "nonexistent.txt";
            string text = File.ReadAllText(nonExistentFilePath);
        }
        catch (FileNotFoundException ex)
        {
            Console.WriteLine("Error: File not found.");
            Console.WriteLine(ex.Message);
        }
        catch (Exception ex)
        {
            Console.WriteLine("An error occurred:");
            Console.WriteLine(ex.Message);
        }
    }
}
```

**Output:**

```text
File written using File.WriteAllText.
Content read using File.ReadAllText:
Hello, World!
Line appended using File.AppendAllText.
Content read using File.ReadAllLines:
Hello, World!
This is an appended line.
File written using StreamWriter.
Content read using StreamReader:
This is a new line written using StreamWriter.
Another line added.
Error: File not found.
Could not find file 'nonexistent.txt'.
```

## 8.2 Working with JSON (System.Text.Json)

JSON (JavaScript Object Notation) គឺជាទ្រង់ទ្រាយទិន្នន័យដែលគេប្រើយ៉ាងទូលំទូលាយសម្រាប់ការផ្លាស់ប្តូរទិន្នន័យ។ C# ផ្តល់នូវ System.Text.Json សម្រាប់ការបំលែង objects ទៅជា JSON និងច្រាសមកវិញ។

ឧទាហរណ៍នៃការប្រើ JSON៖

```csharp
using System.Text.Json;

// Define a Person class
public class Person {
    public string Name { get; set; }
    public int Age { get; set; }
}

// Serialize object to JSON
var person = new Person { Name = "John", Age = 30 };
string json = JsonSerializer.Serialize(person);
Console.WriteLine(json); // Output: {"Name":"John","Age":30}

// Deserialize JSON to object
var deserializedPerson = JsonSerializer.Deserialize<Person>(json);
Console.WriteLine(deserializedPerson.Name); // Output: John
Console.WriteLine(deserializedPerson.Age);  // Output: 30
```

**Output:**

```text
{"Name":"John","Age":30}
John
30
```

## 8.3 Handling CSV Files

CSV (Comma-Separated Values) គឺជាទ្រង់ទ្រាយឯកសារដែលគេប្រើយ៉ាងទូលំទូលាយសម្រាប់ផ្ទុកទិន្នន័យតារាង។ C# អនុញ្ញាតឱ្យអ្នកអាននិងសរសេរទិន្នន័យ CSV ដោយប្រើ StreamReader និង StreamWriter។

ឧទាហរណ៍នៃការប្រើ CSV៖

```csharp
// Writing to a CSV file
string csvPath = "data.csv";
using (StreamWriter writer = new StreamWriter(csvPath)) {
    writer.WriteLine("Name,Age");
    writer.WriteLine("John,30");
    writer.WriteLine("Jane,25");
}

// Reading from a CSV file
using (StreamReader reader = new StreamReader(csvPath)) {
    string line;
    while ((line = reader.ReadLine()) != null) {
        Console.WriteLine(line);
    }
}
```

**Output:**

```text
Name,Age
John,30
Jane,25
```

# 9. LINQ (Language Integrated Query)

LINQ (Language Integrated Query) គឺជាផ្នែកមួយនៃ C# ដែលអនុញ្ញាតឱ្យអ្នកសរសេរសំណួរទៅកាន់ collections, databases, និងទិន្នន័យផ្សេងៗ។ វាធ្វើឱ្យការងារជាមួយទិន្នន័យកាន់តែងាយស្រួលនិងអានបាន។

## 9.1 Introduction to LINQ

LINQ ផ្តល់នូវវិធីសាមញ្ញនិងអានបានដើម្បីសរសេរសំណួរទៅកាន់ទិន្នន័យ។ វាគាំទ្រទិន្នន័យប្រភេទផ្សេងៗដូចជា collections, arrays, XML, និង databases។

ឧទាហរណ៍នៃ LINQ៖

```csharp
int[] numbers = { 1, 2, 3, 4, 5 };
var evenNumbers = from num in numbers
```

where num % 2 == 0

select num;

```csharp
foreach (var num in evenNumbers) {
    Console.WriteLine(num); // Output: 2, 4
}
```

**Output:**

```text
2
4
```

## 9.2 LINQ Queries (Where, Select, OrderBy)

LINQ queries អនុញ្ញាតឱ្យអ្នកច្រាស់ទិន្នន័យដោយប្រើ methods ដូចជា Where, Select, និង OrderBy។

ឧទាហរណ៍នៃ LINQ queries៖

```csharp
var numbers = new List<int> { 5, 3, 1, 4, 2 };

// Filtering with Where
var filteredNumbers = numbers.Where(n => n > 2);

// Projection with Select
var squaredNumbers = numbers.Select(n => n * n);

// Sorting with OrderBy
var sortedNumbers = numbers.OrderBy(n => n);

Console.WriteLine(string.Join(", ", sortedNumbers)); // Output: 1, 2, 3, 4, 5
```

**Output:**

```text
1, 2, 3, 4, 5
```

## 9.3 LINQ with Collections

LINQ អាចត្រូវបានប្រើជាមួយ collections ដូចជា List<T>, Dictionary<TKey, TValue>, និង HashSet<T>។

ឧទាហរណ៍នៃ LINQ with collections៖

```csharp
public class Student {
    public string Name { get; set; }
    public int Age { get; set; }
}

var students = new List<Student> {
    new Student { Name = "John", Age = 20 },
    new Student { Name = "Jane", Age = 22 },
    new Student { Name = "Alice", Age = 21 }
};

var query = from student in students
```

where student.Age > 20

orderby student.Name

select student;

```csharp
foreach (var student in query) {
    Console.WriteLine(student.Name); // Output: Alice, Jane
}
```

**Output:**

```text
Alice
Jane
```

## 9.4 LINQ with Databases (Entity Framework)

LINQ អាចត្រូវបានប្រើជាមួយ databases តាមរយៈ Entity Framework។ វាអនុញ្ញាតឱ្យអ្នកសរសេរសំណួរទៅកាន់ database ដោយប្រើ syntax ដូចគ្នានឹង LINQ with collections។

ឧទាហរណ៍នៃ LINQ with Entity Framework៖

```csharp
using (var context = new SchoolContext()) {
    var students = from student in context.Students
```

where student.Age > 20

orderby student.Name

select student;

```csharp
    foreach (var student in students) {
        Console.WriteLine(student.Name);
    }
}
```

**Output:**

```text
Alice
Jane
```

# 10. Delegates, Events, and Lambda Expressions

Delegates, events, និង lambda expressions គឺជាផ្នែកសំខាន់នៃ C# ដែលអនុញ្ញាតឱ្យអ្នកគ្រប់គ្រងការហៅអនុគមន៍ដោយប្រើវិធីដែលអាចបត់បែននិងអានបាន។ ផ្នែកនេះគ្របដណ្តប់អំពី delegates, lambda expressions, និងការគ្រប់គ្រង events។

## 10.1 Delegates (Func, Action, Predicate)

Delegates គឺជាប្រភេទដែលតំណាងឱ្យអនុគមន៍។ C# ផ្តល់នូវ delegates ដូចជា Func, Action, និង Predicate សម្រាប់ការប្រើប្រាស់ទូទៅ។

ឧទាហរណ៍នៃ delegates៖

```csharp
// Func delegate (returns a value)
Func<int, int, int> add = (a, b) => a + b;
Console.WriteLine(add(2, 3)); // Output: 5

// Action delegate (does not return a value)
Action<string> greet = name => Console.WriteLine("Hello, " + name);
greet("John"); // Output: Hello, John

// Predicate delegate (returns a boolean)
Predicate<int> isEven = num => num % 2 == 0;
Console.WriteLine(isEven(4)); // Output: True
```

**Output:**

```text
5
Hello, John
True
```

## 10.2 Lambda Expressions

Lambda expressions គឺជាវិធីសង្ខេបដើម្បីសរសេរអនុគមន៍ដោយមិនចាំបាច់កំណត់ឈ្មោះ។ ពួកវាត្រូវបានប្រើជាញឹកញាប់ជាមួយ delegates និង LINQ។

ឧទាហរណ៍នៃ lambda expressions៖

```csharp
// Lambda expression with Func delegate
Func<int, int> square = x => x * x;
Console.WriteLine(square(5)); // Output: 25

// Lambda expression with LINQ
var numbers = new List<int> { 1, 2, 3, 4, 5 };
var evenNumbers = numbers.Where(n => n % 2 == 0);
Console.WriteLine(string.Join(", ", evenNumbers)); // Output: 2, 4
```

**Output:**

```text
25
2, 4
```

## 10.3 Events and Event Handling

Events គឺជាវិធីដើម្បីធ្វើឱ្យ class អាចជូនដំណឹងទៅកាន់ class ផ្សេងៗនៅពេលដែលអ្វីមួយកើតឡើង។ Event handling គឺជាការគ្រប់គ្រងការឆ្លើយតបទៅនឹង events។

ឧទាហរណ៍នៃ events និង event handling៖

```csharp
// Define a delegate for the event
public delegate void Notify();

// Define a class with an event
public class Process {
    public event Notify ProcessCompleted;

    public void StartProcess() {
        Console.WriteLine("Process started...");
        OnProcessCompleted();
    }

    protected virtual void OnProcessCompleted() {
        ProcessCompleted?.Invoke();
    }
}

// Subscribe to the event
Process process = new Process();
process.ProcessCompleted += () => Console.WriteLine("Process completed!");
process.StartProcess(); // Output: Process started... Process completed!
```

**Output:**

```text
Process started...
Process completed!
```

# 11. Multithreading and Asynchronous Programming

Multithreading និង asynchronous programming គឺជាបច្ចេកទេសសម្រាប់កែលម្អដំណើរការកម្មវិធីដោយអនុញ្ញាតឱ្យការងារច្រើនអាចដំណើរការក្នុងពេលដំណាលគ្នា។ ផ្នែកនេះគ្របដណ្តប់អំពី threads, tasks, parallel programming, និង background workers។

## 11.1 Threads (Thread Class)

Threads អនុញ្ញាតឱ្យអ្នកដំណើរការកូដជាច្រើនក្នុងពេលដំណាលគ្នា។ អ្នកអាចប្រើ Thread class ដើម្បីបង្កើតនិងគ្រប់គ្រង threads។

ឧទាហរណ៍នៃ threads៖

```csharp
using System.Threading;

void PrintNumbers() {
    for (int i = 1; i <= 5; i++) {
        Console.WriteLine(i);
        Thread.Sleep(500);
    }
}

Thread thread = new Thread(PrintNumbers);
thread.Start(); // Start the thread
thread.Join();  // Wait for the thread to finish
```

**Output:**

```text
1
2
3
4
5
```

## 11.2 Task-Based Asynchronous Pattern (async and await)

Task-based asynchronous pattern (TAP) គឺជាវិធីសាមញ្ញនិងមានប្រសិទ្ធភាពដើម្បីដំណើរការកូដ asynchronous ដោយប្រើ async និង await។

ឧទាហរណ៍នៃ async និង await៖

```csharp
async Task<string> FetchDataAsync() {
    await Task.Delay(2000); // Simulate a delay
    return "Data fetched!";
}

async Task Main() {
    Console.WriteLine("Fetching data...");
    string result = await FetchDataAsync();
    Console.WriteLine(result); // Output: Data fetched!
}

Main().Wait();
```

**Output:**

```text
Fetching data...
Data fetched!
```

## 11.3 Parallel Programming (Parallel.For, Parallel.ForEach)

Parallel programming អនុញ្ញាតឱ្យអ្នកដំណើរការកូដជាច្រើនក្នុងពេលដំណាលគ្នាដោយប្រើ Parallel.For និង Parallel.ForEach។

ឧទាហរណ៍នៃ parallel programming៖

```csharp
using System.Threading.Tasks;

Parallel.For(0, 10, i => {
    Console.WriteLine($"Processing {i} on thread {Thread.CurrentThread.ManagedThreadId}");
});

var numbers = new List<int> { 1, 2, 3, 4, 5 };
Parallel.ForEach(numbers, num => {
    Console.WriteLine($"Processing {num} on thread {Thread.CurrentThread.ManagedThreadId}");
});
```

**Output:**

```text
Processing 0 on thread 1
Processing 1 on thread 2
Processing 2 on thread 3
Processing 3 on thread 4
Processing 4 on thread 5
Processing 5 on thread 6
Processing 6 on thread 7
Processing 7 on thread 8
Processing 8 on thread 9
Processing 9 on thread 10
Processing 1 on thread 1
Processing 2 on thread 2
Processing 3 on thread 3
Processing 4 on thread 4
Processing 5 on thread 5
```

## 11.4 Background Workers

Background workers គឺជាវិធីដើម្បីដំណើរការកូដនៅក្នុងផ្ទៃខាងក្រោយដោយមិនរារាំង UI។ អ្នកអាចប្រើ BackgroundWorker class ដើម្បីគ្រប់គ្រងការងារផ្ទៃខាងក្រោយ។

ឧទាហរណ៍នៃ background workers៖

```csharp
using System.ComponentModel;

BackgroundWorker worker = new BackgroundWorker();
worker.DoWork += (sender, e) => {
    // Simulate a long-running task
    Thread.Sleep(2000);
    e.Result = "Task completed!";
};

worker.RunWorkerCompleted += (sender, e) => {
    Console.WriteLine(e.Result); // Output: Task completed!
};

worker.RunWorkerAsync();
```

**Output:**

```text
Task completed!
```

# 12. Working with Databases in C#

C# ផ្តល់នូវឧបករណ៍ដ៏រឹងមាំសម្រាប់ធ្វើការជាមួយ databases ដូចជា ADO.NET និង Entity Framework Core។ ផ្នែកនេះគ្របដណ្តប់អំពីការភ្ជាប់ទៅកាន់ SQL Server, ការប្រើ SQL queries, និងការប្រើ Entity Framework Core។

## 12.1 ADO.NET Basics

ADO.NET គឺជា framework សម្រាប់ធ្វើការជាមួយ databases នៅក្នុង C#។ វាផ្តល់នូវ classes ដូចជា SqlConnection, SqlCommand, និង SqlDataReader សម្រាប់ការភ្ជាប់និងគ្រប់គ្រងទិន្នន័យ។

ឧទាហរណ៍នៃ ADO.NET៖

```csharp
using System.Data.SqlClient;

string connectionString = "YourConnectionStringHere";
using (SqlConnection connection = new SqlConnection(connectionString)) {
    connection.Open();
    SqlCommand command = new SqlCommand("SELECT * FROM Customers", connection);
    SqlDataReader reader = command.ExecuteReader();
    while (reader.Read()) {
        Console.WriteLine(reader["CustomerName"]);
    }
}
```

**Output:**

```text
John Doe
Jane Smith
Alice Johnson
```

## 12.2 Connecting to SQL Server

ដើម្បីភ្ជាប់ទៅកាន់ SQL Server អ្នកត្រូវប្រើ SqlConnection class ជាមួយ connection string។ Connection string មានព័ត៌មានដូចជា server name, database name, និង credentials។

ឧទាហរណ៍នៃការភ្ជាប់ទៅកាន់ SQL Server៖

```csharp
string connectionString = "Server=your_server;Database=your_db;User Id=your_user;Password=your_password;";
using (SqlConnection connection = new SqlConnection(connectionString)) {
    connection.Open();
    Console.WriteLine("Connected to SQL Server!");
}
```

**Output:**

```text
Connected to SQL Server!
```

## 12.3 Executing SQL Queries with C#

អ្នកអាចប្រើ SqlCommand ដើម្បីអនុវត្ត SQL queries និង stored procedures។ វាអនុញ្ញាតឱ្យអ្នកអាន, សរសេរ, និងធ្វើបច្ចុប្បន្នភាពទិន្នន័យនៅក្នុង database។

ឧទាហរណ៍នៃការអនុវត្ត SQL queries៖

```csharp
using (SqlConnection connection = new SqlConnection(connectionString)) {
    connection.Open();
    SqlCommand command = new SqlCommand("INSERT INTO Customers (CustomerName) VALUES (@Name)", connection);
    command.Parameters.AddWithValue("@Name", "John Doe");
    int rowsAffected = command.ExecuteNonQuery();
    Console.WriteLine($"{rowsAffected} row(s) inserted.");
}
```

**Output:**

```text
1 row(s) inserted.
```

## 12.4 Entity Framework Core Basics

Entity Framework Core (EF Core) គឺជា ORM (Object-Relational Mapper) ដែលអនុញ្ញាតឱ្យអ្នកធ្វើការជាមួយ databases ដោយប្រើ objects និង LINQ។ វាធ្វើឱ្យការងារជាមួយ databases កាន់តែងាយស្រួល។

ឧទាហរណ៍នៃ EF Core៖

```csharp
using Microsoft.EntityFrameworkCore;

public class Customer {
    public int Id { get; set; }
    public string Name { get; set; }
}

public class AppDbContext : DbContext {
    public DbSet<Customer> Customers { get; set; }

    protected override void OnConfiguring(DbContextOptionsBuilder optionsBuilder) {
        optionsBuilder.UseSqlServer("YourConnectionStringHere");
    }
}

// Adding a customer
using (var context = new AppDbContext()) {
    var customer = new Customer { Name = "John Doe" };
    context.Customers.Add(customer);
    context.SaveChanges();
}

// Querying customers
using (var context = new AppDbContext()) {
    var customers = context.Customers.ToList();
    foreach (var c in customers) {
        Console.WriteLine(c.Name);
    }
}
```

**Output:**

```text
John Doe
```

# 13. Windows Forms and WPF (GUI Development)

Windows Forms និង WPF (Windows Presentation Foundation) គឺជា frameworks សម្រាប់ការអភិវឌ្ឍកម្មវិធី GUI (Graphical User Interface) នៅក្នុង C#។ ផ្នែកនេះគ្របដណ្តប់អំពីការបង្កើតនិងគ្រប់គ្រងកម្មវិធី GUI ដោយប្រើ Windows Forms និង WPF។

## 13.1 Introduction to Windows Forms

Windows Forms គឺជា framework សម្រាប់ការបង្កើតកម្មវិធី desktop ដែលមាន GUI។ វាផ្តល់នូវ controls ដូចជា buttons, labels, textboxes, និងផ្សេងៗទៀតសម្រាប់ការបង្កើតផ្ទាំងអ្នកប្រើប្រាស់។

ឧទាហរណ៍នៃការបង្កើត Windows Forms application៖

```csharp
using System;
using System.Windows.Forms;

public class MainForm : Form {
    public MainForm() {
        // កំណត់ចំណងជើងនិងទំហំរបស់ form
        this.Text = "My First Windows Form";
        this.Size = new System.Drawing.Size(300, 200);

        // បង្កើត button
        Button button = new Button();
        button.Text = "Click Me";
        button.Location = new System.Drawing.Point(100, 50);
        button.Click += (sender, e) => MessageBox.Show("Button clicked!");

        // បន្ថែម button ទៅក្នុង form
        this.Controls.Add(button);
    }

    [STAThread]
    static void Main() {
        // បើក application
        Application.Run(new MainForm());
    }
}
```

លទ្ធផល៖ វីនដូមួយដែលមានចំណងជើង "My First Windows Form" នឹងបង្ហាញឡើងជាមួយ button ដែលមានចំណងជើង "Click Me"។ នៅពេលចុច button នេះ ប្រអប់សារមួយនឹងបង្ហាញឡើងដោយសារអត្ថបទ "Button clicked!"។

## 13.2 Working with Controls (Buttons, Labels, Textboxes)

Controls គឺជាធាតុដែលអ្នកប្រើប្រាស់អាចធ្វើអន្តរកម្មជាមួយនៅក្នុងកម្មវិធី GUI។ Windows Forms ផ្តល់នូវ controls ជាច្រើនដូចជា buttons, labels, textboxes, និងផ្សេងៗទៀត។

ឧទាហរណ៍នៃការប្រើ controls៖

```csharp
using System;
using System.Windows.Forms;

public class MainForm : Form {
    public MainForm() {
        this.Text = "User Input Form";
        this.Size = new System.Drawing.Size(300, 200);

        // បង្កើត label
        Label label = new Label();
        label.Text = "Enter your name:";
        label.Location = new System.Drawing.Point(20, 20);

        // បង្កើត textbox
        TextBox textBox = new TextBox();
        textBox.Location = new System.Drawing.Point(20, 50);
        textBox.Size = new System.Drawing.Size(200, 20);

        // បង្កើត button
        Button button = new Button();
        button.Text = "Submit";
        button.Location = new System.Drawing.Point(20, 80);
        button.Click += (sender, e) => MessageBox.Show("Hello, " + textBox.Text);

        // បន្ថែម controls ទៅក្នុង form
        this.Controls.Add(label);
        this.Controls.Add(textBox);
        this.Controls.Add(button);
    }

    [STAThread]
    static void Main() {
        Application.Run(new MainForm());
    }
}
```

លទ្ធផល៖ វីនដូមួយដែលមានចំណងជើង "User Input Form" នឹងបង្ហាញឡើងជាមួយ label "Enter your name:", textbox សម្រាប់បញ្ចូលឈ្មោះ និង button "Submit"។ នៅពេលអ្នកប្រើប្រាស់បញ្ចូលឈ្មោះរបស់ពួកគេ ហើយចុច "Submit" ប្រអប់សារមួយនឹងបង្ហាញឡើងដោយសារអត្ថបទ "Hello, [name]"។

## 13.3 Event Handling in Windows Forms

Event handling គឺជាការគ្រប់គ្រងការឆ្លើយតបទៅនឹងសកម្មភាពរបស់អ្នកប្រើប្រាស់ដូចជាការចុចប៊ូតុង។ អ្នកអាចប្រើ event handlers ដើម្បីកំណត់អ្វីដែលត្រូវធ្វើនៅពេលដែល event កើតឡើង។

ឧទាហរណ៍នៃ event handling៖

```csharp
using System;
using System.Windows.Forms;

public class MainForm : Form {
    public MainForm() {
        this.Text = "Event Handling Example";
        this.Size = new System.Drawing.Size(300, 200);

        // បង្កើត button
        Button button = new Button();
        button.Text = "Click Me";
        button.Location = new System.Drawing.Point(100, 50);
        button.Click += (sender, e) => {
            MessageBox.Show("Button clicked!");
        };

        // បន្ថែម button ទៅក្នុង form
        this.Controls.Add(button);
    }

    [STAThread]
    static void Main() {
        Application.Run(new MainForm());
    }
}
```

លទ្ធផល៖ វីនដូមួយដែលមានចំណងជើង "Event Handling Example" នឹងបង្ហាញឡើងជាមួយ button ដែលមានចំណងជើង "Click Me"។ នៅពេលចុច button នេះ ប្រអប់សារមួយនឹងបង្ហាញឡើងដោយសារអត្ថបទ "Button clicked!"។

## 13.4 Introduction to WPF (Windows Presentation Foundation)

WPF គឺជា framework ទំនើបសម្រាប់ការបង្កើតកម្មវិធី desktop ដែលមាន GUI។ វាផ្តល់នូវការគាំទ្រសម្រាប់ graphics, animations, និង data binding។

ឧទាហរណ៍នៃ WPF application៖

```xml
<!-- MainWindow.xaml -->
<Window x:Class="WpfApp.MainWindow"
```

xmlns="http://schemas.microsoft.com/winfx/2006/xaml/presentation"

xmlns:x="http://schemas.microsoft.com/winfx/2006/xaml"

Title="My WPF App" Height="200" Width="300">

```xml
    <StackPanel>
        <Label Content="Enter your name:" />
        <TextBox x:Name="txtName" />
        <Button Content="Submit" Click="Button_Click" />
    </StackPanel>
</Window>
```

```csharp
// MainWindow.xaml.cs
using System.Windows;

public partial class MainWindow : Window {
    public MainWindow() {
        InitializeComponent();
    }

    private void Button_Click(object sender, RoutedEventArgs e) {
        MessageBox.Show("Hello, " + txtName.Text);
    }
}
```

លទ្ធផល៖ វីនដូមួយដែលមានចំណងជើង "My WPF App" នឹងបង្ហាញឡើងជាមួយ label "Enter your name:", textbox សម្រាប់បញ្ចូលឈ្មោះ និង button "Submit"។ នៅពេលអ្នកប្រើប្រាស់បញ្ចូលឈ្មោះរបស់ពួកគេ ហើយចុច "Submit" ប្រអប់សារមួយនឹងបង្ហាញឡើងដោយសារអត្ថបទ "Hello, [name]"។

# 14. ASP.NET Core (Web Development)

ASP.NET Core គឺជា framework ទំនើបសម្រាប់ការអភិវឌ្ឍកម្មវិធី web និង web APIs។ វាគាំទ្រការអភិវឌ្ឍន៍ cross-platform និងមានដំណើរការលឿន។ ផ្នែកនេះគ្របដណ្តប់អំពី MVC architecture, Web APIs, និងការគ្រប់គ្រង authentication និង authorization។

## 14.1 Introduction to ASP.NET Core

ASP.NET Core គឺជា framework សម្រាប់ការបង្កើតកម្មវិធី web និង web APIs ដែលអាចដំណើរការបានលើ Windows, macOS, និង Linux។ វាត្រូវបានបង្កើតឡើងដើម្បីធ្វើឱ្យការអភិវឌ្ឍន៍ web កាន់តែមានប្រសិទ្ធភាពនិងអាចពង្រីកបាន។

ឧទាហរណ៍នៃ ASP.NET Core project៖

```bash
dotnet new webapi -o MyWebApi
```

## 14.2 MVC Architecture in ASP.NET

MVC (Model-View-Controller) គឺជារចនាសម្ព័ន្ធសម្រាប់ការអភិវឌ្ឍកម្មវិធី web។ វាបែងចែកកម្មវិធីជា 3 ផ្នែក៖ Model (ទិន្នន័យ), View (ផ្ទាំងអ្នកប្រើប្រាស់), និង Controller (ដែលគ្រប់គ្រងឡូជីខល)។

ឧទាហរណ៍នៃ MVC controller៖

```csharp
public class HomeController : Controller {
    public IActionResult Index() {
        return View();
    }

    public IActionResult About() {
        ViewData["Message"] = "Your application description page.";
        return View();
    }
}
```

## 14.3 Building a Web API with ASP.NET Core

ASP.NET Core ផ្តល់នូវឧបករណ៍ដ៏រឹងមាំសម្រាប់ការបង្កើត Web APIs។ Web APIs អនុញ្ញាតឱ្យអ្នកបង្កើត RESTful services ដែលអាចត្រូវបានប្រើដោយកម្មវិធីផ្សេងៗ។

ឧទាហរណ៍នៃ Web API controller៖

```csharp
[ApiController]
[Route("api/[controller]")]
public class ProductsController : ControllerBase {
    [HttpGet]
    public IEnumerable<string> Get() {
        return new string[] { "Product1", "Product2" };
    }

    [HttpGet("{id}")]
    public string Get(int id) {
        return $"Product {id}";
    }
}
```

## 14.4 Authentication and Authorization

Authentication គឺជាការផ្ទៀងផ្ទាត់អត្តសញ្ញាណរបស់អ្នកប្រើប្រាស់ ខណៈពេលដែល authorization គឺជាការកំណត់អ្វីដែលអ្នកប្រើប្រាស់អាចធ្វើបាន។ ASP.NET Core ផ្តល់នូវឧបករណ៍សម្រាប់ការគ្រប់គ្រង authentication និង authorization។

ឧទាហរណ៍នៃការកំណត់ authentication៖

```csharp
public void ConfigureServices(IServiceCollection services) {
    services.AddAuthentication("Bearer")
            .AddJwtBearer("Bearer", options => {
                options.Authority = "https://localhost:5001";
                options.Audience = "api1";
            });
}

public void Configure(IApplicationBuilder app) {
    app.UseAuthentication();
    app.UseAuthorization();
}
```

# 15. Unit Testing in C#

Unit testing គឺជាវិធីសាស្រ្តសម្រាប់សាកល្បងកូដដោយបែងចែកវាជាផ្នែកតូចៗ។ វាជួយធានាថាកូដដំណើរការត្រឹមត្រូវនិងអាចពង្រីកបាន។ ផ្នែកនេះគ្របដណ្តប់អំពីការសរសេរ unit tests, mocking, និង test-driven development (TDD)។

## 15.1 Writing Unit Tests with MSTest and NUnit

MSTest និង NUnit គឺជា frameworks សម្រាប់សរសេរ unit tests នៅក្នុង C#។ ពួកវាផ្តល់នូវ attributes និង methods សម្រាប់ការកំណត់និងដំណើរការ tests។

ឧទាហរណ៍នៃ unit test ជាមួយ MSTest៖

```csharp
using Microsoft.VisualStudio.TestTools.UnitTesting;

[TestClass]
public class MathTests {
    [TestMethod]
    public void Add_TwoNumbers_ReturnsSum() {
        // Arrange
        int a = 5;
        int b = 3;

        // Act
        int result = a + b;

        // Assert
        Assert.AreEqual(8, result);
    }
}
```

ឧទាហរណ៍នៃ unit test ជាមួយ NUnit៖

```csharp
using NUnit.Framework;

[TestFixture]
public class MathTests {
    [Test]
    public void Add_TwoNumbers_ReturnsSum() {
        // Arrange
        int a = 5;
        int b = 3;

        // Act
        int result = a + b;

        // Assert
        Assert.AreEqual(8, result);
    }
}
```

## 15.2 Mocking with Moq

Mocking គឺជាវិធីសាស្រ្តសម្រាប់បង្កើត objects ប្លែកដែលជំនួស dependencies នៅក្នុង unit tests។ Moq គឺជា library ដ៏ពេញនិយមសម្រាប់ mocking នៅក្នុង C#។

ឧទាហរណ៍នៃ mocking ជាមួយ Moq៖

```csharp
using Moq;

public interface ICalculator {
    int Add(int a, int b);
}

[TestClass]
public class CalculatorTests {
    [TestMethod]
    public void Add_TwoNumbers_ReturnsSum() {
        // Arrange
        var mockCalculator = new Mock<ICalculator>();
        mockCalculator.Setup(x => x.Add(5, 3)).Returns(8);

        // Act
        int result = mockCalculator.Object.Add(5, 3);

        // Assert
        Assert.AreEqual(8, result);
    }
}
```

## 15.3 Test-Driven Development (TDD) in C#

Test-Driven Development (TDD) គឺជាវិធីសាស្រ្តសម្រាប់ការអភិវឌ្ឍកូដដោយសរសេរ tests មុនពេលសរសេរកូដដែលធ្វើឱ្យ tests ឆ្លង។ TDD ជួយធានាថាកូដមានគុណភាពខ្ពស់និងអាចពង្រីកបាន។

ឧទាហរណ៍នៃ TDD៖

```csharp
// Step 1: Write a failing test
[TestMethod]
public void Add_TwoNumbers_ReturnsSum() {
    // Arrange
    var calculator = new Calculator();

    // Act
    int result = calculator.Add(5, 3);

    // Assert
    Assert.AreEqual(8, result);
}

// Step 2: Write the minimal code to pass the test
public class Calculator {
    public int Add(int a, int b) {
        return a + b;
    }
}

// Step 3: Refactor the code (if necessary)
```

# 16. Advanced C# Topics

Advanced C# topics គឺជាផ្នែកដែលពង្រីកចំណេះដឹងរបស់អ្នកអំពី C# ដោយគ្របដណ្តប់អំពី reflection, attributes, dependency injection, design patterns, និង microservices។ ផ្នែកនេះជួយអ្នកក្លាយជា developer ដែលមានជំនាញខ្ពស់។

## 16.1 Reflection in C#

Reflection គឺជាបច្ចេកទេសដែលអនុញ្ញាតឱ្យអ្នកពិនិត្យនិងគ្រប់គ្រង metadata នៃ types, methods, properties, និង fields នៅ runtime។

ឧទាហរណ៍នៃ reflection៖

```csharp
using System.Reflection;

Type type = typeof(string);
Console.WriteLine("Type Name: " + type.Name);

MethodInfo[] methods = type.GetMethods();
foreach (var method in methods) {
    Console.WriteLine("Method: " + method.Name);
}
```

## 16.2 Attributes and Annotations

Attributes គឺជាវិធីដើម្បីបន្ថែម metadata ទៅកាន់ types, methods, properties, និង fields។ ពួកវាត្រូវបានប្រើជាញឹកញាប់ក្នុង serialization, validation, និង dependency injection។

ឧទាហរណ៍នៃ attributes៖

```csharp
[Serializable]
public class Person {
    [Required]
    public string Name { get; set; }

    [Range(1, 100)]
    public int Age { get; set; }
}
```

## 16.3 Dependency Injection (DI)

Dependency Injection (DI) គឺជាវិធីសាស្រ្តសម្រាប់ការគ្រប់គ្រង dependencies នៅក្នុងកម្មវិធី។ វាជួយធ្វើឱ្យកូដកាន់តែអាចធ្វើតេស្តបាននិងអាចពង្រីកបាន។

ឧទាហរណ៍នៃ dependency injection៖

```csharp
public interface IMessageService {
    void SendMessage(string message);
}

public class EmailService : IMessageService {
    public void SendMessage(string message) {
        Console.WriteLine("Email sent: " + message);
    }
}

public class Notification {
    private readonly IMessageService _messageService;

    public Notification(IMessageService messageService) {
        _messageService = messageService;
    }

    public void Notify(string message) {
        _messageService.SendMessage(message);
    }
}

// Registering services in ASP.NET Core
public void ConfigureServices(IServiceCollection services) {
    services.AddTransient<IMessageService, EmailService>();
}
```

## 16.4 Design Patterns (Singleton, Factory, Observer)

Design patterns គឺជាដំណោះស្រាយដែលបានបង្កើតឡើងសម្រាប់បញ្ហាទូទៅនៅក្នុងការអភិវឌ្ឍកម្មវិធី។ ពួកវាជួយធ្វើឱ្យកូដកាន់តែអាចរក្សាទុកបាននិងអាចពង្រីកបាន។

ឧទាហរណ៍នៃ design patterns៖

```csharp
// Singleton Pattern
public class Singleton {
    private static Singleton _instance;
    private Singleton() {}

    public static Singleton Instance {
        get {
            if (_instance == null) {
                _instance = new Singleton();
            }
            return _instance;
        }
    }
}

// Factory Pattern
public interface IProduct {
    void Create();
}

public class ProductA : IProduct {
    public void Create() {
        Console.WriteLine("Product A created.");
    }
}

public class ProductB : IProduct {
    public void Create() {
        Console.WriteLine("Product B created.");
    }
}

public class ProductFactory {
    public IProduct CreateProduct(string type) {
        switch (type) {
            case "A": return new ProductA();
            case "B": return new ProductB();
            default: throw new ArgumentException("Invalid product type.");
        }
    }
}

// Observer Pattern
public class Subject {
    private List<IObserver> _observers = new List<IObserver>();

    public void Attach(IObserver observer) {
        _observers.Add(observer);
    }

    public void Notify() {
        foreach (var observer in _observers) {
            observer.Update();
        }
    }
}

public interface IObserver {
    void Update();
}

public class Observer : IObserver {
    public void Update() {
        Console.WriteLine("Observer updated.");
    }
}
```

## 16.5 Microservices with .NET

Microservices គឺជារចនាសម្ព័ន្ធសម្រាប់ការអភិវឌ្ឍកម្មវិធីដែលបែងចែកកម្មវិធីជាសេវាកម្មតូចៗដែលអាចដំណើរការដាច់ដោយឡែកពីគ្នា។ .NET ផ្តល់នូវឧបករណ៍ដូចជា ASP.NET Core សម្រាប់ការបង្កើត microservices។

ឧទាហរណ៍នៃ microservice៖

```csharp
[ApiController]
[Route("api/[controller]")]
public class ProductsController : ControllerBase {
    [HttpGet]
    public IEnumerable<string> Get() {
        return new string[] { "Product1", "Product2" };
    }
}
```
