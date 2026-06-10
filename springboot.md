# មេរៀនទី១: ការណែនាំអំពី Java និង Spring Boot (Module 1: Introduction to Java & Spring Boot)

### 📖 សេចក្តីផ្តើម (Introduction):
Java គឺជាភាសាសរសេរកម្មវិធីដ៏មានអានុភាព តម្រង់ទិសវត្ថុ (Object-Oriented) ដែលត្រូវបានប្រើប្រាស់យ៉ាងទូលំទូលាយសម្រាប់កម្មវិធីសហគ្រាស (Enterprise Applications)។ Spring Boot គឺជា Framework ដែលបង្កើតឡើងនៅលើ Spring Framework ដើម្បីសម្រួលដល់ការបង្កើតកម្មវិធី Java ដែលត្រៀមផលិតកម្ម (Production-Ready Applications) ជាមួយនឹងការកំណត់រចនាសម្ព័ន្ធតិចតួចបំផុត (Minimal Configuration)។

## 1.1. តើ Java ជាអ្វី? (What is Java?)

### 📌 និយមន័យ (Definition):

**Java** គឺជាភាសាសរសេរកម្មវិធីកម្រិតខ្ពស់ (High-level Programming Language) ដែលផ្អែកលើ Class (Class-based) និងតម្រង់ទិសវត្ថុ (Object-Oriented)។ វាត្រូវបានបង្កើតឡើងដោយ **James Gosling** នៅ **Sun Microsystems**(ឥឡូវជាកម្មសិទ្ធិរបស់ Oracle) ហើយបានចេញផ្សាយជាលើកដំបូងក្នុងឆ្នាំ 1995។

**គោលការណ៍សំខាន់របស់ Java:** *"Write Once, Run Anywhere" (WORA)* — មានន័យថា កូដ Java ដែលបាន Compile (Bytecode) អាចដំណើរការលើវេទិកាណាមួយដែលមាន Java Virtual Machine (JVM) ដោយមិនចាំបាច់ Compile ឡើងវិញ។

### 🔹 លក្ខណៈពិសេសសំខាន់ៗរបស់ Java (Key Features):

- **Platform Independent** – កូដ Java អាចដំណើរការលើប្រព័ន្ធប្រតិបត្តិការផ្សេងៗ (Windows, macOS, Linux) ដោយមិនចាំបាច់កែប្រែ។

- **Object-Oriented** – គាំទ្រ OOP Concepts: Classes, Objects, Inheritance, Polymorphism, Encapsulation, Abstraction។

- **Robust** – មានការគ្រប់គ្រងអង្គចងចាំល្អ (Garbage Collection) និង Exception Handling រឹងមាំ។

- **Secure** – មាន Security Manager និង Bytecode Verifier ដើម្បីការពារការវាយប្រហារ។

- **Multithreaded** – គាំទ្រការសរសេរកម្មវិធីប្រតិបត្តិដំណាលគ្នា (Concurrent Programming)។

- **Rich Standard Library** – មានបណ្ណាល័យស្តង់ដារធំទូលាយសម្រាប់ Data Structures, I/O, Networking, និង Utilities។

- **High Performance** – ប្រើ Just-In-Time (JIT) Compiler ដើម្បីបង្កើនល្បឿន។

### 📝 ឧទាហរណ៍កូដ Java ដំបូង (First Java Code Example):

```java
// This is a simple Java program
public class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, Welcome to Java!");
        System.out.println("Java is platform independent.");
    }
}

// Output:
// Hello, Welcome to Java!
// Java is platform independent.
```

## 1.2. តើ Spring Framework ជាអ្វី? (What is Spring Framework?)

### 📌 និយមន័យ (Definition):

**Spring Framework** គឺជា Framework បើកចំហរ (Open-source) និងស្រាល (Lightweight) សម្រាប់ភាសា Java។ វាផ្តល់នូវហេដ្ឋារចនាសម្ព័ន្ធគាំទ្រយ៉ាងទូលំទូលាយ (Comprehensive Infrastructure Support) សម្រាប់ការអភិវឌ្ឍកម្មវិធី Java កម្រិតសហគ្រាស (Enterprise Applications)។

Spring Framework គ្រប់គ្រងផ្នែកបច្ចេកទេសផ្សេងៗ (Plumbing) ដូចជា Object Creation, Dependency Management, Transaction Management ជាដើម ដើម្បីឱ្យអ្នកអភិវឌ្ឍអាចផ្តោតលើតក្កវិជ្ជាអាជីវកម្ម (Business Logic) តែប៉ុណ្ណោះ។

### 🔹 លក្ខណៈពិសេសស្នូលរបស់ Spring Framework (Core Features):

- **Inversion of Control (IoC) Container** – គ្រប់គ្រងការបង្កើតវត្ថុ (Object Creation) និងភាពអាស្រ័យ (Dependencies) តាមរយៈ Dependency Injection (DI)។

- **Aspect-Oriented Programming (AOP)** – បំបែកកង្វល់ឆ្លងកាត់ (Cross-cutting Concerns) ដូចជា Logging, Security, Transaction Management។

- **Data Access / Integration** – សម្រួលដល់ការចូលដំណើរការទិន្នន័យតាមរយៈ JDBC, ORM (JPA, Hibernate), JMS និង Transaction Management។

- **Web MVC Framework** – ផ្តល់នូវស្ថាបត្យកម្ម Model-View-Controller (MVC) សម្រាប់បង្កើតកម្មវិធី Web Application និង REST APIs។

- **Security** – គាំទ្រការផ្ទៀងផ្ទាត់អត្តសញ្ញាណ (Authentication) និងការអនុញ្ញាត (Authorization) យ៉ាងទូលំទូលាយ។

- **Testing** – គាំទ្រការធ្វើតេស្ត (Unit Testing, Integration Testing) ជាមួយ JUnit និង Mock Objects។

### 📝 ឧទាហរណ៍ Spring Framework Configuration (Java Config):

```java
// Spring Configuration using Java Config (without Spring Boot)
@Configuration
public class AppConfig {

    @Bean
    public UserService userService() {
        return new UserServiceImpl();
    }

    @Bean
    public UserRepository userRepository() {
        return new JdbcUserRepository();
    }
}

// Usage
ApplicationContext context = new AnnotationConfigApplicationContext(AppConfig.class);
UserService service = context.getBean(UserService.class);
service.getUserById(1L);
```

## 1.3. តើ Spring Boot ជាអ្វី? (What is Spring Boot?)

### 📌 និយមន័យ (Definition):

**Spring Boot** គឺជា Project មួយដែលត្រូវបានបង្កើតឡើងនៅលើ Spring Framework ដើម្បីសម្រួលដល់ការបង្កើត Spring Applications ដែលឈរដោយឯករាជ្យ (Stand-alone) និងត្រៀមផលិតកម្ម (Production-grade Applications)។

Spring Boot លុបបំបាត់ការកំណត់រចនាសម្ព័ន្ធដដែលៗ (Boilerplate Configuration) ដែលត្រូវការដោយ Spring Applications បែបប្រពៃណី។ វាអនុវត្តតាមគោលការណ៍ **"Convention over Configuration"** — មានន័យថា វាផ្តល់នូវការកំណត់លំនាំដើម (Default Configurations) ដោយស្វ័យប្រវត្តិ ដោយផ្អែកលើ Dependencies ដែលអ្នកបានបន្ថែម។

### 🔹 អ្វីដែល Spring Boot ផ្តល់ឱ្យ (What Spring Boot Provides):

- **Auto-configuration** – កំណត់រចនាសម្ព័ន្ធ Spring Beans ដោយស្វ័យប្រវត្តិផ្អែកលើ Dependencies ក្នុង Classpath។

- **Embedded Servers** – បង្កប់ Web Servers (Tomcat, Jetty, Undertow) ក្នុងកម្មវិធី — មិនត្រូវការដាក់ពង្រាយជា WAR ទេ។

- **Starter Dependencies** – ផ្តល់ Starter POMs ដែលប្រមូលផ្តុំ Dependencies ដែលពាក់ព័ន្ធជាកញ្ចប់តែមួយ (ឧ. spring-boot-starter-web)។

- **Production-Ready Features** – ផ្តល់ Actuator សម្រាប់ Monitoring, Metrics, Health Checks, និង Externalized Configuration។

- **No Code Generation** – មិនតម្រូវឱ្យបង្កើតកូដបន្ថែម ឬ XML Configuration ទេ។

- **Embedded Development Tools** – ផ្តល់ DevTools សម្រាប់ Automatic Restart និង Live Reload កំឡុងពេលអភិវឌ្ឍ។

## 1.4. គុណសម្បត្តិរបស់ Spring Boot (Advantages of Spring Boot)

### 📌 គុណសម្បត្តិសំខាន់ៗ (Key Advantages):

- **Easy to Start** – ការរៀបចំតិចតួចបំផុត ដើម្បីបង្កើត និងដំណើរការ Spring Application។

- **Auto-Configuration** – កំណត់រចនាសម្ព័ន្ធដោយស្វ័យប្រវត្តិ ផ្អែកលើ Classpath Dependencies។

- **Embedded Servers** – ដំណើរការកម្មវិធីជា Standalone JAR ជាមួយ Embedded Server (Tomcat, Jetty)។

- **Production-Ready** – ផ្តល់ Actuator សម្រាប់ការត្រួតពិនិត្យ (Monitoring) និង Health Checks។

- **Opinionated but Flexible** – ផ្តល់ការកំណត់លំនាំដើមសមរម្យ ប៉ុន្តែអាចកែប្រែបានតាមតម្រូវការ (Override Defaults)។

- **Microservices Ready** – សមស្របសម្រាប់ការបង្កើត Microservices Architecture តាមបែប Cloud-native។

- **Large Ecosystem** – ភ្ជាប់ជាមួយ Spring Projects ផ្សេងទៀតដូចជា Spring Cloud, Spring Data, Spring Security, Spring Kafka។

- **Reduced Development Time** – កាត់បន្ថយពេលវេលាអភិវឌ្ឍន៍យ៉ាងច្រើន ដោយសារ Auto-configuration និង Starter Dependencies។

## 1.5. ស្ថាបត្យកម្ម Spring Boot (Spring Boot Architecture)

### 📌 ស្ថាបត្យកម្មជាស្រទាប់ (Layered Architecture):

Spring Boot អនុវត្តតាមស្ថាបត្យកម្មជាស្រទាប់ (Layered Architecture) ដែលបែងចែកកម្មវិធីជា ៤ ស្រទាប់សំខាន់ៗ៖

### 1. Presentation Layer

គ្រប់គ្រង HTTP Requests និង Responses — ប្រើ Spring MVC Controllers និង REST Controllers។

```java
@RestController, @RequestMapping, @GetMapping
```

### 2. Business/Service Layer

ផ្ទុកតក្កវិជ្ជាអាជីវកម្ម (Business Logic) និង Transaction Management។

```java
@Service, @Transactional
```

### 3. Persistence Layer

គ្រប់គ្រងអន្តរកម្មជាមួយ Database — CRUD Operations, Query Methods។

```java
@Repository, JpaRepository, CrudRepository
```

### 4. Database Layer

Database ពិតប្រាកដ — MySQL, PostgreSQL, MongoDB, H2, etc.

Database Tables, Schema, Indexes

### 🔹 សមាសធាតុសំខាន់ៗរបស់ Spring Boot (Key Components):

- **Spring Boot Starter** – Dependency descriptors (ឧ. spring-boot-starter-web, spring-boot-starter-data-jpa)

- **Spring Boot AutoConfigurator** – កំណត់រចនាសម្ព័ន្ធ Spring Beans ដោយស្វ័យប្រវត្តិ

- **Spring Boot CLI** – Command-line tool សម្រាប់ដំណើរការ Groovy Scripts

- **Spring Boot Actuator** – ផ្តល់ Production-ready endpoints (health, info, metrics, env)

- **Spring Boot DevTools** – ឧបករណ៍ជំនួយសម្រាប់អភិវឌ្ឍន៍ (auto-restart, live reload)

```text
┌─────────────────────────────────────────────────────────────┐ │ Client (Browser / Mobile) │ │ HTTP Request │ └─────────────────────────────────┬───────────────────────────────┘ │ ▼ ┌─────────────────────────────────────────────────────────────┐ │ Presentation Layer │ │ ┌─────────────────────────────────────────────────────┐ │ │ │ Spring MVC / REST Controllers │ │ │ │ @RestController, @RequestMapping, @GetMapping │ │ │ └─────────────────────────────────────────────────────┘ │ └─────────────────────────────────┬───────────────────────────────┘ │ ▼ ┌─────────────────────────────────────────────────────────────┐ │ Business Layer │ │ ┌─────────────────────────────────────────────────────┐ │ │ │ Service Layer (@Service) │ │ │ │ Business Logic, Validation │ │ │ │ Transaction Management (@Transactional) │ │ │ └─────────────────────────────────────────────────────┘ │ └─────────────────────────────────┬───────────────────────────────┘ │ ▼ ┌─────────────────────────────────────────────────────────────┐ │ Persistence Layer │ │ ┌─────────────────────────────────────────────────────┐ │ │ │ Repository Layer (@Repository, JPA/Hibernate) │ │ │ │ Data Access Objects (DAOs) │ │ │ └─────────────────────────────────────────────────────┘ │ └─────────────────────────────────┬───────────────────────────────┘ │ ▼ ┌─────────────────────────────────────────────────────────────┐ │ Database Layer │ │ ┌─────────────────────────────────────────────────────┐ │ │ │ MySQL / PostgreSQL / MongoDB / H2 │ │ │ └─────────────────────────────────────────────────────┘ │ └─────────────────────────────────────────────────────────────┘
```

## 1.6. ការប្រៀបធៀប Spring Boot និង Spring Framework (Spring Boot vs Spring Framework)

| Spring Framework | Spring Boot |
| --- | --- |
| ត្រូវការការកំណត់រចនាសម្ព័ន្ធដោយដៃ (XML/Java Config) | ផ្តល់ Auto-configuration ដោយស្វ័យប្រវត្តិ |
| ត្រូវការ Dependency Management ច្បាស់លាស់ (explicit) | ប្រើ Starter Dependencies ដើម្បីសម្រួល |
| ដាក់ពង្រាយជា WAR ទៅកាន់ External Server | ដំណើរការជា Standalone JAR ជាមួយ Embedded Server |
| មិនមានលក្ខណៈពិសេស Production-ready | ផ្តល់ Actuator សម្រាប់ Monitoring និង Metrics |
| ត្រូវការកូដដដែលៗច្រើន (Boilerplate code) | កាត់បន្ថយ Boilerplate code យ៉ាងច្រើន |
| ការរៀបចំកម្មវិធីយឺតជាង (Slow setup) | ចាប់ផ្តើមកម្មវិធីលឿនតាមរយៈ Spring Initializr |
| ត្រូវការ Embedded Server Configuration ដោយដៃ | Embedded Server ត្រូវបានកំណត់ដោយស្វ័យប្រវត្តិ |

## 1.7. ការដំឡើង JDK (Installing JDK)

### 📌 JDK ជាអ្វី? (What is JDK?):

**JDK (Java Development Kit)** គឺជាកញ្ចប់ឧបករណ៍សម្រាប់អភិវឌ្ឍកម្មវិធី Java។ វារួមបញ្ចូល **JRE (Java Runtime Environment)** (សម្រាប់ដំណើរការកម្មវិធី) និង **Development Tools** (javac, jar, javadoc) សម្រាប់ Compile និង Build កម្មវិធី។

### 🔹 ជំហានដំឡើង JDK (Installation Steps):

1. ទាញយក JDK ពី **Oracle JDK** ឬ **OpenJDK** (Adoptium/Eclipse Temurin) — ណែនាំឱ្យប្រើ JDK 17 ឬ 21 (LTS versions)។

2. ដំណើរការ installer ហើយធ្វើតាមការណែនាំ (ប្រើ Default Settings ក៏បាន)។

3. កំណត់ **JAVA_HOME** Environment Variable៖

  - **Windows:** Control Panel → System → Advanced System Settings → Environment Variables → Add JAVA_HOME = C:\Program Files\Java\jdk-17

  - **macOS/Linux:** បន្ថែមក្នុង ~/.bashrc ឬ ~/.zshrc: export JAVA_HOME=/usr/lib/jvm/java-17-openjdk

4. បន្ថែម %JAVA_HOME%/bin (Windows) ឬ $JAVA_HOME/bin (macOS/Linux) ទៅ PATH variable។

5. ផ្ទៀងផ្ទាត់ការដំឡើងដោយបើក Terminal/Command Prompt ហើយវាយ:

```bash
java -version
javac -version
```

លទ្ធផលរំពឹងទុក (Expected Output):

```bash
java version "17.0.9" 2023-10-17 LTS
Java(TM) SE Runtime Environment (build 17.0.9+11-LTS-201)
javac 17.0.9
```

## 1.8. ការដំឡើង IDE (Installing IDE: IntelliJ IDEA / VS Code / Eclipse)

### 📌 IDE ជាអ្វី? (What is IDE?):

**IDE (Integrated Development Environment)** គឺជាកម្មវិធីដែលផ្តល់នូវឧបករណ៍គ្រប់គ្រងសម្រាប់ការសរសេរកូដ (Code Editor, Compiler, Debugger, Build Tools) រួមបញ្ចូលគ្នាក្នុងកម្មវិធីតែមួយ។

**IntelliJ IDEA (Recommended)**

- ទាញយក **IntelliJ IDEA Community Edition** (Free) ពី [jetbrains.com/idea](https://www.jetbrains.com/idea/download)

- ដំឡើងដោយធ្វើតាមការណែនាំ (Next → Next → Install)

- បើក IDE → New Project → Spring Initializr → ជ្រើសរើស Dependencies

- គុណសម្បត្តិ: Spring Boot Integration ល្អបំផុត, Intelligent Code Completion, Built-in Terminal

**VS Code**

- ទាញយក **Visual Studio Code** ពី [code.visualstudio.com](https://code.visualstudio.com/)

- ដំឡើង Extensions ខាងក្រោម៖

  - "Extension Pack for Java" (Microsoft)

  - "Spring Boot Extension Pack" (VMware)

  - "Spring Initializr Java Support"

- Ctrl+Shift+P → "Spring Initializr: Generate a Maven Project"

**Eclipse IDE**

- ទាញយក **Eclipse IDE for Enterprise Java and Web Developers** ពី [eclipse.org/downloads](https://www.eclipse.org/downloads)

- ដំឡើង Spring Tools 4 (STS) Plugin: Help → Eclipse Marketplace → Search "Spring Tools 4" → Install

- File → New → Spring Starter Project

## 1.9. ការដំឡើង Maven & Gradle (Installing Maven & Gradle)

### 📌 Build Tools ជាអ្វី? (What are Build Tools?):

**Build Tools** (Maven, Gradle) គឺជាឧបករណ៍សម្រាប់គ្រប់គ្រង Dependencies, Compile, Test, Package, និង Deploy កម្មវិធី Java។ Spring Boot គាំទ្រទាំង Maven និង Gradle។

**Maven**

- ទាញយកពី [maven.apache.org](https://maven.apache.org/download.cgi)

- ស្រង់ចេញ (Extract) ទៅថតមួយ (ឧ. C:\maven ឬ /opt/maven)

- កំណត់ MAVEN_HOME Environment Variable

- បន្ថែម %MAVEN_HOME%\bin (Windows) ឬ $MAVEN_HOME/bin (Linux/macOS) ទៅ PATH

- ផ្ទៀងផ្ទាត់: mvn -version

**Gradle**

- ទាញយកពី [gradle.org/releases](https://gradle.org/releases)

- ស្រង់ចេញ (Extract) ទៅថតមួយ (ឧ. C:\gradle ឬ /opt/gradle)

- កំណត់ GRADLE_HOME Environment Variable

- បន្ថែម %GRADLE_HOME%\bin ទៅ PATH

- ផ្ទៀងផ្ទាត់: gradle -version

### 💡 Note:

Spring Boot Projects រួមបញ្ចូល **Maven Wrapper** (mvnw) ឬ **Gradle Wrapper** (gradlew) ដែលទាញយក និងប្រើប្រាស់ Maven/Gradle ដោយស្វ័យប្រវត្តិ — អ្នកមិនចាំបាច់ដំឡើងដោយដៃទេ។ ទោះយ៉ាងណា ការដំឡើងដោយដៃជួយឱ្យអ្នកប្រើប្រាស់ Build Tools សម្រាប់គម្រោងផ្សេងទៀតផងដែរ។

## 1.10. ការបង្កើត Spring Boot Project ដំបូង (Creating First Spring Boot Project)

### 🔹 វិធីសាស្រ្ត ៣ យ៉ាង (3 Methods):

**Method 1: Spring Initializr (Web)** **—** **សាមញ្ញបំផុត**

1. ចូលទៅកាន់ [start.spring.io](https://start.spring.io/)

2. ជ្រើសរើស Project: **Maven** ឬ **Gradle**

3. ជ្រើសរើស Language: **Java**

4. ជ្រើសរើស Spring Boot Version: **3.2.x (stable)**

5. កំណត់ Group: com.example, Artifact: demo

6. ជ្រើសរើស Java Version: **17** ឬ **21**

7. បន្ថែម Dependencies: **Spring Web** (សម្រាប់ REST APIs)

8. ចុច **GENERATE** → ទាញយក ZIP file

9. ស្រង់ចេញ (Extract) និងបើកក្នុង IDE

**Method 2: IntelliJ IDEA (Built-in Spring Initializr)**

1. File → New → Project

2. ជ្រើសរើស **Spring Initializr**

3. កំណត់ SDK (JDK 17+)

4. កំណត់ Group, Artifact, Dependencies (Spring Web)

5. ចុច Finish → IDEA បង្កើត Project ដោយស្វ័យប្រវត្តិ

**Method 3: Spring Boot CLI (Command Line)**

```bash
# Install Spring Boot CLI (via SDKMAN - Mac/Linux)
sdk install springboot

# Or via Homebrew (Mac)
brew install springboot

# Generate project
spring init --dependencies=web --groupId=com.example --artifactId=demo --java-version=17 demo-app

# Navigate to project
cd demo-app
```

## 1.11. ការដំណើរការ Spring Boot Application (Running Spring Boot Application)

### 📌 Main Application Class:

រាល់ Spring Boot Application មាន Main Class ដែលមាន **@SpringBootApplication** annotation និង **main()** method។ @SpringBootApplication គឺជា combination នៃ annotations បី៖

```java
@Configuration – កំណត់ថា class នេះផ្តល់ Bean definitions
@EnableAutoConfiguration – បើក Auto-configuration mechanism
@ComponentScan – Scan រក Components, Services, Repositories ក្នុង package ដូចគ្នា
package com.example.demo;

import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.SpringBootApplication;
import org.springframework.web.bind.annotation.GetMapping;
import org.springframework.web.bind.annotation.RestController;

@SpringBootApplication
@RestController
public class DemoApplication {

    public static void main(String[] args) {
        SpringApplication.run(DemoApplication.class, args);
    }

    // Add a simple REST endpoint
    @GetMapping("/hello")
    public String sayHello() {
        return "Hello, Spring Boot!";
    }
}
```

### 🔹 វិធីដំណើរការ (Ways to Run):

**1. Run from IDE**

ចុចកណ្ដុរស្ដាំលើ DemoApplication.java → Run 'DemoApplication.main()'

**2. Run with Maven Wrapper**

```bash
# Windows
mvnw spring-boot:run

# Mac/Linux
./mvnw spring-boot:run
```

**3. Run with Gradle Wrapper**

```bash
# Windows
gradlew bootRun

# Mac/Linux
./gradlew bootRun
```

**4. Build and run as JAR**

```bash
# Build JAR
./mvnw package

# Run JAR
java -jar target/demo-0.0.1-SNAPSHOT.jar
```

**🌐 Access the Application:**

បន្ទាប់ពីដំណើរការដោយជោគជ័យ អ្នកនឹងឃើញលទ្ធផលក្នុង Console៖

```bash
Tomcat started on port(s): 8080 (http)
Started DemoApplication in 2.5 seconds
```

បើក Browser ហើយចូលទៅកាន់៖
http://localhost:8080/hello

## 1.12. រចនាសម្ព័ន្ធ Spring Boot Project (Spring Boot Project Structure)

### 📌 រចនាសម្ព័ន្ធថត (Directory Structure):

```text
demo-app/
├── pom.xml                          # Maven configuration (dependencies, plugins)
├── mvnw / mvnw.cmd                  # Maven wrapper scripts
├── .gitignore                       # Git ignore file
│
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/example/demo/
│   │   │       ├── DemoApplication.java          # Main application class
│   │   │       │
│   │   │       ├── controller/                   # REST API controllers
│   │   │       │   └── HelloController.java
│   │   │       │
│   │   │       ├── service/                      # Business logic layer
│   │   │       │   └── UserService.java
│   │   │       │
│   │   │       ├── repository/                   # Data access layer
│   │   │       │   └── UserRepository.java
│   │   │       │
│   │   │       ├── model/                        # Entity/DTO classes
│   │   │       │   └── User.java
│   │   │       │
│   │   │       └── config/                       # Configuration classes
│   │   │           └── AppConfig.java
│   │   │
│   │   └── resources/
│   │       ├── application.properties            # Main configuration file
│   │       ├── application-dev.properties        # Dev environment config
│   │       ├── application-prod.properties       # Production config
│   │       │
│   │       ├── static/                           # Static files (CSS, JS, images)
│   │       │   ├── css/
│   │       │   ├── js/
│   │       │   └── images/
│   │       │
│   │       ├── templates/                        # View templates (Thymeleaf)
│   │       │   └── index.html
│   │       │
│   │       └── db/
│   │           └── migration/                    # Database migration scripts
│   │
│   └── test/
│       └── java/
│           └── com/example/demo/
│               ├── DemoApplicationTests.java     # Integration tests
│               └── controller/
│                   └── HelloControllerTest.java  # Unit tests
```

### 🔹 ឯកសារសំខាន់ៗ (Important Files):

| File | Description | Example<br>// ERROR: This line has incorrect JSX syntax |
| --- | --- | --- |
| pom.xml (Maven) | Project Object Model — កំណត់ dependencies, plugins, project metadata | spring-boot-starter-web |
| build.gradle (Gradle) | Gradle build script — កំណត់ dependencies និង tasks | implementation 'org.springframework.boot:spring-boot-starter-web' |
| application.properties | Main configuration file — server port, database connection, logging | server.port=9090 |
| DemoApplication.java | Entry point — contains @SpringBootApplication and main() | SpringApplication.run() |

### 📝 Example: application.properties

```properties
# Server configuration
server.port=8080
server.servlet.context-path=/api

# Database configuration (for MySQL)
spring.datasource.url=jdbc:mysql://localhost:3306/mydb
spring.datasource.username=root
spring.datasource.password=secret

# JPA configuration
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQL8Dialect

# Logging
logging.level.org.springframework=INFO
logging.level.com.example.demo=DEBUG
```

### 📚 សង្ខេបមេរៀនទី១ (Module 1 Summary)

នៅក្នុងមេរៀននេះ អ្នកបានរៀនអំពី៖

- **Java** – ភាសាសរសេរកម្មវិធី Platform-independent, Object-Oriented, Robust, Secure

- **Spring Framework** – Framework សម្រាប់ Enterprise Java Development (IoC, AOP, MVC)

- **Spring Boot** – Extension of Spring for rapid development with Auto-configuration, Embedded Servers, Starter Dependencies

- **Advantages of Spring Boot** – Easy setup, Production-ready, Microservices support

- **Spring Boot Architecture** – Layered architecture (Presentation, Business, Persistence, Database)

- **Environment Setup** – JDK installation, IDE setup (IntelliJ/VS Code/Eclipse), Maven/Gradle

- **Creating Spring Boot Project** – Using Spring Initializr, IntelliJ, or CLI

- **Running the Application** – IDE, Maven/Gradle commands, or JAR file

- **Project Structure** – Understanding the directory layout and key files

# មេរៀនទី២: មូលដ្ឋានគ្រឹះ Java សម្រាប់ Spring Boot (Java Fundamentals for Spring Boot)

### 📖 សេចក្តីផ្តើម (Introduction):
Java គឺជាភាសាសរសេរកម្មវិធីដ៏មានអានុភាព និងពេញនិយមបំផុតក្នុងពិភពកម្មវិធី។ Spring Boot គឺជា Framework ដែលបង្កើតឡើងនៅលើ Java ដូច្នេះការយល់ដឹងពី Java គឺជារឿងចាំបាច់បំផុតមុននឹងរៀន Spring Boot។ មេរៀននេះនឹងពន្យល់លម្អិតពីគ្រប់មូលដ្ឋានគ្រឹះរបស់ Java ដែលអ្នកត្រូវការសម្រាប់ Spring Boot។

## 2.1. អថេរ និងប្រភេទទិន្នន័យ (Variables and Data Types)

### 📌 និយមន័យ (Definition):

**Variable (****អថេរ)** គឺជាឈ្មោះដែលប្រើសម្រាប់សំដៅទៅកាន់ទីតាំងផ្ទុកទិន្នន័យក្នុងអង្គចងចាំ (Memory)។ វាដូចជា "ប្រអប់" មួយដែលយើងដាក់តម្លៃទុក ហើយយើងអាចហៅវាមកប្រើវិញតាមរយៈឈ្មោះរបស់វា។

**Data Type (****ប្រភេទទិន្នន័យ)** គឺជាការកំណត់ថា variable អាចផ្ទុកទិន្នន័យប្រភេទណាខ្លះ (ចំនួនគត់, ចំនួនទសភាគ, តួអក្សរ, ។ល។) និងកំណត់ទំហំអង្គចងចាំដែលត្រូវប្រើ។

### 🔹 ប្រភេទទិន្នន័យបឋម (Primitive Data Types) មាន ៨ ប្រភេទ៖

| Data Type | Size | Range | Example |
| --- | --- | --- | --- |
| byte | 1 byte | -128 to 127 | byte b = 100; |
| short | 2 bytes | -32,768 to 32,767 | short s = 30000; |
| int | 4 bytes | -2B to 2B | int age = 25; |
| long | 8 bytes | -9 quintillion to 9 quintillion | long l = 100000L; |
| float | 4 bytes | ~6-7 decimal digits | float f = 3.14f; |
| double | 8 bytes | ~15-16 decimal digits | double d = 99.99; |
| char | 2 bytes | Single character (Unicode) | char c = 'A'; |
| boolean | 1 bit | true or false | boolean b = true; |

### 📝 ឧទាហរណ៍កូដ (Code Example):

```java
// Declaration and Initialization
int age = 25;
double salary = 55000.50;
boolean isEmployed = true;
char grade = 'A';
String name = "Sok Dara";

// Output
System.out.println("Name: " + name);
System.out.println("Age: " + age);
```

## 2.2. ប្រមាណវិធី (Operators)

### 📌 និយមន័យ (Definition):

**Operators (****ប្រមាណវិធី)** គឺជានិមិត្តសញ្ញាពិសេសដែលប្រើដើម្បីអនុវត្តប្រតិបត្តិការលើអថេរ (variables) និងតម្លៃ (values)។ ឧទាហរណ៍៖ + ប្រើសម្រាប់បូក, - ប្រើសម្រាប់ដក, * ប្រើសម្រាប់គុណ។

### 🔹 ប្រភេទ Operators សំខាន់ៗ៖

| Category | Operators | Description | Example |
| --- | --- | --- | --- |
| Arithmetic | + - * / % | Basic math operations | 10 % 3 = 1 |
| Relational | == != > < >= <= | Compare values → true/false | 5 > 3 → true |
| Logical | && \|\| ! | AND, OR, NOT operations | true && false = false |
| Assignment | = += -= *= /= %= | Assign values to variables | x += 5 |
| Increment/Decrement | ++ -- | Increase/decrease by 1 | x++ |

```text
int a = 10, b = 3;
int sum = a + b;        // 13
int product = a * b;    // 30
int remainder = a % b;  // 1

boolean isEqual = (a == b);     // false
boolean isGreater = (a > b);    // true
boolean result = (a > 5 && b < 5); // true

a++;  // a becomes 11
b--;  // b becomes 2
```

## 2.3. សេចក្តីថ្លែងលក្ខខណ្ឌ (Conditional Statements)

### 📌 និយមន័យ (Definition):

**Conditional Statements (****សេចក្តីថ្លែងលក្ខខណ្ឌ)** ត្រូវបានប្រើដើម្បីធ្វើការសម្រេចចិត្ត (Decision Making) ក្នុងកម្មវិធី។ វាអនុញ្ញាតឱ្យកម្មវិធីប្រតិបត្តិកូដផ្សេងគ្នា អាស្រ័យលើលក្ខខណ្ឌដែលបានកំណត់។

```java
int score = 85;

if (score >= 90) {
    System.out.println("Grade A");
} else if (score >= 80) {
    System.out.println("Grade B");  // This runs
} else if (score >= 70) {
    System.out.println("Grade C");
} else {
    System.out.println("Need Improvement");
}
```

## 2.4. វដ្ត (Loops)

### 📌 និយមន័យ (Definition):

**Loops (****វដ្ត)** ត្រូវបានប្រើដើម្បីធ្វើប្រតិបត្តិការដដែលៗ (Repeat) ច្រើនដង។ Loops ជួយសន្សំសំចៃពេលវេលា និងកាត់បន្ថយកូដដដែលៗ។

```java
// for loop
for (int i = 1; i <= 5; i++) {
    System.out.println("Count: " + i);
}

// while loop
int count = 0;
while (count < 5) {
    System.out.println("While count: " + count);
    count++;
}

// do-while loop
int x = 0;
do {
    System.out.println("Do-while: " + x);
    x++;
} while (x < 3);

// for-each loop
int[] numbers = {10, 20, 30, 40, 50};
for (int num : numbers) {
    System.out.print(num + " ");
}
```

## 2.5. អារេ (Arrays)

### 📌 និយមន័យ (Definition):

**Array (****អារេ)** គឺជា container ដែលផ្ទុកធាតុច្រើន (multiple elements) ដែលមានប្រភេទទិន្នន័យដូចគ្នា និងទំហំ (size) ថេរ។ ធាតុនីមួយៗក្នុង array អាចចូលដំណើរការបានតាមរយៈ index (ចាប់ផ្តើមពី 0)។

```java
// Array declaration and initialization
int[] numbers = {10, 20, 30, 40, 50};
String[] names = new String[3];
names[0] = "Sok";
names[1] = "Dara";
names[2] = "Cheata";

// Accessing array elements
System.out.println("First number: " + numbers[0]);
System.out.println("Second name: " + names[1]);

// Loop through array
for (int i = 0; i < numbers.length; i++) {
    System.out.println("numbers[" + i + "] = " + numbers[i]);
}
```

## 2.6. មេតូដ (Methods / Functions)

### 📌 និយមន័យ (Definition):

**Method (****មេតូដ)** គឺជា block នៃកូដដែលអនុវត្តការងារជាក់លាក់មួយ។ Method ជួយឱ្យកូដអាចប្រើឡើងវិញបាន (reusability) និងធ្វើឱ្យកម្មវិធីងាយស្រួលថែទាំ។

```java
// Method without parameters and no return value
public void sayHello() {
    System.out.println("Hello!");
}

// Method with parameters and return value
public int add(int a, int b) {
    return a + b;
}

// Method with return type String
public String greetUser(String name) {
    return "Welcome, " + name + "!";
}

// Method overloading
public int multiply(int a, int b) { return a * b; }
public int multiply(int a, int b, int c) { return a * b * c; }

// Calling methods
sayHello();
int sum = add(5, 3);
String message = greetUser("Sok");
```

## 2.7. ការសរសេរកម្មវិធីតម្រង់ទិសវត្ថុ (Object-Oriented Programming - OOP)

### 📌 និយមន័យ (Definition):

**Object-Oriented Programming (OOP)** គឺជា Programming Paradigm ដែលរៀបចំកូដជុំវិញ **Objects** (វត្ថុ) ជំនួសឱ្យ functions ឬ logic ។ Objects នីមួយៗមាន data (fields/attributes) និង behavior (methods)។

### 🔹 គោលការណ៍សំខាន់ៗរបស់ OOP (4 Pillars of OOP):

- **Encapsulation** – លាក់ data មិនឱ្យចូលដំណើរការដោយផ្ទាល់

- **Inheritance** – ទទួលមរតក properties/methods ពី parent class

- **Polymorphism** – ទម្រង់ច្រើន - method ដូចគ្នា ឥរិយាបថខុសគ្នា

- **Abstraction** – លាក់ implementation details បង្ហាញតែ functionality

## 2.8. ថ្នាក់ និងវត្ថុ (Classes and Objects)

### 📌 និយមន័យ (Definition):

**Class (****ថ្នាក់)** គឺជា blueprint ឬ template ដែលកំណត់ properties (fields) និង behaviors (methods) របស់ object។

**Object (****វត្ថុ)** គឺជា instance មួយនៃ class។ Object មានស្ថានភាព (state) និងឥរិយាបថ (behavior)។

```properties
// Class definition
public class Student {
    String name;
    int age;
    String studentId;

    // Constructor
    public Student(String name, int age, String studentId) {
        this.name = name;
        this.age = age;
        this.studentId = studentId;
    }

    // Method
    public void study() {
        System.out.println(name + " is studying...");
    }
}

// Creating objects
Student student1 = new Student("Sokha", 20, "S001");
Student student2 = new Student("Dara", 22, "S002");

student1.study();  // Sokha is studying...
student2.study();  // Dara is studying...
```

## 2.9. មរតក (Inheritance)

### 📌 និយមន័យ (Definition):

**Inheritance (****មរតក)** គឺជាយន្តការដែលអនុញ្ញាតឱ្យ class មួយ (child class / subclass) ទទួលមរតក fields និង methods ពី class មួយទៀត (parent class / superclass)។ ប្រើពាក្យគន្លឹះ extends។

```properties
// Parent class
class Animal {
    String name;
    public void eat() {
        System.out.println(name + " is eating...");
    }
}

// Child class
class Dog extends Animal {
    public void bark() {
        System.out.println(name + " is barking!");
    }
}

// Usage
Dog myDog = new Dog();
myDog.name = "Bobby";
myDog.eat();   // Inherited method
myDog.bark();  // Dog's own method
```

## 2.10. ពហុរូបភាព (Polymorphism)

### 📌 និយមន័យ (Definition):

**Polymorphism (****ពហុរូបភាព)** មានន័យថា "ទម្រង់ច្រើន"។ វាអនុញ្ញាតឱ្យ objects នៃ classes ផ្សេងគ្នាឆ្លើយតបទៅនឹង method ដូចគ្នាតាមរបៀបផ្សេងៗគ្នា។

```java
class Shape {
    public void draw() {
        System.out.println("Drawing a shape...");
    }
}

class Circle extends Shape {
    @Override
    public void draw() {
        System.out.println("Drawing a circle");
    }
}

class Rectangle extends Shape {
    @Override
    public void draw() {
        System.out.println("Drawing a rectangle");
    }
}

// Polymorphic behavior
Shape shape1 = new Circle();
Shape shape2 = new Rectangle();
shape1.draw();  // Drawing a circle
shape2.draw();  // Drawing a rectangle
```

## 2.11. ការបិទបាំងទិន្នន័យ (Encapsulation)

### 📌 និយមន័យ (Definition):

**Encapsulation (****ការបិទបាំងទិន្នន័យ)** គឺជាការលាក់ data (fields) ដោយធ្វើឱ្យវា privateនិងផ្តល់ access តាមរយៈ public methods (getters/setters)។

```java
public class BankAccount {
    private double balance;

    public void deposit(double amount) {
        if (amount > 0) {
            balance += amount;
        }
    }

    public double getBalance() {
        return balance;
    }
}

// Usage
BankAccount account = new BankAccount();
account.deposit(500);
System.out.println("Balance: " + account.getBalance());
```

## 2.12. អរូបីកម្ម (Abstraction)

### 📌 និយមន័យ (Definition):

**Abstraction (****អរូបីកម្ម)** គឺជាការលាក់ implementation details និងបង្ហាញតែ essential features ដល់អ្នកប្រើប្រាស់។ ក្នុង Java, abstraction សម្រេចបានតាមរយៈ **Abstract Classes** និង **Interfaces**។

```java
abstract class Vehicle {
    public abstract void startEngine();
}

class Car extends Vehicle {
    @Override
    public void startEngine() {
        System.out.println("Car engine started!");
    }
}

Vehicle myCar = new Car();
myCar.startEngine();  // Car engine started!
```

## 2.13. អ៊ីនធឺហ្វេស (Interfaces)

### 📌 និយមន័យ (Definition):

**Interface (****អ៊ីនធឺហ្វេស)** គឺជា contract ដែលកំណត់ methods ដែល class ត្រូវតែ implement។ Interface អនុញ្ញាតឱ្យ Java សម្រេចបាន Multiple Inheritance (class មួយអាច implement interfaces បានច្រើន)។

```properties
interface Drawable {
    void draw();
}

interface Colorable {
    void setColor(String color);
}

class Circle implements Drawable, Colorable {
    private String color;

    @Override
    public void draw() {
        System.out.println("Drawing a " + color + " circle");
    }

    @Override
    public void setColor(String color) {
        this.color = color;
    }
}

Circle circle = new Circle();
circle.setColor("Red");
circle.draw();  // Drawing a Red circle
```

## 2.14. ការគ្រប់គ្រងករណីលើកលែង (Exception Handling)

### 📌 និយមន័យ (Definition):

**Exception (****ករណីលើកលែង)** គឺជា event ដែលរំខានដល់លំហូរធម្មតានៃកម្មវិធី។**Exception Handling** គឺជាយន្តការដែលការពារកម្មវិធីពីការបរាជ័យ (crash)។

```java
try {
    int[] numbers = {1, 2, 3};
    System.out.println(numbers[5]);
} catch (ArrayIndexOutOfBoundsException e) {
    System.out.println("Array index out of bounds!");
} finally {
    System.out.println("This always executes!");
}

// Custom exception
public void validateAge(int age) {
    if (age < 0) {
        throw new IllegalArgumentException("Age cannot be negative!");
    }
}
```

## 2.15. បណ្តុំនៃការប្រមូលទិន្នន័យ (Collections Framework)

### 📌 និយមន័យ (Definition):

**Java Collections Framework** គឺជាសំណុំនៃ classes និង interfaces ដែលផ្តល់នូវ data structures សម្រាប់ផ្ទុក និងរៀបចំក្រុមទិន្នន័យ (groups of objects)។

```java
import java.util.*;

// List - ordered, allows duplicates
List<String> names = new ArrayList<>();
names.add("Sok");
names.add("Dara");
names.add("Sok");

// Set - no duplicates
Set<String> uniqueNames = new HashSet<>();
uniqueNames.add("Sok");
uniqueNames.add("Dara");

// Map - key-value pairs
Map<String, Integer> scores = new HashMap<>();
scores.put("Sok", 85);
scores.put("Dara", 92);

System.out.println("Sok's score: " + scores.get("Sok"));
```

## 2.16. ហ្សេណេរិច (Generics)

### 📌 និយមន័យ (Definition):

**Generics (****ហ្សេណេរិច)** គឺជា feature ដែលអនុញ្ញាតឱ្យ class, interface, ឬ method ដំណើរការលើប្រភេទទិន្នន័យផ្សេងៗ ខណៈពេលដែលរក្សាបាននូវ type safety។

```java
// Generic class
class Box<T> {
    private T content;
    public void setContent(T content) { this.content = content; }
    public T getContent() { return content; }
}

// Usage
Box<String> stringBox = new Box<>();
stringBox.setContent("Hello");
String value = stringBox.getContent();

Box<Integer> intBox = new Box<>();
intBox.setContent(100);
```

## 2.17. ឡាំបដា អិចស្ប្រេសស្យុង (Lambda Expressions)

### 📌 និយមន័យ (Definition):

**Lambda Expression (****ឡាំបដា អិចស្ប្រេសស្យុង)** គឺជា function គ្មានឈ្មោះ (anonymous function) ដែលអាចឆ្លងកាត់ជា argument ឬរក្សាទុកជា variable។

```java
Syntax: (parameters) -> body
// Lambda with no parameter
Runnable task = () -> System.out.println("Hello Lambda!");

// Lambda with one parameter
Consumer<String> printer = msg -> System.out.println(msg);

// Lambda with two parameters
BinaryOperator<Integer> add = (a, b) -> a + b;

// Using lambda with collections
List<String> names = Arrays.asList("Dara", "Sok", "Cheata");
names.sort((a, b) -> a.compareTo(b));
names.forEach(name -> System.out.println(name));

// Method reference
names.forEach(System.out::println);
```

## 2.18. ស្ទ្រីម API (Streams API)

### 📌 និយមន័យ (Definition):

**Stream API (Java 8+)** គឺជា feature ដែលអនុញ្ញាតឱ្យយើងដំណើរការ collections of objects តាមបែប functional programming ជំនួសឱ្យការសរសេរ loops ដោយដៃ។

```java
import java.util.*;
import java.util.stream.*;

List<Integer> numbers = Arrays.asList(1, 2, 3, 4, 5, 6, 7, 8, 9, 10);

// filter - select elements
List<Integer> evenNumbers = numbers.stream()
```

.filter(n -> n % 2 == 0)

```text
    .collect(Collectors.toList());

// map - transform elements
List<Integer> squares = numbers.stream()
```

.map(n -> n * n)

```java
    .collect(Collectors.toList());

// reduce - combine elements
int sum = numbers.stream()
    .reduce(0, (a, b) -> a + b);

// forEach - perform action
numbers.stream().forEach(n -> System.out.print(n + " "));

// Collectors grouping
Map<Boolean, List<Integer>> partitioned = numbers.stream()
    .collect(Collectors.partitioningBy(n -> n > 5));
```

### 📚 សង្ខេបមេរៀនទី២ (Module 2 Summary)

នៅក្នុងមេរៀននេះ អ្នកបានរៀនអំពីមូលដ្ឋានគ្រឹះសំខាន់ៗរបស់ Java ដែលអ្នកត្រូវការសម្រាប់ Spring Boot៖

- **Variables & Data Types** – int, double, boolean, String

- **Operators** – Arithmetic, Relational, Logical, Assignment

- **Conditionals** – if-else, switch

- **Loops** – for, while, do-while, for-each

- **Arrays** – single and multi-dimensional arrays

- **Methods** – parameters, return types, overloading

- **OOP (4 Pillars)** – Encapsulation, Inheritance, Polymorphism, Abstraction

- **Classes & Objects** – creating and using objects

- **Interfaces** – contracts, multiple inheritance

- **Exception Handling** – try-catch-finally, throw, throws

- **Collections Framework** – List, Set, Map, Queue

- **Generics** – type-safe classes and methods

- **Lambda Expressions** – functional programming

- **Streams API** – declarative data processing

# មេរៀនទី៣: មូលដ្ឋានគ្រឹះ Spring Boot (Module 3: Spring Boot Basics)

### 📖 សេចក្តីផ្តើម (Introduction):
មេរៀននេះនឹងណែនាំអ្នកអំពីមូលដ្ឋានគ្រឹះសំខាន់ៗរបស់ Spring Boot ដែលអ្នកត្រូវការដើម្បីចាប់ផ្តើមបង្កើតកម្មវិធី។ អ្នកនឹងរៀនពី Spring Initializr, Dependencies Management, Configuration Files (properties/yml), Auto Configuration, DevTools, Running on Different Ports, Profiles, និង Logging។

## 3.1. Spring Initializr

### 📌 និយមន័យ (Definition):

**Spring Initializr** គឺជា Web-based tool (https://start.spring.io) ដែលផ្តល់ដោយ Spring Team សម្រាប់បង្កើត (Bootstrap) Spring Boot Projects យ៉ាងរហ័ស។ វាអនុញ្ញាតឱ្យអ្នកជ្រើសរើស៖

- Build Tool: **Maven** ឬ **Gradle**

- Language: **Java**, **Kotlin**, ឬ **Groovy**

- Spring Boot Version (Stable Release)

- Project Metadata: Group, Artifact, Name, Description, Package Name

- Java Version: 17, 21, ឬ 22

- Dependencies (Starters) ដែលត្រូវការ

### 🔹 ជំហានបង្កើត Project តាមរយៈ Spring Initializr:

1. ចូលទៅកាន់ [start.spring.io](https://start.spring.io/)

2. ជ្រើសរើស Project: **Maven** (សម្រាប់អ្នកចាប់ផ្តើម) ឬ **Gradle**

3. ជ្រើសរើស Language: **Java**

4. ជ្រើសរើស Spring Boot Version: **3.2.x** (Latest Stable)

5. កំណត់ Group: com.example (បញ្ច្រាស domain name)

6. កំណត់ Artifact: demo (ឈ្មោះ project)

7. កំណត់ Name: demo (ឈ្មោះ application)

8. កំណត់ Description: ពិពណ៌នាអំពី project

9. កំណត់ Package name: com.example.demo

10. កំណត់ Packaging: **Jar** (សម្រាប់ microservices) ឬ **War** (សម្រាប់ deployment ទៅ server)

11. កំណត់ Java Version: **17** ឬ **21** (LTS versions)

12. បន្ថែម Dependencies: ឧ. **Spring Web**, **Spring Data JPA**, **Lombok**, **DevTools**

13. ចុច **GENERATE** → ទាញយក ZIP file

14. ស្រង់ចេញ (Extract) ZIP file ហើយបើកក្នុង IDE

### 💡 Alternative Methods:

- **IntelliJ IDEA Ultimate** → New Project → Spring Initializr

- **VS Code** → Command Palette → Spring Initializr: Generate a Maven Project

- **Spring Boot CLI**: spring init --dependencies=web,data-jpa demo-app

## 3.2. ការគ្រប់គ្រង Dependencies (Dependencies Management)

### 📌 និយមន័យ (Definition):

**Dependencies Management** គឺជាការគ្រប់គ្រងបណ្ណាល័យ (Libraries) និង Framework ដែលកម្មវិធីរបស់អ្នកត្រូវការ។ Spring Boot ប្រើ **Maven** ឬ **Gradle** ដើម្បីគ្រប់គ្រង dependencies ដោយស្វ័យប្រវត្តិ។

### 🔹 Maven (pom.xml) - Dependency Declaration:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<project xmlns="http://maven.apache.org/POM/4.0.0">
    <modelVersion>4.0.0</modelVersion>

    <!-- Parent: Spring Boot Starter Parent -->
    <parent>
        <groupId>org.springframework.boot</groupId>
        <artifactId>spring-boot-starter-parent</artifactId>
        <version>3.2.0</version>
    </parent>

    <groupId>com.example</groupId>
    <artifactId>demo</artifactId>
    <version>0.0.1-SNAPSHOT</version>
    <name>demo</name>
    <description>Demo Spring Boot Application</description>

    <properties>
        <java.version>17</java.version>
    </properties>

    <dependencies>
        <!-- Spring Boot Web Starter (REST APIs, Tomcat embedded) -->
        <dependency>
            <groupId>org.springframework.boot</groupId>
            <artifactId>spring-boot-starter-web</artifactId>
        </dependency>

        <!-- Spring Boot Data JPA (Database access) -->
        <dependency>
            <groupId>org.springframework.boot</groupId>
            <artifactId>spring-boot-starter-data-jpa</artifactId>
        </dependency>

        <!-- MySQL Driver -->
        <dependency>
            <groupId>com.mysql</groupId>
            <artifactId>mysql-connector-j</artifactId>
            <scope>runtime</scope>
        </dependency>

        <!-- Lombok (Reduce boilerplate code) -->
        <dependency>
            <groupId>org.projectlombok</groupId>
            <artifactId>lombok</artifactId>
            <optional>true</optional>
        </dependency>

        <!-- Spring Boot DevTools (Auto-restart, Live reload) -->
        <dependency>
            <groupId>org.springframework.boot</groupId>
            <artifactId>spring-boot-devtools</artifactId>
            <scope>runtime</scope>
            <optional>true</optional>
        </dependency>

        <!-- Spring Boot Test -->
        <dependency>
            <groupId>org.springframework.boot</groupId>
            <artifactId>spring-boot-starter-test</artifactId>
            <scope>test</scope>
        </dependency>
    </dependencies>

    <build>
        <plugins>
            <plugin>
                <groupId>org.springframework.boot</groupId>
                <artifactId>spring-boot-maven-plugin</artifactId>
            </plugin>
        </plugins>
    </build>
</project>
```

### 🔹 Gradle (build.gradle) - Dependency Declaration:

```groovy
plugins {
```

id 'java'

id 'org.springframework.boot' version '3.2.0'

id 'io.spring.dependency-management' version '1.1.4'

```groovy
}

group = 'com.example'
version = '0.0.1-SNAPSHOT'

java {
    sourceCompatibility = '17'
}

repositories {
```

mavenCentral()

```groovy
}

dependencies {
```

implementation 'org.springframework.boot:spring-boot-starter-web'

implementation 'org.springframework.boot:spring-boot-starter-data-jpa'

runtimeOnly 'com.mysql:mysql-connector-j'

compileOnly 'org.projectlombok:lombok'

annotationProcessor 'org.projectlombok:lombok'

developmentOnly 'org.springframework.boot:spring-boot-devtools'

testImplementation 'org.springframework.boot:spring-boot-starter-test'

```groovy
}

tasks.named('test') {
```

useJUnitPlatform()

```text
}
```

### 💡 Maven vs Gradle Comparison:

| កត្តា (Factor) | Maven | Gradle |
| --- | --- | --- |
| Configuration Language | XML (pom.xml) | Groovy/Kotlin DSL |
| Syntax Length | Verbose (វែង) | Concise (ខ្លី) |
| Performance | Slower | Faster (Incremental builds) |
| Learning Curve | Easier | Steeper |
| Popularity | Most popular | Growing fast |

## 3.3. application.properties

### 📌 និយមន័យ (Definition):

**application.properties** គឺជាឯកសារកំណត់រចនាសម្ព័ន្ធ (Configuration File) លំនាំដើមរបស់ Spring Boot ដែលមានទីតាំងក្នុង src/main/resources/។ វាប្រើទ្រង់ទ្រាយ **key=value**សម្រាប់កំណត់រចនាសម្ព័ន្ធ Server Port, Database Connection, Logging Level, និង Custom Properties។

```properties
# ============================================================
# SERVER CONFIGURATION
# ============================================================
# Server port (default: 8080)
server.port=9090

# Context path (default: /)
server.servlet.context-path=/api

# Session timeout (in seconds)
server.servlet.session.timeout=1800

# ============================================================
# DATABASE CONFIGURATION (MySQL)
# ============================================================
# Database connection URL
spring.datasource.url=jdbc:mysql://localhost:3306/mydb?useSSL=false&serverTimezone=UTC

# Database credentials
spring.datasource.username=root
spring.datasource.password=secret123

# Database driver
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver

# Connection pool settings
spring.datasource.hikari.maximum-pool-size=10
spring.datasource.hikari.minimum-idle=5

# ============================================================
# JPA / HIBERNATE CONFIGURATION
# ============================================================
# DDL auto mode: none, validate, update, create, create-drop
spring.jpa.hibernate.ddl-auto=update

# Show SQL queries in console
spring.jpa.show-sql=true

# Format SQL queries
spring.jpa.properties.hibernate.format_sql=true

# SQL dialect
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQL8Dialect

# ============================================================
# LOGGING CONFIGURATION
# ============================================================
# Logging levels: TRACE, DEBUG, INFO, WARN, ERROR
logging.level.root=INFO
logging.level.org.springframework.web=DEBUG
logging.level.com.example.demo=DEBUG

# Log file configuration
logging.file.name=logs/application.log
logging.logback.rollingpolicy.max-file-size=10MB
logging.logback.rollingpolicy.max-history=7

# ============================================================
# SPRING BOOT ACTUATOR
# ============================================================
# Enable all actuator endpoints
management.endpoints.web.exposure.include=*

# Change actuator base path
management.endpoints.web.base-path=/actuator

# ============================================================
# CUSTOM PROPERTIES
# ============================================================
app.name=My Spring Boot Application
app.version=1.0.0
app.description=Demo application for learning Spring Boot

# ============================================================
# MULTIPART FILE UPLOAD
# ============================================================
# Max file size
spring.servlet.multipart.max-file-size=10MB
# Max request size
spring.servlet.multipart.max-request-size=10MB

# ============================================================
# INTERNATIONALIZATION (i18n)
# ============================================================
spring.messages.basename=messages
spring.messages.encoding=UTF-8

# ============================================================
# DEVTOOLS
# ============================================================
# Automatic restart
spring.devtools.restart.enabled=true
spring.devtools.restart.additional-paths=src/main/java

# Live reload (requires browser extension)
spring.devtools.livereload.enabled=true
```

### 💡 Access Properties in Code:

```java
// Method 1: Using @Value
@RestController
public class AppController {
    @Value("${app.name}")
    private String appName;

    @Value("${server.port}")
    private int serverPort;

    @GetMapping("/info")
    public String getInfo() {
        return "App: " + appName + ", Port: " + serverPort;
    }
}

// Method 2: Using @ConfigurationProperties
@Component
@ConfigurationProperties(prefix = "app")
public class AppProperties {
    private String name;
    private String version;
    private String description;

    // Getters and Setters
}
```

## 3.4. application.yml (YAML Format)

### 📌 និយមន័យ (Definition):

**application.yml** គឺជាឯកសារកំណត់រចនាសម្ព័ន្ធជំនួស application.propertiesដែលប្រើទ្រង់ទ្រាយ **YAML (YAML Ain't Markup Language)**។ YAML មានរចនាសម្ព័ន្ធដូច JSON ប៉ុន្តែងាយស្រួលអានជាង (human-readable) និងគាំទ្រ hierarchical configuration។

```yaml
# ============================================================
# SERVER CONFIGURATION
# ============================================================
server:
  port: 9090
  servlet:
    context-path: /api
    session:
      timeout: 1800

# ============================================================
# DATABASE CONFIGURATION
# ============================================================
spring:
  datasource:
    url: jdbc:mysql://localhost:3306/mydb?useSSL=false&serverTimezone=UTC
    username: root
    password: secret123
    driver-class-name: com.mysql.cj.jdbc.Driver
    hikari:
      maximum-pool-size: 10
      minimum-idle: 5

  # ============================================================
  # JPA / HIBERNATE CONFIGURATION
  # ============================================================
  jpa:
    hibernate:
      ddl-auto: update
    show-sql: true
    properties:
      hibernate:
        format_sql: true
        dialect: org.hibernate.dialect.MySQL8Dialect

  # ============================================================
  # MULTIPART FILE UPLOAD
  # ============================================================
  servlet:
    multipart:
      max-file-size: 10MB
      max-request-size: 10MB

# ============================================================
# LOGGING CONFIGURATION
# ============================================================
logging:
  level:
    root: INFO
    org.springframework.web: DEBUG
    com.example.demo: DEBUG
  file:
    name: logs/application.log
  logback:
    rollingpolicy:
      max-file-size: 10MB
      max-history: 7

# ============================================================
# SPRING BOOT ACTUATOR
# ============================================================
management:
  endpoints:
    web:
      exposure:
        include: "*"
      base-path: /actuator

# ============================================================
# CUSTOM PROPERTIES
# ============================================================
app:
  name: My Spring Boot Application
  version: 1.0.0
  description: Demo application for learning Spring Boot

  # Nested properties
  database:
    host: localhost
    port: 3306
    name: mydb
```

### 📊 properties vs yml Comparison:

| application.properties | application.yml |
| --- | --- |
| Format: key=value | Format: YAML (hierarchical) |
| Flat structure | Tree/Nested structure |
| Less readable for complex config | More readable for complex config |
| No list/map syntax | Supports lists and maps natively |
| Uses $ for placeholders | Uses $ for placeholders as well |

## 3.5. Spring Boot Starter Packages

### 📌 និយមន័យ (Definition):

**Spring Boot Starters** គឺជា Dependency Descriptors ដែលប្រមូលផ្តុំ (bundle) dependencies ដែលពាក់ព័ន្ធនឹងគ្នាទៅក្នុងកញ្ចប់តែមួយ។ ឧទាហរណ៍ spring-boot-starter-webរួមបញ្ចូល Tomcat, Spring MVC, Jackson, និង Validation — ដូច្នេះអ្នកមិនចាំបាច់បន្ថែមរៀងៗខ្លួនទេ។

**Web / REST APIs**

- spring-boot-starter-web - REST APIs, Tomcat, Spring MVC

- spring-boot-starter-webflux - Reactive web (Netty, WebFlux)

- spring-boot-starter-websocket - WebSocket support

**Database / Data Access**

- spring-boot-starter-data-jpa - JPA, Hibernate, HikariCP

- spring-boot-starter-data-mongodb - MongoDB

- spring-boot-starter-jdbc - JDBC with HikariCP

- spring-boot-starter-data-redis - Redis

**Security**

- spring-boot-starter-security - Spring Security

- spring-boot-starter-oauth2-client - OAuth2 Client

- spring-boot-starter-oauth2-resource-server - OAuth2 Resource Server

**Testing**

- spring-boot-starter-test - JUnit, Mockito, AssertJ, Testcontainers

**Development Tools**

- spring-boot-devtools - Auto-restart, Live Reload

- spring-boot-configuration-processor - @ConfigurationProperties metadata

**Production / Monitoring**

- spring-boot-starter-actuator - Health checks, Metrics, Info endpoints

**Message Queue**

- spring-boot-starter-amqp - RabbitMQ

- spring-boot-starter-kafka - Apache Kafka

**Template Engines (View)**

- spring-boot-starter-thymeleaf - Thymeleaf

- spring-boot-starter-freemarker - FreeMarker

- spring-boot-starter-mustache - Mustache

## 3.6. Auto Configuration

### 📌 និយមន័យ (Definition):

**Auto Configuration** គឺជាលក្ខណៈពិសេស (feature) ដ៏សំខាន់របស់ Spring Boot ដែលកំណត់រចនាសម្ព័ន្ធ Spring Beans ដោយស្វ័យប្រវត្តិ ផ្អែកលើ Dependencies ដែលមានក្នុង Classpath។ វាត្រូវបានបើកដោយ @EnableAutoConfiguration ឬ @SpringBootApplication annotation។

### 🔹 របៀប Auto Configuration ដំណើរការ (How it works):

1. Spring Boot scans classpath for dependencies (starter packages)

2. Based on dependencies, it applies default configurations from META-INF/spring/org.springframework.boot.autoconfigure.AutoConfiguration.imports

3. Conditions are checked using annotations like @ConditionalOnClass, @ConditionalOnMissingBean

4. If condition matches, Spring Boot creates the necessary beans automatically

### 🔹 ឧទាហរណ៍ Conditional Annotations:

```java
// This configuration applies only if JdbcTemplate class exists
@Configuration
@ConditionalOnClass(JdbcTemplate.class)
public class DatabaseAutoConfiguration {

    @Bean
    @ConditionalOnMissingBean
    public JdbcTemplate jdbcTemplate(DataSource dataSource) {
        return new JdbcTemplate(dataSource);
    }
}

// Example: Spring Boot's built-in conditions
@ConditionalOnClass              // Class must be on classpath
@ConditionalOnMissingBean        // Bean must not already exist
@ConditionalOnProperty           // Property must have specific value
@ConditionalOnWebApplication     // Must be web application
@ConditionalOnExpression          // SpEL expression must be true
```

### 💡 Overriding Auto Configuration:

អ្នកអាច override auto configuration ដោយ៖

- កំណត់តម្លៃក្នុង application.properties / application.yml

- បង្កើត Bean ផ្ទាល់ខ្លួនជាមួយ @Bean

- ប្រើ @ConditionalOnMissingBean ដើម្បីការពារ auto configuration

- ប្រើ spring.autoconfigure.exclude ក្នុង configuration:

```properties
# Exclude specific auto configuration classes
spring.autoconfigure.exclude=  org.springframework.boot.autoconfigure.jdbc.DataSourceAutoConfiguration,  org.springframework.boot.autoconfigure.orm.jpa.HibernateJpaAutoConfiguration
```

## 3.7. Spring Boot DevTools

### 📌 និយមន័យ (Definition):

**Spring Boot DevTools** គឺជា set នៃ development-time tools ដែលធ្វើអោយការអភិវឌ្ឍកម្មវិធី Spring Boot កាន់តែលឿន និងងាយស្រួល។ វារួមបញ្ចូល **Automatic Restart**, **Live Reload**,**Default Property Values**, និង **Remote Debugging**។

### 🔹 ការបន្ថែម DevTools (Add DevTools to project):

```xml
<!-- Maven -->
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-devtools</artifactId>
    <scope>runtime</scope>
    <optional>true</optional>
</dependency>
// Gradle
```

developmentOnly 'org.springframework.boot:spring-boot-devtools'

**1. Automatic Restart**

ពេលអ្នកកែប្រែកូដក្នុង classpath, application នឹង restart ដោយស្វ័យប្រវត្តិ។

```properties
spring.devtools.restart.enabled=true
```

**2. Live Reload**

ធ្វើឱ្យ browser refresh ដោយស្វ័យប្រវត្តិ ពេលមានការផ្លាស់ប្តូរ (ត្រូវការ LiveReload browser extension)។

```properties
spring.devtools.livereload.enabled=true
```

**3. Property Defaults**

កំណត់តម្លៃលំនាំដើមសម្រាប់ development (ឧ. template caching off)។

```properties
spring.thymeleaf.cache=false
```

**4. Remote Debug**

គាំទ្រការ debugging ពីចម្ងាយ (remote) សម្រាប់ applications ដែលកំពុងរត់។

### 🔹 DevTools Configuration (application.properties):

```properties
# Enable/disable automatic restart
spring.devtools.restart.enabled=true

# Additional paths to watch for restart
spring.devtools.restart.additional-paths=src/main/java,src/main/resources

# Exclude specific paths from restart
spring.devtools.restart.exclude=static/**,public/**

# Enable/disable live reload
spring.devtools.livereload.enabled=true

# Port for live reload (default: 35729)
spring.devtools.livereload.port=35729

# Remote application secret (for remote debugging)
spring.devtools.remote.secret=mysecret
```

### ⚠️ Important Notes:

- DevTools ត្រូវបានដកចេញ (automatically disabled) នៅពេលដំណើរការ production (jar file)

- Restart vs Reload: Restart is faster than cold start because it uses two classloaders

- ការផ្លាស់ប្តូរឯកសារ application.properties មិន trigger restart ទេ → ត្រូវ restart ដោយដៃ

## 3.8. ការដំណើរការលើ Ports ផ្សេងៗ (Running on Different Ports)

### 📌 និយមន័យ (Definition):

តាមលំនាំដើម (default) Spring Boot ដំណើរការលើ **port 8080**។ អ្នកអាចប្តូរ port តាមរយៈ configuration files, command line arguments, ឬ environment variables។

**Method 1: application.properties**

```properties
# Default port 8080
server.port=8080

# Custom port
server.port=9090

# Using environment variable
server.port=${PORT:8080}
```

**Method 2: application.yml**

```yaml
server:
  port: 9090
```

**Method 3: Command Line**

```bash
# Using Maven
./mvnw spring-boot:run -Dspring-boot.run.arguments=--server.port=9090

# Using JAR
java -jar demo.jar --server.port=9090

# Multiple ports (random available port)
java -jar demo.jar --server.port=0
```

**Method 4: Environment Variable**

```properties
# Windows
set SERVER_PORT=9090
java -jar demo.jar

# Mac/Linux
export SERVER_PORT=9090
java -jar demo.jar

# Cross-platform
SERVER_PORT=9090 java -jar demo.jar
```

### 💡 Random Port (for testing):

កំណត់ server.port=0 ដើម្បីឱ្យ Spring Boot ជ្រើសរើស port ដែល available ដោយស្វ័យប្រវត្តិ៖

```properties
# Will assign a random available port (e.g., 54321)
server.port=0

# Access the random port in code
@Value("${local.server.port}")
private int serverPort;
```

## 3.9. Profiles (dev, test, prod)

### 📌 និយមន័យ (Definition):

**Spring Profiles** គឺជាយន្តការដែលអនុញ្ញាតឱ្យអ្នកកំណត់រចនាសម្ព័ន្ធផ្សេងៗគ្នា សម្រាប់បរិស្ថាន (environments) ផ្សេងៗគ្នា — Development (dev), Testing (test), Production (prod)។ Profile នីមួយៗអាចមាន configuration file ផ្ទាល់ខ្លួន (ឧ. application-dev.properties) ហើយអ្នកអាចប្តូរ profile បានដោយមិនចាំបាច់កែប្រែកូដ។

### 🔹 ការបង្កើត Profile-specific Configuration Files:

```text
src/main/resources/
├── application.properties          # Common configuration (all profiles)
├── application-dev.properties      # Development profile
├── application-test.properties     # Testing profile
├── application-prod.properties     # Production profile
│
# Or using YAML with multi-document
├── application.yml                 # Supports multiple profiles in one file
```

### 🔹 application-dev.properties (Development):

```properties
# Development Profile
server.port=8080
spring.datasource.url=jdbc:h2:mem:testdb
spring.datasource.driver-class-name=org.h2.Driver
spring.jpa.hibernate.ddl-auto=create-drop
spring.h2.console.enabled=true
logging.level.com.example.demo=DEBUG
spring.thymeleaf.cache=false
```

### 🔹 application-test.properties (Testing):

```properties
# Testing Profile
server.port=0  # Random port for tests
spring.datasource.url=jdbc:h2:mem:testdb;MODE=MySQL
spring.jpa.hibernate.ddl-auto=create
logging.level.com.example.demo=INFO
```

### 🔹 application-prod.properties (Production):

```properties
# Production Profile
server.port=8080
spring.datasource.url=jdbc:mysql://prod-db-server:3306/mydb
spring.datasource.username=prod_user
spring.datasource.password=secure_password
spring.jpa.hibernate.ddl-auto=none
spring.jpa.show-sql=false
logging.level.com.example.demo=WARN
management.endpoints.web.exposure.include=health,info
```

### 🔹 Multi-Profile YAML (Single file approach):

```yaml
# Common configuration for all profiles
spring:
  application:
    name: my-spring-boot-app
```

---

```yaml
# Development profile
spring:
  config:
    activate:
      on-profile: dev
server:
  port: 8080
logging:
  level:
    com.example: DEBUG
```

---

```yaml
# Production profile
spring:
  config:
    activate:
      on-profile: prod
server:
  port: 80
logging:
  level:
    com.example: WARN
```

### 🔹 វិធីកំណត់ Active Profile (Ways to activate profile):

**1. application.properties**

```properties
spring.profiles.active=dev
```

**2. Command Line**

```bash
java -jar app.jar --spring.profiles.active=prod
```

**3. Environment Variable**

```bash
export SPRING_PROFILES_ACTIVE=test
```

**4. Maven/Gradle**

```bash
./mvnw spring-boot:run -Dspring-boot.run.profiles=dev
```

**5. In Code (Programmatic)**

```text
SpringApplication.setAdditionalProfiles("prod");
```

**6. Using @Profile Annotation**

```text
@Profile("dev")
```

### 🔹 Using @Profile Annotation in Code:

```java
// Component only active for 'dev' profile
@Component
@Profile("dev")
public class DevDatabaseConfig {
    public DevDatabaseConfig() {
        System.out.println("Development Database Configuration");
    }
}

// Component only active for 'prod' profile
@Component
@Profile("prod")
public class ProdDatabaseConfig {
    public ProdDatabaseConfig() {
        System.out.println("Production Database Configuration");
    }
}

// Component active for multiple profiles
@Component
@Profile({"dev", "test"})
public class DevTestConfig {
    // This runs in both dev and test profiles
}

// Component active for all profiles except 'prod'
@Component
@Profile("!prod")
public class NonProdConfig {
    // This runs for dev, test, and any profile other than prod
}

// Active if 'dev' is NOT active
@Component
@Profile("!dev")
public class NotDevConfig {
    // Runs for test, prod, etc.
}

// Inject active profiles in code
@Service
public class ProfileService {
    @Autowired
    private Environment env;

    public void showActiveProfiles() {
        String[] profiles = env.getActiveProfiles();
        System.out.println("Active Profiles: " + Arrays.toString(profiles));
    }
}
```

## 3.10. Logging in Spring Boot

### 📌 និយមន័យ (Definition):

**Logging** គឺជាការកត់ត្រាព័ត៌មានអំពីការដំណើរការរបស់កម្មវិធី (debugging, monitoring, troubleshooting)។ Spring Boot ប្រើ **SLF4J (Simple Logging Facade for Java)** ជា abstraction layer និង **Logback** ជា default implementation។

### 🔹 Logging Levels (កម្រិត Log):

| Level | Description | When to Use |
| --- | --- | --- |
| ERROR | Error events that may still allow the application to continue running | Exceptions, database connection failures |
| WARN | Potentially harmful situations | Deprecated API usage, low disk space |
| INFO | General application events | Application startup, shutdown, major steps |
| DEBUG | Detailed information for debugging | Development only, request/response details |
| TRACE | More detailed than DEBUG | Very detailed tracing, method entry/exit |

### 🔹 ការប្រើប្រាស់ Logger ក្នុងកូដ (Using Logger in Code):

```java
import org.slf4j.Logger;
import org.slf4j.LoggerFactory;
import org.springframework.web.bind.annotation.*;

@RestController
@RequestMapping("/api/users")
public class UserController {

    // Create logger instance
    private static final Logger logger = LoggerFactory.getLogger(UserController.class);

    // Or use Lombok @Slf4j annotation (simpler!)
    // @Slf4j
    // public class UserController { ... }

    @GetMapping("/{id}")
    public User getUser(@PathVariable Long id) {
        // Different logging levels
        logger.trace("Entering getUser method with id: {}", id);
        logger.debug("Fetching user with id: {}", id);
        logger.info("User request received for id: {}", id);

        try {
            User user = userService.findById(id);
            logger.info("User found: {}", user);
            return user;
        } catch (Exception e) {
            logger.error("Error fetching user with id: {}", id, e);
            throw e;
        }
    }

    @PostMapping
    public User createUser(@RequestBody User user) {
        logger.info("Creating new user: {}", user);
        logger.warn("User creation - check for duplicates: {}", user.getEmail());
        return userService.save(user);
    }
}
```

### 🔹 Logging Configuration (application.yml):

```yaml
logging:
  # Logging levels for different packages
  level:
    root: INFO
    com.example.demo: DEBUG
    org.springframework.web: DEBUG
    org.hibernate.SQL: DEBUG
    org.hibernate.type.descriptor.sql.BasicBinder: TRACE

  # Log file configuration
  file:
    name: logs/myapp.log
    path: /var/log/myapp

  # Log pattern
  pattern:
    console: "%d{yyyy-MM-dd HH:mm:ss} - %msg%n"
    file: "%d{yyyy-MM-dd HH:mm:ss} [%thread] %-5level %logger{36} - %msg%n"

  # Logback configuration file (custom)
  config: classpath:logback-spring.xml

  # Rolling policy (log rotation)
  logback:
    rollingpolicy:
      max-file-size: 10MB
      max-history: 30
      total-size-cap: 1GB
```

### 🔹 Custom Logback Configuration (logback-spring.xml):

```xml
<?xml version="1.0" encoding="UTF-8"?>
<configuration>
    <!-- Console Appender -->
    <appender name="CONSOLE" class="ch.qos.logback.core.ConsoleAppender">
        <encoder>
            <pattern>%d{yyyy-MM-dd HH:mm:ss} [%thread] %-5level %logger{36} - %msg%n</pattern>
        </encoder>
    </appender>

    <!-- File Appender -->
    <appender name="FILE" class="ch.qos.logback.core.rolling.RollingFileAppender">
        <file>logs/application.log</file>
        <rollingPolicy class="ch.qos.logback.core.rolling.TimeBasedRollingPolicy">
            <fileNamePattern>logs/application.%d{yyyy-MM-dd}.log</fileNamePattern>
            <maxHistory>30</maxHistory>
        </rollingPolicy>
        <encoder>
            <pattern>%d{yyyy-MM-dd HH:mm:ss} [%thread] %-5level %logger{36} - %msg%n</pattern>
        </encoder>
    </appender>

    <!-- JSON Appender (for production) -->
    <appender name="JSON" class="ch.qos.logback.core.ConsoleAppender">
        <encoder class="ch.qos.logback.classic.encoder.JsonEncoder"/>
    </appender>

    <!-- Development profile -->
    <springProfile name="dev">
        <root level="DEBUG">
            <appender-ref ref="CONSOLE"/>
            <appender-ref ref="FILE"/>
        </root>
    </springProfile>

    <!-- Production profile -->
    <springProfile name="prod">
        <root level="WARN">
            <appender-ref ref="JSON"/>
        </root>
    </springProfile>

    <!-- Default configuration -->
    <springProfile name="default">
        <root level="INFO">
            <appender-ref ref="CONSOLE"/>
        </root>
    </springProfile>
</configuration>
```

### 💡 Lombok @Slf4j Annotation (Simplified logging):

```java
import lombok.extern.slf4j.Slf4j;

@Slf4j  // This automatically creates a 'log' object
@RestController
public class DemoController {

    @GetMapping("/hello")
    public String hello() {
        // Use 'log' directly - no need to create Logger instance
        log.info("Hello endpoint called");
        log.debug("Debug information: {}", "some data");
        log.error("Error occurred", new RuntimeException("Test"));

        return "Hello World";
    }
}
```

Note: Need Lombok dependency and annotation processing enabled

### ✅ Best Practices for Logging:

- ប្រើ **SLF4J** + **Logback** (default)

- កុំ log sensitive data (passwords, tokens, personal information)

- ប្រើ parameterized logging: log.debug("User: ", user) instead of string concatenation

- កំណត់ appropriate logging level for each environment (DEBUG for dev, WARN/ERROR for prod)

- ប្រើ @Slf4j annotation from Lombok to reduce boilerplate

- Include stack trace in error logs: log.error("Message", exception)

- Rotate log files to prevent disk space issues

### 📚 សង្ខេបមេរៀនទី៣ (Module 3 Summary)

នៅក្នុងមេរៀននេះ អ្នកបានរៀនអំពី Spring Boot Basics សំខាន់ៗ៖

- **Spring Initializr** – Web tool សម្រាប់បង្កើត Spring Boot projects

- **Dependencies Management** – Maven/Gradle configuration with starter packages

- **Configuration Files** – application.properties vs application.yml

- **Spring Boot Starters** – Web, Data JPA, Security, Testing, DevTools, etc.

- **Auto Configuration** – Automatic bean configuration based on dependencies

- **DevTools** – Auto-restart, Live Reload for faster development

- **Different Ports** – Configure server.port with various methods

- **Profiles** – Environment-specific configuration (dev, test, prod)

- **Logging** – SLF4J + Logback, logging levels, log configuration

# មេរៀនទី៤: Dependency Injection & Beans (ការចាក់បញ្ចូលភាពអាស្រ័យ និង Beans)

### 📖 សេចក្តីផ្តើម (Introduction):
Dependency Injection (DI) និង Inversion of Control (IoC) គឺជាគោលការណ៍ស្នូល (core concepts) របស់ Spring Framework។ Spring Container គ្រប់គ្រងការបង្កើត objects (Beans) និងការចាក់បញ្ចូលភាពអាស្រ័យ (dependencies) រវាងពួកវា។ មេរៀននេះនឹងពន្យល់លម្អិតអំពី IoC, DI, Bean Lifecycle, Annotations (@Component, @Service, @Repository, @Controller, @RestController, @Autowired), Injection Types (Constructor, Setter, Field), Bean Scopes, និង Configuration Classes។

## 4.1. តើ IoC ជាអ្វី? (What is Inversion of Control?)

### 📌 និយមន័យ (Definition):

**Inversion of Control (IoC)** គឺជាគោលការណ៍ (principle) ដែលបញ្ច្រាស់ការគ្រប់គ្រងលំហូរកម្មវិធី (control flow) ពីកម្មវិធីទៅកាន់ framework ឬ container។ ជំនួសឱ្យកូដរបស់អ្នកបង្កើត objects ដោយខ្លួនឯង (using new keyword), IoC container (Spring Container) នឹងបង្កើត និងគ្រប់គ្រង objects ឱ្យអ្នក — នេះហៅថា **"Don't call us, we'll call you"**។

### 🔹 របៀបដែល IoC ដំណើរការ (How IoC Works):

- **Traditional Approach (Without IoC):** កូដរបស់អ្នកបង្កើត objects ដោយផ្ទាល់ និងគ្រប់គ្រង dependencies។

- **IoC Approach (With Spring):** Spring Container (IoC Container) បង្កើត objects (Beans), គ្រប់គ្រង lifecycle, និងចាក់បញ្ចូល dependencies។ កូដរបស់អ្នកគ្រាន់តែប្រកាសថាត្រូវការអ្វីខ្លះ (ឧ. តាមរយៈ @Autowired ឬ constructor)។

```java
// Without IoC (Traditional)
UserService service = new UserService(new UserRepository());
// With IoC (Spring)
@Autowired
private UserService service; // Spring injects it automatically
```

## 4.2. Dependency Injection (DI) — ការចាក់បញ្ចូលភាពអាស្រ័យ

### 📌 និយមន័យ (Definition):

**Dependency Injection (DI)** គឺជា design pattern ដែលជាការអនុវត្តន៍ជាក់ស្តែងនៃ IoC។ DI មានន័យថា objects មិនបង្កើត dependencies របស់ខ្លួនឯងទេ ប៉ុន្តែត្រូវបាន "ចាក់បញ្ចូល" (injected) ដោយ IoC container។ នេះធ្វើឱ្យកូដកាន់តែរលុង (loosely coupled), ងាយស្រួលក្នុងការធ្វើតេស្ត (testable), និងថែទាំ (maintainable)។

**❌** **Without DI (Tightly Coupled)**

```java
public class UserService {
    // UserService creates its own dependency
    private UserRepository repository = new UserRepository();

    public User getUser(Long id) {
        return repository.findById(id);
    }
}
// Problem: Cannot test UserService without UserRepository
// Cannot easily swap implementation
```

### ✅ With DI (Loosely Coupled)

```properties
public class UserService {
    // Dependency is injected from outside
    private final UserRepository repository;

    // Constructor Injection
    public UserService(UserRepository repository) {
        this.repository = repository;
    }

    public User getUser(Long id) {
        return repository.findById(id);
    }
}
// Benefit: Easy to test with mock implementation
```

### 🔹 ប្រភេទនៃ Dependency Injection (Types of DI):

- **Constructor Injection** – ចាក់ dependencies តាមរយៈ constructor (recommended)

- **Setter Injection** – ចាក់ dependencies តាមរយៈ setter methods

- **Field Injection** – ចាក់ dependencies ដោយផ្ទាល់ទៅ fields (using @Autowired)

## 4.3. វដ្តជីវិតរបស់ Bean (Bean Lifecycle)

### 📌 និយមន័យ (Definition):

**Bean Lifecycle** គឺជាដំណាក់កាលនានា (stages) ដែល Spring Bean ឆ្លងកាត់ ចាប់ពីពេលដែលវាត្រូវបានបង្កើត (instantiation) រហូតដល់ពេលដែលវាត្រូវបានបំផ្លាញ (destruction)។ Spring Container គ្រប់គ្រង lifecycle ទាំងមូល។

**Spring Bean Lifecycle Steps:**

```text
1. Instantiation ──▶ 2. Populate Properties ──▶ 3. BeanNameAware.setBeanName()
4. BeanClassLoaderAware.setBeanClassLoader() ──▶ 5. BeanFactoryAware.setBeanFactory()
6. EnvironmentAware.setEnvironment() ──▶ 7. ApplicationContextAware.setApplicationContext()
```

8. BeanPostProcessor.postProcessBeforeInitialization()

9. @PostConstruct / InitializingBean.afterPropertiesSet() / init-method

10. BeanPostProcessor.postProcessAfterInitialization()

```text
11. Bean is Ready for Use ──▶ 12. @PreDestroy / DisposableBean.destroy() / destroy-method
import javax.annotation.PostConstruct;
import javax.annotation.PreDestroy;
import org.springframework.beans.factory.DisposableBean;
import org.springframework.beans.factory.InitializingBean;
import org.springframework.stereotype.Component;

@Component
public class DemoBean implements InitializingBean, DisposableBean {

    public DemoBean() {
        System.out.println("1. Constructor - Bean Instantiation");
    }

    // Method called after properties are set
    @PostConstruct
    public void init() {
        System.out.println("2. @PostConstruct - Initialization");
    }

    // InitializingBean interface method
    @Override
    public void afterPropertiesSet() throws Exception {
        System.out.println("3. afterPropertiesSet() - InitializingBean");
    }

    // Custom init method (configured in @Bean)
    public void customInit() {
        System.out.println("4. Custom init method");
    }

    // Business method
    public void doWork() {
        System.out.println("5. Bean is ready - Doing work...");
    }

    // @PreDestroy - called before bean destruction
    @PreDestroy
    public void preDestroy() {
        System.out.println("6. @PreDestroy - Before destruction");
    }

    // DisposableBean interface method
    @Override
    public void destroy() throws Exception {
        System.out.println("7. destroy() - DisposableBean");
    }

    // Custom destroy method
    public void customDestroy() {
        System.out.println("8. Custom destroy method");
    }
}
```

## 4.4. @Component Annotation

### 📌 និយមន័យ (Definition):

```java
@Component គឺជា annotation ទូទៅ (generic stereotype) សម្រាប់ប្រាប់ Spring Container ថា class នេះគឺជា Spring Bean — Spring នឹងបង្កើត instance មួយ (singleton by default) និងគ្រប់គ្រងវា។ @Component គឺជា base annotation សម្រាប់ @Service, @Repository, @Controller។
import org.springframework.stereotype.Component;

@Component  // Spring will create a bean named "myComponent" (default: lowercase class name)
public class MyComponent {

    public void doSomething() {
        System.out.println("Doing something in MyComponent...");
    }
}

// Custom bean name
@Component("customBeanName")
public class AnotherComponent {
    public void execute() {
        System.out.println("Executing...");
    }
}

// Using the component
@Service
public class MyService {
    @Autowired
    private MyComponent myComponent;  // Spring injects the bean

    public void useComponent() {
        myComponent.doSomething();
    }
}
```

## 4.5. @Service Annotation

### 📌 និយមន័យ (Definition):

```java
@Service គឺជា specialization នៃ @Component ដែលប្រើសម្រាប់ Service Layer (Business Logic Layer)។ វាប្រាប់ Spring ថា class នេះផ្ទុកតក្កវិជ្ជាអាជីវកម្ម (business logic), calculations, និងការហៅ repository methods។ @Service beans ជាធម្មតាមាន @Transactional annotation។
import org.springframework.stereotype.Service;
import org.springframework.transaction.annotation.Transactional;

@Service  // Indicates this is a Service Layer bean
@Transactional  // All methods will be transactional
public class UserService {

    @Autowired
    private UserRepository userRepository;

    public User findUserById(Long id) {
        // Business logic
        return userRepository.findById(id)
            .orElseThrow(() -> new RuntimeException("User not found"));
    }

    public User createUser(UserDto userDto) {
        // Validation and business logic
        if (userDto.getEmail() == null) {
            throw new IllegalArgumentException("Email is required");
        }

        User user = new User();
        user.setName(userDto.getName());
        user.setEmail(userDto.getEmail());

        return userRepository.save(user);
    }

    public void deleteUser(Long id) {
        // Business logic before deletion
        userRepository.deleteById(id);
    }
}
```

## 4.6. @Repository Annotation

### 📌 និយមន័យ (Definition):

```java
@Repository គឺជា specialization នៃ @Component ដែលប្រើសម្រាប់ Data Access Layer (Persistence Layer)។ វាប្រាប់ Spring ថា class នេះទទួលខុសត្រូវផ្នែក CRUD operations (Create, Read, Update, Delete) និងការចូលដំណើរការទិន្នន័យពី database។ @Repository ក៏ផ្តល់នូវការបកប្រែ exception (exception translation) ផងដែរ — បំលែង database exceptions ទៅជា Spring's DataAccessException។
import org.springframework.stereotype.Repository;
import org.springframework.data.jpa.repository.JpaRepository;
import java.util.Optional;

// Traditional @Repository
@Repository
public class UserRepository {

    @PersistenceContext
    private EntityManager entityManager;

    public User save(User user) {
        entityManager.persist(user);
        return user;
    }

    public Optional<User> findById(Long id) {
        User user = entityManager.find(User.class, id);
        return Optional.ofNullable(user);
    }

    public void delete(User user) {
        entityManager.remove(user);
    }
}

// Modern approach: Spring Data JPA (no need @Repository)
public interface UserJpaRepository extends JpaRepository<User, Long> {
    // Spring Data JPA automatically implements CRUD methods
    Optional<User> findByEmail(String email);
    List<User> findByNameContaining(String keyword);
}
```

## 4.7. @Controller Annotation

### 📌 និយមន័យ (Definition):

```java
@Controller គឺជា specialization នៃ @Component ដែលប្រើសម្រាប់ Web Controller Layer ក្នុង Spring MVC។ @Controller ដំណើរការ HTTP requests និងត្រឡប់ View (HTML page) តាមរយៈ View Resolvers (Thymeleaf, JSP, etc.)។ Method ក្នុង @Controller ជាធម្មតាត្រឡប់ String (view name) ឬ ModelAndView object។
import org.springframework.stereotype.Controller;
import org.springframework.ui.Model;
import org.springframework.web.bind.annotation.GetMapping;
import org.springframework.web.bind.annotation.PathVariable;
import org.springframework.web.bind.annotation.RequestParam;

@Controller
public class HomeController {

    // Returns view (HTML page)
    @GetMapping("/")
    public String home() {
        return "index";  // Returns index.html or index.jsp
    }

    // Passing data to view
    @GetMapping("/hello")
    public String hello(@RequestParam(name = "name", defaultValue = "Guest") String name,
                        Model model) {
        model.addAttribute("userName", name);
        model.addAttribute("message", "Welcome to Spring Boot!");
        return "greeting";  // greeting.html
    }

    // Dynamic URL
    @GetMapping("/users/{id}")
    public String getUserProfile(@PathVariable Long id, Model model) {
        User user = userService.findById(id);
        model.addAttribute("user", user);
        return "user-profile";
    }
}
```

## 4.8. @RestController Annotation

### 📌 និយមន័យ (Definition):

```java
@RestController គឺជា convenience annotation ដែលផ្សំ @Controller និង @ResponseBody។ វាប្រើសម្រាប់បង្កើត RESTful Web Services — method នីមួយៗត្រឡប់ data (JSON/XML) ដោយផ្ទាល់ទៅកាន់ HTTP response body ជំនួសឱ្យ view។ នេះគឺជា annotation ទូទៅបំផុតសម្រាប់ការបង្កើត REST APIs។
import org.springframework.web.bind.annotation.*;
import org.springframework.http.ResponseEntity;
import java.util.List;

@RestController
@RequestMapping("/api/users")
public class UserRestController {

    @Autowired
    private UserService userService;

    // GET /api/users
    @GetMapping
    public List<User> getAllUsers() {
        return userService.findAll();
    }

    // GET /api/users/1
    @GetMapping("/{id}")
    public ResponseEntity<User> getUserById(@PathVariable Long id) {
        return userService.findById(id)
```

.map(ResponseEntity::ok)

```java
            .orElse(ResponseEntity.notFound().build());
    }

    // POST /api/users
    @PostMapping
    public ResponseEntity<User> createUser(@RequestBody UserDto userDto) {
        User created = userService.create(userDto);
        return ResponseEntity.status(HttpStatus.CREATED).body(created);
    }

    // PUT /api/users/1
    @PutMapping("/{id}")
    public ResponseEntity<User> updateUser(@PathVariable Long id,
                                           @RequestBody UserDto userDto) {
        User updated = userService.update(id, userDto);
        return ResponseEntity.ok(updated);
    }

    // DELETE /api/users/1
    @DeleteMapping("/{id}")
    public ResponseEntity<Void> deleteUser(@PathVariable Long id) {
        userService.delete(id);
        return ResponseEntity.noContent().build();
    }
}
```

## 4.9. @Autowired Annotation

### 📌 និយមន័យ (Definition):

```text
@Autowired គឺជា annotation ដែលប្រាប់ Spring Container ឱ្យធ្វើ Dependency Injection (ចាក់បញ្ចូល dependency) ដោយស្វ័យប្រវត្តិ។ Spring នឹងស្វែងរក bean ដែលត្រូវគ្នានឹង type (by type) ហើយចាក់បញ្ចូលទៅកាន់ field, constructor, ឬ setter method។
```

**1. Field Injection (not recommended for production)**

```java
@Component
public class MyService {
    @Autowired  // Spring injects directly to field
    private UserRepository userRepository;
}
```

**2. Setter Injection**

```properties
@Component
public class MyService {
    private UserRepository userRepository;

    @Autowired  // Spring injects via setter method
    public void setUserRepository(UserRepository userRepository) {
        this.userRepository = userRepository;
    }
}
```

**3. Constructor Injection (Recommended)**

```properties
@Component
public class MyService {
    private final UserRepository userRepository;

    // @Autowired optional for constructor injection (Spring 4.3+)
    public MyService(UserRepository userRepository) {
        this.userRepository = userRepository;
    }
}
```

### ⚠️ @Autowired vs Constructor Injection (Recommendation):

Constructor injection is recommended because:

- Makes fields immutable (can use final)

- Easier to unit test (no reflection needed)

- Prevents null pointer exceptions

- Clearly shows required dependencies

## 4.10. Constructor Injection (ការចាក់តាម Constructor)

### 📌 និយមន័យ (Definition):

**Constructor Injection** គឺជាប្រភេទ DI ដែល dependencies ត្រូវបានចាក់បញ្ចូលតាមរយៈ constructor របស់ class។ នេះគឺជាវិធីសាស្រ្តដែលត្រូវបានណែនាំ (recommended) ដោយ Spring team។

```java
import org.springframework.stereotype.Service;

@Service
public class UserService {

    private final UserRepository userRepository;
    private final EmailService emailService;
    private final AuditService auditService;

    // Constructor Injection - all dependencies are provided via constructor
    // @Autowired is optional for single constructor (Spring 4.3+)
    public UserService(UserRepository userRepository,
```

EmailService emailService,

```properties
                       AuditService auditService) {
        this.userRepository = userRepository;
        this.emailService = emailService;
        this.auditService = auditService;
    }

    public User createUser(UserDto userDto) {
        // Use injected dependencies
        User user = userRepository.save(new User(userDto));
        emailService.sendWelcomeEmail(user.getEmail());
        auditService.log("User created: " + user.getId());
        return user;
    }
}

// Benefits:
// 1. Fields can be final (immutable)
// 2. Clear which dependencies are required
// 3. Easy to test (just pass mocks to constructor)
// 4. No need for @Autowired on constructor
```

## 4.11. Setter Injection (ការចាក់តាម Setter)

### 📌 និយមន័យ (Definition):

**Setter Injection** គឺជាប្រភេទ DI ដែល dependencies ត្រូវបានចាក់បញ្ចូលតាមរយៈ setter methods បន្ទាប់ពី object ត្រូវបានបង្កើត (post-construction)។ Setter injection គឺល្អសម្រាប់ optional dependencies (dependencies that are not required for the object to function).

```properties
import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.stereotype.Service;

@Service
public class NotificationService {

    private EmailService emailService;      // Required
    private SmsService smsService;          // Optional
    private PushNotificationService pushService; // Optional

    // Constructor for required dependencies
    public NotificationService(EmailService emailService) {
        this.emailService = emailService;
    }

    // Setter for optional dependencies
    @Autowired(required = false)  // Not required - can be null
    public void setSmsService(SmsService smsService) {
        this.smsService = smsService;
    }

    @Autowired(required = false)
    public void setPushService(PushNotificationService pushService) {
        this.pushService = pushService;
    }

    public void sendNotification(String message, String recipient) {
        // Always send email (required)
        emailService.send(recipient, message);

        // Send SMS if available (optional)
        if (smsService != null) {
            smsService.send(recipient, message);
        }

        // Send push if available (optional)
        if (pushService != null) {
            pushService.send(recipient, message);
        }
    }
}
```

## 4.12. Bean Scope (វិសាលភាពរបស់ Bean)

### 📌 និយមន័យ (Definition):

**Bean Scope** កំណត់ពីវដ្តជីវិត (lifecycle) និងចំនួន instances នៃ bean មួយដែលត្រូវបានបង្កើត និងគ្រប់គ្រងដោយ Spring Container។ Spring ផ្តល់ scope ផ្សេងៗគ្នាសម្រាប់ករណីប្រើប្រាស់ផ្សេងៗគ្នា។

| Scope | Description | When to Use |
| --- | --- | --- |
| singleton | មាន instance តែមួយ (default) | Stateless services, repositories, configuration |
| prototype | Instance ថ្មីរាល់ពេលដែលបានស្នើសុំ | Stateful objects, beans with mutable state |
| request | Instance ថ្មីសម្រាប់ HTTP request នីមួយៗ | Web applications only |
| session | Instance ថ្មីសម្រាប់ HTTP session នីមួយៗ | User session data (shopping cart, user preferences) |
| application | Instance តែមួយសម្រាប់ ServletContext | Application-wide singleton for web apps |
| websocket | Instance ថ្មីសម្រាប់ WebSocket session | WebSocket applications |

```java
import org.springframework.context.annotation.Scope;
import org.springframework.stereotype.Component;
import org.springframework.web.context.annotation.RequestScope;
import org.springframework.web.context.annotation.SessionScope;

// Default scope - Singleton (one instance for entire application)
@Component
public class SingletonBean {
    // All components/services get the same instance
}

// Prototype scope - new instance every time
@Component
@Scope("prototype")
public class PrototypeBean {
    // Each injection/create gets a new instance
}

// Request scope (web only)
@Component
@RequestScope
// or @Scope(value = "request", proxyMode = ScopedProxyMode.TARGET_CLASS)
public class RequestScopedBean {
    // New instance per HTTP request
}

// Session scope (web only)
@Component
@SessionScope
// or @Scope(value = "session", proxyMode = ScopedProxyMode.TARGET_CLASS)
public class SessionScopedBean {
    // New instance per HTTP session (user)
}

// Using @Scope with bean definition
@Configuration
public class AppConfig {

    @Bean
    @Scope("prototype")
    public ShoppingCart shoppingCart() {
        return new ShoppingCart();
    }
}
```

## 4.13. Configuration Class (@Configuration)

### 📌 និយមន័យ (Definition):

```java
@Configuration គឺជា annotation ដែលប្រាប់ Spring Container ថា class នេះផ្ទុក Bean definitions (methods ដែលមាន @Bean)។ Configuration classes ជំនួស XML configuration files (ដូចជា applicationContext.xml) ដោយប្រើ Java-based configuration។
import org.springframework.context.annotation.Bean;
import org.springframework.context.annotation.Configuration;
import org.springframework.context.annotation.PropertySource;
import org.springframework.beans.factory.annotation.Value;
import java.util.Properties;

@Configuration
@PropertySource("classpath:application.properties")  // Load external properties
public class AppConfig {

    @Value("$" + "{app.name}")
    private String appName;

    // Define a custom bean
    @Bean
    public DataSource dataSource() {
        HikariDataSource dataSource = new HikariDataSource();
        dataSource.setJdbcUrl("jdbc:mysql://localhost:3306/mydb");
        dataSource.setUsername("root");
        dataSource.setPassword("secret");
        dataSource.setMaximumPoolSize(10);
        return dataSource;
    }

    @Bean
    public JdbcTemplate jdbcTemplate(DataSource dataSource) {
        return new JdbcTemplate(dataSource);
    }

    @Bean
    public RestTemplate restTemplate() {
        return new RestTemplate();
    }

    @Bean
    public ObjectMapper objectMapper() {
        ObjectMapper mapper = new ObjectMapper();
        mapper.registerModule(new JavaTimeModule());
        mapper.disable(SerializationFeature.WRITE_DATES_AS_TIMESTAMPS);
        return mapper;
    }

    @Bean
    public Properties customProperties() {
        Properties props = new Properties();
        props.setProperty("app.version", "1.0.0");
        props.setProperty("app.environment", "development");
        return props;
    }
}
```

## 4.14. @Bean Annotation

### 📌 និយមន័យ (Definition):

```java
@Bean គឺជា method-level annotation ដែលប្រាប់ Spring Container ថា method នេះ បង្កើត និងត្រឡប់ (returns) Spring Bean មួយដែលត្រូវបានគ្រប់គ្រងដោយ IoC container។ @Bean ត្រូវបានប្រើតែក្នុង @Configuration classes ឬ @Component classes (ឬ component scanning)។
```

**1. Basic @Bean Usage**

```java
@Configuration
public class Config {

    @Bean
    public MyService myService() {
        return new MyService();
    }

    @Bean(name = "customBeanName")
    public AnotherService anotherService() {
        return new AnotherService();
    }
}
```

**2. Bean with Dependencies**

```java
@Configuration
public class Config {

    @Bean
    public ServiceA serviceA() {
        return new ServiceA();
    }

    @Bean
    public ServiceB serviceB(ServiceA serviceA) {
        // Spring injects ServiceA automatically
        return new ServiceB(serviceA);
    }
}
```

**3. Bean with Init/Destroy**

```java
@Configuration
public class Config {

    @Bean(initMethod = "init", destroyMethod = "cleanup")
    public DatabaseConnection databaseConnection() {
        return new DatabaseConnection();
    }
}
```

**4. Conditional Bean**

```properties
@Configuration
public class Config {

    @Bean
    @ConditionalOnProperty(name = "cache.enabled", havingValue = "true")
    public CacheManager cacheManager() {
        return new RedisCacheManager();
    }

    @Bean
    @Profile("dev")
    public DataSource devDataSource() { ... }
}
import org.springframework.context.annotation.Bean;
import org.springframework.context.annotation.Configuration;
import org.springframework.context.annotation.Primary;

@Configuration
public class DatabaseConfig {

    // Simple bean
    @Bean
    public DataSource dataSource() {
        HikariDataSource ds = new HikariDataSource();
        ds.setJdbcUrl("jdbc:mysql://localhost:3306/mydb");
        ds.setUsername("root");
        ds.setPassword("secret");
        return ds;
    }

    // Bean with custom name
    @Bean(name = "testDataSource")
    public DataSource testDataSource() {
        HikariDataSource ds = new HikariDataSource();
        ds.setJdbcUrl("jdbc:h2:mem:testdb");
        ds.setUsername("sa");
        ds.setPassword("");
        return ds;
    }

    // Primary bean (used when multiple beans of same type exist)
    @Bean
    @Primary
    public DataSource primaryDataSource() {
        return dataSource();  // Reuse existing bean definition
    }

    // Bean with dependencies - Spring auto-wires by parameter type
    @Bean
    public JdbcTemplate jdbcTemplate(DataSource dataSource) {
        return new JdbcTemplate(dataSource);
    }

    // Bean with init and destroy methods
    @Bean(initMethod = "connect", destroyMethod = "disconnect")
    public DatabaseConnection databaseConnection() {
        return new DatabaseConnection();
    }

    // Bean that depends on other beans
    @Bean
    public TransactionManager transactionManager(DataSource dataSource) {
        return new DataSourceTransactionManager(dataSource);
    }
}

// Using the beans
@Service
public class MyService {
    private final JdbcTemplate jdbcTemplate;

    public MyService(JdbcTemplate jdbcTemplate) {
        this.jdbcTemplate = jdbcTemplate;  // Spring injects the bean
    }
}
```

### 📊 Comparing @Component vs @Bean

| @Component | @Bean |
| --- | --- |
| Class-level annotation | Method-level annotation |
| Auto-detected via component scanning | Explicitly declared in @Configuration class |
| Cannot be used for third-party classes | Can create beans for third-party classes |
| Less flexible | More flexible (custom init/destroy logic) |
| Preferred for classes you own | Required for classes you don't own |

### 💡 When to use which: Use @Component (and stereotypes @Service, @Repository, @Controller) for classes that you write. Use @Bean for:

- Third-party classes (e.g., DataSource, RestTemplate, ObjectMapper)

- When you need custom initialization logic

- When you need to create multiple instances of the same class

- When you need conditional bean creation

### 📚 សង្ខេបមេរៀនទី៤ (Module 4 Summary)

នៅក្នុងមេរៀននេះ អ្នកបានរៀនអំពី Dependency Injection និង Beans ដែលជាគោលការណ៍ស្នូលរបស់ Spring Boot៖

- **IoC (Inversion of Control)** – Principle where container controls object lifecycle

- **DI (Dependency Injection)** – Pattern implementing IoC (Constructor, Setter, Field injection)

- **Bean Lifecycle** – Instantiation → Properties → Aware interfaces → PostProcessors → Init → Ready → Destroy

```java
@Component – Generic stereotype for Spring Beans
@Service – Business logic layer
@Repository – Data access layer with exception translation
@Controller – Web controller returning views (MVC)
@RestController – REST API controller returning JSON/XML
@Autowired – Automatic dependency injection
```

- **Constructor Injection** – Recommended approach (immutable, testable)

- **Setter Injection** – For optional dependencies

- **Bean Scopes** – Singleton, Prototype, Request, Session, Application, WebSocket

```java
@Configuration – Java-based configuration class
@Bean – Method-level bean declaration for third-party classes
```

# មេរៀនទី៥: ការបង្កើត REST API (Building REST API)

### 📖 សេចក្តីផ្តើម (Introduction):
REST API (Representational State Transfer) គឺជាស្ថាបត្យកម្ម (architectural style) សម្រាប់បង្កើត Web Services ដែលអនុញ្ញាតឱ្យកម្មវិធីផ្សេងៗគ្នា (frontend, mobile, third-party services) ទំនាក់ទំនងគ្នាតាមរយៈ HTTP protocol។ មេរៀននេះនឹងបង្រៀនអ្នកពីរបៀបបង្កើត REST API ជាមួយ Spring Boot ដោយប្រើ HTTP Methods, Request Mapping, Path Variables, Query Parameters, Request Body, Response Entity, និង CRUD Operations។

## 5.1. តើ REST API ជាអ្វី? (What is REST API?)

### 📌 និយមន័យ (Definition):

**REST (Representational State Transfer)** គឺជា architectural style ដែលបង្កើតឡើងដោយ Roy Fielding ក្នុងឆ្នាំ 2000។ **REST API** គឺជា web service ដែលអនុវត្តតាមគោលការណ៍ REST។ API មានន័យថា Application Programming Interface — ជាសំណុំនៃច្បាប់ (rules) ដែលកំណត់ពីរបៀប ដែលកម្មវិធីអាចទំនាក់ទំនងគ្នាបាន។

### 🔹 គោលការណ៍សំខាន់ៗរបស់ REST (REST Principles):

- **Client-Server Architecture** – បំបែក client (frontend) និង server (backend) ដាច់ពីគ្នា

- **Stateless** – server មិនរក្សាទុក state របស់ client ទេ; request នីមួយៗផ្ទុកព័ត៌មានចាំបាច់ទាំងអស់

- **Cacheable** – responses អាចត្រូវបាន cache ដើម្បីបង្កើនប្រសិទ្ធភាព

- **Uniform Interface** – ប្រើ HTTP methods ស្តង់ដារ (GET, POST, PUT, DELETE)

- **Layered System** – client មិនដឹងថាកំពុងទំនាក់ទំនងផ្ទាល់ជាមួយ server ឬតាមរយៈ proxy/load balancer

- **Code on Demand (optional)** – server អាចបញ្ជូន executable code ទៅ client

```http
// REST API Example
GET /api/users → Get all users
GET /api/users/1 → Get user with ID 1
POST /api/users → Create a new user
PUT /api/users/1 → Update user with ID 1
DELETE /api/users/1 → Delete user with ID 1
```

## 5.2. HTTP Methods (GET, POST, PUT, DELETE)

### 📌 និយមន័យ (Definition):

**HTTP Methods** (ឬ Verbs) គឺជាសកម្មភាព (actions) ដែល client ចង់ឱ្យ server អនុវត្តលើ resource។ វាកំណត់ពីប្រភេទប្រតិបត្តិការដែលត្រូវធ្វើ។

| Method | Description | Idempotent? | Safe? | Has Body? |
| --- | --- | --- | --- | --- |
| GET | ទាញយក (retrieve) data | ✅ Yes | ✅ Yes | ❌ No |
| POST | បង្កើត (create) resource ថ្មី | ❌ No | ❌ No | ✅ Yes |
| PUT | ធ្វើបច្ចុប្បន្នភាព (update/replace) resource ទាំងមូល | ✅ Yes | ❌ No | ✅ Yes |
| PATCH | ធ្វើបច្ចុប្បន្នភាព (partial update) resource ខ្លះ | ❌ No | ❌ No | ✅ Yes |
| DELETE | លុប (remove) resource | ✅ Yes | ❌ No | ❌ No |

### 💡 Important Definitions:

- **Idempotent** – ការហៅ method ដដែលៗច្រើនដង ផ្តល់លទ្ធផលដូចគ្នានឹងការហៅម្តង (GET, PUT, DELETE are idempotent).

- **Safe** – method ដែលមិនផ្លាស់ប្តូរ state របស់ resource (GET is safe).

## 5.3. Request Mapping (@RequestMapping)

### 📌 និយមន័យ (Definition):

```java
@RequestMapping គឺជា annotation ដែលប្រើដើម្បី map HTTP requests ទៅកាន់ controller methods។ វាអាចប្រើនៅ class level (base URL) ឬ method level (specific endpoint)។ Spring Boot ក៏មាន annotations ជំនួយផងដែរ: @GetMapping, @PostMapping, @PutMapping, @DeleteMapping, @PatchMapping។
import org.springframework.web.bind.annotation.*;

@RestController
@RequestMapping("/api/products")  // Base URL for all methods in this controller
public class ProductController {

    // @RequestMapping with method attribute
    @RequestMapping(value = "/all", method = RequestMethod.GET)
    public List<Product> getAllProducts() {
        return productService.findAll();
    }

    // @GetMapping (shortcut for RequestMethod.GET)
    @GetMapping("/{id}")
    public Product getProductById(@PathVariable Long id) {
        return productService.findById(id);
    }

    // @PostMapping (shortcut for RequestMethod.POST)
    @PostMapping
    public Product createProduct(@RequestBody Product product) {
        return productService.save(product);
    }

    // @PutMapping (shortcut for RequestMethod.PUT)
    @PutMapping("/{id}")
    public Product updateProduct(@PathVariable Long id, @RequestBody Product product) {
        return productService.update(id, product);
    }

    // @DeleteMapping (shortcut for RequestMethod.DELETE)
    @DeleteMapping("/{id}")
    public void deleteProduct(@PathVariable Long id) {
        productService.delete(id);
    }

    // @PatchMapping (shortcut for RequestMethod.PATCH)
    @PatchMapping("/{id}")
    public Product partialUpdate(@PathVariable Long id, @RequestBody Map<String, Object> updates) {
        return productService.partialUpdate(id, updates);
    }

    // RequestMapping with headers
    @GetMapping(value = "/export", headers = "Accept=application/json")
    public String exportAsJson() {
        return "JSON export";
    }

    // RequestMapping with produces (response content type)
    @GetMapping(value = "/xml", produces = MediaType.APPLICATION_XML_VALUE)
    public Product getProductAsXml() {
        return new Product(1L, "Laptop");
    }

    // RequestMapping with consumes (request content type)
    @PostMapping(consumes = MediaType.APPLICATION_JSON_VALUE)
    public Product createFromJson(@RequestBody Product product) {
        return productService.save(product);
    }
}
```

## 5.4. Path Variables (@PathVariable)

### 📌 និយមន័យ (Definition):

```java
@PathVariable គឺជា annotation ដែលប្រើដើម្បី extract values ពី URI template (path)។ Path variables ត្រូវបានប្រើដើម្បីកំណត់អត្តសញ្ញាណ (identify) specific resources (ឧ. /users/1, /products/abc)។
import org.springframework.web.bind.annotation.*;

@RestController
@RequestMapping("/api/users")
public class UserController {

    // Single path variable
    @GetMapping("/{id}")
    public User getUserById(@PathVariable Long id) {
        // URL: /api/users/123
        // id = 123
        return userService.findById(id);
    }

    // Path variable with custom name (if different from parameter name)
    @GetMapping("/{userId}")
    public User getUserByIdCustom(@PathVariable("userId") Long id) {
        // URL: /api/users/123
        // id = 123 (parameter name is 'id' but path variable is 'userId')
        return userService.findById(id);
    }

    // Multiple path variables
    @GetMapping("/{category}/{id}")
    public Product getProductByCategoryAndId(@PathVariable String category, @PathVariable Long id) {
        // URL: /api/products/electronics/456
        // category = "electronics", id = 456
        return productService.findByCategoryAndId(category, id);
    }

    // Path variable with regex pattern
    @GetMapping("/{id:\d+}")  // Only digits allowed
    public User getUserByIdWithRegex(@PathVariable Long id) {
        // URL: /api/users/123 (works)
        // URL: /api/users/abc (404 - not found)
        return userService.findById(id);
    }

    // Optional path variable (using required = false)
    @GetMapping({"/{id}", "/"})
    public List<User> getUsers(@PathVariable(required = false) Long id) {
        if (id != null) {
            return List.of(userService.findById(id));
        }
        return userService.findAll();
    }

    // Multiple path variables with Map
    @GetMapping("/{category}/{subcategory}/{id}")
    public Map<String, String> getAllPathVariables(
            @PathVariable Map<String, String> pathVariables) {
        // URL: /api/products/electronics/phones/123
        // pathVariables = {category=electronics, subcategory=phones, id=123}
        return pathVariables;
    }
}
```

## 5.5. Query Parameters (@RequestParam)

### 📌 និយមន័យ (Definition):

```java
@RequestParam គឺជា annotation ដែលប្រើដើម្បី extract query parameters ពី URL (បន្ទាប់ពី ?)។ Query parameters ត្រូវបានប្រើសម្រាប់ filtering, pagination, sorting, និង optional data។
import org.springframework.web.bind.annotation.*;
import org.springframework.data.domain.Page;
import java.util.List;

@RestController
@RequestMapping("/api/products")
public class ProductController {

    // Basic query parameter
    @GetMapping("/search")
    public List<Product> searchByName(@RequestParam String name) {
        // URL: /api/products/search?name=laptop
        // name = "laptop"
        return productService.findByName(name);
    }

    // Query parameter with default value
    @GetMapping
    public List<Product> getAllProducts(
            @RequestParam(defaultValue = "0") int page,
            @RequestParam(defaultValue = "10") int size) {
        // URL: /api/products?page=2&size=20
        // page = 2, size = 20
        // If not provided: page = 0, size = 10
        return productService.findAll(page, size);
    }

    // Optional query parameter (required = false)
    @GetMapping("/filter")
    public List<Product> filterProducts(
            @RequestParam(required = false) String category,
            @RequestParam(required = false) Double minPrice,
            @RequestParam(required = false) Double maxPrice) {
        // URL: /api/products/filter?category=electronics&minPrice=100
        // category = "electronics", minPrice = 100, maxPrice = null
        return productService.filter(category, minPrice, maxPrice);
    }

    // Query parameter with custom name
    @GetMapping("/by-category")
    public List<Product> getByCategory(@RequestParam("cat") String category) {
        // URL: /api/products/by-category?cat=books
        // category = "books" (parameter name is 'cat' but variable is 'category')
        return productService.findByCategory(category);
    }

    // Multiple query parameters (all optional)
    @GetMapping("/advanced-search")
    public List<Product> advancedSearch(
            @RequestParam(required = false) String name,
            @RequestParam(required = false) String category,
            @RequestParam(required = false) Double minPrice,
            @RequestParam(required = false) Double maxPrice,
            @RequestParam(defaultValue = "name") String sortBy,
            @RequestParam(defaultValue = "asc") String sortDirection) {
        // URL: /api/products/advanced-search?name=phone&minPrice=200&sortBy=price&sortDirection=desc
        return productService.advancedSearch(name, category, minPrice, maxPrice, sortBy, sortDirection);
    }

    // Map for all query parameters
    @GetMapping("/all-params")
    public Map<String, String> getAllParams(@RequestParam Map<String, String> allParams) {
        // URL: /api/products/all-params?key1=value1&key2=value2&key3=value3
        // allParams = {key1=value1, key2=value2, key3=value3}
        return allParams;
    }

    // List of values for same parameter name
    @GetMapping("/by-ids")
    public List<Product> getProductsByIds(@RequestParam List<Long> ids) {
        // URL: /api/products/by-ids?ids=1&ids=2&ids=3
        // ids = [1, 2, 3]
        return productService.findAllByIds(ids);
    }

    // Pagination with sorting
    @GetMapping("/paginated")
    public Page<Product> getPaginatedProducts(
            @RequestParam(defaultValue = "0") int page,
            @RequestParam(defaultValue = "10") int size,
            @RequestParam(defaultValue = "id") String sortBy,
            @RequestParam(defaultValue = "asc") String direction) {

        Sort.Direction sortDirection = Sort.Direction.fromString(direction);
        Pageable pageable = PageRequest.of(page, size, Sort.by(sortDirection, sortBy));
        return productService.findAll(pageable);
    }
}
```

### 💡 @PathVariable vs @RequestParam:

| @PathVariable | @RequestParam |
| --- | --- |
| Extracts from URI path (/) | Extracts from query string (?id=123) |
| Used to identify specific resource | Used for filtering, pagination, sorting |
| Required by default | Can be optional with default value |
| Example: /users/123 | Example: /users?page=2&size=10 |

## 5.6. Request Body (@RequestBody)

### 📌 និយមន័យ (Definition):

```java
@RequestBody គឺជា annotation ដែលប្រើដើម្បី bind HTTP request body (JSON/XML) ទៅកាន់ Java object។ Spring Boot ប្រើ Jackson library ដើម្បី deserialize JSON ទៅជា Java object ដោយស្វ័យប្រវត្តិ។
import org.springframework.web.bind.annotation.*;
import javax.validation.Valid;

@RestController
@RequestMapping("/api/users")
public class UserController {

    // Basic RequestBody usage
    @PostMapping
    public User createUser(@RequestBody User user) {
        // JSON: {"name": "Sok Dara", "email": "sok@example.com", "age": 25}
        // Automatically converted to User object
        return userService.save(user);
    }

    // RequestBody with validation
    @PostMapping("/valid")
    public User createUserValid(@Valid @RequestBody User user) {
        // Validation annotations like @NotNull, @Email, @Size are checked
        return userService.save(user);
    }

    // RequestBody with custom object
    @PostMapping("/register")
    public ResponseEntity<String> registerUser(@RequestBody RegisterRequest request) {
        // RegisterRequest contains: username, password, email, firstName, lastName
        userService.register(request);
        return ResponseEntity.ok("User registered successfully");
    }

    // RequestBody as Map (for dynamic fields)
    @PostMapping("/dynamic")
    public Map<String, Object> handleDynamicJson(@RequestBody Map<String, Object> payload) {
        // Accepts any JSON structure
        System.out.println("Received: " + payload);
        return payload;  // Echo back
    }

    // RequestBody as String (raw JSON)
    @PostMapping("/raw")
    public String handleRawJson(@RequestBody String jsonBody) {
        // Receives raw JSON string
        System.out.println("Raw JSON: " + jsonBody);
        return "Received: " + jsonBody;
    }

    // Combining @RequestBody with other annotations
    @PostMapping("/{userId}/orders")
    public Order createOrder(
            @PathVariable Long userId,
            @RequestBody OrderRequest orderRequest,
            @RequestParam(required = false) boolean expressDelivery) {
        // URL: /api/users/123/orders?expressDelivery=true
        // userId = 123
        // orderRequest from JSON body
        // expressDelivery = true
        return orderService.create(userId, orderRequest, expressDelivery);
    }
}

// Example DTO (Data Transfer Object)
public class RegisterRequest {
    @NotNull
    @Size(min = 3, max = 20)
    private String username;

    @NotNull
    @Size(min = 6, max = 100)
    private String password;

    @NotNull
    @Email
    private String email;

    private String firstName;
    private String lastName;

    // Getters and setters
}

// JSON request example:
// {
//   "username": "sokdara",
//   "password": "secret123",
//   "email": "sok@example.com",
//   "firstName": "Sok",
//   "lastName": "Dara"
// }
```

## 5.7. Response Entity (@ResponseEntity)

### 📌 និយមន័យ (Definition):

**ResponseEntity** គឺជា class ដែលតំណាងឱ្យ HTTP response ទាំងមូល — រួមបញ្ចូល**status code**, **headers**, និង **body**។ វាផ្តល់នូវការបត់បែន (flexibility) ច្រើនជាងការត្រឡប់ object ធម្មតា។

```java
import org.springframework.http.HttpStatus;
import org.springframework.http.ResponseEntity;
import org.springframework.web.bind.annotation.*;
import java.net.URI;
import java.time.LocalDateTime;
import java.util.Map;

@RestController
@RequestMapping("/api/products")
public class ProductController {

    // 1. Basic ResponseEntity with status code
    @GetMapping("/{id}")
    public ResponseEntity<Product> getProduct(@PathVariable Long id) {
        Optional<Product> product = productService.findById(id);

        if (product.isPresent()) {
            // Return 200 OK with product
            return ResponseEntity.ok(product.get());
        } else {
            // Return 404 Not Found
            return ResponseEntity.notFound().build();
        }
    }

    // 2. ResponseEntity with custom status code
    @PostMapping
    public ResponseEntity<Product> createProduct(@RequestBody Product product) {
        Product saved = productService.save(product);
        // Return 201 Created with the created resource
        return ResponseEntity.status(HttpStatus.CREATED).body(saved);
    }

    // 3. ResponseEntity with location header (for REST best practices)
    @PostMapping("/with-location")
    public ResponseEntity<Product> createProductWithLocation(@RequestBody Product product) {
        Product saved = productService.save(product);
        URI location = URI.create("/api/products/" + saved.getId());
        return ResponseEntity.created(location).body(saved);
    }

    // 4. ResponseEntity with custom headers
    @GetMapping("/export")
    public ResponseEntity<byte[]> exportProducts() {
        byte[] csvData = productService.exportToCsv();
        return ResponseEntity.ok()
```

.header("Content-Type", "text/csv")

```text
                .header("Content-Disposition", "attachment; filename=products.csv")
```

.contentLength(csvData.length)

```java
                .body(csvData);
    }

    // 5. ResponseEntity with no body
    @DeleteMapping("/{id}")
    public ResponseEntity<Void> deleteProduct(@PathVariable Long id) {
        if (productService.existsById(id)) {
            productService.delete(id);
            return ResponseEntity.noContent().build();  // 204 No Content
        }
        return ResponseEntity.notFound().build();  // 404 Not Found
    }

    // 6. ResponseEntity with custom status and message
    @PutMapping("/{id}")
    public ResponseEntity<?> updateProduct(@PathVariable Long id, @RequestBody Product product) {
        try {
            Product updated = productService.update(id, product);
            return ResponseEntity.ok(updated);
        } catch (ResourceNotFoundException e) {
            return ResponseEntity.status(HttpStatus.NOT_FOUND)
                    .body(Map.of("error", "Product not found", "id", id));
        } catch (Exception e) {
            return ResponseEntity.status(HttpStatus.INTERNAL_SERVER_ERROR)
                    .body(Map.of("error", "Internal server error", "message", e.getMessage()));
        }
    }

    // 7. ResponseEntity with builder pattern
    @GetMapping("/builder-example")
    public ResponseEntity<Product> builderExample() {
        return ResponseEntity.ok()
```

.header("X-Custom-Header", "CustomValue")

.header("X-Request-ID", "12345")

```java
                .body(new Product(1L, "Laptop"));
    }

    // 8. ResponseEntity with cache control
    @GetMapping("/cached")
    public ResponseEntity<Product> getCachedProduct() {
        return ResponseEntity.ok()
```

.cacheControl(CacheControl.maxAge(30, TimeUnit.SECONDS))

```java
                .body(productService.getCachedProduct());
    }

    // 9. Common ResponseEntity static methods:
    // ResponseEntity.ok(body)           → 200 OK
    // ResponseEntity.created(location)  → 201 Created
    // ResponseEntity.noContent()        → 204 No Content
    // ResponseEntity.badRequest()       → 400 Bad Request
    // ResponseEntity.notFound()         → 404 Not Found
    // ResponseEntity.status(HttpStatus) → Custom status
}
```

## 5.8. JSON Response

### 📌 និយមន័យ (Definition):

**JSON (JavaScript Object Notation)** គឺជា lightweight data-interchange format ដែលងាយស្រួលសម្រាប់មនុស្សអាន និងងាយស្រួលសម្រាប់ម៉ាស៊ីន parse។ Spring Boot ដោយប្រើ Jackson library បំលែង Java objects ទៅជា JSON ដោយស្វ័យប្រវត្តិនៅពេលដែល method returns object ហើយមាន @ResponseBody ឬ @RestController។

```java
import com.fasterxml.jackson.annotation.*;
import java.time.LocalDateTime;
import java.util.List;

@RestController
@RequestMapping("/api/orders")
public class OrderController {

    // Automatically converts to JSON
    @GetMapping("/{id}")
    public Order getOrder(@PathVariable Long id) {
        // Spring converts Order object to JSON automatically
        return orderService.findById(id);
    }

    // List of objects → JSON array
    @GetMapping
    public List<Order> getAllOrders() {
        // Returns JSON array: [{...}, {...}]
        return orderService.findAll();
    }

    // Custom JSON response structure
    @GetMapping("/response")
    public ApiResponse<Order> getOrderWithMetadata(@PathVariable Long id) {
        Order order = orderService.findById(id);
        return ApiResponse.success(order, "Order retrieved successfully");
    }
}

// Example DTO with JSON control annotations
public class Order {
    private Long id;
    private String orderNumber;
    private Double totalAmount;

    @JsonFormat(pattern = "yyyy-MM-dd HH:mm:ss")
    private LocalDateTime orderDate;

    @JsonIgnore  // This field will NOT be included in JSON
    private String internalTrackingCode;

    @JsonProperty("customer_name")  // Custom JSON field name
    private String customerName;

    @JsonInclude(JsonInclude.Include.NON_NULL)  // Include only if not null
    private String specialInstructions;

    // Getters and setters
}

// Generic API Response wrapper
public class ApiResponse<T> {
    private boolean success;
    private String message;
    private T data;
    private LocalDateTime timestamp;
    private List<String> errors;

    public static <T> ApiResponse<T> success(T data, String message) {
        ApiResponse<T> response = new ApiResponse<>();
        response.setSuccess(true);
        response.setData(data);
        response.setMessage(message);
        response.setTimestamp(LocalDateTime.now());
        return response;
    }

    public static <T> ApiResponse<T> error(String message, List<String> errors) {
        ApiResponse<T> response = new ApiResponse<>();
        response.setSuccess(false);
        response.setMessage(message);
        response.setErrors(errors);
        response.setTimestamp(LocalDateTime.now());
        return response;
    }
}

// Example JSON output:
// {
//   "success": true,
//   "message": "Order retrieved successfully",
//   "data": {
//     "id": 1,
//     "orderNumber": "ORD-001",
//     "totalAmount": 299.99,
//     "orderDate": "2024-01-15 10:30:00",
//     "customer_name": "Sok Dara"
//   },
//   "timestamp": "2024-01-15T10:30:00"
// }
```

### 📝 Common Jackson Annotations for JSON:

```text
@JsonProperty – Custom JSON field name
@JsonIgnore – Exclude field from JSON
@JsonInclude – Include field conditionally (NON_NULL, NON_EMPTY)
@JsonFormat – Format date/time fields
@JsonUnwrapped – Flatten nested objects
@JsonManagedReference / @JsonBackReference – Handle circular references
```

## 5.9. CRUD API (Create, Read, Update, Delete)

### 📌 និយមន័យ (Definition):

**CRUD** គឺជា acronym សម្រាប់ **Create, Read, Update, Delete** — ប្រតិបត្តិការមូលដ្ឋានទាំងបួនដែលកម្មវិធីភាគច្រើនត្រូវការសម្រាប់គ្រប់គ្រងទិន្នន័យ។ នេះគឺជា example ពេញលេញនៃ REST API ដែលអនុវត្ត CRUD operations។

```java
// ============================================================
// Entity Class
// ============================================================
import javax.persistence.*;
import javax.validation.constraints.*;
import java.time.LocalDateTime;

@Entity
@Table(name = "products")
public class Product {
    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)
    private Long id;

    @NotBlank
    @Size(min = 2, max = 100)
    private String name;

    @Size(max = 500)
    private String description;

    @NotNull
    @Positive
    private Double price;

    @Min(0)
    @Max(10000)
    private Integer quantity;

    private String category;

    private LocalDateTime createdAt;
    private LocalDateTime updatedAt;

    // Constructors, Getters, Setters
}

// ============================================================
// DTO (Data Transfer Object)
// ============================================================
public class ProductDto {
    @NotBlank
    private String name;
    private String description;
    @NotNull
    private Double price;
    private Integer quantity;
    private String category;
    // Getters and Setters
}

// ============================================================
// Repository
// ============================================================
@Repository
public interface ProductRepository extends JpaRepository<Product, Long> {
    List<Product> findByCategory(String category);
    List<Product> findByNameContainingIgnoreCase(String name);
    List<Product> findByPriceBetween(Double minPrice, Double maxPrice);
}

// ============================================================
// Service Layer
// ============================================================
@Service
@Transactional
public class ProductService {

    @Autowired
    private ProductRepository productRepository;

    // Create
    public Product createProduct(ProductDto productDto) {
        Product product = new Product();
        product.setName(productDto.getName());
        product.setDescription(productDto.getDescription());
        product.setPrice(productDto.getPrice());
        product.setQuantity(productDto.getQuantity());
        product.setCategory(productDto.getCategory());
        product.setCreatedAt(LocalDateTime.now());
        product.setUpdatedAt(LocalDateTime.now());
        return productRepository.save(product);
    }

    // Read (All)
    public List<Product> getAllProducts() {
        return productRepository.findAll();
    }

    // Read (Single)
    public Product getProductById(Long id) {
        return productRepository.findById(id)
            .orElseThrow(() -> new ResourceNotFoundException("Product not found with id: " + id));
    }

    // Update (Full)
    public Product updateProduct(Long id, ProductDto productDto) {
        Product product = getProductById(id);
        product.setName(productDto.getName());
        product.setDescription(productDto.getDescription());
        product.setPrice(productDto.getPrice());
        product.setQuantity(productDto.getQuantity());
        product.setCategory(productDto.getCategory());
        product.setUpdatedAt(LocalDateTime.now());
        return productRepository.save(product);
    }

    // Delete
    public void deleteProduct(Long id) {
        Product product = getProductById(id);
        productRepository.delete(product);
    }

    // Additional methods
    public List<Product> getProductsByCategory(String category) {
        return productRepository.findByCategory(category);
    }

    public List<Product> searchProducts(String keyword) {
        return productRepository.findByNameContainingIgnoreCase(keyword);
    }
}

// ============================================================
// Controller (REST API)
// ============================================================
@RestController
@RequestMapping("/api/products")
public class ProductController {

    @Autowired
    private ProductService productService;

    // CREATE - POST /api/products
    @PostMapping
    public ResponseEntity<Product> createProduct(@Valid @RequestBody ProductDto productDto) {
        Product created = productService.createProduct(productDto);
        URI location = URI.create("/api/products/" + created.getId());
        return ResponseEntity.created(location).body(created);
    }

    // READ ALL - GET /api/products
    @GetMapping
    public ResponseEntity<List<Product>> getAllProducts() {
        List<Product> products = productService.getAllProducts();
        return ResponseEntity.ok(products);
    }

    // READ ONE - GET /api/products/{id}
    @GetMapping("/{id}")
    public ResponseEntity<Product> getProductById(@PathVariable Long id) {
        Product product = productService.getProductById(id);
        return ResponseEntity.ok(product);
    }

    // UPDATE - PUT /api/products/{id}
    @PutMapping("/{id}")
    public ResponseEntity<Product> updateProduct(
            @PathVariable Long id,
            @Valid @RequestBody ProductDto productDto) {
        Product updated = productService.updateProduct(id, productDto);
        return ResponseEntity.ok(updated);
    }

    // DELETE - DELETE /api/products/{id}
    @DeleteMapping("/{id}")
    public ResponseEntity<Void> deleteProduct(@PathVariable Long id) {
        productService.deleteProduct(id);
        return ResponseEntity.noContent().build();
    }

    // Additional endpoints
    @GetMapping("/category/{category}")
    public ResponseEntity<List<Product>> getByCategory(@PathVariable String category) {
        return ResponseEntity.ok(productService.getProductsByCategory(category));
    }

    @GetMapping("/search")
    public ResponseEntity<List<Product>> search(@RequestParam String q) {
        return ResponseEntity.ok(productService.searchProducts(q));
    }
}
```

## 5.10. REST Best Practices (ការអនុវត្តល្អបំផុត)

### 📌 ការអនុវត្តល្អបំផុតសម្រាប់ REST API:

**1. Use nouns for resources (not verbs)**

❌ /getUsers, /createUser, /deleteUser

### ✅ GET /users, POST /users, DELETE /users/

**2. Use plural nouns for collections**

❌ /user, /product, /order

### ✅ /users, /products, /orders

**3. Use HTTP status codes correctly**

200 OK, 201 Created, 204 No Content, 400 Bad Request, 401 Unauthorized, 403 Forbidden, 404 Not Found, 500 Internal Server Error

**4. Version your API**

### ✅ /api/v1/users, /api/v2/users

### ✅ Accept: application/vnd.example.v1+json

**5. Use query parameters for filtering, pagination, sorting**

### ✅ /users?page=2&size=20&sort=name

### ✅ /products?category=electronics&minPrice=100

**6. Return appropriate response structures**

### ✅ Wrap responses in consistent format: { success, data, message, errors }

**7. Use HTTPS (always in production)**

### ✅ Secure your API with SSL/TLS

**8. Document your API**

### ✅ Use Springdoc OpenAPI (Swagger) → http://localhost:8080/swagger-ui.html

**9. Validate input data**

### ✅ Use @Valid and Bean Validation annotations (@NotNull, @Email, @Size)

**10. Use semantic HTTP methods**

GET (retrieve), POST (create), PUT (full update), PATCH (partial update), DELETE (remove)

## 5.11. HTTP Status Codes (កូដស្ថានភាព HTTP)

### 📌 HTTP Status Codes ចែកចេញជា ៥ ក្រុម:

```text
1xx: Informational
```

- 100 Continue – Request received, continue

- 101 Switching Protocols – Switching protocols

```text
2xx: Success
```

- 200 OK – Request successful

- 201 Created – Resource created successfully

- 202 Accepted – Request accepted for processing

- 204 No Content – Request successful, no content to return

```text
3xx: Redirection
```

- 301 Moved Permanently – Resource moved permanently

- 302 Found – Temporary redirect

- 304 Not Modified – Resource not modified (cached)

```text
4xx: Client Error
```

- 400 Bad Request – Invalid request syntax

- 401 Unauthorized – Authentication required

- 403 Forbidden – No permission to access

- 404 Not Found – Resource not found

- 405 Method Not Allowed – HTTP method not supported

- 409 Conflict – Conflict with current state

- 422 Unprocessable Entity – Validation failed

- 429 Too Many Requests – Rate limit exceeded

```text
5xx: Server Error
```

- 500 Internal Server Error – Generic server error

- 501 Not Implemented – Method not implemented

- 502 Bad Gateway – Invalid response from upstream

- 503 Service Unavailable – Server temporarily unavailable

- 504 Gateway Timeout – Upstream timeout

```java
import org.springframework.http.HttpStatus;
import org.springframework.web.bind.annotation.*;

@RestController
public class StatusCodeExampleController {

    // 200 OK
    @GetMapping("/users")
    public ResponseEntity<List<User>> getUsers() {
        return ResponseEntity.ok(userService.findAll());
    }

    // 201 Created
    @PostMapping("/users")
    public ResponseEntity<User> createUser(@RequestBody User user) {
        User saved = userService.save(user);
        return ResponseEntity.status(HttpStatus.CREATED).body(saved);
    }

    // 204 No Content
    @DeleteMapping("/users/{id}")
    public ResponseEntity<Void> deleteUser(@PathVariable Long id) {
        userService.delete(id);
        return ResponseEntity.noContent().build();
    }

    // 400 Bad Request
    @PostMapping("/validate")
    public ResponseEntity<?> validateData(@RequestBody Map<String, String> data) {
        if (data.get("name") == null || data.get("name").isEmpty()) {
            return ResponseEntity.badRequest().body(Map.of("error", "Name is required"));
        }
        return ResponseEntity.ok().build();
    }

    // 401 Unauthorized
    @GetMapping("/admin")
    public ResponseEntity<?> adminOnly() {
        // In real app, use Spring Security
        if (!isAuthenticated()) {
            return ResponseEntity.status(HttpStatus.UNAUTHORIZED)
                    .body(Map.of("error", "Authentication required"));
        }
        return ResponseEntity.ok(adminData);
    }

    // 403 Forbidden
    @GetMapping("/super-admin")
    public ResponseEntity<?> superAdminOnly() {
        if (!hasRole("SUPER_ADMIN")) {
            return ResponseEntity.status(HttpStatus.FORBIDDEN)
                    .body(Map.of("error", "Insufficient permissions"));
        }
        return ResponseEntity.ok(superAdminData);
    }

    // 404 Not Found
    @GetMapping("/users/{id}")
    public ResponseEntity<User> getUser(@PathVariable Long id) {
        return userService.findById(id)
```

.map(ResponseEntity::ok)

```java
                .orElse(ResponseEntity.notFound().build());
    }

    // 409 Conflict
    @PostMapping("/users/email")
    public ResponseEntity<?> checkEmail(@RequestParam String email) {
        if (userService.emailExists(email)) {
            return ResponseEntity.status(HttpStatus.CONFLICT)
                    .body(Map.of("error", "Email already exists"));
        }
        return ResponseEntity.ok().build();
    }

    // 422 Unprocessable Entity (Validation Error)
    @PostMapping("/products")
    public ResponseEntity<?> createProduct(@Valid @RequestBody Product product) {
        // With @Valid, Spring automatically returns 400
        // For custom validation logic returning 422:
        if (product.getPrice() < 0) {
            return ResponseEntity.unprocessableEntity()
                    .body(Map.of("error", "Price cannot be negative"));
        }
        return ResponseEntity.ok(productService.save(product));
    }
}
```

## 5.12. API Testing with Postman

### 📌 Postman ជាអ្វី? (What is Postman?):

**Postman** គឺជា popular tool សម្រាប់ testing REST APIs។ វាអនុញ្ញាតឱ្យអ្នកផ្ញើ HTTP requests (GET, POST, PUT, DELETE) ទៅកាន់ API endpoints និងមើល responses។

### 📝 GET Request Example

```http
Method: GET
URL: http://localhost:8080/api/users
Headers: Content-Type: application/json
Response: 200 OK
[
  { "id": 1, "name": "Sok", "email": "sok@example.com" },
  { "id": 2, "name": "Dara", "email": "dara@example.com" }
]
```

### 📝 GET with Parameters

```http
Method: GET
URL: http://localhost:8080/api/users/1
Response: 200 OK
{ "id": 1, "name": "Sok", "email": "sok@example.com" }
```

### 📝 POST Request Example

```http
Method: POST
URL: http://localhost:8080/api/users
```

Body (raw JSON):

```json
{
  "name": "Cheata",
  "email": "cheata@example.com",
  "age": 25
}
Response: 201 Created
```

### 📝 PUT Request Example

```http
Method: PUT
URL: http://localhost:8080/api/users/1
```

Body (raw JSON):

```json
{
  "name": "Sok Dara",
  "email": "sok.dara@example.com",
  "age": 26
}
Response: 200 OK
```

### 📝 DELETE Request Example

```http
Method: DELETE
URL: http://localhost:8080/api/users/1
Response: 204 No Content
```

### 📝 Query Parameters Example

```http
Method: GET
URL: http://localhost:8080/api/users?page=1&size=10&sort=name,asc
Params: page=1, size=10, sort=name,asc
```

### 🔧 How to Test API with Postman - Step by Step:

1. Download and install Postman from [postman.com](https://www.postman.com/downloads/)

2. Open Postman and click **New** **→** **HTTP Request**

3. Select HTTP method (GET, POST, PUT, DELETE)

4. Enter URL (e.g., http://localhost:8080/api/users)

5. For POST/PUT: Go to **Body** tab → Select **raw** → Select **JSON** → Enter JSON data

6. For headers: Go to **Headers** tab → Add Content-Type: application/json

7. Click **Send** button

8. View response in the bottom panel (Status code, Body, Headers)

9. Save requests to Collections for reusability

10. Use **Environment Variables** for different environments (dev, test, prod)

### 🧪 Postman Testing Tips:

- Use **Collections** to organize your API tests

```text
Use Environment Variables for base URL (e.g., {{base_url}}/api/users)
```

- Write **Tests** in the Tests tab to automate validation:

```text
pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});

pm.test("Response has users array", function () {
    pm.expect(pm.response.json()).to.be.an('array');
});
```

- Use **Collection Runner** to run multiple requests automatically

- Export collections as JSON to share with team

- Use **Mock Servers** for testing without backend

- Use **Monitors** to schedule automated API tests

### 📚 សង្ខេបមេរៀនទី៥ (Module 5 Summary)

នៅក្នុងមេរៀននេះ អ្នកបានរៀនអំពីការបង្កើត REST API ជាមួយ Spring Boot៖

- **REST API** – Architectural style for web services, stateless, uniform interface

- **HTTP Methods** – GET (retrieve), POST (create), PUT (full update), DELETE (remove)

```text
@RequestMapping – Map HTTP requests to controller methods
@PathVariable – Extract values from URL path (/users/123)
@RequestParam – Extract query parameters (?page=1&size=10)
@RequestBody – Bind HTTP request body to Java object (JSON)
```

- **ResponseEntity** – Full control over HTTP response (status, headers, body)

- **JSON Response** – Automatic serialization using Jackson, @JsonIgnore, @JsonProperty

- **CRUD API** – Complete example with Entity, Repository, Service, Controller layers

- **REST Best Practices** – Use nouns, plural, versioning, correct status codes, validation

- **HTTP Status Codes** – 2xx (Success), 3xx (Redirect), 4xx (Client Error), 5xx (Server Error)

- **Postman Testing** – Tool for testing APIs, collections, environments, automated tests

# មេរៀនទី៦: Spring Boot MVC (Model-View-Controller)

### 📖 សេចក្តីផ្តើម (Introduction):
Spring MVC (Model-View-Controller) គឺជា framework សម្រាប់បង្កើត web applications ដោយប្រើស្ថាបត្យកម្ម MVC។ វាបំបែកកម្មវិធីជា ៣ ផ្នែក៖ Model (ទិន្នន័យ), View (UI), Controller (logic)។ មេរៀននេះនឹងបង្រៀនអ្នកពី MVC Architecture, Controllers, Views, Thymeleaf, Form Handling, Validation, Redirect/Forward, Template Layout, Static Resources, និង Error Pages។

## 6.1. ស្ថាបត្យកម្ម MVC (MVC Architecture)

### 📌 និយមន័យ (Definition):

**MVC (Model-View-Controller)** គឺជា design pattern ដែលបំបែកកម្មវិធីជា ៣ សមាសភាគសំខាន់ៗ៖

**Model**

តំណាងឱ្យទិន្នន័យ (data) និងតក្កវិជ្ជាអាជីវកម្ម (business logic)។ Model ផ្ទុក data, validate data, និងទំនាក់ទំនងជាមួយ database។

Entity, DTO, Service, Repository

**View**

តំណាងឱ្យ UI (User Interface) ដែលអ្នកប្រើប្រាស់ឃើញ។ View ទទួល data ពី Model ហើយបង្ហាញវា។

HTML, Thymeleaf, JSP, CSS, JavaScript

**Controller**

ទទួល requests ពីអ្នកប្រើប្រាស់, ដំណើរការ (process) request, ហៅ Model, ហើយត្រឡប់ View វិញ។

```text
@Controller, @RequestMapping
```

**Spring MVC Request Flow:**

1. Browser ▶ DispatcherServlet (Front Controller)

2. DispatcherServlet ▶ HandlerMapping (find controller)

3. HandlerMapping ▶ Controller (process request)

4. Controller ▶ Service/Model (business logic)

5. Controller ▶ ViewResolver (resolve view name)

6. ViewResolver ▶ View (render HTML)

7. View ▶ DispatcherServlet ▶ Browser

```java
// Example of MVC in Spring Boot
@Controller
public class UserController {

    @Autowired
    private UserService userService;  // Model

    @GetMapping("/users")
    public String listUsers(Model model) {  // Controller
        List<User> users = userService.findAll();  // Get data from Model
        model.addAttribute("users", users);  // Add data to Model
        return "user-list";  // Return View name
    }
}
```

## 6.2. Controllers (@Controller)

### 📌 និយមន័យ (Definition):

```java
@Controller គឺជា annotation ដែលប្រាប់ Spring ថា class នេះគឺជា web controller។ Controller methods ត្រឡប់ view names (HTML pages) ហើយ data ត្រូវបានបញ្ជូនទៅ view តាមរយៈ Model object។
import org.springframework.stereotype.Controller;
import org.springframework.ui.Model;
import org.springframework.web.bind.annotation.*;

@Controller
@RequestMapping("/products")
public class ProductController {

    @Autowired
    private ProductService productService;

    // Display list of products
    @GetMapping
    public String listProducts(Model model) {
        List<Product> products = productService.findAll();
        model.addAttribute("products", products);
        return "products/list";
    }

    // Show form to create new product
    @GetMapping("/new")
    public String showCreateForm(Model model) {
        model.addAttribute("product", new Product());
        return "products/create";
    }

    // Process form submission
    @PostMapping
    public String createProduct(@ModelAttribute Product product) {
        productService.save(product);
        return "redirect:/products";
    }

    // Show form to edit product
    @GetMapping("/edit/{id}")
    public String showEditForm(@PathVariable Long id, Model model) {
        Product product = productService.findById(id);
        model.addAttribute("product", product);
        return "products/edit";
    }

    // Process update
    @PostMapping("/update/{id}")
    public String updateProduct(@PathVariable Long id, @ModelAttribute Product product) {
        product.setId(id);
        productService.update(product);
        return "redirect:/products";
    }

    // Delete product
    @GetMapping("/delete/{id}")
    public String deleteProduct(@PathVariable Long id) {
        productService.delete(id);
        return "redirect:/products";
    }

    // Pass multiple objects to view
    @GetMapping("/dashboard")
    public String dashboard(Model model) {
        model.addAttribute("totalProducts", productService.count());
        model.addAttribute("recentProducts", productService.findRecent(5));
        model.addAttribute("categories", productService.getAllCategories());
        return "dashboard";
    }
}
```

## 6.3. Views (ទិដ្ឋភាព)

### 📌 និយមន័យ (Definition):

**Views** គឺជា template files (HTML) ដែលបង្ហាញទិន្នន័យដល់អ្នកប្រើប្រាស់។ Spring Boot គាំទ្រ template engines ជាច្រើន៖ **Thymeleaf** (recommended), **JSP**, **FreeMarker**, **Mustache**, **Groovy Templates**។

### 🔹 ViewResolver Configuration (application.properties):

```properties
# Thymeleaf Configuration
spring.thymeleaf.prefix=classpath:/templates/
spring.thymeleaf.suffix=.html
spring.thymeleaf.mode=HTML
spring.thymeleaf.encoding=UTF-8
spring.thymeleaf.cache=false

# JSP Configuration (if using JSP)
spring.mvc.view.prefix=/WEB-INF/views/
spring.mvc.view.suffix=.jsp

# FreeMarker Configuration
spring.freemarker.template-loader-path=classpath:/templates/
spring.freemarker.suffix=.ftlh
```

### 🔹 Project Structure for Views:

```text
src/main/resources/
├── templates/
│   ├── index.html
│   ├── products/
│   │   ├── list.html
│   │   ├── create.html
│   │   └── edit.html
│   ├── users/
│   │   ├── list.html
│   │   └── profile.html
│   └── error/
│       ├── 404.html
│       └── 500.html
└── static/
    ├── css/
    ├── js/
    └── images/
```

## 6.4. Thymeleaf Introduction

### 📌 និយមន័យ (Definition):

**Thymeleaf** គឺជា modern server-side Java template engine ដែលត្រូវបានរចនាឡើងសម្រាប់ web applications។ វាអនុញ្ញាតឱ្យអ្នកបង្កើត dynamic HTML pages ដោយប្រើ natural templates (templates ដែលអាចមើលបានក្នុង browser ដោយមិនបាច់ run server)។

### 🔹 ការបន្ថែម Thymeleaf Dependency (pom.xml):

```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-thymeleaf</artifactId>
</dependency>
```

### 🔹 Common Thymeleaf Attributes:

| Attribute | Description | Example |
| --- | --- | --- |
| th:text | Set text content | <p th:text="${user.name}"></p> |
| th:each | Iterate over collection | <tr th:each="item : ${list}"> |
| th:if | Conditional render | <div th:if="${user.active}"> |
| th:unless | Opposite of th:if | <div th:unless="${user.active}"> |
| th:href | Set href attribute | <a th:href="@{/users/{id}}">Link</a> |
| th:src | Set src attribute | <img th:src="@{/images/logo.png}"> |
| th:action | Set form action | <form th:action="@{/users/save}" th:object="${user}"> |
| th:field | Bind input field | <input type="text" th:field="*{name}"> |
| th:value | Set value attribute | <input th:value="${user.name}"> |
| th:switch/th:case | Switch statement | <div th:switch="${user.role}"> |

## 6.5. Form Handling (ការគ្រប់គ្រងទម្រង់)

### 📌 និយមន័យ (Definition):

**Form Handling** គឺជាដំណើរការនៃការទទួល (receive), ផ្ទៀងផ្ទាត់ (validate), និងដំណើរការ (process) data ពី HTML forms។ Spring MVC ផ្តល់ @ModelAttribute ដើម្បី bind form fields ទៅកាន់ Java objects ដោយស្វ័យប្រវត្តិ។

```java
import org.springframework.stereotype.Controller;
import org.springframework.ui.Model;
import org.springframework.web.bind.annotation.*;

@Controller
@RequestMapping("/users")
public class UserFormController {

    @Autowired
    private UserService userService;

    // Show form for creating new user
    @GetMapping("/register")
    public String showRegistrationForm(Model model) {
        model.addAttribute("user", new UserDto());
        return "users/register";
    }

    // Process registration form submission
    @PostMapping("/register")
    public String registerUser(@ModelAttribute("user") UserDto userDto,
```

BindingResult result,

```java
                               Model model) {
        if (result.hasErrors()) {
            return "users/register";
        }
        userService.register(userDto);
        return "redirect:/users/login";
    }

    // Show edit form with pre-filled data
    @GetMapping("/edit/{id}")
    public String showEditForm(@PathVariable Long id, Model model) {
        User user = userService.findById(id);
        model.addAttribute("user", user);
        return "users/edit";
    }

    // Process edit form
    @PostMapping("/update/{id}")
    public String updateUser(@PathVariable Long id,
                             @ModelAttribute User user,
                             BindingResult result) {
        if (result.hasErrors()) {
            return "users/edit";
        }
        userService.update(id, user);
        return "redirect:/users";
    }
}
```

## 6.6. Validation (ការផ្ទៀងផ្ទាត់)

### 📌 និយមន័យ (Definition):

**Validation** គឺជាការពិនិត្យមើលថាទិន្នន័យដែលបានបញ្ចូល (user input) គោរពតាមច្បាប់ដែលបានកំណត់ (rules)។ Spring Boot គាំទ្រ Bean Validation (JSR-303) តាមរយៈ annotations ដូចជា @NotNull, @Size, @Email, @Pattern ។ល។

```java
import javax.validation.Valid;
import org.springframework.validation.BindingResult;
import org.springframework.web.bind.annotation.*;

@Controller
@RequestMapping("/products")
public class ProductValidationController {

    @Autowired
    private ProductService productService;

    @PostMapping("/save")
    public String saveProduct(@Valid @ModelAttribute Product product,
```

BindingResult result,

```java
                              Model model) {
        if (result.hasErrors()) {
            return "products/form";
        }
        productService.save(product);
        return "redirect:/products";
    }
}

// Entity with validation annotations
@Entity
public class Product {
    @Id
    @GeneratedValue
    private Long id;

    @NotBlank(message = "Product name is required")
    @Size(min = 3, max = 100, message = "Product name must be between 3 and 100 characters")
    private String name;

    @NotNull(message = "Price is required")
    @DecimalMin(value = "0.01", message = "Price must be at least 0.01")
    @DecimalMax(value = "99999.99", message = "Price cannot exceed 99999.99")
    private Double price;

    @Min(value = 0, message = "Quantity cannot be negative")
    @Max(value = 10000, message = "Quantity cannot exceed 10000")
    private Integer quantity;
}
```

## 6.7. Redirect and Forward (ការបញ្ជូនបន្ត)

### 📌 និយមន័យ (Definition):

**Redirect** ប្រាប់ browser ឱ្យផ្ញើ request ថ្មីទៅកាន់ URL ផ្សេង (client-side redirect) — បណ្តាលឱ្យ URL ផ្លាស់ប្តូរក្នុង browser។**Forward** គឺជា server-side transfer ដែលបញ្ជូន request ទៅកាន់ resource ផ្សេងទៀតក្នុង server ដដែល — URL មិនផ្លាស់ប្តូរទេ។

```java
@PostMapping("/save")
public String saveProduct(Product product) {
    productService.save(product);
    // Redirect
    return "redirect:/products";
}

// Redirect with flash attributes
@PostMapping("/create")
public String create(User user, RedirectAttributes ra) {
    userService.save(user);
    ra.addFlashAttribute("message", "User created!");
    return "redirect:/users";
}

// Forward
@GetMapping("/details")
public String showDetails(Model model) {
    return "forward:/api/user/data";
}
```

## 6.8. Template Layout (ការរៀបចំទំព័រ)

### 📌 និយមន័យ (Definition):

**Template Layout** គឺជាការប្រើប្រាស់ fragments (ផ្នែក) ដូចគ្នាសម្រាប់ទំព័រជាច្រើន — header, footer, navigation, sidebar។ Thymeleaf ផ្តល់ **th:replace**, **th:insert** សម្រាប់ប្រើប្រាស់ fragments ឡើងវិញ។

```text
<!-- layout.html -->
```

<!DOCTYPE html>

```text
<html xmlns:th="http://www.thymeleaf.org">
<head>
    <title th:text="">My Application</title>
</head>
<body>
    <div th:replace="fragments/header :: header"></div>
    <div th:replace="fragments/nav :: nav"></div>
    <main>
        <div th:replace="~{::content}"></div>
    </main>
    <div th:replace="fragments/footer :: footer"></div>
</body>
</html>

<!-- Child page -->
<html th:replace="~{layout :: layout}">
<body>
    <div th:fragment="content">
        <h2>Product List</h2>
        <!-- page content -->
    </div>
</body>
</html>
```

## 6.9. Static Resources (CSS, JS, Images)

### 📌 និយមន័យ (Definition):

**Static Resources** គឺជាឯកសារដែលបម្រើដោយផ្ទាល់ទៅកាន់ client ដោយមិនឆ្លងកាត់ controller — CSS, JavaScript, images, fonts, etc. Spring Boot បម្រើ static resources ដោយស្វ័យប្រវត្តិពីទីតាំង /static, /public, /resources។

### 🔹 Default Static Resource Locations:

```text
src/main/resources/static/ (recommended)
src/main/resources/public/
src/main/resources/resources/
<!-- Accessing static resources in Thymeleaf -->
<link rel="stylesheet" th:href="@{/css/style.css}">
<script th:src="@{/js/custom.js}"></script>
<img th:src="@{/images/logo.png}" alt="Logo">
```

## 6.10. Error Pages (ទំព័រកំហុស)

### 📌 និយមន័យ (Definition):

**Error Pages** គឺជា custom HTML pages ដែលបង្ហាញនៅពេលមានកំហុសកើតឡើង (404 Not Found, 500 Internal Server Error, etc.)។ Spring Boot ផ្តល់ default error handling ប៉ុន្តែអ្នកអាច customize error pages ដោយបង្កើត HTML files ក្នុង templates/error/ folder។

### 🔹 Project Structure for Error Pages:

```text
src/main/resources/templates/error/
├── 404.html          # Not Found
├── 400.html          # Bad Request
├── 403.html          # Forbidden
├── 500.html          # Internal Server Error
└── error.html        # Generic error page
<!-- error/404.html -->
```

<!DOCTYPE html>

```java
<html>
<head>
    <title>404 - Page Not Found</title>
</head>
<body>
    <h1>404 - Page Not Found</h1>
    <p>The page you are looking for does not exist.</p>
    <a href="/">Return to Home</a>
</body>
</html>
// Global Exception Handler
@ControllerAdvice
public class GlobalExceptionHandler {

    @ExceptionHandler(ResourceNotFoundException.class)
    public ModelAndView handleNotFound(ResourceNotFoundException ex) {
        ModelAndView mav = new ModelAndView("error/404");
        mav.addObject("message", ex.getMessage());
        return mav;
    }

    @ExceptionHandler(Exception.class)
    public ModelAndView handleGeneric(Exception ex) {
        ModelAndView mav = new ModelAndView("error/500");
        mav.addObject("message", ex.getMessage());
        return mav;
    }
}
```

### 📚 សង្ខេបមេរៀនទី៦ (Module 6 Summary)

នៅក្នុងមេរៀននេះ អ្នកបានរៀនអំពី Spring Boot MVC និងការបង្កើត web applications៖

- **MVC Architecture** – Model (data), View (UI), Controller (logic)

```text
@Controller – Handle web requests and return view names
```

- **Views** – Templates (Thymeleaf) for displaying data

- **Thymeleaf** – Modern template engine with natural templates

- **Form Handling** – @ModelAttribute for binding form data

- **Validation** – Bean Validation (@NotNull, @Size, @Email)

- **Redirect & Forward** – Client-side redirect vs server-side forward

- **Template Layout** – Reusable fragments (header, footer, nav)

- **Static Resources** – CSS, JS, images from /static folder

- **Error Pages** – Custom 404, 500 pages, @ControllerAdvice

# មេរៀនទី៧: Database Integration (ការភ្ជាប់ប្រព័ន្ធទិន្នន័យ)

### 📖 សេចក្តីផ្តើម (Introduction):
Database Integration គឺជាផ្នែកសំខាន់មួយក្នុងការអភិវឌ្ឍន៍កម្មវិធី Spring Boot ដើម្បីរក្សាទុកទិន្នន័យជាអចិន្ត្រៃយ៍ (persist data)។ មេរៀននេះនឹងបង្រៀនអ្នកពី Introduction to Databases, SQL Basics, MySQL/PostgreSQL Setup, JDBC, Spring Data JPA, Hibernate ORM, Entity Class, Repository Interface, CRUD Repository, JpaRepository, Relationships (One-to-One, One-to-Many, Many-to-Many), Lazy vs Eager Loading, និង Transactions។

## 7.1. សេចក្តីផ្តើមអំពីប្រព័ន្ធទិន្នន័យ (Introduction to Databases)

### 📌 និយមន័យ (Definition):

**Database** គឺជាកន្លែងផ្ទុកទិន្នន័យដែលមានរចនាសម្ព័ន្ធ (organized collection of data) ដែលអនុញ្ញាតឱ្យយើង បញ្ចូល (insert), ទាញយក (retrieve), ធ្វើបច្ចុប្បន្នភាព (update), និងលុប (delete) ទិន្នន័យបានយ៉ាងមានប្រសិទ្ធភាព។

### 🔹 ប្រភេទនៃ Databases (Types of Databases):

**SQL Databases (Relational)**

- MySQL

- PostgreSQL

- Oracle

- Microsoft SQL Server

- H2 (in-memory for testing)

**NoSQL Databases (Non-Relational)**

- MongoDB (Document)

- Redis (Key-Value)

- Cassandra (Column)

- Neo4j (Graph)

### 💡 Why Use Database in Spring Boot?

- **Data Persistence** – ទិន្នន័យមិនបាត់នៅពេលកម្មវិធីបិទ

- **Data Sharing** – អ្នកប្រើប្រាស់ច្រើនអាចចូលដំណើរការទិន្នន័យដូចគ្នា

- **Data Integrity** – ការពារទិន្នន័យមិនឱ្យមានភាពមិនត្រឹមត្រូវ

- **Data Security** – គ្រប់គ្រងការចូលដំណើរការទិន្នន័យ

- **Scalability** – អាចពង្រីកបាននៅពេលទិន្នន័យកើនឡើង

## 7.2. មូលដ្ឋានគ្រឹះ SQL (SQL Basics)

### 📌 និយមន័យ (Definition):

**SQL (Structured Query Language)** គឺជាភាសាស្តង់ដារសម្រាប់ធ្វើការជាមួយ Relational Databases។ វាត្រូវបានប្រើសម្រាប់ CRUD Operations (Create, Read, Update, Delete)។

### 🔹 SQL Commands សំខាន់ៗ:

| Category | Command | Description | Example |
| --- | --- | --- | --- |
| DDL | CREATE, ALTER, DROP | Define database schema | CREATE TABLE users (...) |
| DML | INSERT, UPDATE, DELETE | Manipulate data | INSERT INTO users VALUES (...) |
| DQL | SELECT | Query data | SELECT * FROM users |
| DCL | GRANT, REVOKE | Control permissions | GRANT SELECT ON users TO user |

-- CREATE TABLE (បង្កើតតារាង)

CREATE TABLE users (

id BIGINT PRIMARY KEY AUTO_INCREMENT,

username VARCHAR(50) NOT NULL UNIQUE,

email VARCHAR(100) NOT NULL UNIQUE,

age INT,

created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP

```text
);
```

-- INSERT (បញ្ចូលទិន្នន័យ)

INSERT INTO users (username, email, age)

```text
VALUES ('sokdara', 'sok@example.com', 25);
```

-- SELECT (ទាញយកទិន្នន័យ)

```text
SELECT * FROM users;
SELECT id, username, email FROM users WHERE age > 18;
SELECT * FROM users ORDER BY created_at DESC LIMIT 10;
```

-- UPDATE (ធ្វើបច្ចុប្បន្នភាព)

```text
UPDATE users SET age = 26 WHERE username = 'sokdara';
```

-- DELETE (លុបទិន្នន័យ)

```text
DELETE FROM users WHERE id = 1;
```

-- JOIN (ភ្ជាប់តារាង)

SELECT u.username, o.order_date, o.total_amount

FROM users u

```text
INNER JOIN orders o ON u.id = o.user_id;
```

## 7.3. MySQL Installation (ការដំឡើង MySQL)

### 📌 MySQL ជាអ្វី? (What is MySQL?):

**MySQL** គឺជា Open-source Relational Database Management System (RDBMS) ដ៏ពេញនិយមបំផុតមួយ ដែលប្រើ SQL សម្រាប់គ្រប់គ្រងទិន្នន័យ។ វាត្រូវបានប្រើប្រាស់យ៉ាងទូលំទូលាយជាមួយ Spring Boot។

### 🔹 ជំហានដំឡើង MySQL (Windows/macOS/Linux):

1. ទាញយក MySQL Installer ពី [dev.mysql.com](https://dev.mysql.com/downloads/installer/)

2. ដំណើរការ installer ហើយជ្រើសរើស "Developer Default"

3. កំណត់ root password (ចងចាំពាក្យសម្ងាត់នេះ!)

4. ជ្រើសរើស port (default: 3306)

5. បញ្ចប់ការដំឡើង

### 🔹 Basic MySQL Commands:

-- Login to MySQL

mysql -u root -p

-- Show all databases

```text
SHOW DATABASES;
```

-- Create new database

```text
CREATE DATABASE springboot_db;
```

-- Use database

```text
USE springboot_db;
```

-- Show all tables

```text
SHOW TABLES;
```

-- Exit MySQL

```text
EXIT;
```

## 7.4. PostgreSQL Setup (ការដំឡើង PostgreSQL)

### 📌 PostgreSQL ជាអ្វី? (What is PostgreSQL?):

**PostgreSQL** គឺជា Advanced Open-source Relational Database ដែលមានលក្ខណៈពិសេសច្រើន និងគាំទ្រ JSON, Array, និង Full-text search។ វាត្រូវបានប្រើប្រាស់ក្នុងកម្មវិធីធំៗជាច្រើន។

### 🔹 ជំហានដំឡើង PostgreSQL:

1. ទាញយក PostgreSQL ពី [postgresql.org](https://www.postgresql.org/download/)

2. ដំណើរការ installer ហើយកំណត់ password for postgres user

3. កំណត់ port (default: 5432)

4. បញ្ចប់ការដំឡើង

-- Connect to PostgreSQL

psql -U postgres

-- Create database

```text
CREATE DATABASE springboot_db;
```

-- List databases

l

-- Connect to database

```text
c springboot_db;
```

-- List tables

dt

-- Exit

q

## 7.5. Connecting Database (ការភ្ជាប់ប្រព័ន្ធទិន្នន័យ)

### 📌 Database Connection ក្នុង Spring Boot:

Spring Boot អនុញ្ញាតឱ្យយើងភ្ជាប់ database យ៉ាងងាយស្រួលតាមរយៈ configuration ក្នុង application.propertiesឬ application.yml។

### 🔹 Maven Dependencies (pom.xml):

```xml
<!-- Spring Data JPA -->
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-data-jpa</artifactId>
</dependency>

<!-- MySQL Driver -->
<dependency>
    <groupId>com.mysql</groupId>
    <artifactId>mysql-connector-j</artifactId>
    <scope>runtime</scope>
</dependency>

<!-- PostgreSQL Driver -->
<dependency>
    <groupId>org.postgresql</groupId>
    <artifactId>postgresql</artifactId>
    <scope>runtime</scope>
</dependency>

<!-- H2 Database (for testing) -->
<dependency>
    <groupId>com.h2database</groupId>
    <artifactId>h2</artifactId>
    <scope>runtime</scope>
</dependency>
```

### 🔹 MySQL Connection Configuration (application.properties):

```properties
# MySQL Configuration
spring.datasource.url=jdbc:mysql://localhost:3306/springboot_db?useSSL=false&serverTimezone=UTC
spring.datasource.username=root
spring.datasource.password=yourpassword
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver

# Connection Pool (HikariCP)
spring.datasource.hikari.maximum-pool-size=10
spring.datasource.hikari.minimum-idle=5

# JPA Configuration
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.format_sql=true
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQL8Dialect
```

### 🔹 PostgreSQL Connection Configuration:

```properties
# PostgreSQL Configuration
spring.datasource.url=jdbc:postgresql://localhost:5432/springboot_db
spring.datasource.username=postgres
spring.datasource.password=yourpassword
spring.datasource.driver-class-name=org.postgresql.Driver

# JPA Configuration
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.format_sql=true
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.PostgreSQLDialect
```

### 🔹 H2 Database (In-Memory for Testing):

```properties
# H2 Database Configuration
spring.datasource.url=jdbc:h2:mem:testdb
spring.datasource.driver-class-name=org.h2.Driver
spring.datasource.username=sa
spring.datasource.password=

# H2 Console
spring.h2.console.enabled=true
spring.h2.console.path=/h2-console

# JPA Configuration
spring.jpa.database-platform=org.hibernate.dialect.H2Dialect
```

## 7.6. JDBC Basics (មូលដ្ឋាន JDBC)

### 📌 និយមន័យ (Definition):

**JDBC (Java Database Connectivity)** គឺជា API ស្តង់ដារក្នុង Java សម្រាប់ភ្ជាប់ និងធ្វើការជាមួយ databases។ Spring Boot ប្រើ JDBC នៅក្រោមកម្រិត (low-level) ប៉ុន្តែយើងអាចប្រើ JdbcTemplate ដើម្បីងាយស្រួលជាង។

```java
import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.jdbc.core.JdbcTemplate;
import org.springframework.jdbc.core.RowMapper;
import org.springframework.stereotype.Repository;
import java.sql.ResultSet;
import java.sql.SQLException;
import java.util.List;

@Repository
public class UserDao {

    @Autowired
    private JdbcTemplate jdbcTemplate;

    // INSERT
    public int save(User user) {
        String sql = "INSERT INTO users (name, email, age) VALUES (?, ?, ?)";
        return jdbcTemplate.update(sql, user.getName(), user.getEmail(), user.getAge());
    }

    // SELECT - Single
    public User findById(Long id) {
        String sql = "SELECT * FROM users WHERE id = ?";
        return jdbcTemplate.queryForObject(sql, new UserRowMapper(), id);
    }

    // SELECT - All
    public List<User> findAll() {
        String sql = "SELECT * FROM users";
        return jdbcTemplate.query(sql, new UserRowMapper());
    }

    // UPDATE
    public int update(User user) {
        String sql = "UPDATE users SET name = ?, email = ?, age = ? WHERE id = ?";
        return jdbcTemplate.update(sql, user.getName(), user.getEmail(), user.getAge(), user.getId());
    }

    // DELETE
    public int deleteById(Long id) {
        String sql = "DELETE FROM users WHERE id = ?";
        return jdbcTemplate.update(sql, id);
    }

    // RowMapper Implementation
    private static class UserRowMapper implements RowMapper<User> {
        @Override
        public User mapRow(ResultSet rs, int rowNum) throws SQLException {
            User user = new User();
            user.setId(rs.getLong("id"));
            user.setName(rs.getString("name"));
            user.setEmail(rs.getString("email"));
            user.setAge(rs.getInt("age"));
            return user;
        }
    }
}
```

## 7.7. Spring Data JPA

### 📌 និយមន័យ (Definition):

**Spring Data JPA** គឺជា module មួយរបស់ Spring Data ដែលធ្វើឱ្យការចូលដំណើរការទិន្នន័យកាន់តែងាយស្រួល ដោយប្រើ JPA (Java Persistence API)។ វាកាត់បន្ថយកូដ boilerplate និងផ្តល់ Repository implementation ដោយស្វ័យប្រវត្តិ។

### 🔹 Spring Data JPA Features:

- **Repository Interface** – CrudRepository, JpaRepository, PagingAndSortingRepository

- **Query Methods** – findBy... , findAllBy... , deleteBy... (method naming convention)

```text
@Query Annotation – Custom JPQL or native SQL queries
```

- **Pagination & Sorting** – Pageable, Sort, Page, PageRequest

- **Auditing** – @CreatedDate, @LastModifiedDate, @CreatedBy, @LastModifiedBy

- **Entity Mapping** – @Entity, @Table, @Id, @GeneratedValue, @Column, @OneToMany, etc.

### 💡 Benefits of Spring Data JPA:

- មិនចាំបាច់សរសេរ SQL queries ដោយដៃ (for basic operations)

- កាត់បន្ថយកូដយ៉ាងច្រើន (no need for DAO implementation)

- គាំទ្រ pagination and sorting ដោយស្វ័យប្រវត្តិ

- គាំទ្រ caching (second-level cache, query cache)

- ងាយស្រួលក្នុងការធ្វើតេស្ត (testing)

## 7.8. Hibernate ORM

### 📌 និយមន័យ (Definition):

**Hibernate** គឺជា ORM (Object-Relational Mapping) framework ដែលបំលែង Java objects ទៅជា database tables និងបញ្ច្រាស់ (vice versa)។ Spring Boot ប្រើ Hibernate ជា default JPA implementation។

### 🔹 Hibernate Concepts:

**Entity**

Java class mapped to database table (@Entity)

**Session / EntityManager**

Interface for database operations

**Transaction**

Unit of work (@Transactional)

**HQL / JPQL**

Object-oriented query language

```properties
// Hibernate configuration properties
# DDL Auto (Schema generation)
# validate: validates schema, no changes
# update: updates schema if needed
# create: creates schema (drops existing)
# create-drop: creates schema, drops on app shutdown
spring.jpa.hibernate.ddl-auto=update

# Show SQL
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.format_sql=true

# Batch operations
spring.jpa.properties.hibernate.jdbc.batch_size=20
spring.jpa.properties.hibernate.order_inserts=true
spring.jpa.properties.hibernate.order_updates=true
```

## 7.9. Entity Class (ថ្នាក់ Entity)

### 📌 និយមន័យ (Definition):

**Entity** គឺជា Java class ដែលត្រូវបាន map ទៅកាន់ database table។ Entity class ត្រូវបាន annotated ដោយ @Entity ហើយ fields ត្រូវបាន map ទៅ columns។

```properties
import javax.persistence.*;
import java.time.LocalDateTime;

@Entity
@Table(name = "users")  // Table name (default: class name)
public class User {

    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)  // Auto-increment
    private Long id;

    @Column(nullable = false, length = 50)
    private String name;

    @Column(unique = true, nullable = false)
    private String email;

    @Column(name = "user_age")  // Custom column name
    private Integer age;

    @Column(updatable = false)
    private LocalDateTime createdAt;

    @Transient  // This field will NOT be persisted
    private String temporaryData;

    // Constructors
    public User() {}  // Required by JPA

    public User(String name, String email) {
        this.name = name;
        this.email = email;
    }

    // Getters and Setters
    // ...
}
```

### 🔹 Common JPA Annotations:

| Annotation | Description |
| --- | --- |
| @Entity | Marks class as JPA entity |
| @Table(name = "...") | Specifies table name |
| @Id | Primary key |
| @GeneratedValue | Auto-generate primary key value |
| @Column | Maps field to column |
| @Transient | Field not persisted |
| @Lob | Large Object (BLOB, CLOB) |
| @Enumerated | Maps enum type |
| @Temporal | Maps date/time |

## 7.10. Repository Interface

### 📌 និយមន័យ (Definition):

**Repository Interface** គឺជា interface ដែល Spring Data JPA ប្រើដើម្បីបង្កើត implementation សម្រាប់ database operations ដោយស្វ័យប្រវត្តិ។ យើងគ្រាន់តែ extends JpaRepositoryឬ CrudRepository ហើយ Spring នឹងបង្កើត bean ដោយស្វ័យប្រវត្តិ។

```java
import org.springframework.data.jpa.repository.JpaRepository;
import org.springframework.data.repository.CrudRepository;
import org.springframework.stereotype.Repository;
import java.util.List;
import java.util.Optional;

@Repository
public interface UserRepository extends JpaRepository<User, Long> {

    // Derived query methods (Spring Data JPA will implement automatically)

    // Find by field
    Optional<User> findByEmail(String email);

    // Find by field (multiple results)
    List<User> findByName(String name);

    // Find by field containing (LIKE query)
    List<User> findByNameContaining(String keyword);

    // Find with multiple conditions (AND)
    List<User> findByNameAndAge(String name, Integer age);

    // Find with multiple conditions (OR)
    List<User> findByNameOrEmail(String name, String email);

    // Find by field with ordering
    List<User> findAllByOrderByNameAsc();
    List<User> findAllByOrderByCreatedAtDesc();

    // Count
    long countByAgeGreaterThan(int age);

    // Exists
    boolean existsByEmail(String email);

    // Delete
    void deleteByEmail(String email);

    // Top/Limit
    List<User> findTop3ByOrderByIdDesc();
}
```

## 7.11. CRUD Repository

### 📌 CrudRepository Interface:

**CrudRepository** គឺជា interface មូលដ្ឋានសម្រាប់ generic CRUD operations។ វាផ្តល់ methods មូលដ្ឋានដូចជា save, findById, findAll, delete ជាដើម។

```java
import org.springframework.data.repository.CrudRepository;

@Repository
public interface ProductRepository extends CrudRepository<Product, Long> {
    // CrudRepository provides these methods automatically:
    // - <S extends T> S save(S entity)
    // - Optional<T> findById(ID id)
    // - Iterable<T> findAll()
    // - Iterable<T> findAllById(Iterable<ID> ids)
    // - long count()
    // - void deleteById(ID id)
    // - void delete(T entity)
    // - void deleteAll()
    // - boolean existsById(ID id)
}

// Usage in Service
@Service
public class ProductService {

    @Autowired
    private ProductRepository productRepository;

    public Product createProduct(Product product) {
        return productRepository.save(product);
    }

    public Optional<Product> getProduct(Long id) {
        return productRepository.findById(id);
    }

    public Iterable<Product> getAllProducts() {
        return productRepository.findAll();
    }

    public void deleteProduct(Long id) {
        productRepository.deleteById(id);
    }
}
```

## 7.12. JpaRepository

### 📌 JpaRepository Interface:

**JpaRepository** គឺជា extension នៃ CrudRepository និង PagingAndSortingRepository។ វាបន្ថែម methods សម្រាប់ pagination, sorting, batch operations, flush, និង JPA-specific features។

```java
import org.springframework.data.jpa.repository.JpaRepository;
import org.springframework.data.domain.Page;
import org.springframework.data.domain.Pageable;
import org.springframework.data.domain.Sort;

@Repository
public interface UserRepository extends JpaRepository<User, Long> {

    // Pagination
    Page<User> findByAgeGreaterThan(int age, Pageable pageable);

    // Sorting
    List<User> findByAgeGreaterThan(int age, Sort sort);

    // Custom query with JPQL
    @Query("SELECT u FROM User u WHERE u.email LIKE %:domain")
    List<User> findByEmailDomain(@Param("domain") String domain);

    // Native SQL query
    @Query(value = "SELECT * FROM users WHERE age > :minAge", nativeQuery = true)
    List<User> findUsersByAgeNative(@Param("minAge") int minAge);

    // Update query
    @Modifying
    @Query("UPDATE User u SET u.age = :age WHERE u.id = :id")
    int updateUserAge(@Param("id") Long id, @Param("age") int age);
}

// Usage with Pagination
@Service
public class UserService {

    @Autowired
    private UserRepository userRepository;

    public Page<User> getUsersByAge(int age, int page, int size) {
        Pageable pageable = PageRequest.of(page, size, Sort.by("name").ascending());
        return userRepository.findByAgeGreaterThan(age, pageable);
    }
}
```

## 7.13. Relationships (ទំនាក់ទំនងក្នុង Database)

### 📌 ប្រភេទទំនាក់ទំនង (Types of Relationships):

នៅក្នុង Relational Databases, មានទំនាក់ទំនង ៣ ប្រភេទសំខាន់ៗ៖ One-to-One, One-to-Many, Many-to-Many។

## 7.14. One-to-One Relationship (@OneToOne)

### 📌 One-to-One Relationship:

One-to-One មានន័យថា record នីមួយៗក្នុងតារាង A ភ្ជាប់នឹង record តែមួយក្នុងតារាង B។ ឧទាហរណ៍: User ↔ Address (អ្នកប្រើប្រាស់ម្នាក់មានអាសយដ្ឋានតែមួយ)។

```java
// User Entity (Owner side)
@Entity
@Table(name = "users")
public class User {
    @Id
    @GeneratedValue
    private Long id;
    private String name;

    @OneToOne(cascade = CascadeType.ALL, fetch = FetchType.LAZY)
    @JoinColumn(name = "address_id", referencedColumnName = "id")
    private Address address;

    // getters and setters
}

// Address Entity (Inverse side)
@Entity
@Table(name = "addresses")
public class Address {
    @Id
    @GeneratedValue
    private Long id;
    private String street;
    private String city;
    private String zipCode;

    @OneToOne(mappedBy = "address")
    private User user;

    // getters and setters
}

// Usage
User user = new User();
user.setName("Sok Dara");

Address address = new Address();
address.setStreet("123 Main St");
address.setCity("Phnom Penh");

user.setAddress(address);  // Cascading will save both

userRepository.save(user);
```

## 7.15. One-to-Many Relationship (@OneToMany)

### 📌 One-to-Many Relationship:

One-to-Many មានន័យថា record មួយក្នុងតារាង A អាចភ្ជាប់នឹង records ច្រើនក្នុងតារាង B។ ឧទាហរណ៍: User ↔ Order (អ្នកប្រើប្រាស់ម្នាក់អាចមានការបញ្ជាទិញច្រើន)។

```java
// User Entity (One side)
@Entity
@Table(name = "users")
public class User {
    @Id
    @GeneratedValue
    private Long id;
    private String name;

    @OneToMany(mappedBy = "user", cascade = CascadeType.ALL, fetch = FetchType.LAZY)
    private List<Order> orders = new ArrayList<>();

    // Helper methods
    public void addOrder(Order order) {
        orders.add(order);
        order.setUser(this);
    }

    public void removeOrder(Order order) {
        orders.remove(order);
        order.setUser(null);
    }
}

// Order Entity (Many side)
@Entity
@Table(name = "orders")
public class Order {
    @Id
    @GeneratedValue
    private Long id;
    private String orderNumber;
    private Double totalAmount;

    @ManyToOne
    @JoinColumn(name = "user_id")
    private User user;
}

// Usage
User user = new User();
user.setName("Sok Dara");

Order order1 = new Order();
order1.setOrderNumber("ORD-001");
order1.setTotalAmount(100.0);

Order order2 = new Order();
order2.setOrderNumber("ORD-002");
order2.setTotalAmount(200.0);

user.addOrder(order1);
user.addOrder(order2);

userRepository.save(user);  // Saves user and both orders
```

## 7.16. Many-to-Many Relationship (@ManyToMany)

### 📌 Many-to-Many Relationship:

Many-to-Many មានន័យថា records ក្នុងតារាង A អាចភ្ជាប់នឹង records ច្រើនក្នុងតារាង B ហើយបញ្ច្រាស់។ ឧទាហរណ៍: Student ↔ Course (សិស្សម្នាក់អាចចុះឈ្មោះមុខវិជ្ជាច្រើន, មុខវិជ្ជាមួយអាចមានសិស្សច្រើន)។

```properties
// Student Entity
@Entity
@Table(name = "students")
public class Student {
    @Id
    @GeneratedValue
    private Long id;
    private String name;

    @ManyToMany
    @JoinTable(
        name = "student_courses",
        joinColumns = @JoinColumn(name = "student_id"),
        inverseJoinColumns = @JoinColumn(name = "course_id")
```

)

```java
    private Set<Course> courses = new HashSet<>();
}

// Course Entity
@Entity
@Table(name = "courses")
public class Course {
    @Id
    @GeneratedValue
    private Long id;
    private String title;

    @ManyToMany(mappedBy = "courses")
    private Set<Student> students = new HashSet<>();
}

// Usage
Student student1 = new Student();
student1.setName("Sok Dara");

Student student2 = new Student();
student2.setName("Cheata");

Course course1 = new Course();
course1.setTitle("Java Programming");

Course course2 = new Course();
course2.setTitle("Spring Boot");

student1.getCourses().add(course1);
student1.getCourses().add(course2);
student2.getCourses().add(course1);

studentRepository.save(student1);
studentRepository.save(student2);
```

## 7.17. Lazy vs Eager Loading

### 📌 និយមន័យ (Definition):

**Lazy Loading** - ទិន្នន័យដែលទាក់ទង (related data) ត្រូវបានផ្ទុកតែនៅពេលដែលគេចូលប្រើ (access) ប៉ុណ្ណោះ។
**Eager Loading** - ទិន្នន័យដែលទាក់ទងត្រូវបានផ្ទុកភ្លាមៗជាមួយ parent entity (ដោយប្រើ JOIN)។

**LAZY (Default for @OneToMany, @ManyToMany)**

```java
@OneToMany(fetch = FetchType.LAZY)
private List<Order> orders;

// Data loaded only when accessed
User user = userRepository.findById(1L);
// orders NOT loaded yet
List<Order> orders = user.getOrders();
// orders loaded NOW (additional query)
```

**EAGER (Default for @ManyToOne, @OneToOne)**

```java
@ManyToOne(fetch = FetchType.EAGER)
private User user;

// Data loaded immediately with main query
Order order = orderRepository.findById(1L);
// user already loaded (JOIN query)
```

### 💡 Best Practices:

- ប្រើ **LAZY** សម្រាប់ associations ភាគច្រើន (ដើម្បីបង្កើនប្រសិទ្ធភាព)

- ប្រើ **EAGER** តែពេលដែលអ្នកត្រូវការ related data គ្រប់ពេល

- ដើម្បីជៀសវាង LazyInitializationException, ប្រើ @Transactional ឬ JOIN FETCH in JPQL

- ប្រើ @EntityGraph ដើម្បី control loading strategy

## 7.18. Transactions (@Transactional)

### 📌 និយមន័យ (Definition):

**Transaction** គឺជា unit of work ដែលធានាថា operations ទាំងអស់ក្នុង transaction ត្រូវបានអនុវត្ត (commit) ឬមិនអនុវត្តទាំងអស់ (rollback) ប្រសិនបើមានកំហុស។ Spring ប្រើ @Transactionalannotation ដើម្បីគ្រប់គ្រង transactions។

```properties
import org.springframework.stereotype.Service;
import org.springframework.transaction.annotation.Transactional;
import org.springframework.transaction.annotation.Propagation;
import org.springframework.transaction.annotation.Isolation;

@Service
public class BankService {

    @Autowired
    private AccountRepository accountRepository;

    // Basic transaction
    @Transactional
    public void transferMoney(Long fromId, Long toId, Double amount) {
        Account from = accountRepository.findById(fromId).orElseThrow();
        Account to = accountRepository.findById(toId).orElseThrow();

        from.setBalance(from.getBalance() - amount);
        to.setBalance(to.getBalance() + amount);

        accountRepository.save(from);
        accountRepository.save(to);
        // Both saved or none (if exception occurs)
    }

    // Transaction with rollback for specific exceptions
    @Transactional(rollbackFor = Exception.class)
    public void processPayment(Payment payment) throws Exception {
        // operations
        if (payment.getAmount() < 0) {
            throw new Exception("Invalid amount");
        }
    }

    // Transaction with no rollback for specific exceptions
    @Transactional(noRollbackFor = IllegalArgumentException.class)
    public void updateAccount(Account account) {
        // IllegalArgumentException won't trigger rollback
    }

    // Transaction with propagation and isolation
    @Transactional(
        propagation = Propagation.REQUIRED,
        isolation = Isolation.READ_COMMITTED,
        timeout = 30,
        readOnly = false
```

)

```text
    public void updateUser(User user) {
        // propagation: REQUIRED (uses existing or creates new)
        // isolation: READ_COMMITTED (prevents dirty reads)
        // timeout: 30 seconds
        userRepository.save(user);
    }

    // Read-only transaction (for performance)
    @Transactional(readOnly = true)
    public List<User> getAllUsers() {
        return userRepository.findAll();
    }

    // Transaction management with manual rollback
    @Transactional
    public void processOrder(Order order) {
        try {
            // operations
        } catch (Exception e) {
            TransactionAspectSupport.currentTransactionStatus().setRollbackOnly();
        }
    }
}
```

### 🔹 Transaction Propagation Levels:

| Propagation | Description |
| --- | --- |
| REQUIRED | Uses existing transaction or creates new (default) |
| REQUIRES_NEW | Always creates new transaction, suspends existing |
| SUPPORTS | Uses existing if available, else non-transactional |
| NOT_SUPPORTED | Executes non-transactionally, suspends existing |
| MANDATORY | Requires existing transaction, throws exception if none |
| NEVER | Executes non-transactionally, throws exception if transaction exists |
| NESTED | Executes within nested transaction if exists |

### 💡 Transaction Best Practices:

- ដាក់ @Transactional នៅ Service Layer (មិនមែន Controller)

- ប្រើ readOnly = true សម្រាប់ query methods ដើម្បីបង្កើនប្រសិទ្ធភាព

- កំណត់ rollbackFor សម្រាប់ checked exceptions

- ជៀសវាង @Transactional លើ private methods (Spring proxy doesn't intercept)

- យកចិត្តទុកដាក់លើ transaction propagation ពេល calling method ពី method ផ្សេងក្នុង class ដូចគ្នា

### 📚 សង្ខេបមេរៀនទី៧ (Module 7 Summary)

នៅក្នុងមេរៀននេះ អ្នកបានរៀនអំពី Database Integration ជាមួយ Spring Boot៖

- **Introduction to Databases** – SQL vs NoSQL, database types

- **SQL Basics** – DDL, DML, DQL, DCL commands

- **MySQL/PostgreSQL Setup** – Installation and configuration

- **Database Connection** – application.properties configuration for MySQL, PostgreSQL, H2

- **JDBC Basics** – JdbcTemplate, RowMapper, manual queries

- **Spring Data JPA** – Simplifies data access with repositories

- **Hibernate ORM** – Object-Relational Mapping framework

- **Entity Class** – @Entity, @Id, @Column, @Table annotations

- **Repository Interface** – Derived query methods, custom queries

- **CrudRepository vs JpaRepository** – Basic vs advanced features

- **Relationships** – @OneToOne, @OneToMany, @ManyToMany with examples

- **Lazy vs Eager Loading** – Performance considerations

- **Transactions** – @Transactional, propagation, isolation, rollback

# មេរៀនទី៨: Advanced JPA & Hibernate (JPA និង Hibernate កម្រិតខ្ពស់)

### 📖 សេចក្តីផ្តើម (Introduction):
មេរៀននេះនឹងបង្រៀនអ្នកអំពីលក្ខណៈពិសេសកម្រិតខ្ពស់របស់ JPA និង Hibernate ដែលជួយឱ្យការគ្រប់គ្រងទិន្នន័យកាន់តែមានប្រសិទ្ធភាព។ អ្នកនឹងរៀនពី JPQL, Native Query, Pagination, Sorting, Auditing, Entity Lifecycle, Caching, Locking (Optimistic & Pessimistic), Performance Optimization, N+1 Query Problem, និង DTO Projection។

## 8.1. JPQL (Java Persistence Query Language)

### 📌 និយមន័យ (Definition):

**JPQL (Java Persistence Query Language)** គឺជា query language ដែលប្រើសម្រាប់ធ្វើការជាមួយ JPA entities ជំនួសឱ្យ database tables។ JPQL គឺស្រដៀងនឹង SQL ដែរ ប៉ុន្តែវាដំណើរការលើ entity objects និង entity fields (ជំនួសឱ្យ table names និង column names)។

### 💡 JPQL vs SQL:

| SQL | JPQL |
| --- | --- |
| SELECT * FROM users | SELECT u FROM User u |
| SELECT id, name FROM users | SELECT u.id, u.name FROM User u |
| FROM users WHERE age > 18 | FROM User u WHERE u.age > 18 |
| JOIN users u ON orders.user_id = u.id | JOIN u.orders o |

```java
import org.springframework.data.jpa.repository.JpaRepository;
import org.springframework.data.jpa.repository.Query;
import org.springframework.data.repository.query.Param;
import java.util.List;
import java.util.Optional;

@Repository
public interface UserRepository extends JpaRepository<User, Long> {

    // 1. Basic JPQL query
    @Query("SELECT u FROM User u WHERE u.email = :email")
    Optional<User> findByEmailJPQL(@Param("email") String email);

    // 2. JPQL with multiple conditions
    @Query("SELECT u FROM User u WHERE u.name = :name AND u.age >= :minAge")
    List<User> findByNameAndMinAge(@Param("name") String name, @Param("minAge") int minAge);

    // 3. JPQL with LIKE operator
    @Query("SELECT u FROM User u WHERE u.name LIKE %:keyword%")
    List<User> searchByName(@Param("keyword") String keyword);

    // 4. JPQL with ORDER BY
    @Query("SELECT u FROM User u ORDER BY u.createdAt DESC")
    List<User> findAllOrderByCreatedDateDesc();

    // 5. JPQL with JOIN
    @Query("SELECT u FROM User u JOIN u.orders o WHERE o.totalAmount > :amount")
    List<User> findUsersWithOrdersAbove(@Param("amount") Double amount);

    // 6. JPQL with aggregate functions
    @Query("SELECT AVG(u.age) FROM User u")
    Double getAverageAge();

    @Query("SELECT COUNT(u) FROM User u WHERE u.age > :minAge")
    Long countUsersAboveAge(@Param("minAge") int minAge);

    // 7. JPQL with GROUP BY and HAVING
    @Query("SELECT u.city, COUNT(u) FROM User u GROUP BY u.city HAVING COUNT(u) > 2")
    List<Object[]> getCityStatistics();

    // 8. JPQL with IN clause
    @Query("SELECT u FROM User u WHERE u.id IN :ids")
    List<User> findUsersByIds(@Param("ids") List<Long> ids);

    // 9. JPQL with BETWEEN
    @Query("SELECT u FROM User u WHERE u.age BETWEEN :minAge AND :maxAge")
    List<User> findUsersByAgeRange(@Param("minAge") int minAge, @Param("maxAge") int maxAge);

    // 10. JPQL with IS EMPTY
    @Query("SELECT u FROM User u WHERE u.orders IS EMPTY")
    List<User> findUsersWithNoOrders();

    // 11. JPQL with subquery
    @Query("SELECT u FROM User u WHERE u.age > (SELECT AVG(u2.age) FROM User u2)")
    List<User> findUsersAboveAverageAge();

    // 12. JPQL with constructor expression (DTO projection)
    @Query("SELECT new com.example.dto.UserDto(u.id, u.name, u.email) FROM User u WHERE u.active = true")
    List<UserDto> findActiveUserDtos();
}
```

## 8.2. Native Query (SQL សុទ្ធ)

### 📌 និយមន័យ (Definition):

**Native Query** គឺជា SQL query សុទ្ធ (plain SQL) ដែលអ្នកអាចប្រើក្នុង Spring Data JPA តាមរយៈ @Query(nativeQuery = true)។ Native query គឺល្អនៅពេលដែលអ្នកត្រូវការ database-specific features ដែល JPQL មិនគាំទ្រ។

```properties
import org.springframework.data.jpa.repository.JpaRepository;
import org.springframework.data.jpa.repository.Modifying;
import org.springframework.data.jpa.repository.Query;
import org.springframework.data.repository.query.Param;
import org.springframework.transaction.annotation.Transactional;
import java.util.List;
import java.util.Map;

@Repository
public interface UserRepository extends JpaRepository<User, Long> {

    // 1. Basic native query
    @Query(value = "SELECT * FROM users WHERE email = :email", nativeQuery = true)
    Optional<User> findByEmailNative(@Param("email") String email);

    // 2. Native query with multiple parameters
    @Query(value = "SELECT * FROM users WHERE name = :name AND age >= :minAge", nativeQuery = true)
    List<User> findByNameAndMinAgeNative(@Param("name") String name, @Param("minAge") int minAge);

    // 3. Native query with LIKE
    @Query(value = "SELECT * FROM users WHERE name LIKE CONCAT('%', :keyword, '%')", nativeQuery = true)
    List<User> searchByNameNative(@Param("keyword") String keyword);

    // 4. Native query with ORDER BY
    @Query(value = "SELECT * FROM users ORDER BY created_at DESC", nativeQuery = true)
    List<User> findAllOrderByCreatedDateDescNative();

    // 5. Native query with JOIN
    @Query(value = "SELECT u.* FROM users u INNER JOIN orders o ON u.id = o.user_id WHERE o.total_amount > :amount", nativeQuery = true)
    List<User> findUsersWithOrdersAboveNative(@Param("amount") Double amount);

    // 6. Native query with aggregate functions
    @Query(value = "SELECT AVG(age) FROM users", nativeQuery = true)
    Double getAverageAgeNative();

    // 7. Native query with GROUP BY
    @Query(value = "SELECT city, COUNT(*) FROM users GROUP BY city", nativeQuery = true)
    List<Object[]> getCityStatisticsNative();

    // 8. Native query for update (needs @Modifying)
    @Modifying
    @Transactional
    @Query(value = "UPDATE users SET age = :age WHERE id = :id", nativeQuery = true)
    int updateUserAgeNative(@Param("id") Long id, @Param("age") int age);

    // 9. Native query for delete
    @Modifying
    @Transactional
    @Query(value = "DELETE FROM users WHERE age < :minAge", nativeQuery = true)
    int deleteInactiveUsersNative(@Param("minAge") int minAge);

    // 10. Native query returning custom columns (Map)
    @Query(value = "SELECT id, name, email FROM users WHERE active = 1", nativeQuery = true)
    List<Map<String, Object>> getActiveUserSummary();

    // 11. Native query with pagination
    @Query(value = "SELECT * FROM users WHERE age > :minAge",
           countQuery = "SELECT COUNT(*) FROM users WHERE age > :minAge",
           nativeQuery = true)
    Page<User> findUsersByAgeNative(@Param("minAge") int minAge, Pageable pageable);

    // 12. Native query with database-specific functions (MySQL)
    @Query(value = "SELECT * FROM users WHERE YEAR(created_at) = :year", nativeQuery = true)
    List<User> findUsersByYearNative(@Param("year") int year);

    // 13. Native query with JSON functions (PostgreSQL)
    @Query(value = "SELECT * FROM users WHERE data->>'city' = :city", nativeQuery = true)
    List<User> findUsersByCityNative(@Param("city") String city);
}
```

## 8.3. Pagination (ការបែងចែកទំព័រ)

### 📌 និយមន័យ (Definition):

**Pagination** គឺជាបច្ចេកទេសបែងចែកលទ្ធផលជាទំព័រតូចៗ ដើម្បីកុំឱ្យផ្ទុកទិន្នន័យទាំងអស់ក្នុងពេលតែមួយ (improves performance and user experience)។ Spring Data JPA ផ្តល់ Pageable interface និង Page class សម្រាប់ pagination។

```properties
import org.springframework.data.domain.Page;
import org.springframework.data.domain.PageRequest;
import org.springframework.data.domain.Pageable;
import org.springframework.data.domain.Sort;
import org.springframework.data.jpa.repository.JpaRepository;
import org.springframework.data.jpa.repository.Query;
import org.springframework.stereotype.Service;

@Repository
public interface UserRepository extends JpaRepository<User, Long> {

    // 1. Pagination with derived query
    Page<User> findAll(Pageable pageable);

    // 2. Pagination with condition
    Page<User> findByAgeGreaterThan(int age, Pageable pageable);

    // 3. Pagination with JPQL
    @Query("SELECT u FROM User u WHERE u.active = true")
    Page<User> findActiveUsers(Pageable pageable);

    // 4. Pagination with native query (requires countQuery)
    @Query(value = "SELECT * FROM users WHERE age > :minAge",
           countQuery = "SELECT COUNT(*) FROM users WHERE age > :minAge",
           nativeQuery = true)
    Page<User> findUsersByAgeNative(@Param("minAge") int minAge, Pageable pageable);
}

// Service Layer Usage
@Service
public class UserService {

    @Autowired
    private UserRepository userRepository;

    // Basic pagination
    public Page<User> getUsers(int page, int size) {
        Pageable pageable = PageRequest.of(page, size);
        return userRepository.findAll(pageable);
    }

    // Pagination with sorting
    public Page<User> getUsersSorted(int page, int size, String sortBy, String direction) {
```

Sort sort = direction.equalsIgnoreCase("asc") ?

```java
                    Sort.by(sortBy).ascending() :
                    Sort.by(sortBy).descending();
        Pageable pageable = PageRequest.of(page, size, sort);
        return userRepository.findAll(pageable);
    }

    // Pagination with condition
    public Page<User> getUsersByAge(int age, int page, int size) {
        Pageable pageable = PageRequest.of(page, size);
        return userRepository.findByAgeGreaterThan(age, pageable);
    }

    // Get paginated result with metadata
    public Map<String, Object> getPaginatedUsers(int page, int size) {
        Page<User> pageResult = getUsers(page, size);

        Map<String, Object> response = new HashMap<>();
        response.put("content", pageResult.getContent());           // List of users
        response.put("currentPage", pageResult.getNumber());        // Current page number
        response.put("totalPages", pageResult.getTotalPages());     // Total pages
        response.put("totalElements", pageResult.getTotalElements()); // Total records
        response.put("pageSize", pageResult.getSize());             // Page size
        response.put("hasNext", pageResult.hasNext());              // Has next page
        response.put("hasPrevious", pageResult.hasPrevious());      // Has previous page
        response.put("isFirst", pageResult.isFirst());              // Is first page
        response.put("isLast", pageResult.isLast());                // Is last page

        return response;
    }
}

// Controller Example
@RestController
@RequestMapping("/api/users")
public class UserController {

    @Autowired
    private UserService userService;

    @GetMapping
    public ResponseEntity<Map<String, Object>> getUsers(
            @RequestParam(defaultValue = "0") int page,
            @RequestParam(defaultValue = "10") int size) {

        Map<String, Object> response = userService.getPaginatedUsers(page, size);
        return ResponseEntity.ok(response);
    }
}
```

## 8.4. Sorting (ការតម្រៀប)

### 📌 និយមន័យ (Definition):

**Sorting** គឺជាការតម្រៀបលទ្ធផលតាមលំដាប់ឡើង (ascending) ឬចុះ (descending) តាម field មួយ ឬច្រើន។ Spring Data JPA ផ្តល់ Sort class សម្រាប់ sorting។

```java
import org.springframework.data.domain.Sort;
import org.springframework.data.domain.PageRequest;
import org.springframework.data.domain.Pageable;
import org.springframework.data.jpa.repository.JpaRepository;
import org.springframework.data.jpa.repository.Query;
import java.util.List;

@Repository
public interface UserRepository extends JpaRepository<User, Long> {

    // 1. Sorting with derived query
    List<User> findAll(Sort sort);

    // 2. Sorting by single field
    List<User> findAllByOrderByNameAsc();
    List<User> findAllByOrderByNameDesc();
    List<User> findAllByOrderByCreatedAtDesc();

    // 3. Sorting with condition
    List<User> findByAgeGreaterThanOrderByNameAsc(int age);
    List<User> findByAgeGreaterThanOrderByCreatedAtDesc(int age);

    // 4. Sorting with JPQL
    @Query("SELECT u FROM User u ORDER BY u.name ASC")
    List<User> findAllSortedByNameAsc();

    @Query("SELECT u FROM User u ORDER BY u.age DESC, u.name ASC")
    List<User> findAllSortedByAgeDescThenNameAsc();

    // 5. Sorting with native query
    @Query(value = "SELECT * FROM users ORDER BY :sortColumn :sortDirection", nativeQuery = true)
    List<User> findAllSortedNative(@Param("sortColumn") String sortColumn,
                                   @Param("sortDirection") String sortDirection);
}

// Service Usage
@Service
public class UserService {

    @Autowired
    private UserRepository userRepository;

    // Single field sorting
    public List<User> getUsersSortedByName() {
        return userRepository.findAll(Sort.by("name").ascending());
    }

    // Multiple field sorting
    public List<User> getUsersSortedByAgeAndName() {
```

Sort sort = Sort.by("age").descending()

```text
                        .and(Sort.by("name").ascending());
        return userRepository.findAll(sort);
    }

    // Dynamic sorting
    public List<User> getUsersWithDynamicSort(String sortBy, String direction) {
```

Sort sort = direction.equalsIgnoreCase("asc") ?

```text
                    Sort.by(sortBy).ascending() :
                    Sort.by(sortBy).descending();
        return userRepository.findAll(sort);
    }

    // Sorting with multiple fields
    public List<User> getUsersWithMultipleSort(String[] sortFields, String[] directions) {
        Sort sort = Sort.unsorted();
        for (int i = 0; i < sortFields.length; i++) {
```

Sort currentSort = directions[i].equalsIgnoreCase("asc") ?

```properties
                               Sort.by(sortFields[i]).ascending() :
                               Sort.by(sortFields[i]).descending();
            sort = sort.and(currentSort);
        }
        return userRepository.findAll(sort);
    }

    // Sorting with pagination
    public Page<User> getUsersPaginatedSorted(int page, int size, String sortBy, String direction) {
```

Sort sort = direction.equalsIgnoreCase("asc") ?

```java
                    Sort.by(sortBy).ascending() :
                    Sort.by(sortBy).descending();
        Pageable pageable = PageRequest.of(page, size, sort);
        return userRepository.findAll(pageable);
    }
}

// Controller Example
@RestController
@RequestMapping("/api/users")
public class UserController {

    @Autowired
    private UserService userService;

    @GetMapping("/sorted")
    public ResponseEntity<List<User>> getSortedUsers(
            @RequestParam(defaultValue = "id") String sortBy,
            @RequestParam(defaultValue = "asc") String direction) {

        List<User> users = userService.getUsersWithDynamicSort(sortBy, direction);
        return ResponseEntity.ok(users);
    }
}
```

## 8.5. Auditing (ការតាមដានការផ្លាស់ប្តូរ)

### 📌 និយមន័យ (Definition):

**Auditing** គឺជាការកត់ត្រាពេលវេលានៃការបង្កើត (creation) និងការកែប្រែ (modification) នៃ entity នីមួយៗ ក៏ដូចជាអ្នកដែលបង្កើត ឬកែប្រែ។ Spring Data JPA ផ្តល់ auditing features តាមរយៈ @CreatedDate, @LastModifiedDate, @CreatedBy, @LastModifiedBy។

### 🔹 Enable Auditing in Spring Boot:

```java
// 1. Enable JPA Auditing
@Configuration
@EnableJpaAuditing(auditorAwareRef = "auditorProvider")
public class JpaConfig {

    @Bean
    public AuditorAware<String> auditorProvider() {
        return () -> {
            // Get current user from SecurityContext (if using Spring Security)
            Authentication auth = SecurityContextHolder.getContext().getAuthentication();
            if (auth == null || !auth.isAuthenticated()) {
                return Optional.of("system");
            }
            return Optional.of(auth.getName());
        };
    }
}

// 2. Base Auditing Entity
@MappedSuperclass
@EntityListeners(AuditingEntityListener.class)
public abstract class BaseEntity {

    @CreatedDate
    @Column(updatable = false)
    private LocalDateTime createdAt;

    @LastModifiedDate
    private LocalDateTime updatedAt;

    @CreatedBy
    @Column(updatable = false)
    private String createdBy;

    @LastModifiedBy
    private String updatedBy;

    // Getters and setters
}

// 3. Entity extending BaseEntity
@Entity
@Table(name = "users")
public class User extends BaseEntity {
    @Id
    @GeneratedValue
    private Long id;
    private String name;
    private String email;
    // ... other fields
}

// 4. Alternative: Direct annotations on entity
@Entity
@Table(name = "products")
@EntityListeners(AuditingEntityListener.class)
public class Product {

    @Id
    @GeneratedValue
    private Long id;

    private String name;
    private Double price;

    @CreatedDate
    @Column(updatable = false)
    private LocalDateTime createdDate;

    @LastModifiedDate
    private LocalDateTime lastModifiedDate;

    @CreatedBy
    @Column(updatable = false)
    private String createdBy;

    @LastModifiedBy
    private String lastModifiedBy;

    // Getters and setters
}

// Usage - Auditing happens automatically when entity is saved
@Service
public class ProductService {

    @Autowired
    private ProductRepository productRepository;

    public Product createProduct(Product product) {
        // createdAt, createdBy will be set automatically
        return productRepository.save(product);
    }

    public Product updateProduct(Long id, Product product) {
        Product existing = productRepository.findById(id).orElseThrow();
        existing.setName(product.getName());
        existing.setPrice(product.getPrice());
        // updatedAt, updatedBy will be set automatically
        return productRepository.save(existing);
    }
}
```

## 8.6. Entity Lifecycle Callbacks (វដ្តជីវិត Entity)

### 📌 និយមន័យ (Definition):

**Entity Lifecycle Callbacks** គឺជា methods ដែលត្រូវបានហៅ (invoke) ដោយ JPA នៅពេលដែល entity ឆ្លងកាត់ lifecycle events ផ្សេងៗគ្នា (persist, update, remove, load)។

```text
@PrePersist
```

Called before entity is persisted (saved) for the first time

```text
@PostPersist
```

Called after entity is persisted

```text
@PreUpdate
```

Called before entity is updated

```text
@PostUpdate
```

Called after entity is updated

```text
@PreRemove
```

Called before entity is deleted

```text
@PostRemove
```

Called after entity is deleted

```text
@PostLoad
```

Called after entity is loaded from database

```properties
import javax.persistence.*;

@Entity
@Table(name = "audit_logs")
public class AuditLog {

    @Id
    @GeneratedValue
    private Long id;

    private String action;
    private String entityType;
    private String entityId;
    private String oldValue;
    private String newValue;
    private LocalDateTime timestamp;

    @PrePersist
    protected void onCreate() {
        timestamp = LocalDateTime.now();
        System.out.println("PrePersist: About to save entity with action: " + action);
    }

    @PostPersist
    protected void onPostPersist() {
        System.out.println("PostPersist: Entity saved with ID: " + id);
    }

    @PreUpdate
    protected void onUpdate() {
        System.out.println("PreUpdate: About to update entity ID: " + id);
    }

    @PostUpdate
    protected void onPostUpdate() {
        System.out.println("PostUpdate: Entity updated");
    }

    @PreRemove
    protected void onRemove() {
        System.out.println("PreRemove: About to delete entity ID: " + id);
    }

    @PostRemove
    protected void onPostRemove() {
        System.out.println("PostRemove: Entity deleted");
    }

    @PostLoad
    protected void onLoad() {
        System.out.println("PostLoad: Entity loaded from database");
    }
}

// Entity with lifecycle callbacks for business logic
@Entity
public class Order {

    @Id
    @GeneratedValue
    private Long id;

    private String orderNumber;
    private String status;
    private Double totalAmount;

    @PrePersist
    public void prePersist() {
        // Generate order number before saving
        if (orderNumber == null) {
            orderNumber = "ORD-" + System.currentTimeMillis();
        }
        // Set default status
        if (status == null) {
            status = "PENDING";
        }
        System.out.println("Generating order number: " + orderNumber);
    }

    @PreUpdate
    public void preUpdate() {
        // Log status change
        System.out.println("Order " + orderNumber + " status changed to: " + status);

        // Validate before update
        if ("CANCELLED".equals(status) && totalAmount > 1000) {
            throw new IllegalStateException("Cannot cancel orders over $1000");
        }
    }

    @PostLoad
    public void postLoad() {
        // Calculate discount based on total amount
        System.out.println("Order loaded: " + orderNumber);
    }
}
```

## 8.7. Caching (ការផ្ទុកក្នុង Cache)

### 📌 និយមន័យ (Definition):

**Caching** គឺជាបច្ចេកទេសផ្ទុកទិន្នន័យដែលបានប្រើថ្មីៗ (frequently accessed data) ក្នុង memory ដើម្បីកាត់បន្ថយការចូលដំណើរការ database (improves performance)។ Hibernate គាំទ្រពីរកម្រិតនៃ caching៖ **First-level cache** (session) និង **Second-level cache** (SessionFactory)។

### 🔹 Enable Second-Level Cache:

```properties
# Enable second-level cache
spring.jpa.properties.hibernate.cache.use_second_level_cache=true
spring.jpa.properties.hibernate.cache.use_query_cache=true
spring.jpa.properties.hibernate.cache.region.factory_class=org.hibernate.cache.jcache.JCacheRegionFactory

# Cache provider (EHCache)
spring.jpa.properties.javax.persistence.sharedCache.mode=ENABLE_SELECTIVE
```

### 🔹 Maven Dependency for EHCache:

```xml
<dependency>
    <groupId>org.hibernate.orm</groupId>
    <artifactId>hibernate-jcache</artifactId>
</dependency>
<dependency>
    <groupId>org.ehcache</groupId>
    <artifactId>ehcache</artifactId>
</dependency>
import org.hibernate.annotations.Cache;
import org.hibernate.annotations.CacheConcurrencyStrategy;
import javax.persistence.*;

@Entity
@Table(name = "products")
@Cacheable
@org.hibernate.annotations.Cache(usage = CacheConcurrencyStrategy.READ_WRITE, region = "productCache")
public class Product {

    @Id
    @GeneratedValue
    private Long id;

    private String name;
    private Double price;

    // Second-level cache for relationships
    @ManyToOne
    @Cache(usage = CacheConcurrencyStrategy.READ_ONLY)
    private Category category;
}

// Spring Cache Abstraction
@Service
@CacheConfig(cacheNames = "users")
public class UserService {

    @Autowired
    private UserRepository userRepository;

    // Cache result - stores in cache after first call
    @Cacheable(key = "#id")
    public User getUserById(Long id) {
        System.out.println("Fetching from database for id: " + id);
        return userRepository.findById(id).orElseThrow();
    }

    // Cache eviction - removes from cache when data is updated
    @CachePut(key = "#user.id")
    public User updateUser(User user) {
        System.out.println("Updating user in database: " + user.getId());
        return userRepository.save(user);
    }

    // Cache evict - removes from cache
    @CacheEvict(key = "#id")
    public void deleteUser(Long id) {
        System.out.println("Deleting user from database: " + id);
        userRepository.deleteById(id);
    }

    // Evict all cache entries
    @CacheEvict(allEntries = true)
    public void clearCache() {
        System.out.println("Clearing all user cache");
    }

    // Cache with condition
    @Cacheable(key = "#id", condition = "#id > 10")
    public User getUserWithCondition(Long id) {
        return userRepository.findById(id).orElseThrow();
    }

    // Cache with unless (don't cache if condition is true)
    @Cacheable(key = "#id", unless = "#result == null")
    public Optional<User> getUserOptional(Long id) {
        return userRepository.findById(id);
    }
}
```

### 💡 Cache Concurrency Strategies:

- **READ_ONLY** – សម្រាប់ data ដែលមិនផ្លាស់ប្តូរ (configuration, reference data)

- **NONSTRICT_READ_WRITE** – សម្រាប់ data ដែលផ្លាស់ប្តូរកម្រ (rarely updated)

- **READ_WRITE** – សម្រាប់ data ដែលផ្លាស់ប្តូរញឹកញាប់

- **TRANSACTIONAL** – សម្រាប់ transactional environments

## 8.8. Optimistic Locking (សោសុទិដ្ឋិនិយម)

### 📌 និយមន័យ (Definition):

**Optimistic Locking** គឺជាយន្តការការពារ (concurrency control) ដែលសន្មត់ថាការ conflict កើតឡើងកម្រ (rare)។ វាប្រើ @Version annotation ដើម្បីតាមដាន version number ឬ timestamp នៃ entity។ នៅពេលដែលអ្នកព្យាយាមធ្វើបច្ចុប្បន្នភាព entity, Hibernate នឹងពិនិត្យមើល version ហើយបោះ OptimisticLockException ប្រសិនបើ version មិនត្រូវគ្នា។

```java
import javax.persistence.*;
import org.springframework.dao.OptimisticLockingFailureException;

@Entity
@Table(name = "products")
public class Product {

    @Id
    @GeneratedValue
    private Long id;

    private String name;
    private Double price;
    private Integer quantity;

    // Version field for optimistic locking
    @Version
    private Long version;  // or @Version private LocalDateTime lastModified;

    // Getters and setters
}

// Service with optimistic locking handling
@Service
public class ProductService {

    @Autowired
    private ProductRepository productRepository;

    @Transactional
    public void updateProductPrice(Long id, Double newPrice) {
        try {
            Product product = productRepository.findById(id).orElseThrow();
            product.setPrice(newPrice);
            productRepository.save(product);
            System.out.println("Product updated successfully");
        } catch (OptimisticLockingFailureException e) {
            System.err.println("Conflict: Product was modified by another user. Please retry.");
            // Retry logic or notify user
            throw new RuntimeException("Update failed due to concurrent modification", e);
        }
    }

    // Retry mechanism for optimistic lock failures
    @Transactional
    public void updateProductWithRetry(Long id, Double newPrice, int maxRetries) {
        int retryCount = 0;
        while (retryCount < maxRetries) {
            try {
                Product product = productRepository.findById(id).orElseThrow();
                product.setPrice(newPrice);
                productRepository.save(product);
                return; // Success
            } catch (OptimisticLockingFailureException e) {
                retryCount++;
                if (retryCount >= maxRetries) {
                    throw new RuntimeException("Failed after " + maxRetries + " retries", e);
                }
                // Refresh entity and retry
                productRepository.flush();
            }
        }
    }
}

// Entity with timestamp versioning
@Entity
public class Customer {

    @Id
    @GeneratedValue
    private Long id;

    private String name;

    @Version
    private LocalDateTime lastModified;

    // When entity is updated, lastModified will be automatically updated
}
```

## 8.9. Pessimistic Locking (សោទុទិដ្ឋិនិយម)

### 📌 និយមន័យ (Definition):

**Pessimistic Locking** គឺជាយន្តការការពារ (concurrency control) ដែលសន្មត់ថាការ conflict កើតឡើងញឹកញាប់។ វាអនុញ្ញាតឱ្យអ្នក "lock" database row នៅពេលដែលអ្នកអានវា ដើម្បីការពារអ្នកដទៃ ពីការកែប្រែរហូតដល់អ្នកបញ្ចប់ការងារ។ Spring Data JPA ផ្តល់ @Lock annotation សម្រាប់ pessimistic locking។

**LockModeType.PESSIMISTIC_READ**

Shared lock: other transactions can read but not write

**LockModeType.PESSIMISTIC_WRITE**

Exclusive lock: other transactions cannot read or write

**LockModeType.PESSIMISTIC_FORCE_INCREMENT**

Write lock with version increment

```java
import org.springframework.data.jpa.repository.JpaRepository;
import org.springframework.data.jpa.repository.Lock;
import org.springframework.data.jpa.repository.Query;
import org.springframework.data.repository.query.Param;
import javax.persistence.LockModeType;
import java.util.Optional;

@Repository
public interface ProductRepository extends JpaRepository<Product, Long> {

    // 1. Pessimistic Write Lock
    @Lock(LockModeType.PESSIMISTIC_WRITE)
    @Query("SELECT p FROM Product p WHERE p.id = :id")
    Optional<Product> findByIdWithPessimisticWriteLock(@Param("id") Long id);

    // 2. Pessimistic Read Lock
    @Lock(LockModeType.PESSIMISTIC_READ)
    @Query("SELECT p FROM Product p WHERE p.id = :id")
    Optional<Product> findByIdWithPessimisticReadLock(@Param("id") Long id);

    // 3. Pessimistic Force Increment (increments version even for read)
    @Lock(LockModeType.PESSIMISTIC_FORCE_INCREMENT)
    @Query("SELECT p FROM Product p WHERE p.id = :id")
    Optional<Product> findByIdWithPessimisticForceIncrement(@Param("id") Long id);
}

// Service using pessimistic locking
@Service
public class InventoryService {

    @Autowired
    private ProductRepository productRepository;

    @Transactional
    public boolean decreaseStock(Long productId, int quantity) {
        // Acquire exclusive lock on the product row
        Product product = productRepository.findByIdWithPessimisticWriteLock(productId)
                .orElseThrow(() -> new RuntimeException("Product not found"));

        // Check and update stock (protected by lock)
        if (product.getQuantity() >= quantity) {
            product.setQuantity(product.getQuantity() - quantity);
            productRepository.save(product);
            return true;
        }
        return false;
    }

    // With timeout
    @Transactional
    public Product getProductWithLockAndTimeout(Long id) {
        EntityManager em = entityManagerFactory.createEntityManager();
        Product product = em.find(Product.class, id,
```

LockModeType.PESSIMISTIC_WRITE,

```text
            Map.of("javax.persistence.lock.timeout", 5000)); // 5 seconds timeout
        return product;
    }
}
```

## 8.10. Performance Optimization (ការបង្កើនប្រសិទ្ធភាព)

### 📌 គន្លឹះសម្រាប់បង្កើនប្រសិទ្ធភាព:

**1. Use Batch Operations**

```properties
# application.properties
spring.jpa.properties.hibernate.jdbc.batch_size=20
spring.jpa.properties.hibernate.order_inserts=true
spring.jpa.properties.hibernate.order_updates=true
```

**2. Use DTO Projections (instead of full entities)**

```text
@Query("SELECT new com.example.dto.UserDto(u.id, u.name) FROM User u")
List<UserDto> findAllUserDtos();
```

**3. Use JOIN FETCH to avoid N+1 queries**

```text
@Query("SELECT u FROM User u JOIN FETCH u.orders WHERE u.id = :id")
Optional<User> findByIdWithOrders(@Param("id") Long id);
```

**4. Enable Hibernate Statistics for Monitoring**

```properties
spring.jpa.properties.hibernate.generate_statistics=true
logging.level.org.hibernate.stat=DEBUG
```

**5. Use Pagination for Large Result Sets**

```text
Page<User> page = userRepository.findAll(PageRequest.of(0, 20));
```

**6. Index Database Columns**

```java
@Entity
@Table(name = "users", indexes = {
    @Index(name = "idx_email", columnList = "email"),
    @Index(name = "idx_name_age", columnList = "name, age")
})
public class User { ... }
```

**7. Use Second-Level Cache**

```java
@Entity
@Cacheable
@org.hibernate.annotations.Cache(usage = CacheConcurrencyStrategy.READ_WRITE)
public class Product { ... }
```

**8. Set Appropriate Fetch Types**

```text
@OneToMany(fetch = FetchType.LAZY)  // Default and recommended
@ManyToOne(fetch = FetchType.EAGER)   // Can be changed to LAZY
```

## 8.11. N+1 Query Problem (បញ្ហា N+1 Query)

### 📌 និយមន័យ (Definition):

**N+1 Query Problem** គឺជា performance anti-pattern ដែលកើតឡើងនៅពេលដែល Hibernate ប្រតិបត្តិ N+1 SQL queries៖ 1 query ដើម្បីទាញយក parent entities និង N queries ដើម្បីទាញយក child entities សម្រាប់ parent នីមួយៗ។ នេះបណ្តាលឱ្យ performance យឺត។

**❌** **Problematic Code (N+1)**

```java
// This causes N+1 queries
List<User> users = userRepository.findAll();
for (User user : users) {
    // This triggers additional query for each user
    System.out.println(user.getOrders().size());
}
```

### ✅ Solutions

```java
// Solution 1: JOIN FETCH
@Query("SELECT u FROM User u JOIN FETCH u.orders")
List<User> findAllWithOrders();

// Solution 2: Entity Graph
@EntityGraph(attributePaths = {"orders"})
List<User> findAll();

// Solution 3: Batch Fetching
@BatchSize(size = 10)
@OneToMany(mappedBy = "user")
private List<Order> orders;
// Solution 1: JOIN FETCH in JPQL
@Repository
public interface UserRepository extends JpaRepository<User, Long> {

    // Single query with JOIN FETCH
    @Query("SELECT DISTINCT u FROM User u LEFT JOIN FETCH u.orders")
    List<User> findAllWithOrders();

    @Query("SELECT u FROM User u LEFT JOIN FETCH u.orders WHERE u.id = :id")
    Optional<User> findByIdWithOrders(@Param("id") Long id);

    // Multiple associations
    @Query("SELECT DISTINCT u FROM User u " +
```

"LEFT JOIN FETCH u.orders " +

"LEFT JOIN FETCH u.addresses")

```java
    List<User> findAllWithOrdersAndAddresses();
}

// Solution 2: Entity Graph
@Entity
@NamedEntityGraph(name = "User.withOrders", attributeNodes = @NamedAttributeNode("orders"))
public class User {
    // ...
}

@Repository
public interface UserRepository extends JpaRepository<User, Long> {

    @EntityGraph("User.withOrders")
    List<User> findAll();

    @EntityGraph("User.withOrders")
    Optional<User> findById(Long id);

    // Dynamic entity graph
    @EntityGraph(attributePaths = {"orders", "addresses"})
    List<User> findAll();
}

// Solution 3: Batch Fetching
@Entity
public class User {

    @BatchSize(size = 20)  // Fetches child collections in batches
    @OneToMany(mappedBy = "user", fetch = FetchType.LAZY)
    private List<Order> orders;
}

// Solution 4: Subquery (for count)
@Query("SELECT u, (SELECT COUNT(o) FROM Order o WHERE o.user = u) as orderCount FROM User u")
List<Object[]> findAllWithOrderCount();
```

**🔍 How to Detect N+1 Problem:**

- Enable Hibernate SQL logging: spring.jpa.show-sql=true

- Enable statistics: spring.jpa.properties.hibernate.generate_statistics=true

- Use tools like **Hibernate Statistics** or **Spring Boot Actuator**

- Monitor number of queries executed in logs

## 8.12. DTO Projection (ការព្យាករទិន្នន័យ)

### 📌 និយមន័យ (Definition):

**DTO Projection** គឺជាបច្ចេកទេសទាញយកតែ fields ដែលត្រូវការពី database ជំនួសឱ្យទាញយក entity ទាំងមូល។ នេះជួយកាត់បន្ថយចំនួន data ដែលត្រូវបានផ្ទេរ និងបង្កើន performance (especially for large datasets)។

**Interface-based Projection**

```java
public interface UserView {
    String getName();
    String getEmail();
    int getAge();
}

// Repository
@Query("SELECT u.name as name, u.email as email, u.age as age FROM User u")
List<UserView> findAllUserViews();
```

**Class-based Projection (DTO)**

```java
public class UserDto {
    private String name;
    private String email;
    private int age;
    // constructor, getters, setters
}

// Repository
@Query("SELECT new com.example.dto.UserDto(u.name, u.email, u.age) FROM User u")
List<UserDto> findAllUserDtos();
```

**Dynamic Projection**

```properties
<T> List<T> findAllBy(Class<T> type);

// Usage
List<UserView> views = repository.findAllBy(UserView.class);
List<UserDto> dtos = repository.findAllBy(UserDto.class);
// 1. Interface-based Projection (recommended for simple projections)
public interface UserSummary {
    String getName();
    String getEmail();
    int getAge();

    // Nested projection
    String getCity();

    // Default method
    default String getDisplayName() {
        return getName() + " (" + getEmail() + ")";
    }
}

@Repository
public interface UserRepository extends JpaRepository<User, Long> {

    // Spring Data automatically creates implementation
    List<UserSummary> findAllByOrderByNameAsc();

    // With condition
    List<UserSummary> findByAgeGreaterThan(int age);

    // Open projection (can use SpEL)
    @Value("#{target.name + ' - ' + target.email}")
    String getFullInfo();
}

// 2. Class-based Projection (DTO) - more control
public class UserDTO {
    private Long id;
    private String name;
    private String email;
    private int age;
    private String city;
    private int orderCount;

    // Constructor for JPQL
    public UserDTO(Long id, String name, String email, int age, String city) {
        this.id = id;
        this.name = name;
        this.email = email;
        this.age = age;
        this.city = city;
    }

    // Constructor for native query
    public UserDTO(Long id, String name, String email, int age, String city, int orderCount) {
        this(id, name, email, age, city);
        this.orderCount = orderCount;
    }

    // Getters and setters
}

@Repository
public interface UserRepository extends JpaRepository<User, Long> {

    // JPQL with constructor expression
    @Query("SELECT new com.example.dto.UserDTO(u.id, u.name, u.email, u.age, u.address.city) " +
```

"FROM User u WHERE u.active = true")

```text
    List<UserDTO> findActiveUserDTOs();

    // Native query with DTO (using SQLResultSetMapping)
    @Query(value = "SELECT u.id, u.name, u.email, u.age, a.city, COUNT(o.id) as order_count " +
```

"FROM users u " +

"LEFT JOIN addresses a ON u.address_id = a.id " +

"LEFT JOIN orders o ON u.id = o.user_id " +

"GROUP BY u.id", nativeQuery = true)

```java
    List<UserDTO> findUserDTOsWithOrderCount();
}

// 3. Dynamic Projection
@Repository
public interface UserRepository extends JpaRepository<User, Long> {

    <T> List<T> findAllBy(Class<T> type);

    <T> List<T> findByAgeGreaterThan(int age, Class<T> type);

    <T> Optional<T> findById(Long id, Class<T> type);
}

// Usage
@Service
public class UserService {

    @Autowired
    private UserRepository userRepository;

    public List<UserSummary> getUserSummaries() {
        return userRepository.findAllByOrderByNameAsc();
    }

    public List<UserDTO> getUserDTOs() {
        return userRepository.findActiveUserDTOs();
    }

    public List<UserProjection> getDynamicProjections(Class<UserProjection> type) {
        return userRepository.findAllBy(type);
    }
}

// 4. Tuple projection (for dynamic fields)
@Query("SELECT u.id as id, u.name as name, u.email as email FROM User u")
List<Tuple> findUserTuples();

// Usage
List<Tuple> tuples = userRepository.findUserTuples();
for (Tuple tuple : tuples) {
    Long id = tuple.get("id", Long.class);
    String name = tuple.get("name", String.class);
    String email = tuple.get("email", String.class);
}
```

### 💡 When to Use DTO Projection:

- When you need only a subset of entity fields

- For API responses (avoid exposing entire entity)

- When you need to aggregate data from multiple tables

- For reporting and dashboard data

- When dealing with large datasets (performance improvement)

- When you need to combine data from different entities

### 📊 Projection Comparison:

| Type | Pros | Cons |
| --- | --- | --- |
| Interface Projection | Simple, no boilerplate, nested projections | Limited control, no custom logic |
| Class DTO (JPQL) | Full control, can add business logic | Requires constructor, more boilerplate |
| Tuple Projection | Flexible, dynamic fields | Type safety, verbose access |
| Native Query DTO | Best performance, database-specific features | Database dependent, harder to maintain |

### 📚 សង្ខេបមេរៀនទី៨ (Module 8 Summary)

នៅក្នុងមេរៀននេះ អ្នកបានរៀនអំពី Advanced JPA & Hibernate features៖

- **JPQL** – Object-oriented query language for JPA entities

- **Native Query** – Plain SQL for database-specific features

- **Pagination** – Pageable, Page, PageRequest for large datasets

- **Sorting** – Sort.by(), multiple field sorting

- **Auditing** – @CreatedDate, @LastModifiedDate, @CreatedBy, @LastModifiedBy

- **Entity Lifecycle** – @PrePersist, @PostPersist, @PreUpdate, @PostUpdate, @PreRemove, @PostRemove, @PostLoad

- **Caching** – First-level cache, Second-level cache, @Cacheable, @CacheEvict

- **Optimistic Locking** – @Version, handles concurrent updates with retry

- **Pessimistic Locking** – @Lock, database row locks

- **Performance Optimization** – Batch operations, indexing, fetch strategies, statistics

- **N+1 Query Problem** – JOIN FETCH, Entity Graph, Batch Fetching solutions

- **DTO Projection** – Interface-based, class-based, dynamic projections

# មេរៀនទី៩: Validation & Exception Handling (ការផ្ទៀងផ្ទាត់ និងការគ្រប់គ្រងករណីលើកលែង)

### 📖 សេចក្តីផ្តើម (Introduction):
Validation និង Exception Handling គឺជាផ្នែកសំខាន់ក្នុងការអភិវឌ្ឍន៍ API ដើម្បីធានាថាទិន្នន័យដែលបានបញ្ចូលមានភាពត្រឹមត្រូវ និងដើម្បីគ្រប់គ្រងកំហុសបានត្រឹមត្រូវ។ មេរៀននេះនឹងបង្រៀនអ្នកពី Bean Validation, @Valid Annotation, Validation Constraints, Custom Validation, Global Exception Handling, @ControllerAdvice, Custom Exceptions, និង API Error Response។

## 9.1. Bean Validation (JSR-303/JSR-380)

### 📌 និយមន័យ (Definition):

**Bean Validation** គឺជា Java specification (JSR-303, JSR-380) ដែលផ្តល់នូវ annotations សម្រាប់ផ្ទៀងផ្ទាត់ (validate) Java objects។ Spring Boot គាំទ្រ Bean Validation ដោយស្វ័យប្រវត្តិ តាមរយៈ Hibernate Validator (implementation)។

### 🔹 Maven Dependencies:

```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-validation</artifactId>
</dependency>

<!-- Already included in spring-boot-starter-web -->
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-web</artifactId>
</dependency>
```

### 🔹 Basic Example:

```java
import javax.validation.constraints.*;

public class UserRequest {

    @NotBlank(message = "Name is required")
    @Size(min = 2, max = 50, message = "Name must be between 2 and 50 characters")
    private String name;

    @NotBlank(message = "Email is required")
    @Email(message = "Invalid email format")
    private String email;

    @NotNull(message = "Age is required")
    @Min(value = 18, message = "Age must be at least 18")
    @Max(value = 120, message = "Age must be less than 120")
    private Integer age;

    @Pattern(regexp = "^\+?[0-9]{10,15}$", message = "Invalid phone number")
    private String phone;

    @Past(message = "Birth date must be in the past")
    private LocalDate birthDate;

    @Future(message = "Expiry date must be in the future")
    private LocalDate expiryDate;

    @DecimalMin(value = "0.0", inclusive = false, message = "Price must be positive")
    @DecimalMax(value = "999999.99", message = "Price cannot exceed 999999.99")
    private BigDecimal price;

    @AssertTrue(message = "Must agree to terms")
    private boolean agreeTerms;

    @NotEmpty(message = "Roles cannot be empty")
    private List<@NotBlank String> roles;

    // Getters and setters
}
```

### 💡 Validation Groups:

Validation groups អនុញ្ញាតឱ្យអ្នកអនុវត្ត validation ផ្សេងគ្នាសម្រាប់ករណីប្រើប្រាស់ផ្សេងគ្នា (create vs update)។

## 9.2. @Valid Annotation

### 📌 និយមន័យ (Definition):

```java
@Valid គឺជា annotation ដែលប្រាប់ Spring ឱ្យធ្វើ validation លើ object ដែលបានបញ្ជូនមកក្នុង request body (@RequestBody), path variable, ឬ request parameter។ ប្រសិនបើ validation fails, Spring នឹងបោះ MethodArgumentNotValidException។
import org.springframework.validation.annotation.Validated;
import org.springframework.web.bind.annotation.*;
import javax.validation.Valid;
import javax.validation.constraints.*;

@RestController
@RequestMapping("/api/users")
@Validated  // For method-level validation
public class UserController {

    @Autowired
    private UserService userService;

    // 1. Validate @RequestBody
    @PostMapping
    public ResponseEntity<User> createUser(@Valid @RequestBody UserRequest userRequest) {
        User user = userService.create(userRequest);
        return ResponseEntity.status(HttpStatus.CREATED).body(user);
    }

    // 2. Validate @PathVariable
    @GetMapping("/{id}")
    public ResponseEntity<User> getUserById(@PathVariable @Min(1) Long id) {
        return ResponseEntity.ok(userService.findById(id));
    }

    // 3. Validate @RequestParam
    @GetMapping("/search")
    public ResponseEntity<List<User>> searchUsers(
            @RequestParam @NotBlank String name,
            @RequestParam @Min(18) @Max(100) Integer age) {
        return ResponseEntity.ok(userService.searchByNameAndAge(name, age));
    }

    // 4. Validate nested objects
    @PostMapping("/orders")
    public ResponseEntity<Order> createOrder(@Valid @RequestBody OrderRequest orderRequest) {
        return ResponseEntity.ok(orderService.create(orderRequest));
    }

    // 5. Validate with groups
    @PutMapping("/{id}")
    public ResponseEntity<User> updateUser(
            @PathVariable Long id,
            @Valid @RequestBody UserUpdateRequest userUpdateRequest) {
        return ResponseEntity.ok(userService.update(id, userUpdateRequest));
    }
}

// Entity with nested validation
public class OrderRequest {
    @Valid  // This will also validate the Customer object
    private Customer customer;

    @Valid
    private List<@Valid OrderItem> items;

    // Getters and setters
}

// Validation Groups
public interface CreateGroup {}
public interface UpdateGroup {}

public class UserRequest {
    @NotNull(groups = CreateGroup.class)
    private String id;

    @NotBlank(groups = {CreateGroup.class, UpdateGroup.class})
    private String name;

    @Email(groups = CreateGroup.class)
    @NotBlank(groups = CreateGroup.class)
    private String email;

    // Getters and setters
}

// Controller with validation groups
@PostMapping
public ResponseEntity<User> createUser(
        @Validated(CreateGroup.class) @RequestBody UserRequest userRequest) {
    // Only validates fields with CreateGroup
    return ResponseEntity.ok(userService.create(userRequest));
}

@PutMapping("/{id}")
public ResponseEntity<User> updateUser(
        @Validated(UpdateGroup.class) @RequestBody UserRequest userRequest) {
    // Only validates fields with UpdateGroup
    return ResponseEntity.ok(userService.update(userRequest));
}
```

## 9.3. Validation Constraints (ការកំណត់សម្រាប់ផ្ទៀងផ្ទាត់)

### 📌 បញ្ជី Validation Constraints:

| Annotation | Description | Example |
| --- | --- | --- |
| @NotNull | Value cannot be null | @NotNull String name; |
| @NotBlank | Not null, not empty, not whitespace | @NotBlank String title; |
| @NotEmpty | Not null and not empty (for collections/arrays) | @NotEmpty List<String> items; |
| @Size | String/Collection length between min and max | @Size(min=2, max=50) String name; |
| @Min | Minimum numeric value | @Min(18) int age; |
| @Max | Maximum numeric value | @Max(100) int score; |
| @DecimalMin | Minimum decimal value | @DecimalMin("0.01") double price; |
| @DecimalMax | Maximum decimal value | @DecimalMax("999.99") double amount; |
| @Email | Valid email format | @Email String email; |
| @Pattern | Regex pattern match | @Pattern(regexp="^[A-Z].*") String code; |
| @Past | Date in the past | @Past LocalDate birthDate; |
| @PastOrPresent | Date in the past or present | @PastOrPresent LocalDate modifiedDate; |
| @Future | Date in the future | @Future LocalDate expiryDate; |
| @FutureOrPresent | Date in the future or present | @FutureOrPresent LocalDate startDate; |
| @AssertTrue | Must be true | @AssertTrue boolean agreeTerms; |
| @AssertFalse | Must be false | @AssertFalse boolean isDeleted; |
| @Positive | Positive number (greater than 0) | @Positive int quantity; |
| @PositiveOrZero | Positive number or zero (greater than or equal to 0) | @PositiveOrZero int count; |
| @Negative | Negative number (less than 0) | @Negative int temperature; |
| @NegativeOrZero | Negative number or zero (less than or equal to 0) | @NegativeOrZero int debt; |
| @Digits | Integer and fraction digits | @Digits(integer=10, fraction=2) BigDecimal amount; |

## 9.4. Custom Validation (ការផ្ទៀងផ្ទាត់តាមបំណង)

### 📌 និយមន័យ (Definition):

**Custom Validation** អនុញ្ញាតឱ្យអ្នកបង្កើត validation logic ផ្ទាល់ខ្លួន នៅពេលដែល built-in constraints មិនគ្រប់គ្រាន់។ អ្នកត្រូវបង្កើត annotation ថ្មី និង validator class។

```properties
// 1. Create custom annotation
import javax.validation.Constraint;
import javax.validation.Payload;
import java.lang.annotation.*;

@Target({ElementType.FIELD, ElementType.PARAMETER})
@Retention(RetentionPolicy.RUNTIME)
@Constraint(validatedBy = PhoneNumberValidator.class)
public @interface ValidPhoneNumber {

    String message() default "Invalid phone number";

    Class<?>[] groups() default {};

    Class<? extends Payload>[] payload() default {};

    // Optional: add custom attributes
    String countryCode() default "+855";
}

// 2. Create validator class
import javax.validation.ConstraintValidator;
import javax.validation.ConstraintValidatorContext;

public class PhoneNumberValidator implements ConstraintValidator<ValidPhoneNumber, String> {

    private String countryCode;

    @Override
    public void initialize(ValidPhoneNumber constraintAnnotation) {
        this.countryCode = constraintAnnotation.countryCode();
    }

    @Override
    public boolean isValid(String phoneNumber, ConstraintValidatorContext context) {
        if (phoneNumber == null || phoneNumber.isEmpty()) {
            return true; // Use @NotBlank for required validation
        }

        // Cambodian phone number validation
        String regex = "^(" + countryCode + ")?[0-9]{8,9}$";
        return phoneNumber.matches(regex);
    }
}

// 3. Use custom validation
public class UserRequest {

    @NotBlank
    @ValidPhoneNumber(countryCode = "+855", message = "Invalid Cambodian phone number")
    private String phoneNumber;
}

// 4. Another example: Password match validation
@Target(ElementType.TYPE)
@Retention(RetentionPolicy.RUNTIME)
@Constraint(validatedBy = PasswordMatchValidator.class)
public @interface PasswordMatch {
    String message() default "Passwords do not match";
    String password();
    String confirmPassword();
    Class<?>[] groups() default {};
    Class<? extends Payload>[] payload() default {};
}

public class PasswordMatchValidator implements ConstraintValidator<PasswordMatch, Object> {

    private String passwordFieldName;
    private String confirmPasswordFieldName;

    @Override
    public void initialize(PasswordMatch constraintAnnotation) {
        this.passwordFieldName = constraintAnnotation.password();
        this.confirmPasswordFieldName = constraintAnnotation.confirmPassword();
    }

    @Override
    public boolean isValid(Object value, ConstraintValidatorContext context) {
        try {
            Object password = BeanUtils.getProperty(value, passwordFieldName);
            Object confirmPassword = BeanUtils.getProperty(value, confirmPasswordFieldName);
            return password != null && password.equals(confirmPassword);
        } catch (Exception e) {
            return false;
        }
    }
}

// Usage
@PasswordMatch(password = "password", confirmPassword = "confirmPassword")
public class RegistrationRequest {
    private String username;
    private String password;
    private String confirmPassword;
    // Getters and setters
}

// 5. Custom validation with database check
@Target(ElementType.FIELD)
@Retention(RetentionPolicy.RUNTIME)
@Constraint(validatedBy = UniqueEmailValidator.class)
public @interface UniqueEmail {
    String message() default "Email already exists";
    Class<?>[] groups() default {};
    Class<? extends Payload>[] payload() default {};
}

public class UniqueEmailValidator implements ConstraintValidator<UniqueEmail, String> {

    @Autowired
    private UserRepository userRepository;

    @Override
    public boolean isValid(String email, ConstraintValidatorContext context) {
        if (email == null || email.isEmpty()) {
            return true;
        }
        return !userRepository.existsByEmail(email);
    }
}

// Usage
public class UserRequest {
    @NotBlank
    @Email
    @UniqueEmail
    private String email;
}
```

## 9.5. Global Exception Handling (ការគ្រប់គ្រងករណីលើកលែងសកល)

### 📌 និយមន័យ (Definition):

**Global Exception Handling** គឺជាយន្តការដែលអនុញ្ញាតឱ្យអ្នកគ្រប់គ្រង exceptions ទាំងអស់ក្នុងកម្មវិធីនៅកន្លែងតែមួយ (centralized)។ Spring ផ្តល់ @ControllerAdviceសម្រាប់ global exception handling។

```java
import org.springframework.http.HttpStatus;
import org.springframework.http.ResponseEntity;
import org.springframework.web.bind.annotation.ExceptionHandler;
import org.springframework.web.bind.annotation.RestControllerAdvice;
import org.springframework.web.context.request.WebRequest;
import java.time.LocalDateTime;
import java.util.HashMap;
import java.util.Map;

@RestControllerAdvice
public class GlobalExceptionHandler {

    // Handle generic exception
    @ExceptionHandler(Exception.class)
    public ResponseEntity<ErrorResponse> handleAllExceptions(Exception ex, WebRequest request) {
```

ErrorResponse error = ErrorResponse.builder()

.timestamp(LocalDateTime.now())

.status(HttpStatus.INTERNAL_SERVER_ERROR.value())

.error("Internal Server Error")

.message(ex.getMessage())

.path(request.getDescription(false))

```java
                .build();
        return new ResponseEntity<>(error, HttpStatus.INTERNAL_SERVER_ERROR);
    }

    // Handle resource not found
    @ExceptionHandler(ResourceNotFoundException.class)
    public ResponseEntity<ErrorResponse> handleResourceNotFound(ResourceNotFoundException ex, WebRequest request) {
```

ErrorResponse error = ErrorResponse.builder()

.timestamp(LocalDateTime.now())

.status(HttpStatus.NOT_FOUND.value())

.error("Not Found")

.message(ex.getMessage())

.path(request.getDescription(false))

```java
                .build();
        return new ResponseEntity<>(error, HttpStatus.NOT_FOUND);
    }

    // Handle validation errors
    @ExceptionHandler(MethodArgumentNotValidException.class)
    public ResponseEntity<ErrorResponse> handleValidationExceptions(MethodArgumentNotValidException ex) {
        Map<String, String> errors = new HashMap<>();
        ex.getBindingResult().getAllErrors().forEach((error) -> {
            String fieldName = ((FieldError) error).getField();
            String errorMessage = error.getDefaultMessage();
            errors.put(fieldName, errorMessage);
        });
```

ErrorResponse error = ErrorResponse.builder()

.timestamp(LocalDateTime.now())

.status(HttpStatus.BAD_REQUEST.value())

.error("Validation Failed")

.message("Invalid input data")

.validationErrors(errors)

```java
                .build();
        return new ResponseEntity<>(error, HttpStatus.BAD_REQUEST);
    }

    // Handle illegal argument
    @ExceptionHandler(IllegalArgumentException.class)
    public ResponseEntity<ErrorResponse> handleIllegalArgument(IllegalArgumentException ex, WebRequest request) {
```

ErrorResponse error = ErrorResponse.builder()

.timestamp(LocalDateTime.now())

.status(HttpStatus.BAD_REQUEST.value())

.error("Bad Request")

.message(ex.getMessage())

.path(request.getDescription(false))

```java
                .build();
        return new ResponseEntity<>(error, HttpStatus.BAD_REQUEST);
    }
}
```

## 9.6. @ControllerAdvice / @RestControllerAdvice

### 📌 និយមន័យ (Definition):

```properties
@ControllerAdvice គឺជា annotation ដែលអនុញ្ញាតឱ្យអ្នកប្រមូលផ្តុំ @ExceptionHandler, @InitBinder, និង @ModelAttribute methods សម្រាប់ controllers ទាំងអស់។ @RestControllerAdviceគឺជា combination នៃ @ControllerAdvice និង @ResponseBody។
import org.springframework.http.HttpStatus;
import org.springframework.http.ResponseEntity;
import org.springframework.web.bind.annotation.*;

@RestControllerAdvice(
    basePackages = "com.example.controller",  // Apply to specific packages
    assignableTypes = {UserController.class, ProductController.class},  // Apply to specific controllers
    annotations = RestController.class  // Apply to controllers with specific annotation
```

)

```java
public class CustomControllerAdvice {

    // 1. Exception handler with specific status
    @ExceptionHandler(DataAccessException.class)
    @ResponseStatus(HttpStatus.SERVICE_UNAVAILABLE)
    public ErrorResponse handleDatabaseError(DataAccessException ex) {
        return new ErrorResponse("Database error: " + ex.getMessage());
    }

    // 2. Exception handler with ResponseEntity
    @ExceptionHandler(ConstraintViolationException.class)
    public ResponseEntity<ErrorResponse> handleConstraintViolation(ConstraintViolationException ex) {
        List<String> errors = ex.getConstraintViolations().stream()
```

.map(violation -> violation.getPropertyPath() + ": " + violation.getMessage())

```java
                .collect(Collectors.toList());

        ErrorResponse error = new ErrorResponse("Validation failed", errors);
        return ResponseEntity.badRequest().body(error);
    }

    // 3. Handle multiple exceptions
    @ExceptionHandler({IllegalStateException.class, IllegalArgumentException.class})
    public ResponseEntity<ErrorResponse> handleBadRequest(RuntimeException ex) {
        return ResponseEntity.badRequest()
                .body(new ErrorResponse(ex.getMessage()));
    }

    // 4. Add common model attributes to all controllers
    @ModelAttribute
    public void addGlobalAttributes(Model model) {
        model.addAttribute("appName", "My Spring Boot App");
        model.addAttribute("appVersion", "1.0.0");
    }

    // 5. Customize data binding
    @InitBinder
    public void initBinder(WebDataBinder binder) {
        binder.setDisallowedFields("id");  // Prevent binding id field
        binder.registerCustomEditor(LocalDate.class, new CustomDateEditor());
    }

    // 6. Handle access denied
    @ExceptionHandler(AccessDeniedException.class)
    @ResponseStatus(HttpStatus.FORBIDDEN)
    public ErrorResponse handleAccessDenied(AccessDeniedException ex) {
        return new ErrorResponse("Access denied: " + ex.getMessage());
    }

    // 7. Handle method argument type mismatch
    @ExceptionHandler(MethodArgumentTypeMismatchException.class)
    public ResponseEntity<ErrorResponse> handleTypeMismatch(MethodArgumentTypeMismatchException ex) {
        String message = String.format("Parameter '%s' should be of type '%s'",
                ex.getName(), ex.getRequiredType().getSimpleName());
        return ResponseEntity.badRequest().body(new ErrorResponse(message));
    }

    // 8. Handle missing request parameters
    @ExceptionHandler(MissingServletRequestParameterException.class)
    public ResponseEntity<ErrorResponse> handleMissingParams(MissingServletRequestParameterException ex) {
        String message = String.format("Required parameter '%s' is missing", ex.getParameterName());
        return ResponseEntity.badRequest().body(new ErrorResponse(message));
    }

    // 9. Handle HTTP message not readable (malformed JSON)
    @ExceptionHandler(HttpMessageNotReadableException.class)
    public ResponseEntity<ErrorResponse> handleMalformedJson(HttpMessageNotReadableException ex) {
        return ResponseEntity.badRequest()
                .body(new ErrorResponse("Malformed JSON request"));
    }

    // 10. Handle async request timeout
    @ExceptionHandler(AsyncRequestTimeoutException.class)
    @ResponseStatus(HttpStatus.SERVICE_UNAVAILABLE)
    public ErrorResponse handleAsyncTimeout(AsyncRequestTimeoutException ex) {
        return new ErrorResponse("Request timeout");
    }
}
```

## 9.7. Custom Exceptions (ករណីលើកលែងតាមបំណង)

### 📌 និយមន័យ (Definition):

**Custom Exceptions** អនុញ្ញាតឱ្យអ្នកបង្កើត exceptions ផ្ទាល់ខ្លួន ដើម្បីតំណាងឱ្យកំហុសជាក់លាក់ក្នុងអាជីវកម្ម (business-specific errors)។

```properties
// 1. Basic custom exception
public class ResourceNotFoundException extends RuntimeException {

    public ResourceNotFoundException(String message) {
        super(message);
    }

    public ResourceNotFoundException(String resourceName, String fieldName, Object fieldValue) {
        super(String.format("%s not found with %s : '%s'", resourceName, fieldName, fieldValue));
    }
}

// 2. Custom exception with HTTP status
@ResponseStatus(HttpStatus.BAD_REQUEST)
public class BusinessException extends RuntimeException {

    private final String errorCode;

    public BusinessException(String message) {
        super(message);
        this.errorCode = "BUSINESS_ERROR";
    }

    public BusinessException(String message, String errorCode) {
        super(message);
        this.errorCode = errorCode;
    }

    public String getErrorCode() {
        return errorCode;
    }
}

// 3. Custom exception with additional data
public class ValidationException extends RuntimeException {

    private final Map<String, String> validationErrors;

    public ValidationException(String message) {
        super(message);
        this.validationErrors = new HashMap<>();
    }

    public ValidationException(String message, Map<String, String> errors) {
        super(message);
        this.validationErrors = errors;
    }

    public Map<String, String> getValidationErrors() {
        return validationErrors;
    }

    public void addError(String field, String message) {
        validationErrors.put(field, message);
    }
}

// 4. Custom exception for duplicate data
public class DuplicateResourceException extends RuntimeException {

    private final String resourceName;
    private final String fieldName;
    private final Object fieldValue;

    public DuplicateResourceException(String resourceName, String fieldName, Object fieldValue) {
        super(String.format("%s already exists with %s : '%s'", resourceName, fieldName, fieldValue));
        this.resourceName = resourceName;
        this.fieldName = fieldName;
        this.fieldValue = fieldValue;
    }

    // Getters
}

// 5. Usage in service
@Service
public class UserService {

    @Autowired
    private UserRepository userRepository;

    public User findById(Long id) {
        return userRepository.findById(id)
                .orElseThrow(() -> new ResourceNotFoundException("User", "id", id));
    }

    public User createUser(UserRequest request) {
        if (userRepository.existsByEmail(request.getEmail())) {
            throw new DuplicateResourceException("User", "email", request.getEmail());
        }

        if (request.getAge() < 18) {
            throw new BusinessException("User must be at least 18 years old", "AGE_RESTRICTION");
        }

        return userRepository.save(new User(request));
    }

    public User updateUser(Long id, UserRequest request) {
        User user = findById(id);

        if (!user.getEmail().equals(request.getEmail()) &&
            userRepository.existsByEmail(request.getEmail())) {
            throw new DuplicateResourceException("User", "email", request.getEmail());
        }

        user.setName(request.getName());
        user.setEmail(request.getEmail());
        user.setAge(request.getAge());

        return userRepository.save(user);
    }
}

// 6. Exception handling for custom exceptions
@RestControllerAdvice
public class ExceptionHandlerAdvice {

    @ExceptionHandler(ResourceNotFoundException.class)
    public ResponseEntity<ErrorResponse> handleNotFound(ResourceNotFoundException ex) {
        return ResponseEntity.status(HttpStatus.NOT_FOUND)
                .body(new ErrorResponse(HttpStatus.NOT_FOUND.value(), ex.getMessage()));
    }

    @ExceptionHandler(DuplicateResourceException.class)
    public ResponseEntity<ErrorResponse> handleDuplicate(DuplicateResourceException ex) {
        return ResponseEntity.status(HttpStatus.CONFLICT)
                .body(new ErrorResponse(HttpStatus.CONFLICT.value(), ex.getMessage()));
    }

    @ExceptionHandler(BusinessException.class)
    public ResponseEntity<ErrorResponse> handleBusiness(BusinessException ex) {
```

ErrorResponse error = new ErrorResponse(

HttpStatus.BAD_REQUEST.value(),

ex.getMessage(),

ex.getErrorCode()

```java
        );
        return ResponseEntity.badRequest().body(error);
    }
}
```

## 9.8. API Error Response (ការឆ្លើយតបកំហុសរបស់ API)

### 📌 និយមន័យ (Definition):

**API Error Response** គឺជារចនាសម្ព័ន្ធស្តង់ដារ (standard structure) សម្រាប់ប្រគល់ error information ទៅកាន់ client។ វាជួយឱ្យ client ងាយស្រួលយល់ និងដោះស្រាយកំហុស។

```properties
import com.fasterxml.jackson.annotation.JsonInclude;
import lombok.Builder;
import lombok.Data;
import java.time.LocalDateTime;
import java.util.List;
import java.util.Map;

@Data
@Builder
@JsonInclude(JsonInclude.Include.NON_NULL)
public class ErrorResponse {

    private LocalDateTime timestamp;
    private int status;
    private String error;
    private String message;
    private String path;
    private String errorCode;
    private Map<String, String> validationErrors;
    private List<String> details;

    // Constructors
    public ErrorResponse() {}

    public ErrorResponse(LocalDateTime timestamp, int status, String error,
                         String message, String path, String errorCode,
                         Map<String, String> validationErrors, List<String> details) {
        this.timestamp = timestamp;
        this.status = status;
        this.error = error;
        this.message = message;
        this.path = path;
        this.errorCode = errorCode;
        this.validationErrors = validationErrors;
        this.details = details;
    }

    // Static factory methods
    public static ErrorResponse of(HttpStatus status, String message) {
        return ErrorResponse.builder()
```

.timestamp(LocalDateTime.now())

.status(status.value())

.error(status.getReasonPhrase())

.message(message)

```text
                .build();
    }

    public static ErrorResponse of(HttpStatus status, String message, String path) {
        return ErrorResponse.builder()
```

.timestamp(LocalDateTime.now())

.status(status.value())

.error(status.getReasonPhrase())

.message(message)

.path(path)

```text
                .build();
    }

    public static ErrorResponse of(HttpStatus status, String message, Map<String, String> validationErrors) {
        return ErrorResponse.builder()
```

.timestamp(LocalDateTime.now())

.status(status.value())

.error(status.getReasonPhrase())

.message(message)

.validationErrors(validationErrors)

```java
                .build();
    }
}

// Example response:
// {
//   "timestamp": "2024-01-15T10:30:00",
//   "status": 400,
//   "error": "Bad Request",
//   "message": "Validation failed",
//   "path": "/api/users",
//   "validationErrors": {
//     "email": "Email must be valid",
//     "age": "Age must be at least 18"
//   }
// }

// Complete Global Exception Handler with ErrorResponse
@RestControllerAdvice
@Slf4j
public class GlobalExceptionHandler {

    @ExceptionHandler(MethodArgumentNotValidException.class)
    public ResponseEntity<ErrorResponse> handleValidationExceptions(
```

MethodArgumentNotValidException ex,

```text
            HttpServletRequest request) {

        Map<String, String> errors = new HashMap<>();
        ex.getBindingResult().getAllErrors().forEach((error) -> {
            String fieldName = ((FieldError) error).getField();
            String errorMessage = error.getDefaultMessage();
            errors.put(fieldName, errorMessage);
        });
```

ErrorResponse errorResponse = ErrorResponse.of(

HttpStatus.BAD_REQUEST,

"Validation failed",

request.getRequestURI()

```java
        );
        errorResponse.setValidationErrors(errors);

        log.error("Validation error: {}", errors);
        return new ResponseEntity<>(errorResponse, HttpStatus.BAD_REQUEST);
    }

    @ExceptionHandler(ResourceNotFoundException.class)
    public ResponseEntity<ErrorResponse> handleResourceNotFound(
```

ResourceNotFoundException ex,

```text
            HttpServletRequest request) {
```

ErrorResponse errorResponse = ErrorResponse.of(

HttpStatus.NOT_FOUND,

ex.getMessage(),

request.getRequestURI()

```java
        );

        log.error("Resource not found: {}", ex.getMessage());
        return new ResponseEntity<>(errorResponse, HttpStatus.NOT_FOUND);
    }

    @ExceptionHandler(DuplicateResourceException.class)
    public ResponseEntity<ErrorResponse> handleDuplicateResource(
```

DuplicateResourceException ex,

```text
            HttpServletRequest request) {
```

ErrorResponse errorResponse = ErrorResponse.of(

HttpStatus.CONFLICT,

ex.getMessage(),

request.getRequestURI()

```java
        );
        errorResponse.setErrorCode("DUPLICATE_RESOURCE");

        log.error("Duplicate resource: {}", ex.getMessage());
        return new ResponseEntity<>(errorResponse, HttpStatus.CONFLICT);
    }

    @ExceptionHandler(BusinessException.class)
    public ResponseEntity<ErrorResponse> handleBusinessException(
```

BusinessException ex,

```text
            HttpServletRequest request) {
```

ErrorResponse errorResponse = ErrorResponse.builder()

.timestamp(LocalDateTime.now())

.status(HttpStatus.BAD_REQUEST.value())

.error("Business Rule Violation")

.message(ex.getMessage())

.errorCode(ex.getErrorCode())

.path(request.getRequestURI())

```java
                .build();

        log.error("Business exception: {}", ex.getMessage());
        return new ResponseEntity<>(errorResponse, HttpStatus.BAD_REQUEST);
    }

    @ExceptionHandler(Exception.class)
    public ResponseEntity<ErrorResponse> handleGenericException(
```

Exception ex,

```text
            HttpServletRequest request) {
```

ErrorResponse errorResponse = ErrorResponse.of(

HttpStatus.INTERNAL_SERVER_ERROR,

"An unexpected error occurred. Please try again later.",

request.getRequestURI()

```java
        );

        log.error("Unexpected error: ", ex);
        return new ResponseEntity<>(errorResponse, HttpStatus.INTERNAL_SERVER_ERROR);
    }
}

// Controller Example with validation
@RestController
@RequestMapping("/api/users")
@Validated
public class UserController {

    @Autowired
    private UserService userService;

    @PostMapping
    public ResponseEntity<UserResponse> createUser(@Valid @RequestBody UserRequest request) {
        User user = userService.createUser(request);
        return ResponseEntity.status(HttpStatus.CREATED).body(UserResponse.from(user));
    }

    @GetMapping("/{id}")
    public ResponseEntity<UserResponse> getUser(@PathVariable @Min(1) Long id) {
        User user = userService.findById(id);
        return ResponseEntity.ok(UserResponse.from(user));
    }

    @PutMapping("/{id}")
    public ResponseEntity<UserResponse> updateUser(
            @PathVariable Long id,
            @Valid @RequestBody UserRequest request) {
        User user = userService.updateUser(id, request);
        return ResponseEntity.ok(UserResponse.from(user));
    }

    @DeleteMapping("/{id}")
    public ResponseEntity<Void> deleteUser(@PathVariable Long id) {
        userService.deleteUser(id);
        return ResponseEntity.noContent().build();
    }
}
```

### 💡 Best Practices for Error Responses:

- ប្រើ **consistent error structure** សម្រាប់ API endpoints ទាំងអស់

- រួមបញ្ចូល **timestamp** ដើម្បីដឹងថាពេលណាមានកំហុស

- ប្រើ **appropriate HTTP status codes** (400, 404, 409, 500, etc.)

- ផ្តល់ **meaningful error messages** ដែលងាយយល់សម្រាប់ client developers

- កុំបង្ហាញ **stack traces** ក្នុង production (use logging instead)

- ប្រើ **error codes** សម្រាប់ client ដើម្បីដោះស្រាយ errors programmatically

- ផ្តល់ **validation errors details** (field name + error message) សម្រាប់ bad requests

### 📚 សង្ខេបមេរៀនទី៩ (Module 9 Summary)

នៅក្នុងមេរៀននេះ អ្នកបានរៀនអំពី Validation & Exception Handling នៅក្នុង Spring Boot៖

- **Bean Validation** – JSR-303/JSR-380 specification for Java object validation

```text
@Valid Annotation – Triggers validation on method parameters (@RequestBody, @PathVariable, @RequestParam)
```

- **Validation Constraints** – @NotNull, @NotBlank, @Size, @Min, @Max, @Email, @Pattern, @Past, @Future, etc.

- **Custom Validation** – Create custom annotations with validators for business-specific rules

- **Global Exception Handling** – Centralized exception management with @ControllerAdvice

```java
@ControllerAdvice / @RestControllerAdvice – Handle exceptions across all controllers
```

- **Custom Exceptions** – Business-specific exceptions (ResourceNotFoundException, DuplicateResourceException, BusinessException)

- **API Error Response** – Standard error structure with timestamp, status, message, validation errors

# មេរៀនទី១០: Spring Security (សន្តិសុខក្នុង Spring Boot)

### 📖 សេចក្តីផ្តើម (Introduction):
Spring Security គឺជា framework ដ៏មានអានុភាពសម្រាប់ការពារ (secure) Spring Boot applications។ វាផ្តល់នូវ authentication (ការផ្ទៀងផ្ទាត់អត្តសញ្ញាណ) និង authorization (ការអនុញ្ញាត) សម្រាប់កម្មវិធីរបស់អ្នក។ មេរៀននេះនឹងបង្រៀនអ្នកពី Introduction to Security, Authentication, Authorization, Spring Security Setup, Password Encoding, UserDetailsService, Role-Based Access, JWT Authentication, Security Filters, OAuth2 Login, CORS Configuration, និង CSRF Protection។

## 10.1. សេចក្តីផ្តើមអំពីសន្តិសុខ (Introduction to Security)

### 📌 និយមន័យ (Definition):

**Spring Security** គឺជា framework ដែលផ្តល់នូវ authentication, authorization, និងការការពារប្រឆាំងនឹងការវាយប្រហារទូទៅ (common attacks) សម្រាប់ Spring-based applications។ វាគឺជាស្តង់ដារសម្រាប់ការអនុវត្តសន្តិសុខក្នុង Spring Boot។

### 🔹 គោលការណ៍សំខាន់ៗនៃសន្តិសុខ (Core Security Concepts):

**Authentication**

ការផ្ទៀងផ្ទាត់អត្តសញ្ញាណ — អ្នកជានរណា? (Who are you?)

Login with username/password

**Authorization**

ការអនុញ្ញាត — អ្នកអាចធ្វើអ្វីខ្លះ? (What can you do?)

Role-based access control

**Principal**

អ្នកប្រើប្រាស់ដែលបានផ្ទៀងផ្ទាត់ (Authenticated user)

Currently logged-in user

### 💡 Common Security Threats:

- **CSRF (Cross-Site Request Forgery)** – ការវាយប្រហារដែលបញ្ឆោតអ្នកប្រើប្រាស់ឱ្យធ្វើសកម្មភាពដោយមិនដឹងខ្លួន

- **XSS (Cross-Site Scripting)** – ការបញ្ចូល script ពុលទៅក្នុង web pages

- **SQL Injection** – ការបញ្ចូល SQL code ពុលទៅក្នុង queries

- **Session Fixation** – ការលួច session ID របស់អ្នកប្រើប្រាស់

- **Clickjacking** – ការបញ្ឆោតអ្នកប្រើប្រាស់ឱ្យចុចលើអ្វីដែលខុសពីការពិត

## 10.2. Authentication (ការផ្ទៀងផ្ទាត់អត្តសញ្ញាណ)

### 📌 និយមន័យ (Definition):

**Authentication** គឺជាដំណើរការនៃការផ្ទៀងផ្ទាត់អត្តសញ្ញាណរបស់អ្នកប្រើប្រាស់ (verifying who a user is)។ វាជាធម្មតាត្រូវបានធ្វើតាមរយៈ username/email និង password។

```java
import org.springframework.security.core.Authentication;
import org.springframework.security.core.context.SecurityContextHolder;
import org.springframework.web.bind.annotation.*;

@RestController
@RequestMapping("/api/auth")
public class AuthController {

    // Get current authenticated user
    @GetMapping("/me")
    public ResponseEntity<UserInfo> getCurrentUser() {
        Authentication authentication = SecurityContextHolder.getContext().getAuthentication();

        if (authentication == null || !authentication.isAuthenticated()) {
            return ResponseEntity.status(HttpStatus.UNAUTHORIZED).build();
        }

        String username = authentication.getName();
        List<String> roles = authentication.getAuthorities().stream()
```

.map(GrantedAuthority::getAuthority)

```java
                .collect(Collectors.toList());

        return ResponseEntity.ok(new UserInfo(username, roles));
    }

    // Check if user is authenticated
    @GetMapping("/check")
    public ResponseEntity<Map<String, Boolean>> checkAuthentication() {
        boolean isAuthenticated = SecurityContextHolder.getContext().getAuthentication() != null &&
```

SecurityContextHolder.getContext().getAuthentication().isAuthenticated() &&

```java
                !(SecurityContextHolder.getContext().getAuthentication() instanceof AnonymousAuthenticationToken);

        return ResponseEntity.ok(Map.of("authenticated", isAuthenticated));
    }
}
```

## 10.3. Authorization (ការអនុញ្ញាត)

### 📌 និយមន័យ (Definition):

**Authorization** គឺជាដំណើរការនៃការកំណត់ថាតើអ្នកប្រើប្រាស់ដែលបានផ្ទៀងផ្ទាត់ អាចចូលប្រើ (access) ធនធាន ឬអនុវត្តសកម្មភាពអ្វីខ្លះ (what a user can do)។

```java
import org.springframework.security.access.prepost.PreAuthorize;
import org.springframework.security.core.annotation.AuthenticationPrincipal;
import org.springframework.web.bind.annotation.*;

@RestController
@RequestMapping("/api/admin")
public class AdminController {

    // Only users with ADMIN role can access
    @GetMapping("/users")
    @PreAuthorize("hasRole('ADMIN')")
    public List<User> getAllUsers() {
        return userService.findAll();
    }

    // Only users with ADMIN or MANAGER role can access
    @GetMapping("/reports")
    @PreAuthorize("hasAnyRole('ADMIN', 'MANAGER')")
    public List<Report> getReports() {
        return reportService.findAll();
    }

    // Only the user themselves can access their own data
    @GetMapping("/profile/{userId}")
    @PreAuthorize("#userId == authentication.principal.id or hasRole('ADMIN')")
    public User getUserProfile(@PathVariable Long userId) {
        return userService.findById(userId);
    }

    // Method-level security
    @PostMapping("/users")
    @PreAuthorize("hasAuthority('USER_CREATE')")
    public User createUser(@RequestBody User user) {
        return userService.save(user);
    }

    // Using @AuthenticationPrincipal to get current user
    @GetMapping("/my-profile")
    public User getMyProfile(@AuthenticationPrincipal User user) {
        return user;
    }
}
```

## 10.4. Spring Security Setup (ការដំឡើង Spring Security)

### 📌 ជំហានដំឡើង:

### 🔹 Maven Dependencies:

```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-security</artifactId>
</dependency>

<!-- Optional: Thymeleaf Security integration -->
<dependency>
    <groupId>org.thymeleaf.extras</groupId>
    <artifactId>thymeleaf-extras-springsecurity6</artifactId>
</dependency>
```

### 🔹 Basic Security Configuration:

```java
import org.springframework.context.annotation.Bean;
import org.springframework.context.annotation.Configuration;
import org.springframework.security.config.annotation.web.builders.HttpSecurity;
import org.springframework.security.config.annotation.web.configuration.EnableWebSecurity;
import org.springframework.security.core.userdetails.User;
import org.springframework.security.core.userdetails.UserDetails;
import org.springframework.security.core.userdetails.UserDetailsService;
import org.springframework.security.provisioning.InMemoryUserDetailsManager;
import org.springframework.security.web.SecurityFilterChain;

@Configuration
@EnableWebSecurity
public class SecurityConfig {

    @Bean
    public SecurityFilterChain securityFilterChain(HttpSecurity http) throws Exception {
```

http

.authorizeHttpRequests(auth -> auth

```text
                // Public endpoints - no authentication required
```

.requestMatchers("/", "/index", "/home", "/public/**", "/api/auth/**").permitAll()

```text
                // Static resources
```

.requestMatchers("/css/**", "/js/**", "/images/**").permitAll()

```text
                // Admin only
```

.requestMatchers("/admin/**").hasRole("ADMIN")

```text
                // Manager or Admin
```

.requestMatchers("/manager/**").hasAnyRole("MANAGER", "ADMIN")

```text
                // Authenticated users only
```

.anyRequest().authenticated()

)

.formLogin(form -> form

.loginPage("/login")

.defaultSuccessUrl("/dashboard")

.permitAll()

)

.logout(logout -> logout

.logoutSuccessUrl("/")

.permitAll()

)

.rememberMe(remember -> remember

.key("uniqueAndSecret")

.tokenValiditySeconds(86400) // 24 hours

```text
            );

        return http.build();
    }

    @Bean
    public UserDetailsService userDetailsService() {
```

UserDetails user = User.builder()

.username("user")

```text
                .password("{bcrypt}$2a$10$dXJ3SW6G7P50lGmMkkmwe.20cQQubK3.HZWzG3YB1tlRy.fqvM/BG") // "password"
```

.roles("USER")

```text
                .build();
```

UserDetails admin = User.builder()

.username("admin")

```text
                .password("{bcrypt}$2a$10$dXJ3SW6G7P50lGmMkkmwe.20cQQubK3.HZWzG3YB1tlRy.fqvM/BG")
```

.roles("ADMIN")

```text
                .build();

        return new InMemoryUserDetailsManager(user, admin);
    }
}
```

## 10.5. Password Encoding (ការអ៊ិនគ្រីបពាក្យសម្ងាត់)

### 📌 និយមន័យ (Definition):

**Password Encoding** គឺជាការបំលែងពាក្យសម្ងាត់ធម្មតា (plain text) ទៅជាទម្រង់ដែលមិនអាចអានបាន (hashed) ដើម្បីការពារការលួចទិន្នន័យ។ Spring Security ផ្តល់ PasswordEncoder interface និង implementations ដូចជា BCrypt, Argon2, PBKDF2។

```java
import org.springframework.context.annotation.Bean;
import org.springframework.context.annotation.Configuration;
import org.springframework.security.crypto.bcrypt.BCryptPasswordEncoder;
import org.springframework.security.crypto.password.PasswordEncoder;
import org.springframework.security.crypto.argon2.Argon2PasswordEncoder;
import org.springframework.security.crypto.password.Pbkdf2PasswordEncoder;

@Configuration
public class PasswordEncoderConfig {

    // BCrypt - Recommended (slow, salt included)
    @Bean
    public PasswordEncoder passwordEncoder() {
        return new BCryptPasswordEncoder();
        // or with strength: new BCryptPasswordEncoder(10);
    }

    // Argon2 - Most secure but slower
    public PasswordEncoder argon2PasswordEncoder() {
        return new Argon2PasswordEncoder(16, 32, 1, 6000, 10);
    }

    // PBKDF2 - Good alternative
    public PasswordEncoder pbkdf2PasswordEncoder() {
        return new Pbkdf2PasswordEncoder("secret", 185000, 256);
    }
}

// Usage in Service
@Service
public class UserService {

    @Autowired
    private PasswordEncoder passwordEncoder;

    public User registerUser(RegisterRequest request) {
        User user = new User();
        user.setUsername(request.getUsername());
        user.setEmail(request.getEmail());

        // Encode password before saving to database
        String encodedPassword = passwordEncoder.encode(request.getPassword());
        user.setPassword(encodedPassword);

        return userRepository.save(user);
    }

    public boolean verifyPassword(String rawPassword, String encodedPassword) {
        return passwordEncoder.matches(rawPassword, encodedPassword);
    }
}

// Custom UserDetails with password encoding
@Entity
public class AppUser {
    @Id
    private Long id;
    private String username;
    private String password; // Store encoded password
    private String role;
}

@Service
public class CustomUserDetailsService implements UserDetailsService {

    @Autowired
    private UserRepository userRepository;

    @Override
    public UserDetails loadUserByUsername(String username) throws UsernameNotFoundException {
```

AppUser appUser = userRepository.findByUsername(username)

```text
                .orElseThrow(() -> new UsernameNotFoundException("User not found"));

        return User.builder()
```

.username(appUser.getUsername())

.password(appUser.getPassword()) // Already encoded

.roles(appUser.getRole())

```java
                .build();
    }
}

// Password encoding utilities
@Service
public class PasswordUtils {

    @Autowired
    private PasswordEncoder passwordEncoder;

    // Generate encoded password for testing
    public String encodePassword(String rawPassword) {
        return passwordEncoder.encode(rawPassword);
    }

    // Check password strength
    public boolean isStrongPassword(String password) {
        return password != null &&
```

password.length() >= 8 &&

```text
               password.matches(".*[A-Z].*") && // Has uppercase
               password.matches(".*[a-z].*") && // Has lowercase
               password.matches(".*\d.*") &&    // Has digit
               password.matches(".*[!@#$%^&*].*"); // Has special char
    }
}
```

## 10.6. UserDetailsService

### 📌 និយមន័យ (Definition):

**UserDetailsService** គឺជា core interface ដែល Spring Security ប្រើដើម្បីទាញយក (retrieve) user information ពី database។ អ្នកត្រូវ implement interface នេះ ដើម្បីភ្ជាប់ Spring Security ជាមួយ database របស់អ្នក។

```properties
import org.springframework.security.core.userdetails.UserDetails;
import org.springframework.security.core.userdetails.UserDetailsService;
import org.springframework.security.core.userdetails.UsernameNotFoundException;
import org.springframework.stereotype.Service;
import org.springframework.security.core.authority.SimpleGrantedAuthority;
import java.util.stream.Collectors;

@Entity
@Table(name = "users")
public class AppUser {
    @Id
    @GeneratedValue
    private Long id;

    @Column(unique = true)
    private String username;

    private String password;

    private String email;

    private boolean enabled = true;

    @ManyToMany(fetch = FetchType.EAGER)
    @JoinTable(
        name = "user_roles",
        joinColumns = @JoinColumn(name = "user_id"),
        inverseJoinColumns = @JoinColumn(name = "role_id")
```

)

```properties
    private Set<Role> roles = new HashSet<>();

    // Getters and setters
}

@Entity
@Table(name = "roles")
public class Role {
    @Id
    @GeneratedValue
    private Long id;

    @Column(unique = true)
    private String name; // e.g., "ROLE_USER", "ROLE_ADMIN"

    // Getters and setters
}

// Custom UserDetails implementation
public class CustomUserDetails implements UserDetails {

    private final AppUser user;

    public CustomUserDetails(AppUser user) {
        this.user = user;
    }

    @Override
    public Collection<? extends GrantedAuthority> getAuthorities() {
        return user.getRoles().stream()
```

.map(role -> new SimpleGrantedAuthority(role.getName()))

```java
                .collect(Collectors.toList());
    }

    @Override
    public String getPassword() {
        return user.getPassword();
    }

    @Override
    public String getUsername() {
        return user.getUsername();
    }

    @Override
    public boolean isAccountNonExpired() {
        return true;
    }

    @Override
    public boolean isAccountNonLocked() {
        return true;
    }

    @Override
    public boolean isCredentialsNonExpired() {
        return true;
    }

    @Override
    public boolean isEnabled() {
        return user.isEnabled();
    }

    public Long getId() {
        return user.getId();
    }

    public String getEmail() {
        return user.getEmail();
    }
}

// UserDetailsService implementation
@Service
public class CustomUserDetailsService implements UserDetailsService {

    @Autowired
    private UserRepository userRepository;

    @Override
    public UserDetails loadUserByUsername(String username) throws UsernameNotFoundException {
```

AppUser user = userRepository.findByUsername(username)

```java
                .orElseThrow(() -> new UsernameNotFoundException("User not found with username: " + username));

        return new CustomUserDetails(user);
    }
}

// Security Configuration with custom UserDetailsService
@Configuration
@EnableWebSecurity
public class SecurityConfig {

    @Autowired
    private CustomUserDetailsService userDetailsService;

    @Autowired
    private PasswordEncoder passwordEncoder;

    @Bean
    public AuthenticationProvider authenticationProvider() {
        DaoAuthenticationProvider provider = new DaoAuthenticationProvider();
        provider.setUserDetailsService(userDetailsService);
        provider.setPasswordEncoder(passwordEncoder);
        return provider;
    }

    @Bean
    public SecurityFilterChain securityFilterChain(HttpSecurity http) throws Exception {
```

http

.authenticationProvider(authenticationProvider())

.authorizeHttpRequests(auth -> auth

.requestMatchers("/api/auth/**").permitAll()

.anyRequest().authenticated()

)

```java
            .formLogin(Customizer.withDefaults());

        return http.build();
    }
}

// Repository
@Repository
public interface UserRepository extends JpaRepository<AppUser, Long> {
    Optional<AppUser> findByUsername(String username);
    Optional<AppUser> findByEmail(String email);
    boolean existsByUsername(String username);
}
```

## 10.7. Role-Based Access (ការចូលប្រើតាមតួនាទី)

### 📌 និយមន័យ (Definition):

**Role-Based Access Control (RBAC)** គឺជាវិធីសាស្រ្តកំណត់សិទ្ធិចូលប្រើ ដោយផ្អែកលើតួនាទី (roles) របស់អ្នកប្រើប្រាស់។ អ្នកអាចប្រើ @PreAuthorize,@Secured, @RolesAllowed annotations។

```properties
import org.springframework.security.access.annotation.Secured;
import org.springframework.security.access.prepost.PreAuthorize;
import javax.annotation.security.RolesAllowed;

@RestController
@RequestMapping("/api")
public class RoleBasedController {

    // Method 1: Using @PreAuthorize (recommended)
    @GetMapping("/admin/data")
    @PreAuthorize("hasRole('ADMIN')")
    public String adminData() {
        return "Only ADMIN can see this";
    }

    @GetMapping("/manager/data")
    @PreAuthorize("hasAnyRole('ADMIN', 'MANAGER')")
    public String managerData() {
        return "ADMIN or MANAGER can see this";
    }

    @GetMapping("/user/data")
    @PreAuthorize("hasRole('USER')")
    public String userData() {
        return "Only USER can see this";
    }

    // Method 2: Using @Secured (requires @EnableGlobalMethodSecurity)
    @Secured("ROLE_ADMIN")
    @GetMapping("/secured-admin")
    public String securedAdmin() {
        return "Secured with @Secured";
    }

    // Method 3: Using @RolesAllowed (JSR-250)
    @RolesAllowed({"ADMIN", "MANAGER"})
    @GetMapping("/roles-allowed")
    public String rolesAllowed() {
        return "Using @RolesAllowed";
    }

    // Method level security with conditions
    @PreAuthorize("hasRole('ADMIN') or #id == authentication.principal.id")
    @GetMapping("/users/{id}")
    public User getUserById(@PathVariable Long id) {
        return userService.findById(id);
    }

    // Using SpEL expressions
    @PreAuthorize("hasRole('ADMIN') and hasAuthority('USER_DELETE')")
    @DeleteMapping("/users/{id}")
    public void deleteUser(@PathVariable Long id) {
        userService.delete(id);
    }
}

// Enable method security
@Configuration
@EnableGlobalMethodSecurity(
    prePostEnabled = true,  // Enable @PreAuthorize, @PostAuthorize
    securedEnabled = true,   // Enable @Secured
    jsr250Enabled = true     // Enable @RolesAllowed
```

)

```java
public class MethodSecurityConfig {
    // Configuration
}

// Service with role-based methods
@Service
public class ProductService {

    @PreAuthorize("hasRole('ADMIN')")
    public Product createProduct(Product product) {
        return productRepository.save(product);
    }

    @PreAuthorize("hasAnyRole('ADMIN', 'MANAGER')")
    public Product updateProduct(Long id, Product product) {
        return productRepository.save(product);
    }

    @PreAuthorize("isAuthenticated()")
    public List<Product> getAllProducts() {
        return productRepository.findAll();
    }

    @PostAuthorize("returnObject.owner == authentication.principal.username")
    public Product getProductForOwner(Long id) {
        return productRepository.findById(id).orElseThrow();
    }
}
```

## 10.8. JWT Authentication (ការផ្ទៀងផ្ទាត់ដោយ JWT)

### 📌 និយមន័យ (Definition):

**JWT (JSON Web Token)** គឺជា standard (RFC 7519) សម្រាប់បង្កើត tokens ដែលផ្ទុកទិន្នន័យក្នុងទម្រង់ JSON។ JWT ត្រូវបានប្រើយ៉ាងទូលំទូលាយសម្រាប់ authentication និង authorization ក្នុង REST APIs (stateless)។

### 🔹 Maven Dependency:

```xml
<dependency>
    <groupId>io.jsonwebtoken</groupId>
    <artifactId>jjwt-api</artifactId>
    <version>0.11.5</version>
</dependency>
<dependency>
    <groupId>io.jsonwebtoken</groupId>
    <artifactId>jjwt-impl</artifactId>
    <version>0.11.5</version>
    <scope>runtime</scope>
</dependency>
<dependency>
    <groupId>io.jsonwebtoken</groupId>
    <artifactId>jjwt-jackson</artifactId>
    <version>0.11.5</version>
    <scope>runtime</scope>
</dependency>
```

## 10.9. JWT Access Token

### 📌 JWT Access Token:

```java
import io.jsonwebtoken.*;
import io.jsonwebtoken.security.Keys;
import org.springframework.stereotype.Component;
import java.security.Key;
import java.util.Date;
import java.util.function.Function;

@Component
public class JwtTokenProvider {

    private static final String SECRET_KEY = "your-256-bit-secret-key-for-jwt-signature-must-be-long-enough";
    private static final long EXPIRATION_TIME = 86400000; // 24 hours in milliseconds

    private Key getSigningKey() {
        byte[] keyBytes = SECRET_KEY.getBytes();
        return Keys.hmacShaKeyFor(keyBytes);
    }

    // Generate token
    public String generateToken(String username, List<String> roles) {
        Date now = new Date();
        Date expiryDate = new Date(now.getTime() + EXPIRATION_TIME);

        return Jwts.builder()
```

.setSubject(username)

.claim("roles", roles)

.setIssuedAt(now)

.setExpiration(expiryDate)

.signWith(getSigningKey(), SignatureAlgorithm.HS256)

```java
                .compact();
    }

    // Extract username from token
    public String getUsernameFromToken(String token) {
        return getClaimFromToken(token, Claims::getSubject);
    }

    // Extract expiration date
    public Date getExpirationDateFromToken(String token) {
        return getClaimFromToken(token, Claims::getExpiration);
    }

    // Extract roles
    @SuppressWarnings("unchecked")
    public List<String> getRolesFromToken(String token) {
        Claims claims = getAllClaimsFromToken(token);
        return claims.get("roles", List.class);
    }

    public <T> T getClaimFromToken(String token, Function<Claims, T> claimsResolver) {
        final Claims claims = getAllClaimsFromToken(token);
        return claimsResolver.apply(claims);
    }

    private Claims getAllClaimsFromToken(String token) {
        return Jwts.parserBuilder()
```

.setSigningKey(getSigningKey())

.build()

.parseClaimsJws(token)

```java
                .getBody();
    }

    // Check if token is expired
    private Boolean isTokenExpired(String token) {
        final Date expiration = getExpirationDateFromToken(token);
        return expiration.before(new Date());
    }

    // Validate token
    public Boolean validateToken(String token, UserDetails userDetails) {
        final String username = getUsernameFromToken(token);
        return (username.equals(userDetails.getUsername()) && !isTokenExpired(token));
    }
}
```

## 10.10. Refresh Token

### 📌 Refresh Token:

```java
import javax.persistence.*;
import java.time.LocalDateTime;

@Entity
@Table(name = "refresh_tokens")
public class RefreshToken {
    @Id
    @GeneratedValue
    private Long id;

    @Column(unique = true)
    private String token;

    @OneToOne
    @JoinColumn(name = "user_id")
    private AppUser user;

    private LocalDateTime expiryDate;

    // Getters and setters
}

@Service
public class RefreshTokenService {

    @Autowired
    private RefreshTokenRepository refreshTokenRepository;

    private static final long REFRESH_TOKEN_DURATION = 7 * 24 * 60 * 60 * 1000; // 7 days

    public RefreshToken createRefreshToken(AppUser user) {
        RefreshToken refreshToken = new RefreshToken();
        refreshToken.setToken(UUID.randomUUID().toString());
        refreshToken.setUser(user);
        refreshToken.setExpiryDate(LocalDateTime.now().plusDays(7));
        return refreshTokenRepository.save(refreshToken);
    }

    public Optional<RefreshToken> findByToken(String token) {
        return refreshTokenRepository.findByToken(token);
    }

    public RefreshToken verifyExpiration(RefreshToken token) {
        if (token.getExpiryDate().isBefore(LocalDateTime.now())) {
            refreshTokenRepository.delete(token);
            throw new RuntimeException("Refresh token expired");
        }
        return token;
    }
}

@RestController
@RequestMapping("/api/auth")
public class AuthController {

    @Autowired
    private JwtTokenProvider tokenProvider;

    @Autowired
    private RefreshTokenService refreshTokenService;

    @PostMapping("/refresh")
    public ResponseEntity<?> refreshToken(@RequestBody RefreshTokenRequest request) {
        String refreshToken = request.getRefreshToken();
```

RefreshToken token = refreshTokenService.findByToken(refreshToken)

```java
                .orElseThrow(() -> new RuntimeException("Refresh token not found"));

        refreshTokenService.verifyExpiration(token);

        AppUser user = token.getUser();
        String newAccessToken = tokenProvider.generateToken(user.getUsername(), getRoles(user));

        return ResponseEntity.ok(new JwtResponse(newAccessToken, refreshToken));
    }
}
```

## 10.11. Security Filters (Filters សម្រាប់សន្តិសុខ)

### 📌 និយមន័យ (Definition):

**Security Filters** គឺជា chain នៃ filters ដែល Spring Security ប្រើដើម្បី intercept requests, perform authentication, authorization, និងការការពារផ្សេងៗ។ អ្នកអាចបង្កើត custom filters ដើម្បីបន្ថែម logic ផ្ទាល់ខ្លួន។

```java
import org.springframework.web.filter.OncePerRequestFilter;
import javax.servlet.FilterChain;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;

@Component
public class JwtAuthenticationFilter extends OncePerRequestFilter {

    @Autowired
    private JwtTokenProvider tokenProvider;

    @Autowired
    private CustomUserDetailsService userDetailsService;

    @Override
    protected void doFilterInternal(HttpServletRequest request,
```

HttpServletResponse response,

```text
                                    FilterChain filterChain) throws ServletException, IOException {

        String jwt = getJwtFromRequest(request);

        if (StringUtils.hasText(jwt) && tokenProvider.validateToken(jwt)) {
            String username = tokenProvider.getUsernameFromToken(jwt);
            UserDetails userDetails = userDetailsService.loadUserByUsername(username);
```

UsernamePasswordAuthenticationToken authentication =

```java
                    new UsernamePasswordAuthenticationToken(userDetails, null, userDetails.getAuthorities());

            SecurityContextHolder.getContext().setAuthentication(authentication);
        }

        filterChain.doFilter(request, response);
    }

    private String getJwtFromRequest(HttpServletRequest request) {
        String bearerToken = request.getHeader("Authorization");
        if (StringUtils.hasText(bearerToken) && bearerToken.startsWith("Bearer ")) {
            return bearerToken.substring(7);
        }
        return null;
    }
}

// Register custom filter
@Configuration
@EnableWebSecurity
public class SecurityConfig {

    @Autowired
    private JwtAuthenticationFilter jwtAuthenticationFilter;

    @Bean
    public SecurityFilterChain securityFilterChain(HttpSecurity http) throws Exception {
```

http

.csrf().disable()

.authorizeHttpRequests(auth -> auth

.requestMatchers("/api/auth/**").permitAll()

.anyRequest().authenticated()

)

.sessionManagement(session -> session

.sessionCreationPolicy(SessionCreationPolicy.STATELESS)

)

```java
            .addFilterBefore(jwtAuthenticationFilter, UsernamePasswordAuthenticationFilter.class);

        return http.build();
    }
}

// Logging filter
@Component
public class RequestLoggingFilter extends OncePerRequestFilter {

    private static final Logger log = LoggerFactory.getLogger(RequestLoggingFilter.class);

    @Override
    protected void doFilterInternal(HttpServletRequest request,
```

HttpServletResponse response,

```text
                                    FilterChain filterChain) throws ServletException, IOException {

        long startTime = System.currentTimeMillis();

        log.info("Incoming request: {} {}", request.getMethod(), request.getRequestURI());
        log.info("Remote IP: {}", request.getRemoteAddr());

        filterChain.doFilter(request, response);

        long duration = System.currentTimeMillis() - startTime;
        log.info("Request completed in {} ms with status {}", duration, response.getStatus());
    }
}
```

## 10.12. OAuth2 Login

### 📌 និយមន័យ (Definition):

**OAuth2** គឺជា authorization framework ដែលអនុញ្ញាតឱ្យកម្មវិធីភាគីទីបី (third-party applications) ទទួលបាន access មានកំណត់ទៅកាន់ resources របស់អ្នកប្រើប្រាស់។ Spring Security ផ្តល់ OAuth2 client support សម្រាប់ការចូលតាមរយៈ Google, Facebook, GitHub, etc.

### 🔹 Maven Dependencies:

```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-oauth2-client</artifactId>
</dependency>
```

### 🔹 Application Configuration (application.yml):

```yaml
spring:
  security:
    oauth2:
      client:
        registration:
          google:
            client-id: YOUR_GOOGLE_CLIENT_ID
            client-secret: YOUR_GOOGLE_CLIENT_SECRET
            scope:
```

- email

- profile

```text
          facebook:
            client-id: YOUR_FACEBOOK_CLIENT_ID
            client-secret: YOUR_FACEBOOK_CLIENT_SECRET
            scope:
```

- email

- public_profile

```text
          github:
            client-id: YOUR_GITHUB_CLIENT_ID
            client-secret: YOUR_GITHUB_CLIENT_SECRET
            scope:
```

- read:user

- user:email

```text
        provider:
          google:
            authorization-uri: https://accounts.google.com/o/oauth2/auth
            token-uri: https://oauth2.googleapis.com/token
            user-info-uri: https://www.googleapis.com/oauth2/v3/userinfo
```

## 10.13. Google Login (ការចូលតាម Google)

### 📌 Google OAuth2 Setup:

```java
import org.springframework.security.oauth2.client.userinfo.DefaultOAuth2UserService;
import org.springframework.security.oauth2.client.userinfo.OAuth2UserRequest;
import org.springframework.security.oauth2.core.OAuth2AuthenticationException;
import org.springframework.security.oauth2.core.user.OAuth2User;
import org.springframework.stereotype.Service;

@Service
public class CustomOAuth2UserService extends DefaultOAuth2UserService {

    @Autowired
    private UserRepository userRepository;

    @Override
    public OAuth2User loadUser(OAuth2UserRequest userRequest) throws OAuth2AuthenticationException {
        OAuth2User oAuth2User = super.loadUser(userRequest);

        String email = oAuth2User.getAttribute("email");
        String name = oAuth2User.getAttribute("name");
        String provider = userRequest.getClientRegistration().getRegistrationId();

        // Find or create user
```

AppUser user = userRepository.findByEmail(email)

```java
                .orElseGet(() -> {
                    AppUser newUser = new AppUser();
                    newUser.setEmail(email);
                    newUser.setUsername(email);
                    newUser.setName(name);
                    newUser.setProvider(provider);
                    newUser.setRole("ROLE_USER");
                    return userRepository.save(newUser);
                });

        return new CustomOAuth2User(oAuth2User, user);
    }
}

@Configuration
@EnableWebSecurity
public class SecurityConfig {

    @Bean
    public SecurityFilterChain securityFilterChain(HttpSecurity http) throws Exception {
```

http

.authorizeHttpRequests(auth -> auth

.requestMatchers("/", "/login", "/oauth2/**").permitAll()

.anyRequest().authenticated()

)

.oauth2Login(oauth2 -> oauth2

.loginPage("/login")

.defaultSuccessUrl("/dashboard")

.userInfoEndpoint(userInfo -> userInfo

.userService(customOAuth2UserService())

)

```text
            );

        return http.build();
    }

    @Bean
    public CustomOAuth2UserService customOAuth2UserService() {
        return new CustomOAuth2UserService();
    }
}
```

## 10.14. CORS Configuration

### 📌 និយមន័យ (Definition):

**CORS (Cross-Origin Resource Sharing)** គឺជាយន្តការដែលអនុញ្ញាតឱ្យ web pages ស្នើសុំ resources ពី domain ផ្សេងពី domain ដើម (different origin)។ Spring Security តម្រូវឱ្យកំណត់ CORS configuration សម្រាប់ APIs ដែលត្រូវបានហៅពី frontend នៅ port ផ្សេង។

```java
import org.springframework.context.annotation.Bean;
import org.springframework.context.annotation.Configuration;
import org.springframework.web.cors.CorsConfiguration;
import org.springframework.web.cors.CorsConfigurationSource;
import org.springframework.web.cors.UrlBasedCorsConfigurationSource;
import org.springframework.web.servlet.config.annotation.CorsRegistry;
import org.springframework.web.servlet.config.annotation.WebMvcConfigurer;
import org.springframework.security.config.annotation.web.builders.HttpSecurity;
import java.util.Arrays;

@Configuration
public class CorsConfig {

    // Method 1: Global CORS configuration
    @Bean
    public WebMvcConfigurer corsConfigurer() {
        return new WebMvcConfigurer() {
            @Override
            public void addCorsMappings(CorsRegistry registry) {
```

registry.addMapping("/api/**")

.allowedOrigins("http://localhost:3000", "http://localhost:4200")

.allowedMethods("GET", "POST", "PUT", "DELETE", "OPTIONS")

.allowedHeaders("*")

.allowCredentials(true)

```java
                        .maxAge(3600);
            }
        };
    }

    // Method 2: CORS configuration source for Spring Security
    @Bean
    public CorsConfigurationSource corsConfigurationSource() {
        CorsConfiguration configuration = new CorsConfiguration();
        configuration.setAllowedOrigins(Arrays.asList("http://localhost:3000", "http://localhost:4200"));
        configuration.setAllowedMethods(Arrays.asList("GET", "POST", "PUT", "DELETE", "OPTIONS"));
        configuration.setAllowedHeaders(Arrays.asList("*"));
        configuration.setAllowCredentials(true);
        configuration.setMaxAge(3600L);

        UrlBasedCorsConfigurationSource source = new UrlBasedCorsConfigurationSource();
        source.registerCorsConfiguration("/**", configuration);
        return source;
    }
}

// Security configuration with CORS
@Configuration
@EnableWebSecurity
public class SecurityConfig {

    @Autowired
    private CorsConfigurationSource corsConfigurationSource;

    @Bean
    public SecurityFilterChain securityFilterChain(HttpSecurity http) throws Exception {
```

http

.cors(cors -> cors.configurationSource(corsConfigurationSource))

```text
            .csrf(csrf -> csrf.disable()) // Disable CSRF for stateless APIs
```

.authorizeHttpRequests(auth -> auth

.requestMatchers("/api/auth/**").permitAll()

.anyRequest().authenticated()

```java
            );

        return http.build();
    }
}

// Per-controller CORS
@RestController
@RequestMapping("/api/users")
@CrossOrigin(origins = "http://localhost:3000", maxAge = 3600)
public class UserController {

    // Per-method CORS
    @GetMapping("/{id}")
    @CrossOrigin(origins = "http://localhost:4200")
    public User getUser(@PathVariable Long id) {
        return userService.findById(id);
    }
}
```

## 10.15. CSRF Protection

### 📌 និយមន័យ (Definition):

**CSRF (Cross-Site Request Forgery)** គឺជាការវាយប្រហារដែលបញ្ឆោតអ្នកប្រើប្រាស់ ដែលបានផ្ទៀងផ្ទាត់រួចហើយ (authenticated user) ឱ្យធ្វើសកម្មភាពដែលពួកគេមិនមានបំណង។ Spring Security ផ្តល់ CSRF protection តាមលំនាំដើម (default) សម្រាប់ web applications ប៉ុន្តែអាច disable សម្រាប់ stateless REST APIs។

```java
import org.springframework.security.config.annotation.web.builders.HttpSecurity;
import org.springframework.security.web.csrf.CookieCsrfTokenRepository;
import org.springframework.security.web.csrf.CsrfTokenRequestAttributeHandler;
import org.springframework.security.web.csrf.HttpSessionCsrfTokenRepository;

@Configuration
@EnableWebSecurity
public class SecurityConfig {

    @Bean
    public SecurityFilterChain securityFilterChain(HttpSecurity http) throws Exception {

        // Option 1: Enable CSRF (default for web applications)
```

http

.csrf(csrf -> csrf

.csrfTokenRepository(CookieCsrfTokenRepository.withHttpOnlyFalse())

)

.authorizeHttpRequests(auth -> auth

.anyRequest().authenticated()

)

```java
            .formLogin(Customizer.withDefaults());

        return http.build();
    }
}

// For REST APIs (stateless) - Disable CSRF
@Configuration
@EnableWebSecurity
public class RestApiSecurityConfig {

    @Bean
    public SecurityFilterChain securityFilterChain(HttpSecurity http) throws Exception {
```

http

```text
            .csrf(csrf -> csrf.disable()) // Disable CSRF for stateless REST APIs
```

.sessionManagement(session -> session

.sessionCreationPolicy(SessionCreationPolicy.STATELESS)

)

.authorizeHttpRequests(auth -> auth

.requestMatchers("/api/auth/**").permitAll()

.anyRequest().authenticated()

```java
            );

        return http.build();
    }
}

// Custom CSRF token repository
@Configuration
public class CsrfConfig {

    @Bean
    public CsrfTokenRepository csrfTokenRepository() {
        HttpSessionCsrfTokenRepository repository = new HttpSessionCsrfTokenRepository();
        repository.setSessionAttributeName("_csrf");
        return repository;
    }
}

// Access CSRF token in Thymeleaf (for web apps)
/*
<form th:action="@{/logout}" method="post">
    <input type="submit" value="Logout"/>
</form>

<!-- CSRF token is automatically added -->

<!-- Manual CSRF token -->
<input type="hidden" th:name="undefined" th:value="undefined"/>
*/
```

### 💡 When to disable CSRF:

- **REST APIs** – Stateless APIs using JWT or OAuth2 (no session)

- **Mobile applications** – Mobile apps don't have CSRF vulnerabilities

- **External services** – Services that don't use browser cookies

### ⚠️ When to keep CSRF enabled:

- **Traditional web applications** – Using sessions and cookies

- **Browser-based applications** – Where users interact with forms

- **Admin panels** – Sensitive operations

### 📚 សង្ខេបមេរៀនទី១០ (Module 10 Summary)

នៅក្នុងមេរៀននេះ អ្នកបានរៀនអំពី Spring Security សម្រាប់ការពារកម្មវិធី Spring Boot៖

- **Authentication** – Verifying user identity (username/password, OAuth2, JWT)

- **Authorization** – Access control based on roles and permissions (@PreAuthorize, @Secured)

- **Password Encoding** – BCrypt, Argon2, PBKDF2 for secure password storage

- **UserDetailsService** – Custom user loading from database

- **JWT Authentication** – Stateless authentication with JSON Web Tokens

- **JWT Access Token & Refresh Token** – Token generation, validation, and refresh mechanism

- **Security Filters** – Custom filters for JWT validation, logging, etc.

- **OAuth2 Login** – Social login with Google, Facebook, GitHub

- **CORS Configuration** – Cross-origin resource sharing for frontend integration

- **CSRF Protection** – Protection against cross-site request forgery attacks

# មេរៀនទី១១: File Upload & Storage (ការផ្ទុកឯកសារ)

### 📖 សេចក្តីផ្តើម (Introduction):
File Upload គឺជាលក្ខណៈពិសេសសំខាន់មួយក្នុងកម្មវិធីទំនើបៗ — profile pictures, documents, images, videos។ Spring Boot ផ្តល់នូវការគាំទ្រយ៉ាងងាយស្រួលសម្រាប់ file upload តាមរយៈ MultipartFile។ មេរៀននេះនឹងបង្រៀនអ្នកពី Multipart File, Upload Single File, Upload Multiple Files, Download File, File Validation, Store File in Database, Store File in Server, និង Cloud Storage Basics។

## 11.1. Multipart File

### 📌 និយមន័យ (Definition):

**Multipart File** គឺជាប្រភេទ request ដែលអនុញ្ញាតឱ្យផ្ញើឯកសារ (files) និងទិន្នន័យ (data) ក្នុងពេលតែមួយតាមរយៈ HTTP។ Spring Boot ប្រើ MultipartFile interface ដើម្បីតំណាងឱ្យឯកសារដែលបានផ្ទុកឡើង (uploaded file)។

### 🔹 Multipart Configuration (application.properties):

```properties
# Max file size (default: 1MB)
spring.servlet.multipart.max-file-size=10MB
# Max request size
spring.servlet.multipart.max-request-size=10MB
# Enable multipart upload
spring.servlet.multipart.enabled=true
```

### 💡 Important Notes:

- Default max file size is **1MB** — configure larger values for bigger files

- Form must use enctype="multipart/form-data"

- Controller method must accept @RequestParam("file") MultipartFile file

## 11.2. Upload Single File

### 📌 វិធីផ្ទុកឯកសារតែមួយ:

```java
@RestController
@RequestMapping("/api/files")
public class FileUploadController {

    private static final String UPLOAD_DIR = "uploads/";

    @PostMapping("/upload")
    public ResponseEntity<Map<String, String>> uploadFile(
            @RequestParam("file") MultipartFile file) {
        try {
            if (file.isEmpty()) {
                return ResponseEntity.badRequest()
                        .body(Map.of("error", "Please select a file"));
            }
            String filename = file.getOriginalFilename();
            Path uploadPath = Paths.get(UPLOAD_DIR);
            if (!Files.exists(uploadPath)) {
                Files.createDirectories(uploadPath);
            }
            Path filePath = uploadPath.resolve(filename);
            file.transferTo(filePath.toFile());

            return ResponseEntity.ok(Map.of("message", "File uploaded successfully"));
        } catch (IOException e) {
            return ResponseEntity.internalServerError()
                    .body(Map.of("error", e.getMessage()));
        }
    }
}
```

## 11.3. Upload Multiple Files

### 📌 វិធីផ្ទុកឯកសារច្រើន:

```java
@PostMapping("/upload-multiple")
public ResponseEntity<Map<String, Object>> uploadMultipleFiles(
        @RequestParam("files") MultipartFile[] files) {

    List<String> uploadedFiles = new ArrayList<>();

    for (MultipartFile file : files) {
        if (!file.isEmpty()) {
            String filename = file.getOriginalFilename();
            uploadedFiles.add(filename);
        }
    }

    return ResponseEntity.ok(Map.of(
```

"uploadedFiles", uploadedFiles,

"totalUploaded", uploadedFiles.size()

```text
    ));
}
```

## 11.4. Download File

### 📌 វិធីទាញយកឯកសារ:

```java
@GetMapping("/download/{filename}")
public ResponseEntity<Resource> downloadFile(@PathVariable String filename) {
    try {
        Path filePath = Paths.get("uploads/" + filename);

        if (!Files.exists(filePath)) {
            return ResponseEntity.notFound().build();
        }

        Resource resource = new InputStreamResource(Files.newInputStream(filePath));
        String contentType = Files.probeContentType(filePath);

        return ResponseEntity.ok()
```

.contentType(MediaType.parseMediaType(contentType))

.header(HttpHeaders.CONTENT_DISPOSITION,

```java
                        "attachment; filename=\"" + filename + "\"")
                .body(resource);
    } catch (IOException e) {
        return ResponseEntity.internalServerError().build();
    }
}
```

## 11.5. File Validation

### 📌 ការផ្ទៀងផ្ទាត់ឯកសារ:

```java
@Component
public class FileValidator {

    private static final List<String> ALLOWED_EXTENSIONS =
        Arrays.asList("jpg", "jpeg", "png", "gif", "pdf", "doc", "docx");

    private static final long MAX_FILE_SIZE = 10 * 1024 * 1024; // 10MB

    public void validateFile(MultipartFile file) {
        if (file.isEmpty()) {
            throw new IllegalArgumentException("File is empty");
        }

        if (file.getSize() > MAX_FILE_SIZE) {
            throw new IllegalArgumentException("File size exceeds 10MB");
        }

        String filename = file.getOriginalFilename();
        String extension = filename.substring(filename.lastIndexOf(".") + 1);

        if (!ALLOWED_EXTENSIONS.contains(extension.toLowerCase())) {
            throw new IllegalArgumentException("File type not allowed");
        }
    }
}
```

## 11.6. Store File in Database

### 📌 ការរក្សាទុកឯកសារក្នុង Database:

```java
@Entity
@Table(name = "file_uploads")
public class FileEntity {
    @Id
    @GeneratedValue
    private Long id;
    private String fileName;
    private String fileType;
    private Long fileSize;
    @Lob
    private byte[] data;
    private LocalDateTime uploadedAt;
}

@Repository
public interface FileRepository extends JpaRepository<FileEntity, Long> {
    List<FileEntity> findByUserId(Long userId);
}

@Service
public class DatabaseFileStorageService {

    @Autowired
    private FileRepository fileRepository;

    public FileEntity storeFile(MultipartFile file) throws IOException {
        FileEntity fileEntity = new FileEntity();
        fileEntity.setFileName(file.getOriginalFilename());
        fileEntity.setFileType(file.getContentType());
        fileEntity.setFileSize(file.getSize());
        fileEntity.setData(file.getBytes());
        fileEntity.setUploadedAt(LocalDateTime.now());
        return fileRepository.save(fileEntity);
    }
}
```

## 11.7. Store File in Server

### 📌 ការរក្សាទុកឯកសារក្នុង Server:

```properties
@Service
public class ServerFileStorageService {

    private final Path fileStorageLocation;

    public ServerFileStorageService() {
        this.fileStorageLocation = Paths.get("uploads").toAbsolutePath().normalize();
        try {
            Files.createDirectories(this.fileStorageLocation);
        } catch (Exception ex) {
            throw new RuntimeException("Could not create upload directory", ex);
        }
    }

    public String storeFile(MultipartFile file) throws IOException {
        String fileName = System.currentTimeMillis() + "_" + file.getOriginalFilename();
        Path targetLocation = this.fileStorageLocation.resolve(fileName);
        Files.copy(file.getInputStream(), targetLocation, StandardCopyOption.REPLACE_EXISTING);
        return fileName;
    }
}
```

## 11.8. Cloud Storage Basics

### 📌 សេចក្តីផ្តើមអំពី Cloud Storage:

**Cloud Storage** គឺជាសេវាកម្មផ្ទុកឯកសារនៅលើ cloud ដូចជា AWS S3, Google Cloud Storage, Azure Blob Storage។ វាផ្តល់នូវ scalability, durability, និង accessibility ពីគ្រប់ទីកន្លែង។

### 🔹 Popular Cloud Storage Providers:

- **Amazon Web Services (AWS) S3** – Most popular, highly scalable

- **Google Cloud Storage** – Global edge caching, strong consistency

- **Microsoft Azure Blob Storage** – Integration with Microsoft ecosystem

- **DigitalOcean Spaces** – Simple pricing, CDN included

### 🔹 AWS S3 Maven Dependency:

```xml
<dependency>
    <groupId>com.amazonaws</groupId>
    <artifactId>aws-java-sdk-s3</artifactId>
    <version>1.12.500</version>
</dependency>
```

### 🔹 AWS S3 Configuration (application.properties):

```properties
cloud.aws.credentials.access-key=YOUR_ACCESS_KEY
cloud.aws.credentials.secret-key=YOUR_SECRET_KEY
cloud.aws.region.static=ap-southeast-1
cloud.aws.s3.bucket=my-spring-boot-bucket
```

### 🔹 AWS S3 Service Example:

```java
@Service
public class AwsS3Service {

    @Value("${cloud.aws.s3.bucket}")
    private String bucketName;

    @Autowired
    private AmazonS3 amazonS3;

    public String uploadFile(MultipartFile file, String folder) throws IOException {
        String fileName = folder + "/" + System.currentTimeMillis() + "_" + file.getOriginalFilename();
        amazonS3.putObject(bucketName, fileName, file.getInputStream(), null);
        return amazonS3.getUrl(bucketName, fileName).toString();
    }
}
```

### 📚 សង្ខេបមេរៀនទី១១ (Module 11 Summary)

នៅក្នុងមេរៀននេះ អ្នកបានរៀនអំពី File Upload & Storage នៅក្នុង Spring Boot៖

- **Multipart File** – @RequestParam("file") MultipartFile file

- **Upload Single File** – Save to server filesystem

- **Upload Multiple Files** – MultipartFile[] files array

- **Download File** – Resource, InputStreamResource

- **File Validation** – Check file size, extension, MIME type

- **Store in Database** – @Lob byte[] data, BLOB storage

- **Store in Server** – Filesystem storage

- **Cloud Storage Basics** – AWS S3, Google Cloud Storage, Azure Blob Storage

# មេរៀនទី១២: API Documentation (ការសរសេរឯកសារ API)

### 📖 សេចក្តីផ្តើម (Introduction):
API Documentation គឺជាផ្នែកសំខាន់មួយក្នុងការអភិវឌ្ឍន៍ API ដើម្បីឱ្យអ្នកអភិវឌ្ឍន៍ដទៃទៀតអាចយល់ និងប្រើប្រាស់ API របស់អ្នកបាន។ មេរៀននេះនឹងបង្រៀនអ្នកពី Swagger/OpenAPI, SpringDoc OpenAPI, API Testing, API Versioning, និង Postman Collection។

## 12.1. Swagger/OpenAPI

### 📌 និយមន័យ (Definition):

**OpenAPI (formerly Swagger)** គឺជា specification សម្រាប់ពិពណ៌នា (describe), បង្កើត (produce), ប្រើប្រាស់ (consume), និងមើល (visualize) RESTful APIs។ វាផ្តល់នូវស្តង់ដារមួយសម្រាប់ការសរសេរឯកសារ API។

### 🔹 OpenAPI Specification Features:

- **Machine-readable** – កម្មវិធីអាចអាន និងបកស្រាយបាន

- **Interactive Documentation** – Swagger UI ផ្តល់ interface សម្រាប់សាកល្បង API

- **Code Generation** – អាចបង្កើត client SDKs, server stubs

- **Language Agnostic** – ធ្វើការជាមួយភាសាសរសេរកម្មវិធីណាមួយ

### 💡 Benefits of OpenAPI:

- ឯកសារអាចធ្វើបច្ចុប្បន្នភាពដោយស្វ័យប្រវត្តិ

- អាចសាកល្បង API ដោយផ្ទាល់ពី browser

- កាត់បន្ថយការងារសរសេរឯកសារដោយដៃ

- ភាពស៊ីសង្វាក់គ្នារវាងកូដ និងឯកសារ

## 12.2. SpringDoc OpenAPI

### 📌 និយមន័យ (Definition):

**SpringDoc OpenAPI** គឺជា library ដែលបង្កើត OpenAPI 3.0 documentation ដោយស្វ័យប្រវត្តិ សម្រាប់ Spring Boot applications។ វាផ្តល់ Swagger UI ដើម្បីមើល និងសាកល្បង API ផងដែរ។

### 🔹 Maven Dependency:

```xml
<dependency>
    <groupId>org.springdoc</groupId>
    <artifactId>springdoc-openapi-starter-webmvc-ui</artifactId>
    <version>2.3.0</version>
</dependency>
```

### 🔹 Configuration (application.properties):

```properties
# Swagger UI path
springdoc.swagger-ui.path=/swagger-ui.html

# API docs path
springdoc.api-docs.path=/api-docs

# Packages to scan
springdoc.packages-to-scan=com.example.demo.controller

# Paths to include
springdoc.paths-to-match=/api/**

# Disable swagger for production
springdoc.api-docs.enabled=true
springdoc.swagger-ui.enabled=true
```

### 🔹 Access URLs after running:

- **Swagger UI:** http://localhost:8080/swagger-ui.html

- **OpenAPI JSON:** http://localhost:8080/v3/api-docs

- **OpenAPI YAML:** http://localhost:8080/v3/api-docs.yaml

### 🔹 OpenAPI Annotations:

| Annotation | Description | Example |
| --- | --- | --- |
| OpenAPIDefinition | API information (title, version, description) | @OpenAPIDefinition(info = @Info(title = "My API", version = "1.0")) |
| Operation | Describe an endpoint | @Operation(summary = "Get user by ID", description = "Returns a single user") |
| Parameter | Describe a parameter | @Parameter(description = "User ID", example = "1") |
| ApiResponses | Describe possible responses | @ApiResponses(value = {@ApiResponse(responseCode = "200", description = "Success")}) |
| Schema | Describe a model field | @Schema(description = "User email", example = "user@example.com") |
| Tag | Group endpoints | @Tag(name = "User Controller", description = "User management APIs") |

### 🔹 Configuration Class Example:

```java
import io.swagger.v3.oas.models.OpenAPI;
import io.swagger.v3.oas.models.info.Info;
import io.swagger.v3.oas.models.info.Contact;
import io.swagger.v3.oas.models.info.License;
import org.springframework.context.annotation.Bean;
import org.springframework.context.annotation.Configuration;

@Configuration
public class OpenAPIConfig {

    @Bean
    public OpenAPI customOpenAPI() {
        return new OpenAPI()
```

.info(new Info()

.title("My Spring Boot API")

.version("1.0.0")

.description("This is a sample Spring Boot REST API documentation")

.contact(new Contact()

.name("Your Name")

.email("your.email@example.com")

.url("https://example.com"))

.license(new License()

.name("Apache 2.0")

```text
                                .url("https://www.apache.org/licenses/LICENSE-2.0")));
    }
}
```

### 🔹 Controller with OpenAPI Annotations:

```java
import io.swagger.v3.oas.annotations.Operation;
import io.swagger.v3.oas.annotations.Parameter;
import io.swagger.v3.oas.annotations.responses.ApiResponse;
import io.swagger.v3.oas.annotations.responses.ApiResponses;
import io.swagger.v3.oas.annotations.tags.Tag;
import org.springframework.web.bind.annotation.*;

@RestController
@RequestMapping("/api/users")
@Tag(name = "User Controller", description = "User management APIs")
public class UserController {

    @Autowired
    private UserService userService;

    @GetMapping
    @Operation(summary = "Get all users", description = "Returns a list of all users")
    @ApiResponses(value = {
        @ApiResponse(responseCode = "200", description = "Successfully retrieved"),
        @ApiResponse(responseCode = "401", description = "Unauthorized"),
        @ApiResponse(responseCode = "403", description = "Forbidden")
    })
    public ResponseEntity<List<User>> getAllUsers() {
        return ResponseEntity.ok(userService.findAll());
    }

    @GetMapping("/{id}")
    @Operation(summary = "Get user by ID", description = "Returns a single user based on ID")
    @ApiResponses(value = {
        @ApiResponse(responseCode = "200", description = "User found"),
        @ApiResponse(responseCode = "404", description = "User not found")
    })
    public ResponseEntity<User> getUserById(
            @Parameter(description = "User ID", example = "1", required = true)
            @PathVariable Long id) {
        return userService.findById(id)
```

.map(ResponseEntity::ok)

```java
                .orElse(ResponseEntity.notFound().build());
    }

    @PostMapping
    @Operation(summary = "Create new user", description = "Creates a new user and returns the created user")
    @ApiResponses(value = {
        @ApiResponse(responseCode = "201", description = "User created successfully"),
        @ApiResponse(responseCode = "400", description = "Invalid input")
    })
    public ResponseEntity<User> createUser(@RequestBody UserDto userDto) {
        User created = userService.create(userDto);
        return ResponseEntity.status(HttpStatus.CREATED).body(created);
    }

    @PutMapping("/{id}")
    @Operation(summary = "Update user", description = "Updates an existing user")
    public ResponseEntity<User> updateUser(
            @PathVariable Long id,
            @RequestBody UserDto userDto) {
        return ResponseEntity.ok(userService.update(id, userDto));
    }

    @DeleteMapping("/{id}")
    @Operation(summary = "Delete user", description = "Deletes a user by ID")
    @ApiResponse(responseCode = "204", description = "User deleted successfully")
    public ResponseEntity<Void> deleteUser(@PathVariable Long id) {
        userService.delete(id);
        return ResponseEntity.noContent().build();
    }
}
```

## 12.3. API Testing (ការធ្វើតេស្ត API)

### 📌 និយមន័យ (Definition):

**API Testing** គឺជាការធ្វើតេស្ត API endpoints ដើម្បីធានាថាពួកវាដំណើរការបានត្រឹមត្រូវ (correctness), សុវត្ថិភាព (security), និងមានប្រសិទ្ធភាព (performance)។ Spring Boot ផ្តល់នូវឧបករណ៍ជាច្រើនសម្រាប់ API testing ។

### 🔹 Unit Test for Controller with MockMvc:

```java
import org.junit.jupiter.api.Test;
import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.boot.test.autoconfigure.web.servlet.WebMvcTest;
import org.springframework.boot.test.mock.mockito.MockBean;
import org.springframework.http.MediaType;
import org.springframework.test.web.servlet.MockMvc;
import com.fasterxml.jackson.databind.ObjectMapper;

@WebMvcTest(UserController.class)
class UserControllerTest {

    @Autowired
    private MockMvc mockMvc;

    @Autowired
    private ObjectMapper objectMapper;

    @MockBean
    private UserService userService;

    @Test
    void getAllUsers_ShouldReturnListOfUsers() throws Exception {
        List<User> users = Arrays.asList(new User(1L, "John"), new User(2L, "Jane"));
        when(userService.findAll()).thenReturn(users);
```

mockMvc.perform(get("/api/users"))

.andExpect(status().isOk())

.andExpect(jsonPath("$.length()").value(2))

```text
                .andExpect(jsonPath("$[0].name").value("John"));
    }

    @Test
    void getUserById_ShouldReturnNotFound_WhenUserDoesNotExist() throws Exception {
        when(userService.findById(999L)).thenReturn(Optional.empty());
```

mockMvc.perform(get("/api/users/999"))

```text
                .andExpect(status().isNotFound());
    }
}
```

## 12.4. API Versioning (កំណែរបស់ API)

### 📌 និយមន័យ (Definition):

**API Versioning** គឺជាការគ្រប់គ្រងកំណែផ្សេងៗគ្នានៃ API ដើម្បីឱ្យអ្នកប្រើប្រាស់ចាស់ (existing clients) នៅតែអាចបន្តប្រើប្រាស់ API បាន ខណៈពេលដែលកំណែថ្មីត្រូវបានបង្កើតឡើង។

### 🔹 Versioning Strategies:

| Strategy | Example | Pros | Cons |
| --- | --- | --- | --- |
| URI Path | /api/v1/users | Simple, cacheable, easy to test | URL changes, not RESTful pure |
| Query Parameter | /api/users?version=1 | URL stays same | Not standard, can be ignored |
| Header (Accept) | Accept: application/vnd.example.v1+json | RESTful, URL clean | Complex testing, caching issues |

### 🔹 URI Path Versioning Example:

```java
// Version 1 Controller
@RestController
@RequestMapping("/api/v1/users")
public class UserControllerV1 {

    @GetMapping("/{id}")
    public ResponseEntity<UserV1> getUser(@PathVariable Long id) {
        return ResponseEntity.ok(userService.findByIdV1(id));
    }
}

// Version 2 Controller
@RestController
@RequestMapping("/api/v2/users")
public class UserControllerV2 {

    @GetMapping("/{id}")
    public ResponseEntity<UserV2> getUser(@PathVariable Long id) {
        return ResponseEntity.ok(userService.findByIdV2(id));
    }
}
```

## 12.5. Postman Collection

### 📌 និយមន័យ (Definition):

**Postman Collection** គឺជាក្រុមនៃ API requests ដែលត្រូវបានរៀបចំជាប្រព័ន្ធ (organized group) និងអាចនាំចេញ (export) ចែករំលែក (share) ជាមួយក្រុមការងារ។ Collection អាចផ្ទុកនូវ requests, tests, variables, និង documentation។

### 🔹 Postman Test Script Example:

```text
// Test for GET /api/users
pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});

pm.test("Response is an array", function () {
    pm.expect(pm.response.json()).to.be.an('array');
});

// Test for POST /api/users
pm.test("Status code is 201", function () {
    pm.response.to.have.status(201);
});

// Set environment variable from response
const jsonData = pm.response.json();
pm.environment.set("userId", jsonData.id);
```

### 🔹 Postman Environment Variables:

```json
{
  "id": "environment",
  "name": "Development",
  "values": [
    {
      "key": "baseUrl",
      "value": "http://localhost:8080",
      "enabled": true
    },
    {
      "key": "accessToken",
      "value": "your-jwt-token-here",
      "enabled": true
    }
  ]
}
```

### 🔧 Newman Command for Automated Testing:

```bash
# Install Newman
```

npm install -g newman

```bash
# Run collection
```

newman run MySpringBootAPI.postman_collection.json -e Development.postman_environment.json

```bash
# Run with HTML report
```

newman run MySpringBootAPI.postman_collection.json -e Development.postman_environment.json -r html

### 📚 សង្ខេបមេរៀនទី១២ (Module 12 Summary)

នៅក្នុងមេរៀននេះ អ្នកបានរៀនអំពី API Documentation នៅក្នុង Spring Boot៖

- **Swagger/OpenAPI** – Specification for describing REST APIs, interactive documentation

- **SpringDoc OpenAPI** – Library to auto-generate OpenAPI 3.0 docs, Swagger UI integration

- **API Testing** – Unit tests with MockMvc, integration tests with TestRestTemplate

- **API Versioning** – URI Path, Query Parameter, Header strategies

- **Postman Collection** – Organize requests, tests, variables, automate with Newman

# មេរៀនទី១៣: Spring Boot Testing (ការធ្វើតេស្តក្នុង Spring Boot)

### 📖 សេចក្តីផ្តើម (Introduction):
Testing គឺជាផ្នែកសំខាន់មួយក្នុងការអភិវឌ្ឍន៍កម្មវិធី ដើម្បីធានាថាកូដរបស់អ្នកដំណើរការបានត្រឹមត្រូវ និងមិនមានកំហុស។ Spring Boot ផ្តល់នូវឧបករណ៍យ៉ាងច្រើនសម្រាប់ testing។ មេរៀននេះនឹងបង្រៀនអ្នកពី Unit Testing, JUnit 5, Mockito, MockBean, Integration Testing, Test Containers, API Testing, និង Code Coverage។

## 13.1. Unit Testing (ការធ្វើតេស្តឯកតា)

### 📌 និយមន័យ (Definition):

**Unit Testing** គឺជាការធ្វើតេស្តលើផ្នែកតូចបំផុតនៃកូដ (units) ដូចជា methods, functions ដើម្បីធានាថាពួកវាដំណើរការបានត្រឹមត្រូវ។ Unit tests គួរតែរហ័ស (fast), ឯករាជ្យ (isolated), និងអាចធ្វើឡើងវិញបាន (repeatable)។

### 🔹 Unit Test Example for Service Layer:

```java
import org.junit.jupiter.api.Test;
import org.junit.jupiter.api.extension.ExtendWith;
import org.mockito.InjectMocks;
import org.mockito.Mock;
import org.mockito.junit.jupiter.MockitoExtension;
import java.util.Optional;
import static org.junit.jupiter.api.Assertions.*;
import static org.mockito.Mockito.*;

@ExtendWith(MockitoExtension.class)
class UserServiceTest {

    @Mock
    private UserRepository userRepository;

    @InjectMocks
    private UserService userService;

    @Test
    void findById_ShouldReturnUser_WhenUserExists() {
        // Arrange (រៀបចំ)
        Long userId = 1L;
        User expectedUser = new User(userId, "John Doe");
        when(userRepository.findById(userId)).thenReturn(Optional.of(expectedUser));

        // Act (អនុវត្ត)
        User actualUser = userService.findById(userId);

        // Assert (ផ្ទៀងផ្ទាត់)
        assertNotNull(actualUser);
        assertEquals(expectedUser.getId(), actualUser.getId());
        assertEquals(expectedUser.getName(), actualUser.getName());
        verify(userRepository, times(1)).findById(userId);
    }

    @Test
    void findById_ShouldThrowException_WhenUserNotFound() {
        // Arrange
        Long userId = 999L;
        when(userRepository.findById(userId)).thenReturn(Optional.empty());

        // Act & Assert
        assertThrows(ResourceNotFoundException.class, () -> {
            userService.findById(userId);
        });
        verify(userRepository, times(1)).findById(userId);
    }

    @Test
    void createUser_ShouldSaveAndReturnUser() {
        // Arrange
        UserDto userDto = new UserDto();
        userDto.setName("New User");
        userDto.setEmail("new@example.com");

        User savedUser = new User(1L, "New User");
        when(userRepository.save(any(User.class))).thenReturn(savedUser);

        // Act
        User result = userService.createUser(userDto);

        // Assert
        assertNotNull(result);
        assertEquals(savedUser.getId(), result.getId());
        verify(userRepository, times(1)).save(any(User.class));
    }
}
```

### 💡 Benefits of Unit Testing:

- រកឃើញកំហុសបានឆាប់ (Early bug detection)

- ធ្វើឱ្យកូដមានគុណភាពខ្ពស់ (Better code quality)

- ងាយស្រួលក្នុងការកែប្រែកូដ (Easier refactoring)

- ធ្វើជាឯកសារសម្រាប់កូដ (Documentation)

## 13.2. JUnit 5 (ជូយនីត ៥)

### 📌 និយមន័យ (Definition):

**JUnit 5** គឺជា framework ស្តង់ដារសម្រាប់ unit testing ក្នុង Java។ Spring Boot ប្រើ JUnit 5 ជា default testing framework។ វាផ្តល់នូវ annotations និង assertions ជាច្រើនសម្រាប់សរសេរ tests។

### 🔹 Maven Dependency:

```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-test</artifactId>
    <scope>test</scope>
</dependency>
```

### 🔹 Common JUnit 5 Annotations:

| Annotation | Description | Example |
| --- | --- | --- |
| @Test | Marks a method as a test method | @Test void testMethod() |
| @BeforeEach | Runs before each test method | @BeforeEach void setUp() |
| @AfterEach | Runs after each test method | @AfterEach void tearDown() |
| @BeforeAll | Runs once before all tests (static) | @BeforeAll static void init() |
| @AfterAll | Runs once after all tests (static) | @AfterAll static void cleanup() |
| @Disabled | Disables a test method | @Disabled void notReadyTest() |
| @DisplayName | Custom display name for test | @DisplayName("Test user creation") |
| @ParameterizedTest | Test with multiple parameters | @ParameterizedTest @ValueSource(ints = 3) |

### 🔹 JUnit 5 Examples:

```properties
import org.junit.jupiter.api.*;
import static org.junit.jupiter.api.Assertions.*;

class CalculatorTest {

    private Calculator calculator;

    @BeforeEach
    void setUp() {
        calculator = new Calculator();
        System.out.println("Before each test");
    }

    @AfterEach
    void tearDown() {
        System.out.println("After each test");
    }

    @BeforeAll
    static void initAll() {
        System.out.println("Before all tests - runs once");
    }

    @AfterAll
    static void cleanupAll() {
        System.out.println("After all tests - runs once");
    }

    @Test
    @DisplayName("Test addition of two numbers")
    void add_ShouldReturnSum_WhenTwoNumbersAreGiven() {
        // Given
        int a = 5, b = 3;

        // When
        int result = calculator.add(a, b);

        // Then
        assertEquals(8, result, "5 + 3 should equal 8");
        assertNotEquals(9, result);
    }

    @Test
    void divide_ShouldThrowException_WhenDividingByZero() {
        assertThrows(ArithmeticException.class, () -> {
            calculator.divide(10, 0);
        });
    }

    @Test
    @Disabled("Not yet implemented")
    void notYetImplemented() {
        // This test will be skipped
    }

    @ParameterizedTest
    @ValueSource(ints = {1, 2, 3, 4, 5})
    void testIsPositive(int number) {
        assertTrue(number > 0);
    }

    @ParameterizedTest
    @CsvSource({"1,1,2", "2,3,5", "10,20,30"})
    void testAddWithCSV(int a, int b, int expected) {
        assertEquals(expected, calculator.add(a, b));
    }

    @Test
    void testAssertAll() {
        User user = new User("John", "john@example.com");
```

assertAll("User properties",

() -> assertEquals("John", user.getName()),

() -> assertEquals("john@example.com", user.getEmail()),

() -> assertNotNull(user.getCreatedAt())

```text
        );
    }
}
```

## 13.3. Mockito (ម៉ុកគីតូ)

### 📌 និយមន័យ (Definition):

**Mockito** គឺជា mocking framework ដែលអនុញ្ញាតឱ្យអ្នកបង្កើត mock objects (objects ក្លែង) សម្រាប់ dependency របស់ class ដែលកំពុងធ្វើតេស្ត។ វាជួយឱ្យ unit tests មានភាពឯករាជ្យ (isolated) និងមិនពឹងផ្អែកលើ dependencies ពិតប្រាកដ។

### 🔹 Mockito Annotations:

| Annotation | Description |
| --- | --- |
| @Mock | Creates a mock object |
| @InjectMocks | Injects mocks into the tested object |
| @Spy | Creates a spy (partial mock) |
| @Captor | Captures arguments for verification |

### 🔹 Mockito Examples:

```java
import org.junit.jupiter.api.Test;
import org.junit.jupiter.api.extension.ExtendWith;
import org.mockito.*;
import org.mockito.junit.jupiter.MockitoExtension;
import java.util.List;
import static org.junit.jupiter.api.Assertions.*;
import static org.mockito.Mockito.*;

@ExtendWith(MockitoExtension.class)
class MockitoExamplesTest {

    @Mock
    private List<String> mockList;

    @Mock
    private UserRepository userRepository;

    @InjectMocks
    private UserService userService;

    @Captor
    private ArgumentCaptor<User> userCaptor;

    @Test
    void testMockBehavior() {
        // Stubbing (កំណត់ឥរិយាបថរបស់ mock)
        when(mockList.get(0)).thenReturn("First Element");
        when(mockList.get(1)).thenThrow(new RuntimeException());

        // Verify stubbing works
        assertEquals("First Element", mockList.get(0));

        // Verify method was called
        verify(mockList).get(0);
        verify(mockList, times(1)).get(0);
        verify(mockList, atLeastOnce()).get(0);
    }

    @Test
    void testArgumentMatchers() {
        // Using any() matcher
        when(userRepository.findById(anyLong())).thenReturn(Optional.of(new User()));

        // Using specific matcher
        when(userRepository.findByName(eq("John"))).thenReturn(List.of(new User()));

        // Verify with matchers
        userService.findById(1L);
        verify(userRepository).findById(argThat(id -> id > 0));
    }

    @Test
    void testArgumentCaptor() {
        // Capture argument passed to method
        userService.createUser(new User("John", "john@example.com"));

        verify(userRepository).save(userCaptor.capture());
        User capturedUser = userCaptor.getValue();

        assertEquals("John", capturedUser.getName());
        assertEquals("john@example.com", capturedUser.getEmail());
    }

    @Test
    void testVerifyInteractionCount() {
        userService.findById(1L);
        userService.findById(1L);
        userService.findById(2L);

        verify(userRepository, times(2)).findById(1L);
        verify(userRepository, never()).findById(999L);
        verify(userRepository, atLeast(1)).findById(anyLong());
        verify(userRepository, atMost(3)).findById(anyLong());
    }

    @Test
    void testDoAnswer() {
        when(mockList.get(anyInt())).thenAnswer(invocation -> {
            int index = invocation.getArgument(0);
            return "Element at index " + index;
        });

        assertEquals("Element at index 5", mockList.get(5));
    }
}
```

## 13.4. MockBean

### 📌 និយមន័យ (Definition):

```text
@MockBean គឺជា annotation របស់ Spring Boot ដែលប្រើសម្រាប់បង្កើត mock object និងបន្ថែមវាទៅក្នុង Spring Application Context។ វាមានប្រយោជន៍សម្រាប់ integration tests ដែលអ្នកចង់ mock dependencies មួយចំនួនប៉ុន្តែនៅតែចង់ប្រើ Spring context ពិតប្រាកដ។
```

### 🔹 MockBean Example:

```java
import org.junit.jupiter.api.Test;
import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.boot.test.context.SpringBootTest;
import org.springframework.boot.test.mock.mockito.MockBean;
import static org.mockito.Mockito.*;

@SpringBootTest
class UserServiceIntegrationTest {

    @MockBean
    private UserRepository userRepository;

    @Autowired
    private UserService userService;

    @Test
    void testCreateUser() {
        // Mock the repository behavior
        User mockUser = new User(1L, "John Doe");
        when(userRepository.save(any(User.class))).thenReturn(mockUser);

        // Test the service
        UserDto userDto = new UserDto();
        userDto.setName("John Doe");
        User result = userService.createUser(userDto);

        // Verify
        assertNotNull(result);
        assertEquals(1L, result.getId());
        verify(userRepository, times(1)).save(any(User.class));
    }

    @Test
    void testDeleteUser() {
        // Mock void method
        doNothing().when(userRepository).deleteById(1L);

        userService.deleteUser(1L);

        verify(userRepository, times(1)).deleteById(1L);
    }
}

// WebMvcTest with MockBean
@WebMvcTest(UserController.class)
class UserControllerWebTest {

    @Autowired
    private MockMvc mockMvc;

    @MockBean
    private UserService userService;

    @Test
    void getUser_ShouldReturnUser() throws Exception {
        User user = new User(1L, "John Doe");
        when(userService.findById(1L)).thenReturn(user);
```

mockMvc.perform(get("/api/users/1"))

.andExpect(status().isOk())

```text
                .andExpect(jsonPath("$.name").value("John Doe"));
    }
}
```

## 13.5. Integration Testing (ការធ្វើតេស្តសមាហរណកម្ម)

### 📌 និយមន័យ (Definition):

**Integration Testing** គឺជាការធ្វើតេស្តផ្នែកផ្សេងៗនៃកម្មវិធីធ្វើការជាមួយគ្នា (how different parts work together)។ Spring Boot ផ្តល់ @SpringBootTestannotation សម្រាប់ integration testing ។

### 🔹 Integration Test Examples:

```java
import org.junit.jupiter.api.Test;
import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.boot.test.context.SpringBootTest;
import org.springframework.boot.test.web.client.TestRestTemplate;
import org.springframework.boot.test.web.server.LocalServerPort;
import org.springframework.http.*;

@SpringBootTest(webEnvironment = SpringBootTest.WebEnvironment.RANDOM_PORT)
class UserControllerIntegrationTest {

    @LocalServerPort
    private int port;

    @Autowired
    private TestRestTemplate restTemplate;

    @Test
    void createAndGetUser_ShouldWork() {
        // Create user
        UserDto newUser = new UserDto();
        newUser.setName("Integration Test User");
        newUser.setEmail("integration@test.com");

        ResponseEntity<User> createResponse = restTemplate.postForEntity(
```

"http://localhost:" + port + "/api/users",

newUser,

```java
            User.class
        );

        assertThat(createResponse.getStatusCode()).isEqualTo(HttpStatus.CREATED);
        Long userId = createResponse.getBody().getId();

        // Get user
        ResponseEntity<User> getResponse = restTemplate.getForEntity(
```

"http://localhost:" + port + "/api/users/" + userId,

```java
            User.class
        );

        assertThat(getResponse.getStatusCode()).isEqualTo(HttpStatus.OK);
        assertThat(getResponse.getBody().getName()).isEqualTo("Integration Test User");
    }
}

// Data JPA Integration Test
@DataJpaTest
class UserRepositoryIntegrationTest {

    @Autowired
    private TestEntityManager entityManager;

    @Autowired
    private UserRepository userRepository;

    @Test
    void testFindByEmail() {
        // Save test data
        User user = new User("Test User", "test@example.com");
        entityManager.persist(user);
        entityManager.flush();

        // Test the query
        Optional<User> found = userRepository.findByEmail("test@example.com");

        assertThat(found).isPresent();
        assertThat(found.get().getName()).isEqualTo("Test User");
    }
}
```

## 13.6. Test Containers (តេស្តកុងតឺន័រ)

### 📌 និយមន័យ (Definition):

**Testcontainers** គឺជា library ដែលអនុញ្ញាតឱ្យអ្នកប្រើ Docker containers សម្រាប់ integration testing។ វាអាចបង្កើត containers បណ្តោះអាសន្ន (temporary) សម្រាប់ databases, message brokers, ឬ services ផ្សេងទៀត។

### 🔹 Maven Dependency:

```xml
<dependency>
    <groupId>org.testcontainers</groupId>
    <artifactId>testcontainers</artifactId>
    <version>1.19.3</version>
    <scope>test</scope>
</dependency>
<dependency>
    <groupId>org.testcontainers</groupId>
    <artifactId>mysql</artifactId>
    <version>1.19.3</version>
    <scope>test</scope>
</dependency>
<dependency>
    <groupId>org.testcontainers</groupId>
    <artifactId>junit-jupiter</artifactId>
    <version>1.19.3</version>
    <scope>test</scope>
</dependency>
```

### 🔹 Testcontainers Example:

```java
import org.junit.jupiter.api.Test;
import org.springframework.boot.test.context.SpringBootTest;
import org.springframework.test.context.DynamicPropertyRegistry;
import org.springframework.test.context.DynamicPropertySource;
import org.testcontainers.containers.MySQLContainer;
import org.testcontainers.junit.jupiter.Container;
import org.testcontainers.junit.jupiter.Testcontainers;

@Testcontainers
@SpringBootTest
class DatabaseIntegrationTest {

    @Container
```

static MySQLContainer<?> mysql = new MySQLContainer<>("mysql:8.0")

.withDatabaseName("testdb")

.withUsername("testuser")

```java
            .withPassword("testpass");

    @DynamicPropertySource
    static void properties(DynamicPropertyRegistry registry) {
        registry.add("spring.datasource.url", mysql::getJdbcUrl);
        registry.add("spring.datasource.username", mysql::getUsername);
        registry.add("spring.datasource.password", mysql::getPassword);
    }

    @Autowired
    private UserRepository userRepository;

    @Test
    void testDatabaseConnection() {
        User user = new User("Test User", "test@example.com");
        User saved = userRepository.save(user);

        assertThat(saved.getId()).isNotNull();
        assertThat(saved.getName()).isEqualTo("Test User");
    }
}

// Generic Container Example
@Testcontainers
class GenericContainerTest {

    @Container
```

static GenericContainer<?> redis = new GenericContainer<>("redis:7-alpine")

```text
            .withExposedPorts(6379);

    @Test
    void testRedis() {
        Integer mappedPort = redis.getMappedPort(6379);
        String host = redis.getHost();

        // Use host and port to connect to Redis
        assertNotNull(mappedPort);
        assertNotNull(host);
    }
}
```

## 13.7. API Testing (ការធ្វើតេស្ត API)

### 📌 និយមន័យ (Definition):

**API Testing** គឺជាការធ្វើតេស្ត REST API endpoints ដោយផ្ទាល់ ដើម្បីផ្ទៀងផ្ទាត់ HTTP responses, status codes, headers, និង response bodies។

### 🔹 WebMvcTest Example:

```java
import org.junit.jupiter.api.Test;
import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.boot.test.autoconfigure.web.servlet.WebMvcTest;
import org.springframework.boot.test.mock.mockito.MockBean;
import org.springframework.http.MediaType;
import org.springframework.test.web.servlet.MockMvc;
import com.fasterxml.jackson.databind.ObjectMapper;

@WebMvcTest(UserController.class)
class UserControllerApiTest {

    @Autowired
    private MockMvc mockMvc;

    @Autowired
    private ObjectMapper objectMapper;

    @MockBean
    private UserService userService;

    @Test
    void testGetAllUsers() throws Exception {
        List<User> users = Arrays.asList(
            new User(1L, "John"),
            new User(2L, "Jane")
        );
        when(userService.findAll()).thenReturn(users);
```

mockMvc.perform(get("/api/users")

.contentType(MediaType.APPLICATION_JSON))

.andExpect(status().isOk())

.andExpect(jsonPath("$.length()").value(2))

.andExpect(jsonPath("$[0].name").value("John"))

```text
                .andExpect(jsonPath("$[1].name").value("Jane"));
    }

    @Test
    void testCreateUser() throws Exception {
        UserDto userDto = new UserDto();
        userDto.setName("New User");
        userDto.setEmail("new@example.com");

        User createdUser = new User(1L, "New User");
        when(userService.createUser(any(UserDto.class))).thenReturn(createdUser);
```

mockMvc.perform(post("/api/users")

.contentType(MediaType.APPLICATION_JSON)

.content(objectMapper.writeValueAsString(userDto)))

.andExpect(status().isCreated())

.andExpect(jsonPath("$.id").value(1L))

```text
                .andExpect(jsonPath("$.name").value("New User"));
    }

    @Test
    void testGetUserNotFound() throws Exception {
        when(userService.findById(999L)).thenThrow(new ResourceNotFoundException("User not found"));
```

mockMvc.perform(get("/api/users/999"))

```text
                .andExpect(status().isNotFound());
    }
}
```

## 13.8. Code Coverage (ការគ្របដណ្តប់កូដ)

### 📌 និយមន័យ (Definition):

**Code Coverage** គឺជារង្វាស់ (metric) ដែលបង្ហាញពីភាគរយនៃកូដដែលត្រូវបានធ្វើតេស្ត។ ឧបករណ៍ពេញនិយមសម្រាប់ code coverage ក្នុង Java គឺ **JaCoCo** (Java Code Coverage)។

### 🔹 JaCoCo Maven Plugin:

```xml
<plugin>
    <groupId>org.jacoco</groupId>
    <artifactId>jacoco-maven-plugin</artifactId>
    <version>0.8.11</version>
    <executions>
        <execution>
            <goals>
                <goal>prepare-agent</goal>
            </goals>
        </execution>
        <execution>
            <id>report</id>
            <phase>test</phase>
            <goals>
                <goal>report</goal>
            </goals>
        </execution>
    </executions>
</plugin>
```

### 🔹 Gradle JaCoCo Plugin:

```groovy
plugins {
```

id 'jacoco'

```text
}

jacocoTestReport {
```

dependsOn test

```properties
    reports {
        xml.required = true
        html.required = true
        csv.required = false
    }
}

jacocoTestCoverageVerification {
    violationRules {
        rule {
            limit {
                minimum = 0.8
            }
        }
    }
}
```

### 🔹 Running JaCoCo Commands:

```bash
# Maven
```

mvn clean test jacoco:report

```bash
# Gradle
```

gradle test jacocoTestReport

```bash
# View report
```

open target/site/jacoco/index.html  # Maven

open build/reports/jacoco/test/html/index.html  # Gradle

### 💡 Code Coverage Best Practices:

- គោលដៅល្អគឺ **80% line coverage** ឬខ្ពស់ជាងនេះ

- ផ្តោតលើ **business logic** (Service layer) ជាង getters/setters

- ប្រើ **JaCoCo** violations rules ដើម្បីការពារ coverage ពីការថយចុះ

- **100% coverage** មិនតែងតែល្អទេ — គុណភាពសំខាន់ជាងបរិមាណ

### 📊 Coverage Metrics Types:

- **Line Coverage** – ភាគរយនៃបន្ទាត់កូដដែលត្រូវបានធ្វើតេស្ត

- **Branch Coverage** – ភាគរយនៃ branches (if/else, switch) ដែលត្រូវបានធ្វើតេស្ត

- **Method Coverage** – ភាគរយនៃ methods ដែលត្រូវបានធ្វើតេស្ត

- **Class Coverage** – ភាគរយនៃ classes ដែលត្រូវបានធ្វើតេស្ត

### 📚 សង្ខេបមេរៀនទី១៣ (Module 13 Summary)

នៅក្នុងមេរៀននេះ អ្នកបានរៀនអំពី Testing នៅក្នុង Spring Boot៖

- **Unit Testing** – Testing individual units (methods, classes) in isolation

- **JUnit 5** – Testing framework with annotations: @Test, @BeforeEach, @ParameterizedTest

- **Mockito** – Mocking framework for creating mock objects (@Mock, @InjectMocks, @Captor)

- **MockBean** – Spring Boot annotation for adding mocks to application context

- **Integration Testing** – Testing how different parts work together (@SpringBootTest)

- **Test Containers** – Docker containers for integration testing (MySQL, Redis, etc.)

- **API Testing** – Testing REST endpoints with MockMvc and TestRestTemplate

- **Code Coverage** – Measuring test coverage with JaCoCo (80%+ recommended)

# មេរៀនទី១៤: Spring Boot with Frontend (Spring Boot ជាមួយ Frontend)

### 📖 សេចក្តីផ្តើម (Introduction):
Spring Boot អាចប្រើជា backend API សម្រាប់ frontend frameworks ដូចជា React, Vue, Angular។ មេរៀននេះនឹងបង្រៀនអ្នកពី React + Spring Boot, Vue + Spring Boot, Angular + Spring Boot, CORS Setup, REST API Connection, និង Authentication Integration។

## 14.1. React + Spring Boot

### 📌 ការតភ្ជាប់ React ជាមួយ Spring Boot:

React គឺជា JavaScript library សម្រាប់បង្កើត user interfaces។ វាអាចទំនាក់ទំនងជាមួយ Spring Boot REST API តាមរយៈ HTTP requests (fetch API, axios)។

### 🔹 React Component with Axios:

```bash
import React, { useState, useEffect } from 'react';
import axios from 'axios';

const API_BASE_URL = 'http://localhost:8080/api';

function UserList() {
    const [users, setUsers] = useState([]);
    const [loading, setLoading] = useState(true);
    const [error, setError] = useState(null);

    useEffect(() => {
        fetchUsers();
    }, []);

    const fetchUsers = async () => {
        try {
            const response = await axios.get(API_BASE_URL + '/users');
            setUsers(response.data);
            setLoading(false);
        } catch (err) {
            setError(err.message);
            setLoading(false);
        }
    };

    const deleteUser = async (id) => {
        try {
            await axios.delete(API_BASE_URL + '/users/' + id);
            setUsers(users.filter(user => user.id !== id));
        } catch (err) {
            console.error('Error deleting user:', err);
        }
    };

    if (loading) return <div>Loading...</div>;
    if (error) return <div>Error: {error}</div>;

    return (
        <div>
            <h1>User List</h1>
            <ul>
                {users.map(user => (
                    <li key={user.id}>
                        {user.name} - {user.email}
                        <button onClick={() => deleteUser(user.id)}>Delete</button>
                    </li>
                ))}
            </ul>
        </div>
    );
}

export default UserList;
```

### 🔹 Axios Configuration:

```java
import axios from 'axios';

const apiClient = axios.create({
    baseURL: 'http://localhost:8080/api',
    timeout: 10000,
    headers: {
```

'Content-Type': 'application/json',

```text
    }
});

// Request interceptor for auth token
```

apiClient.interceptors.request.use(

```properties
    (config) => {
        const token = localStorage.getItem('token');
        if (token) {
            config.headers.Authorization = 'Bearer ' + token;
        }
        return config;
    },
```

(error) => Promise.reject(error)

```bash
);

export default apiClient;
```

## 14.2. Vue + Spring Boot

### 📌 ការតភ្ជាប់ Vue ជាមួយ Spring Boot:

Vue.js គឺជា progressive JavaScript framework សម្រាប់បង្កើត user interfaces។ វាអាចប្រើ axios ឬ fetch API ដើម្បីទំនាក់ទំនងជាមួយ Spring Boot REST API។

### 🔹 Vue Component Example:

```properties
<template>
  <div>
    <h1>User Management</h1>
    <div v-if="loading">Loading...</div>
    <div v-if="error" class="error">{{ error }}</div>
    <ul>
      <li v-for="user in users" :key="user.id">
        {{ user.name }} - {{ user.email }}
        <button @click="deleteUser(user.id)">Delete</button>
      </li>
    </ul>
  </div>
</template>

<script>
import axios from 'axios';

const API_URL = 'http://localhost:8080/api';

export default {
  data() {
    return {
      users: [],
      loading: false,
      error: null
    };
  },
  mounted() {
    this.fetchUsers();
  },
  methods: {
    async fetchUsers() {
      this.loading = true;
      try {
        const response = await axios.get(API_URL + '/users');
        this.users = response.data;
      } catch (err) {
        this.error = err.message;
      } finally {
        this.loading = false;
      }
    },

    async deleteUser(id) {
      try {
        await axios.delete(API_URL + '/users/' + id);
        this.users = this.users.filter(user => user.id !== id);
      } catch (err) {
        console.error('Error deleting user:', err);
      }
    }
  }
};
</script>
```

## 14.3. Angular + Spring Boot

### 📌 ការតភ្ជាប់ Angular ជាមួយ Spring Boot:

Angular គឺជា TypeScript-based framework សម្រាប់បង្កើត web applications។ វាប្រើ HttpClient module ដើម្បីទំនាក់ទំនងជាមួយ Spring Boot REST API។

### 🔹 Angular Service Example:

```bash
import { Injectable } from '@angular/core';
import { HttpClient } from '@angular/common/http';
import { Observable } from 'rxjs';

export interface User {
  id: number;
  name: string;
  email: string;
}

@Injectable({
  providedIn: 'root'
})
export class UserService {
  private apiUrl = 'http://localhost:8080/api';

  constructor(private http: HttpClient) { }

  getAllUsers(): Observable<User[]> {
    return this.http.get<User[]>(this.apiUrl + '/users');
  }

  deleteUser(id: number): Observable<void> {
    return this.http.delete<void>(this.apiUrl + '/users/' + id);
  }
}
```

## 14.4. CORS Setup

### 📌 និយមន័យ (Definition):

**CORS (Cross-Origin Resource Sharing)** គឺជាយន្តការដែលអនុញ្ញាតឱ្យ frontend (running on different port/origin) អាចចូលដំណើរការ backend API បាន។ Spring Boot ត្រូវការ CORS configuration ដើម្បីអនុញ្ញាត requests ពី frontend។

### 🔹 Global CORS Configuration:

```java
import org.springframework.context.annotation.Bean;
import org.springframework.context.annotation.Configuration;
import org.springframework.web.servlet.config.annotation.CorsRegistry;
import org.springframework.web.servlet.config.annotation.WebMvcConfigurer;

@Configuration
public class CorsConfig {

    @Bean
    public WebMvcConfigurer corsConfigurer() {
        return new WebMvcConfigurer() {
            @Override
            public void addCorsMappings(CorsRegistry registry) {
```

registry.addMapping("/api/**")

.allowedOrigins("http://localhost:3000", "http://localhost:4200")

.allowedMethods("GET", "POST", "PUT", "DELETE", "OPTIONS")

.allowedHeaders("*")

.allowCredentials(true)

```text
                        .maxAge(3600);
            }
        };
    }
}
```

### 🔹 Using @CrossOrigin Annotation:

```java
@RestController
@RequestMapping("/api/users")
@CrossOrigin(origins = "http://localhost:3000", maxAge = 3600)
public class UserController {

    @GetMapping
    public List<User> getAllUsers() {
        return userService.findAll();
    }
}
```

## 14.5. REST API Connection

### 📌 ការភ្ជាប់ Frontend ទៅកាន់ REST API:

### 🔹 Using Fetch API:

```text
// GET Request
async function getUsers() {
    try {
        const response = await fetch('http://localhost:8080/api/users');
        if (!response.ok) {
            throw new Error('HTTP error! status: ' + response.status);
        }
        const data = await response.json();
        return data;
    } catch (error) {
        console.error('Error fetching users:', error);
    }
}

// POST Request
async function createUser(userData) {
    try {
        const response = await fetch('http://localhost:8080/api/users', {
            method: 'POST',
            headers: {
```

'Content-Type': 'application/json',

```text
            },
            body: JSON.stringify(userData)
        });
        return await response.json();
    } catch (error) {
        console.error('Error creating user:', error);
    }
}

// DELETE Request
async function deleteUser(id) {
    try {
        await fetch('http://localhost:8080/api/users/' + id, {
            method: 'DELETE'
        });
    } catch (error) {
        console.error('Error deleting user:', error);
    }
}
```

## 14.6. Authentication Integration

### 📌 ការភ្ជាប់ JWT Authentication ជាមួយ Frontend:

### 🔹 Login Component (React):

```properties
import React, { useState } from 'react';
import axios from 'axios';

function Login({ onLogin }) {
    const [credentials, setCredentials] = useState({ username: '', password: '' });
    const [error, setError] = useState('');
    const [loading, setLoading] = useState(false);

    const handleSubmit = async (e) => {
        e.preventDefault();
        setLoading(true);
        setError('');

        try {
            const response = await axios.post('http://localhost:8080/api/auth/login', credentials);
            const { token, user } = response.data;

            localStorage.setItem('token', token);
            localStorage.setItem('user', JSON.stringify(user));

            axios.defaults.headers.common['Authorization'] = 'Bearer ' + token;

            onLogin(user);
        } catch (err) {
            setError(err.response?.data?.message || 'Login failed');
        } finally {
            setLoading(false);
        }
    };

    return (
        <form onSubmit={handleSubmit}>
            <h2>Login</h2>
            {error && <div className="error">{error}</div>}
            <input
                type="text"
                name="username"
                placeholder="Username"
                value={credentials.username}
                onChange={(e) => setCredentials({...credentials, username: e.target.value})}
```

required

/>

```properties
            <input
                type="password"
                name="password"
                placeholder="Password"
                value={credentials.password}
                onChange={(e) => setCredentials({...credentials, password: e.target.value})}
```

required

/>

```bash
            <button type="submit" disabled={loading}>
                {loading ? 'Logging in...' : 'Login'}
            </button>
        </form>
    );
}

export default Login;
```

### 🔹 Protected Route Component:

```properties
import React from 'react';
import { Navigate } from 'react-router-dom';

function ProtectedRoute({ children }) {
    const token = localStorage.getItem('token');

    if (!token) {
        return <Navigate to="/login" replace />;
    }

    return children;
}

// Logout function
function logout() {
    localStorage.removeItem('token');
    localStorage.removeItem('user');
    delete axios.defaults.headers.common['Authorization'];
    window.location.href = '/login';
}
```

### 💡 Best Practices:

- ប្រើ environment variables សម្រាប់ API URLs

- អនុវត្ត loading states និង error handling

- ប្រើ interceptors សម្រាប់ adding auth tokens

- Validate data on both frontend and backend

- ប្រើ HTTPS ក្នុង production

### 🔧 Environment Variables:

```properties
// .env file (React)
REACT_APP_API_URL=http://localhost:8080/api

// Usage
const API_URL = process.env.REACT_APP_API_URL;
```

### 📚 សង្ខេបមេរៀនទី១៤ (Module 14 Summary)

នៅក្នុងមេរៀននេះ អ្នកបានរៀនអំពីការភ្ជាប់ Spring Boot ជាមួយ Frontend frameworks៖

- **React + Spring Boot** – Using axios, useState, useEffect

- **Vue + Spring Boot** – Using axios, lifecycle hooks

- **Angular + Spring Boot** – Using HttpClient, services

- **CORS Setup** – Global configuration, @CrossOrigin annotation

- **REST API Connection** – Fetch API, error handling

- **Authentication Integration** – JWT token storage, login flow, protected routes

# មេរៀនទី១៥: Spring Boot Microservices (Spring Boot មីក្រូសេវា)

### 📖 សេចក្តីផ្តើម (Introduction):
Microservices architecture គឺជាវិធីសាស្រ្តក្នុងការអភិវឌ្ឍន៍កម្មវិធីដែលបំបែកកម្មវិធីធំមួយទៅជាសេវាតូចៗ (small, independent services) ដែលអាចដំណើរការដោយឡែកពីគ្នា។ មេរៀននេះនឹងបង្រៀនអ្នកពី What are Microservices, Monolith vs Microservices, Service Discovery, Eureka Server, API Gateway, Load Balancing, Config Server, OpenFeign, Circuit Breaker, និង Distributed Tracing។

## 15.1. តើ Microservices ជាអ្វី? (What are Microservices?)

### 📌 និយមន័យ (Definition):

**Microservices** គឺជា architectural style ដែលបំបែកកម្មវិធីធំមួយទៅជាសេវាតូចៗ (small, loosely coupled services) ដែលនីមួយៗផ្តោតលើ business capability ជាក់លាក់មួយ។ សេវានីមួយៗអាចត្រូវបានអភិវឌ្ឍ, deploy, scale, និងធ្វើតេស្តដោយឯករាជ្យ។

### 🔹 Key Characteristics of Microservices:

- **Single Responsibility** – សេវានីមួយៗផ្តោតលើមុខងារតែមួយ

- **Loosely Coupled** – សេវានីមួយៗឯករាជ្យពីគ្នា

- **Independently Deployable** – អាច deploy សេវានីមួយៗដោយឡែក

- **Polyglot** – អាចប្រើបច្ចេកវិទ្យាផ្សេងៗគ្នាសម្រាប់សេវាផ្សេងៗ

- **Decentralized Data Management** – សេវានីមួយៗមាន database ផ្ទាល់ខ្លួន

- **Resilient** – ការបរាជ័យនៃសេវាមួយមិនប៉ះពាល់ដល់សេវាផ្សេងទៀត

### 💡 Benefits of Microservices:

- Scalability – អាច scale សេវានីមួយៗតាមតម្រូវការ

- Faster development – ក្រុមផ្សេងៗអាចធ្វើការបានប៉ារ៉ាឡែល

- Technology diversity – ប្រើបច្ចេកវិទ្យាល្អបំផុតសម្រាប់សេវានីមួយៗ

- Fault isolation – កំហុសក្នុងសេវាមួយមិនបង្កឱ្យកម្មវិធីទាំងមូលឈប់ដំណើរការ

- Easier deployment – Deploy តែសេវាដែលផ្លាស់ប្តូរ

## 15.2. Monolith vs Microservices (Monolith ទល់នឹង Microservices)

### 📌 ការប្រៀបធៀប:

| លក្ខណៈ (Feature) | Monolith | Microservices |
| --- | --- | --- |
| Deployment | Deploy entire application | Deploy individual services |
| Scalability | Scale entire application | Scale only needed services |
| Development | Single codebase | Multiple codebases |
| Team Structure | Single team | Multiple teams |
| Technology | Single technology stack | Multiple technologies |
| Database | Single database | Multiple databases |
| Complexity | Low complexity (simple) | High complexity (distributed) |
| Communication | Method calls | HTTP/REST or messaging |

**🎯 When to use Monolith:**

- Small applications

- Startup projects (MVP)

- Small development teams

- Simple domain logic

**🎯 When to use Microservices:**

- Large, complex applications

- Multiple development teams

- Need for independent scaling

- Different technology requirements

## 15.3. Service Discovery (ការរកឃើញសេវា)

### 📌 និយមន័យ (Definition):

**Service Discovery** គឺជាយន្តការដែលអនុញ្ញាតឱ្យ microservices រកឃើញ (find) និងទំនាក់ទំនង (communicate) ជាមួយគ្នាដោយមិនចាំបាច់ដឹងពី IP addresses ឬ ports ពិតប្រាកដ។ Spring Cloud Netflix Eureka គឺជា service discovery server ពេញនិយមមួយ។

### 🔹 Service Discovery Flow:

1. Services register themselves with the Service Registry (Eureka) at startup

2. Services send heartbeats to keep their registration active

3. Consumer services query the Service Registry to find provider services

4. Service Registry returns the location (IP + port) of the provider

5. Consumer calls the provider directly

## 15.4. Eureka Server (ម៉ាស៊ីនបម្រើ Eureka)

### 📌 Eureka Server គឺជា Service Registry:

### 🔹 Maven Dependencies:

```xml
<dependency>
    <groupId>org.springframework.cloud</groupId>
    <artifactId>spring-cloud-starter-netflix-eureka-server</artifactId>
</dependency>
<dependency>
    <groupId>org.springframework.cloud</groupId>
    <artifactId>spring-cloud-starter-config</artifactId>
</dependency>
```

### 🔹 Eureka Server Application:

```java
import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.SpringBootApplication;
import org.springframework.cloud.netflix.eureka.server.EnableEurekaServer;

@SpringBootApplication
@EnableEurekaServer
public class EurekaServerApplication {
    public static void main(String[] args) {
        SpringApplication.run(EurekaServerApplication.class, args);
    }
}
```

### 🔹 Eureka Server Configuration (application.yml):

```yaml
server:
  port: 8761

eureka:
  instance:
    hostname: localhost
  client:
    register-with-eureka: false
    fetch-registry: false
    service-url:
      defaultZone: http://localhost:8761/eureka/

spring:
  application:
    name: eureka-server
```

### 🔹 Eureka Client (Microservice) Configuration:

```yaml
spring:
  application:
    name: user-service

eureka:
  client:
    service-url:
      defaultZone: http://localhost:8761/eureka/
  instance:
    prefer-ip-address: true
```

### 🔹 Eureka Client Application:

```java
import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.SpringBootApplication;
import org.springframework.cloud.client.discovery.EnableDiscoveryClient;

@SpringBootApplication
@EnableDiscoveryClient
public class UserServiceApplication {
    public static void main(String[] args) {
        SpringApplication.run(UserServiceApplication.class, args);
    }
}
```

## 15.5. API Gateway (ច្រកទ្វារ API)

### 📌 និយមន័យ (Definition):

**API Gateway** គឺជាចំណុចចូលតែមួយ (single entry point) សម្រាប់ client ដើម្បីចូលដំណើរការ microservices។ វាដើរតួជា reverse proxy, routing requests ទៅកាន់ services ត្រឹមត្រូវ, និងអាចធ្វើ cross-cutting concerns (authentication, logging, rate limiting)។

### 🔹 Spring Cloud Gateway Maven Dependencies:

```xml
<dependency>
    <groupId>org.springframework.cloud</groupId>
    <artifactId>spring-cloud-starter-gateway</artifactId>
</dependency>
<dependency>
    <groupId>org.springframework.cloud</groupId>
    <artifactId>spring-cloud-starter-netflix-eureka-client</artifactId>
</dependency>
```

### 🔹 Gateway Configuration (application.yml):

```yaml
server:
  port: 8080

spring:
  application:
    name: api-gateway
  cloud:
    gateway:
      routes:
```

- id: user-service

```text
          uri: lb://user-service
          predicates:
```

- Path=/api/users/**

```text
          filters:
```

- name: CircuitBreaker

```text
              args:
                name: userService
                fallbackUri: forward:/fallback/users
```

- id: product-service

```text
          uri: lb://product-service
          predicates:
```

- Path=/api/products/**

- id: order-service

```text
          uri: lb://order-service
          predicates:
```

- Path=/api/orders/**

```text
eureka:
  client:
    service-url:
      defaultZone: http://localhost:8761/eureka/
```

## 15.6. Load Balancing (ការចែកចាយបន្ទុក)

### 📌 និយមន័យ (Definition):

**Load Balancing** គឺជាការចែកចាយ traffic ចូលទៅកាន់ instances ច្រើននៃ service ដើម្បីបង្កើន availability និង performance។ Spring Cloud ផ្តល់ client-side load balancing តាមរយៈ Spring Cloud LoadBalancer (ជំនួស Netflix Ribbon)។

### 🔹 Load Balancing Strategies:

- **Round Robin** – ចែកចាយស្មើៗគ្នាតាមលំដាប់ (default)

- **Random** – ជ្រើសរើស instance ចៃដន្យ

- **Weighted** – ចែកចាយតាមទម្ងន់ (instance ខ្លាំងជាងទទួល traffic ច្រើន)

- **Least Connections** – ផ្ញើទៅ instance ដែលមាន connection តិចបំផុត

### 🔹 Using LoadBalanced:

```java
import org.springframework.cloud.client.loadbalancer.LoadBalanced;
import org.springframework.context.annotation.Bean;
import org.springframework.context.annotation.Configuration;
import org.springframework.web.client.RestTemplate;

@Configuration
public class AppConfig {

    @Bean
    @LoadBalanced
    public RestTemplate restTemplate() {
        return new RestTemplate();
    }
}

// Using RestTemplate with service name (not URL)
@Service
public class UserServiceClient {

    @Autowired
    private RestTemplate restTemplate;

    public User getUser(Long id) {
        // Service name 'user-service' will be resolved by load balancer
        String url = "http://user-service/api/users/" + id;
        return restTemplate.getForObject(url, User.class);
    }
}
```

## 15.7. Config Server (ម៉ាស៊ីនបម្រើកំណត់រចនាសម្ព័ន្ធ)

### 📌 និយមន័យ (Definition):

**Spring Cloud Config Server** គឺជា centralized configuration service ដែលអនុញ្ញាតឱ្យអ្នកគ្រប់គ្រង configuration files (application.properties/yml) សម្រាប់ microservices ទាំងអស់ពីកន្លែងតែមួយ (Git repository)។

### 🔹 Config Server Maven Dependency:

```xml
<dependency>
    <groupId>org.springframework.cloud</groupId>
    <artifactId>spring-cloud-config-server</artifactId>
</dependency>
```

### 🔹 Config Server Application:

```java
import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.SpringBootApplication;
import org.springframework.cloud.config.server.EnableConfigServer;

@SpringBootApplication
@EnableConfigServer
public class ConfigServerApplication {
    public static void main(String[] args) {
        SpringApplication.run(ConfigServerApplication.class, args);
    }
}
```

### 🔹 Config Server Configuration (application.yml):

```yaml
server:
  port: 8888

spring:
  application:
    name: config-server
  cloud:
    config:
      server:
        git:
          uri: https://github.com/your-repo/config-repo
          default-label: main
          search-paths: '{application}'
```

### 🔹 Client Configuration (bootstrap.yml):

```yaml
spring:
  application:
    name: user-service
  cloud:
    config:
      uri: http://localhost:8888
      fail-fast: true
      retry:
        max-attempts: 6
        initial-interval: 1000
        multiplier: 1.1
```

## 15.8. OpenFeign (ការហៅសេវាផ្សេងទៀត)

### 📌 និយមន័យ (Definition):

**OpenFeign** គឺជា declarative HTTP client ដែលធ្វើឱ្យការហៅ REST APIs ពី microservice មួយទៅមួយទៀតកាន់តែងាយស្រួល។ វាបង្កើត implementation ដោយស្វ័យប្រវត្តិពី Java interfaces ដែលមាន annotations។

### 🔹 Maven Dependency:

```xml
<dependency>
    <groupId>org.springframework.cloud</groupId>
    <artifactId>spring-cloud-starter-openfeign</artifactId>
</dependency>
```

### 🔹 Enable Feign Clients:

```java
import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.SpringBootApplication;
import org.springframework.cloud.openfeign.EnableFeignClients;

@SpringBootApplication
@EnableFeignClients
public class OrderServiceApplication {
    public static void main(String[] args) {
        SpringApplication.run(OrderServiceApplication.class, args);
    }
}
```

### 🔹 Feign Client Interface:

```java
import org.springframework.cloud.openfeign.FeignClient;
import org.springframework.web.bind.annotation.*;

@FeignClient(name = "user-service", url = "http://user-service:8081")
public interface UserServiceClient {

    @GetMapping("/api/users/{id}")
    User getUserById(@PathVariable("id") Long id);

    @PostMapping("/api/users")
    User createUser(@RequestBody User user);

    @PutMapping("/api/users/{id}")
    User updateUser(@PathVariable("id") Long id, @RequestBody User user);

    @DeleteMapping("/api/users/{id}")
    void deleteUser(@PathVariable("id") Long id);
}

// Using the Feign Client
@Service
public class OrderService {

    @Autowired
    private UserServiceClient userServiceClient;

    public Order createOrder(OrderRequest request) {
        User user = userServiceClient.getUserById(request.getUserId());
        // Create order with user information
        return orderRepository.save(new Order(user, request));
    }
}
```

## 15.9. Circuit Breaker (Resilience4j)

### 📌 និយមន័យ (Definition):

**Circuit Breaker** គឺជា design pattern ដែលការពារការបរាជ័យជាខ្សែសង្វាក់ (cascading failures) នៅក្នុង microservices architecture។ នៅពេលដែល service មួយ បរាជ័យ, circuit breaker នឹង "បើក" (open) ហើយបញ្ជូន fallback response ជំនួសឱ្យការហៅ service ដែលបរាជ័យ។

### 🔹 Circuit Breaker States:

- **CLOSED** – ស្ថានភាពធម្មតា, requests ឆ្លងកាត់

- **OPEN** – ស្ថានភាពបរាជ័យ, requests ត្រូវបានបដិសេធភ្លាមៗ

- **HALF-OPEN** – ស្ថានភាពសាកល្បង, requests មួយចំនួនត្រូវបានអនុញ្ញាតដើម្បីពិនិត្យមើលថាតើ service បានងើបឡើងវិញដែរឬទេ

### 🔹 Maven Dependencies:

```xml
<dependency>
    <groupId>org.springframework.cloud</groupId>
    <artifactId>spring-cloud-starter-circuitbreaker-resilience4j</artifactId>
</dependency>
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-actuator</artifactId>
</dependency>
```

### 🔹 Circuit Breaker Configuration:

```text
resilience4j:
  circuitbreaker:
    instances:
      userService:
        register-health-indicator: true
        sliding-window-size: 10
        minimum-number-of-calls: 5
        permitted-number-of-calls-in-half-open-state: 3
        automatic-transition-from-open-to-half-open-enabled: true
        wait-duration-in-open-state: 5s
        failure-rate-threshold: 50
        event-consumer-buffer-size: 10
```

### 🔹 Using Circuit Breaker:

```java
import io.github.resilience4j.circuitbreaker.annotation.CircuitBreaker;
import org.springframework.stereotype.Service;

@Service
public class UserServiceClient {

    @Autowired
    private UserFeignClient userFeignClient;

    @CircuitBreaker(name = "userService", fallbackMethod = "getUserFallback")
    public User getUser(Long id) {
        return userFeignClient.getUserById(id);
    }

    // Fallback method
    public User getUserFallback(Long id, Exception ex) {
        System.out.println("Circuit breaker opened! Returning cached user.");
        return new User(id, "Cached User", "cached@example.com");
    }

    @CircuitBreaker(name = "userService")
    public List<User> getAllUsers() {
        return userFeignClient.getAllUsers();
    }
}

// Using with RestTemplate
@Service
public class ProductService {

    @Autowired
    private RestTemplate restTemplate;

    @CircuitBreaker(name = "inventoryService", fallbackMethod = "getStockFallback")
    public Integer getStock(Long productId) {
        String url = "http://inventory-service/api/stock/" + productId;
        return restTemplate.getForObject(url, Integer.class);
    }

    public Integer getStockFallback(Long productId, Exception ex) {
        return 0; // Assume out of stock
    }
}
```

## 15.10. Distributed Tracing (ការតាមដានចែកចាយ)

### 📌 និយមន័យ (Definition):

**Distributed Tracing** គឺជាបច្ចេកទេសតាមដានសំណើ (requests) នៅពេលដែលវាឆ្លងកាត់ microservices ច្រើន។ វាជួយក្នុងការ debug, monitor, និង optimize performance នៃ distributed systems។ Spring Cloud Sleuth រួមជាមួយ Zipkin ឬ Jaeger ត្រូវបានប្រើសម្រាប់ distributed tracing។

### 🔹 Maven Dependencies:

```xml
<dependency>
    <groupId>org.springframework.cloud</groupId>
    <artifactId>spring-cloud-starter-sleuth</artifactId>
</dependency>
<dependency>
    <groupId>org.springframework.cloud</groupId>
    <artifactId>spring-cloud-sleuth-zipkin</artifactId>
</dependency>
```

### 🔹 Tracing Configuration (application.yml):

```yaml
spring:
  sleuth:
    sampler:
      probability: 1.0
    trace-id128: true
    baggage-keys:
```

- userId

```text
  zipkin:
    base-url: http://localhost:9411
    sender:
      type: web
```

### 🔧 Zipkin Setup:

- Download Zipkin JAR: curl -sSL https://zipkin.io/quickstart.sh | bash -s

- Run Zipkin: java -jar zipkin.jar

- Access UI: http://localhost:9411

### 💡 Distributed Tracing Benefits:

- Visualize request flow across services

- Identify performance bottlenecks

- Debug distributed errors

- Monitor service dependencies

- Analyze latency issues

### 📚 សង្ខេបមេរៀនទី១៥ (Module 15 Summary)

នៅក្នុងមេរៀននេះ អ្នកបានរៀនអំពី Spring Boot Microservices៖

- **What are Microservices?** – Small, independent, loosely coupled services

- **Monolith vs Microservices** – Trade-offs between simplicity and complexity

- **Service Discovery** – Eureka Server for service registration and discovery

- **API Gateway** – Single entry point with Spring Cloud Gateway

- **Load Balancing** – Client-side load balancing with Spring Cloud LoadBalancer

- **Config Server** – Centralized configuration management with Git backend

- **OpenFeign** – Declarative HTTP client for service-to-service communication

- **Circuit Breaker** – Resilience4j for fault tolerance and fallbacks

- **Distributed Tracing** – Sleuth + Zipkin for request tracing across services

# មេរៀនទី១៦: Messaging & Real-Time (ការផ្ញើសារ និងពេលវេលាជាក់ស្តែង)

### 📖 សេចក្តីផ្តើម (Introduction):
Messaging និង Real-Time communication គឺជាផ្នែកសំខាន់ក្នុងការអភិវឌ្ឍន៍កម្មវិធីទំនើបៗ — chat applications, live notifications, stock trading, gaming។ មេរៀននេះនឹងបង្រៀនអ្នកពី WebSocket, STOMP Protocol, RabbitMQ, Apache Kafka, Event-Driven Architecture, និង Real-Time Notification។

## 16.1. WebSocket (វេបសុកឃីត)

### 📌 និយមន័យ (Definition):

**WebSocket** គឺជា protocol ដែលផ្តល់ full-duplex communication channels តាមរយៈ single TCP connection។ វាអនុញ្ញាតឱ្យ server ផ្ញើ data ទៅ client ដោយមិនចាំបាច់ client ស្នើសុំ (request) ជាមុន — ល្អសម្រាប់ real-time applications។

### 🔹 WebSocket vs HTTP:

| លក្ខណៈ (Feature) | HTTP | WebSocket |
| --- | --- | --- |
| Communication Direction | Client → Server (Request-Response) | Bidirectional (Both ways) |
| Connection | Short-lived (per request) | Persistent (single connection) |
| Overhead | High (headers each request) | Low (after handshake) |
| Real-time | No (polling required) | Yes (server can push data) |

### 🔹 Maven Dependencies:

```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-websocket</artifactId>
</dependency>
```

### 🔹 WebSocket Configuration:

```java
import org.springframework.context.annotation.Configuration;
import org.springframework.web.socket.config.annotation.EnableWebSocket;
import org.springframework.web.socket.config.annotation.WebSocketConfigurer;
import org.springframework.web.socket.config.annotation.WebSocketHandlerRegistry;

@Configuration
@EnableWebSocket
public class WebSocketConfig implements WebSocketConfigurer {

    @Override
    public void registerWebSocketHandlers(WebSocketHandlerRegistry registry) {
```

registry.addHandler(new ChatWebSocketHandler(), "/ws/chat")

```java
                .setAllowedOrigins("*");
    }
}

// WebSocket Handler
import org.springframework.web.socket.TextMessage;
import org.springframework.web.socket.WebSocketSession;
import org.springframework.web.socket.handler.TextWebSocketHandler;
import java.util.concurrent.CopyOnWriteArrayList;

public class ChatWebSocketHandler extends TextWebSocketHandler {

    private final CopyOnWriteArrayList<WebSocketSession> sessions = new CopyOnWriteArrayList<>();

    @Override
    public void afterConnectionEstablished(WebSocketSession session) {
        sessions.add(session);
        System.out.println("New connection: " + session.getId());
    }

    @Override
    protected void handleTextMessage(WebSocketSession session, TextMessage message) throws Exception {
        String payload = message.getPayload();
        System.out.println("Received: " + payload);

        // Broadcast to all connected clients
        for (WebSocketSession s : sessions) {
            if (s.isOpen()) {
                s.sendMessage(new TextMessage("Broadcast: " + payload));
            }
        }
    }

    @Override
    public void afterConnectionClosed(WebSocketSession session, CloseStatus status) {
        sessions.remove(session);
        System.out.println("Connection closed: " + session.getId());
    }
}
```

### 🔹 JavaScript Client:

```text
// Connect to WebSocket
const socket = new WebSocket('ws://localhost:8080/ws/chat');

// Connection opened
socket.addEventListener('open', function (event) {
    console.log('Connected to WebSocket');
    socket.send('Hello Server!');
});

// Listen for messages
socket.addEventListener('message', function (event) {
    console.log('Message from server: ', event.data);
    // Display message in UI
});

// Send message
function sendMessage(msg) {
    socket.send(msg);
}

// Close connection
function closeConnection() {
    socket.close();
}
```

## 16.2. STOMP Protocol (ស្តុប)

### 📌 និយមន័យ (Definition):

**STOMP (Simple Text Oriented Messaging Protocol)** គឺជា protocol សម្រាប់ messaging ដែលដំណើរការលើ WebSocket។ Spring Boot ផ្តល់ STOMP support តាមរយៈspring-messaging module និង SockJS fallback។

### 🔹 STOMP Configuration:

```java
import org.springframework.context.annotation.Configuration;
import org.springframework.messaging.simp.config.MessageBrokerRegistry;
import org.springframework.web.socket.config.annotation.EnableWebSocketMessageBroker;
import org.springframework.web.socket.config.annotation.StompEndpointRegistry;
import org.springframework.web.socket.config.annotation.WebSocketMessageBrokerConfigurer;

@Configuration
@EnableWebSocketMessageBroker
public class StompWebSocketConfig implements WebSocketMessageBrokerConfigurer {

    @Override
    public void configureMessageBroker(MessageBrokerRegistry config) {
        // Enable simple in-memory broker
        config.enableSimpleBroker("/topic", "/queue");
        // Prefix for messages bound for @MessageMapping methods
        config.setApplicationDestinationPrefixes("/app");
        // Prefix for user-specific messages
        config.setUserDestinationPrefix("/user");
    }

    @Override
    public void registerStompEndpoints(StompEndpointRegistry registry) {
```

registry.addEndpoint("/ws")

.setAllowedOrigins("*")

```text
                .withSockJS(); // Fallback for browsers without WebSocket
    }
}
```

### 🔹 STOMP Controller:

```java
import org.springframework.messaging.handler.annotation.MessageMapping;
import org.springframework.messaging.handler.annotation.SendTo;
import org.springframework.messaging.simp.SimpMessagingTemplate;
import org.springframework.stereotype.Controller;
import java.time.LocalDateTime;

@Controller
public class ChatController {

    @Autowired
    private SimpMessagingTemplate messagingTemplate;

    // Send to specific destination
    @MessageMapping("/chat.send")
    @SendTo("/topic/messages")
    public ChatMessage sendMessage(ChatMessage message) {
        message.setTimestamp(LocalDateTime.now());
        return message;
    }

    // Send to specific user
    @MessageMapping("/chat.private")
    public void sendPrivateMessage(PrivateMessage message) {
```

messagingTemplate.convertAndSendToUser(

message.getRecipient(),

"/queue/messages",

message

```java
        );
    }
}

// Message DTO
public class ChatMessage {
    private String sender;
    private String content;
    private LocalDateTime timestamp;
    private String type; // CHAT, JOIN, LEAVE
    // Getters and setters
}
```

### 🔹 JavaScript STOMP Client:

```java
// Include STOMP and SockJS libraries
// <script src="https://cdn.jsdelivr.net/npm/sockjs-client@1/dist/sockjs.min.js"></script>
// <script src="https://cdnjs.cloudflare.com/ajax/libs/stomp.js/2.3.3/stomp.min.js"></script>

// Connect to STOMP endpoint
const socket = new SockJS('/ws');
const stompClient = Stomp.over(socket);

stompClient.connect({}, function(frame) {
    console.log('Connected: ' + frame);

    // Subscribe to public topic
    stompClient.subscribe('/topic/messages', function(message) {
        const chatMessage = JSON.parse(message.body);
        console.log('Received: ', chatMessage);
        displayMessage(chatMessage);
    });

    // Subscribe to private queue
    stompClient.subscribe('/user/queue/messages', function(message) {
        const privateMessage = JSON.parse(message.body);
        console.log('Private message: ', privateMessage);
    });
});

// Send public message
function sendPublicMessage(sender, content) {
    stompClient.send("/app/chat.send", {}, JSON.stringify({
        sender: sender,
        content: content,
        type: 'CHAT'
    }));
}

// Send private message
function sendPrivateMessage(recipient, content) {
    stompClient.send("/app/chat.private", {}, JSON.stringify({
        recipient: recipient,
        content: content,
        sender: currentUser
    }));
}
```

## 16.3. RabbitMQ (រ៉ាប៊ីតអឹមឃ្យូ)

### 📌 និយមន័យ (Definition):

**RabbitMQ** គឺជា message broker ដ៏ពេញនិយមដែលអនុវត្ត AMQP (Advanced Message Queuing Protocol)។ វាអនុញ្ញាតឱ្យ microservices ទំនាក់ទំនងគ្នាតាមរយៈ asynchronous messaging។

### 🔹 Maven Dependencies:

```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-amqp</artifactId>
</dependency>
```

### 🔹 RabbitMQ Configuration (application.yml):

```yaml
spring:
  rabbitmq:
    host: localhost
    port: 5672
    username: guest
    password: guest
    virtual-host: /
    connection-timeout: 5000
```

### 🔹 RabbitMQ Configuration Class:

```java
import org.springframework.amqp.core.*;
import org.springframework.amqp.rabbit.connection.ConnectionFactory;
import org.springframework.amqp.rabbit.core.RabbitTemplate;
import org.springframework.amqp.support.converter.Jackson2JsonMessageConverter;
import org.springframework.context.annotation.Bean;
import org.springframework.context.annotation.Configuration;

@Configuration
public class RabbitMQConfig {

    public static final String QUEUE_NAME = "order.queue";
    public static final String EXCHANGE_NAME = "order.exchange";
    public static final String ROUTING_KEY = "order.routingkey";

    @Bean
    public Queue queue() {
        return new Queue(QUEUE_NAME, true);
    }

    @Bean
    public TopicExchange exchange() {
        return new TopicExchange(EXCHANGE_NAME);
    }

    @Bean
    public Binding binding(Queue queue, TopicExchange exchange) {
        return BindingBuilder.bind(queue).to(exchange).with(ROUTING_KEY);
    }

    @Bean
    public Jackson2JsonMessageConverter messageConverter() {
        return new Jackson2JsonMessageConverter();
    }

    @Bean
    public RabbitTemplate rabbitTemplate(ConnectionFactory connectionFactory) {
        RabbitTemplate template = new RabbitTemplate(connectionFactory);
        template.setMessageConverter(messageConverter());
        return template;
    }
}
```

### 🔹 RabbitMQ Producer:

```java
import org.springframework.amqp.rabbit.core.RabbitTemplate;
import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.stereotype.Service;

@Service
public class OrderProducer {

    @Autowired
    private RabbitTemplate rabbitTemplate;

    public void sendOrder(Order order) {
```

rabbitTemplate.convertAndSend(

RabbitMQConfig.EXCHANGE_NAME,

RabbitMQConfig.ROUTING_KEY,

order

```java
        );
        System.out.println("Order sent: " + order);
    }
}
```

### 🔹 RabbitMQ Consumer:

```java
import org.springframework.amqp.rabbit.annotation.RabbitListener;
import org.springframework.stereotype.Component;

@Component
public class OrderConsumer {

    @RabbitListener(queues = RabbitMQConfig.QUEUE_NAME)
    public void receiveOrder(Order order) {
        System.out.println("Order received: " + order);
        // Process the order
        processOrder(order);
    }

    private void processOrder(Order order) {
        // Business logic
        System.out.println("Processing order: " + order.getId());
    }
}
```

## 16.4. Apache Kafka (អាផាឈី កាហ្វកា)

### 📌 និយមន័យ (Definition):

**Apache Kafka** គឺជា distributed event streaming platform ដែលត្រូវបានប្រើសម្រាប់ high-throughput, low-latency messaging។ វាល្អសម្រាប់ event-driven architectures, real-time analytics, និង data pipelines។

### 🔹 Kafka vs RabbitMQ:

| លក្ខណៈ | RabbitMQ | Kafka |
| --- | --- | --- |
| Message model | Queue-based | Log-based |
| Throughput | Moderate | Very High |
| Message order | Not guaranteed | Guaranteed within partition |
| Message retention | Removed after consumption | Configurable retention period |

### 🔹 Maven Dependencies:

```xml
<dependency>
    <groupId>org.springframework.kafka</groupId>
    <artifactId>spring-kafka</artifactId>
</dependency>
```

### 🔹 Kafka Configuration (application.yml):

```yaml
spring:
  kafka:
    bootstrap-servers: localhost:9092
    producer:
      key-serializer: org.apache.kafka.common.serialization.StringSerializer
      value-serializer: org.springframework.kafka.support.serializer.JsonSerializer
    consumer:
      group-id: my-group
      key-deserializer: org.apache.kafka.common.serialization.StringDeserializer
      value-deserializer: org.springframework.kafka.support.serializer.JsonDeserializer
      properties:
        spring.json.trusted.packages: '*'
```

### 🔹 Kafka Producer:

```java
import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.kafka.core.KafkaTemplate;
import org.springframework.stereotype.Service;

@Service
public class KafkaProducer {

    @Autowired
    private KafkaTemplate<String, Object> kafkaTemplate;

    private static final String TOPIC = "user-events";

    public void sendUserEvent(UserEvent event) {
        kafkaTemplate.send(TOPIC, event);
        System.out.println("Event sent: " + event);
    }

    public void sendWithKey(String key, Object message) {
        kafkaTemplate.send(TOPIC, key, message);
    }
}
```

### 🔹 Kafka Consumer:

```properties
import org.springframework.kafka.annotation.KafkaListener;
import org.springframework.stereotype.Component;

@Component
public class KafkaConsumer {

    @KafkaListener(topics = "user-events", groupId = "my-group")
    public void listen(UserEvent event) {
        System.out.println("Received event: " + event);
        // Process event
    }

    @KafkaListener(topics = "user-events", groupId = "my-group",
                   containerFactory = "batchFactory")
    public void listenBatch(List<UserEvent> events) {
        System.out.println("Received batch of " + events.size() + " events");
        events.forEach(this::processEvent);
    }

    private void processEvent(UserEvent event) {
        // Business logic
    }
}
```

### 🔹 Kafka Configuration Class:

```java
import org.apache.kafka.clients.consumer.ConsumerConfig;
import org.apache.kafka.clients.producer.ProducerConfig;
import org.apache.kafka.common.serialization.StringDeserializer;
import org.apache.kafka.common.serialization.StringSerializer;
import org.springframework.context.annotation.Bean;
import org.springframework.context.annotation.Configuration;
import org.springframework.kafka.config.ConcurrentKafkaListenerContainerFactory;
import org.springframework.kafka.core.*;
import org.springframework.kafka.support.serializer.JsonDeserializer;
import org.springframework.kafka.support.serializer.JsonSerializer;
import java.util.HashMap;
import java.util.Map;

@Configuration
public class KafkaConfig {

    @Bean
    public ProducerFactory<String, Object> producerFactory() {
        Map<String, Object> config = new HashMap<>();
        config.put(ProducerConfig.BOOTSTRAP_SERVERS_CONFIG, "localhost:9092");
        config.put(ProducerConfig.KEY_SERIALIZER_CLASS_CONFIG, StringSerializer.class);
        config.put(ProducerConfig.VALUE_SERIALIZER_CLASS_CONFIG, JsonSerializer.class);
        return new DefaultKafkaProducerFactory<>(config);
    }

    @Bean
    public KafkaTemplate<String, Object> kafkaTemplate() {
        return new KafkaTemplate<>(producerFactory());
    }

    @Bean
    public ConsumerFactory<String, Object> consumerFactory() {
        Map<String, Object> config = new HashMap<>();
        config.put(ConsumerConfig.BOOTSTRAP_SERVERS_CONFIG, "localhost:9092");
        config.put(ConsumerConfig.GROUP_ID_CONFIG, "my-group");
        config.put(ConsumerConfig.KEY_DESERIALIZER_CLASS_CONFIG, StringDeserializer.class);
        config.put(ConsumerConfig.VALUE_DESERIALIZER_CLASS_CONFIG, JsonDeserializer.class);
        config.put(JsonDeserializer.TRUSTED_PACKAGES, "*");
        return new DefaultKafkaConsumerFactory<>(config);
    }

    @Bean
    public ConcurrentKafkaListenerContainerFactory<String, Object> kafkaListenerContainerFactory() {
```

ConcurrentKafkaListenerContainerFactory<String, Object> factory =

```text
            new ConcurrentKafkaListenerContainerFactory<>();
        factory.setConsumerFactory(consumerFactory());
        return factory;
    }
}
```

## 16.5. Event-Driven Architecture (ស្ថាបត្យកម្មជំរុញដោយព្រឹត្តិការណ៍)

### 📌 និយមន័យ (Definition):

**Event-Driven Architecture (EDA)** គឺជា architectural pattern ដែលកម្មវិធីឆ្លើយតប (respond) ទៅនឹង events (state changes)។ Services ទំនាក់ទំនងគ្នាតាមរយៈ asynchronous events ជំនួសឱ្យ synchronous HTTP calls។

### 🔹 Event-Driven Architecture Components:

- **Event Producer** – Service that publishes events

- **Event Broker** – Message queue (RabbitMQ, Kafka) that routes events

- **Event Consumer** – Service that subscribes and processes events

- **Event Store** – Persistent storage for events (for replay)

### 🔹 Event Class:

```java
import lombok.Data;
import java.time.LocalDateTime;
import java.util.UUID;

@Data
public abstract class BaseEvent {
    private String eventId = UUID.randomUUID().toString();
    private LocalDateTime timestamp = LocalDateTime.now();
    private String eventType;
}

public class OrderCreatedEvent extends BaseEvent {
    private Long orderId;
    private Long userId;
    private Double totalAmount;
    private List<OrderItem> items;

    public OrderCreatedEvent() {
        setEventType("ORDER_CREATED");
    }
}

public class PaymentProcessedEvent extends BaseEvent {
    private Long orderId;
    private Double amount;
    private String status; // SUCCESS, FAILED
    private String transactionId;

    public PaymentProcessedEvent() {
        setEventType("PAYMENT_PROCESSED");
    }
}
```

### 🔹 Event Publisher (Producer):

```java
import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.context.ApplicationEventPublisher;
import org.springframework.stereotype.Service;

@Service
public class OrderService {

    @Autowired
    private ApplicationEventPublisher eventPublisher;

    @Autowired
    private KafkaTemplate<String, Object> kafkaTemplate;

    public Order createOrder(OrderRequest request) {
        Order order = orderRepository.save(new Order(request));

        // Publish event using Spring Application Events
        OrderCreatedEvent event = new OrderCreatedEvent();
        event.setOrderId(order.getId());
        event.setUserId(request.getUserId());
        event.setTotalAmount(request.getTotalAmount());
        event.setItems(request.getItems());

        eventPublisher.publishEvent(event);

        // Or publish to Kafka
        kafkaTemplate.send("order-events", event);

        return order;
    }
}
```

### 🔹 Event Listener (Consumer):

```java
import org.springframework.context.event.EventListener;
import org.springframework.kafka.annotation.KafkaListener;
import org.springframework.stereotype.Component;

@Component
public class NotificationService {

    // Listen to Spring Application Events
    @EventListener
    public void handleOrderCreated(OrderCreatedEvent event) {
        System.out.println("Sending confirmation email for order: " + event.getOrderId());
        // Send email to user
    }

    // Listen to Kafka events
    @KafkaListener(topics = "order-events")
    public void handleKafkaEvent(OrderCreatedEvent event) {
        System.out.println("Processing event from Kafka: " + event.getOrderId());
        // Process event
    }
}

@Component
public class InventoryService {

    @EventListener
    public void handleOrderCreated(OrderCreatedEvent event) {
        System.out.println("Reserving inventory for order: " + event.getOrderId());
        // Update inventory
    }
}
```

## 16.6. Real-Time Notification (ការជូនដំណឹងពេលវេលាជាក់ស្តែង)

### 📌 ការបង្កើត Real-Time Notification System:

### 🔹 Notification Controller (WebSocket):

```java
import org.springframework.messaging.handler.annotation.MessageMapping;
import org.springframework.messaging.handler.annotation.SendTo;
import org.springframework.messaging.simp.SimpMessagingTemplate;
import org.springframework.stereotype.Controller;

@Controller
public class NotificationController {

    @Autowired
    private SimpMessagingTemplate messagingTemplate;

    // Send notification to all users
    @MessageMapping("/notification.broadcast")
    @SendTo("/topic/notifications")
    public Notification broadcastNotification(Notification notification) {
        notification.setTimestamp(LocalDateTime.now());
        return notification;
    }

    // Send notification to specific user
    public void sendNotificationToUser(String userId, Notification notification) {
```

messagingTemplate.convertAndSendToUser(

userId,

"/queue/notifications",

notification

```text
        );
    }

    // Send notification to group
    public void sendNotificationToGroup(String groupId, Notification notification) {
        messagingTemplate.convertAndSend("/topic/groups/" + groupId, notification);
    }
}
```

### 🔹 Notification Service:

```java
import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.stereotype.Service;

@Service
public class NotificationService {

    @Autowired
    private NotificationController notificationController;

    @Autowired
    private KafkaTemplate<String, Object> kafkaTemplate;

    public void sendNotification(NotificationRequest request) {
```

Notification notification = Notification.builder()

.id(UUID.randomUUID().toString())

.title(request.getTitle())

.message(request.getMessage())

.type(request.getType())

.userId(request.getUserId())

.createdAt(LocalDateTime.now())

.read(false)

```text
            .build();

        // Save to database
        notificationRepository.save(notification);

        // Send real-time via WebSocket
        if (request.getUserId() != null) {
```

notificationController.sendNotificationToUser(

request.getUserId(),

notification

```text
            );
        } else {
            notificationController.broadcastNotification(notification);
        }

        // Publish to Kafka for other services
        kafkaTemplate.send("notification-events", notification);
    }
}
```

### 🔹 JavaScript Real-Time Notification Client:

```properties
// Connect to STOMP
const stompClient = Stomp.over(new SockJS('/ws'));
const userId = getCurrentUserId();

stompClient.connect({}, function(frame) {
    console.log('Connected for notifications');

    // Subscribe to public notifications
    stompClient.subscribe('/topic/notifications', function(message) {
        const notification = JSON.parse(message.body);
        displayNotification(notification);
    });

    // Subscribe to private notifications
    stompClient.subscribe('/user/' + userId + '/queue/notifications', function(message) {
        const notification = JSON.parse(message.body);
        displayPrivateNotification(notification);
    });

    // Subscribe to group notifications
    const groupId = getUserGroup();
    stompClient.subscribe('/topic/groups/' + groupId, function(message) {
        const notification = JSON.parse(message.body);
        displayGroupNotification(notification);
    });
});

// Display notification in UI
function displayNotification(notification) {
    const toast = document.createElement('div');
    toast.className = 'notification-toast ' + notification.type;
    toast.innerHTML = `
        <strong>${notification.title}</strong>
        <p>${notification.message}</p>
        <small>${new Date(notification.timestamp).toLocaleTimeString()}</small>
    `;
    document.body.appendChild(toast);

    setTimeout(() => toast.remove(), 5000);
}

// Send notification from frontend
function sendNotification(title, message, type) {
    stompClient.send('/app/notification.broadcast', {}, JSON.stringify({
        title: title,
        message: message,
        type: type
    }));
}
```

### 💡 Real-Time Notification Best Practices:

- ប្រើ WebSocket + STOMP សម្រាប់ real-time communication

- ផ្ទុក notifications ក្នុង database សម្រាប់ history

- អនុវត្ត read receipts ដើម្បី track ថាអ្នកណាបានអាន

- ប្រើ notification aggregation ដើម្បីកាត់បន្ថយ spam

- គាំទ្រ do-not-disturb hours

- ប្រើ push notifications សម្រាប់ mobile devices

### 📊 Messaging Summary:

| Technology | Use Case | Pros | Cons |
| --- | --- | --- | --- |
| WebSocket | Real-time bi-directional | Low latency, persistent connection | Stateful, complex scaling |
| RabbitMQ | Task queues, RPC | Mature, flexible routing | Lower throughput |
| Kafka | Event streaming, analytics | High throughput, replayable | Complex operations |

### 📚 សង្ខេបមេរៀនទី១៦ (Module 16 Summary)

នៅក្នុងមេរៀននេះ អ្នកបានរៀនអំពី Messaging & Real-Time នៅក្នុង Spring Boot៖

- **WebSocket** – Full-duplex communication, persistent connection, real-time data push

- **STOMP Protocol** – Messaging protocol over WebSocket, topic/queue semantics, user targeting

- **RabbitMQ** – AMQP message broker, task queues, RPC, flexible routing

- **Apache Kafka** – Distributed event streaming, high throughput, replayable events

- **Event-Driven Architecture** – Asynchronous communication, event producers/consumers, loose coupling

- **Real-Time Notification** – WebSocket + STOMP for notifications, user targeting, broadcast

# មេរៀនទី១៧: Caching & Performance (ការផ្ទុកក្នុង Cache និងប្រសិទ្ធភាព)

### 📖 សេចក្តីផ្តើម (Introduction):
Caching និង Performance optimization គឺជាផ្នែកសំខាន់ក្នុងការបង្កើតកម្មវិធីដែលមានល្បឿនលឿន និងអាចបត់បែនបាន (scalable)។ មេរៀននេះនឹងបង្រៀនអ្នកពី Spring Cache, Redis Integration, Cache Eviction, Performance Monitoring, Profiling, Async Programming, និង Scheduling Tasks។

## 17.1. Spring Cache

### 📌 និយមន័យ (Definition):

**Spring Cache** គឺជា abstraction layer ដែលធ្វើឱ្យការប្រើប្រាស់ caching ក្នុង Spring applications កាន់តែងាយស្រួល។ វាផ្តល់នូវ annotations (@Cacheable, @CacheEvict, @CachePut) ដើម្បីគ្រប់គ្រង cache ដោយស្វ័យប្រវត្តិ។

### 🔹 Maven Dependencies:

```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-cache</artifactId>
</dependency>
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-data-redis</artifactId>
</dependency>
```

### 🔹 Enable Caching:

```java
import org.springframework.cache.annotation.EnableCaching;
import org.springframework.context.annotation.Configuration;

@Configuration
@EnableCaching
public class CacheConfig {
    // Caching is enabled
}
```

### 🔹 Cache Annotations:

| Annotation | Description | Example |
| --- | --- | --- |
| @Cacheable | Store result in cache, return from cache on subsequent calls | @Cacheable("users") |
| @CacheEvict | Remove entries from cache | @CacheEvict("users") |
| @CachePut | Update cache without interfering method execution | @CachePut("users") |
| @Caching | Group multiple cache annotations | @Caching(evict = {@CacheEvict("users")}) |

### 🔹 Using @Cacheable:

```java
import org.springframework.cache.annotation.Cacheable;
import org.springframework.stereotype.Service;

@Service
public class UserService {

    @Autowired
    private UserRepository userRepository;

    // Cache result by id
    @Cacheable(value = "users", key = "#id")
    public User getUserById(Long id) {
        System.out.println("Fetching user from database: " + id);
        return userRepository.findById(id).orElse(null);
    }

    // Cache with condition
    @Cacheable(value = "users", key = "#id", condition = "#id > 10")
    public User getUserWithCondition(Long id) {
        return userRepository.findById(id).orElse(null);
    }

    // Cache with unless (don't cache if condition is true)
    @Cacheable(value = "users", key = "#id", unless = "#result == null")
    public Optional<User> getUserOptional(Long id) {
        return userRepository.findById(id);
    }

    // Cache by multiple keys
    @Cacheable(value = "users", key = "#name + ':' + #email")
    public User findByNameAndEmail(String name, String email) {
        return userRepository.findByNameAndEmail(name, email);
    }

    // Cache list result
    @Cacheable(value = "allUsers", key = "'all'")
    public List<User> getAllUsers() {
        System.out.println("Fetching all users from database");
        return userRepository.findAll();
    }

    // Cache with custom key generator
    @Cacheable(value = "users", keyGenerator = "customKeyGenerator")
    public User getUserByCustomKey(Long id, String name) {
        return userRepository.findById(id).orElse(null);
    }
}
```

### 🔹 Cache Configuration (application.yml):

```yaml
spring:
  cache:
    type: redis
    cache-names:
```

- users

- products

- orders

```text
    redis:
      time-to-live: 60000
      cache-null-values: false
      key-prefix: myapp:
```

## 17.2. Redis Integration

### 📌 និយមន័យ (Definition):

**Redis** គឺជា in-memory data structure store ដែលត្រូវបានប្រើជា database, cache, និង message broker។ វាលឿនណាស់ (sub-millisecond latency) និងគាំទ្រ data structures (strings, hashes, lists, sets, sorted sets)។

### 🔹 Redis Configuration:

```java
import org.springframework.context.annotation.Bean;
import org.springframework.context.annotation.Configuration;
import org.springframework.data.redis.cache.RedisCacheConfiguration;
import org.springframework.data.redis.cache.RedisCacheManager;
import org.springframework.data.redis.connection.RedisConnectionFactory;
import org.springframework.data.redis.core.RedisTemplate;
import org.springframework.data.redis.serializer.Jackson2JsonRedisSerializer;
import org.springframework.data.redis.serializer.RedisSerializationContext;
import org.springframework.data.redis.serializer.StringRedisSerializer;
import java.time.Duration;

@Configuration
public class RedisConfig {

    @Bean
    public RedisTemplate<String, Object> redisTemplate(RedisConnectionFactory factory) {
        RedisTemplate<String, Object> template = new RedisTemplate<>();
        template.setConnectionFactory(factory);

        // Key serializer
        template.setKeySerializer(new StringRedisSerializer());

        // Value serializer (JSON)
```

Jackson2JsonRedisSerializer<Object> jsonSerializer =

```text
            new Jackson2JsonRedisSerializer<>(Object.class);
        template.setValueSerializer(jsonSerializer);

        template.setHashKeySerializer(new StringRedisSerializer());
        template.setHashValueSerializer(jsonSerializer);

        template.afterPropertiesSet();
        return template;
    }

    @Bean
    public RedisCacheManager cacheManager(RedisConnectionFactory factory) {
```

RedisCacheConfiguration config = RedisCacheConfiguration.defaultCacheConfig()

.entryTtl(Duration.ofMinutes(10))

.serializeKeysWith(RedisSerializationContext.SerializationPair

.fromSerializer(new StringRedisSerializer()))

.serializeValuesWith(RedisSerializationContext.SerializationPair

.fromSerializer(new Jackson2JsonRedisSerializer<>(Object.class)))

```text
            .disableCachingNullValues();

        return RedisCacheManager.builder(factory)
```

.cacheDefaults(config)

```text
            .build();
    }
}
```

### 🔹 Redis Operations:

```java
import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.data.redis.core.RedisTemplate;
import org.springframework.stereotype.Service;
import java.util.concurrent.TimeUnit;

@Service
public class RedisService {

    @Autowired
    private RedisTemplate<String, Object> redisTemplate;

    // String operations
    public void setValue(String key, Object value) {
        redisTemplate.opsForValue().set(key, value);
    }

    public void setValueWithExpiry(String key, Object value, long timeout, TimeUnit unit) {
        redisTemplate.opsForValue().set(key, value, timeout, unit);
    }

    public Object getValue(String key) {
        return redisTemplate.opsForValue().get(key);
    }

    public Boolean deleteKey(String key) {
        return redisTemplate.delete(key);
    }

    // Hash operations (like Map)
    public void putHash(String key, String hashKey, Object value) {
        redisTemplate.opsForHash().put(key, hashKey, value);
    }

    public Object getHash(String key, String hashKey) {
        return redisTemplate.opsForHash().get(key, hashKey);
    }

    public Map<Object, Object> getAllHash(String key) {
        return redisTemplate.opsForHash().entries(key);
    }

    // List operations (FIFO)
    public void pushToList(String key, Object value) {
        redisTemplate.opsForList().rightPush(key, value);
    }

    public Object popFromList(String key) {
        return redisTemplate.opsForList().leftPop(key);
    }

    public List<Object> getListRange(String key, long start, long end) {
        return redisTemplate.opsForList().range(key, start, end);
    }

    // Set operations (unique values)
    public void addToSet(String key, Object... values) {
        redisTemplate.opsForSet().add(key, values);
    }

    public Set<Object> getSetMembers(String key) {
        return redisTemplate.opsForSet().members(key);
    }

    // Check if key exists
    public Boolean hasKey(String key) {
        return redisTemplate.hasKey(key);
    }

    // Get expiry time
    public Long getExpire(String key) {
        return redisTemplate.getExpire(key);
    }
}
```

### 🔹 Redis Application Properties:

```yaml
spring:
  data:
    redis:
      host: localhost
      port: 6379
      password:
      timeout: 2000ms
      lettuce:
        pool:
          max-active: 8
          max-idle: 8
          min-idle: 0
          max-wait: -1ms
```

## 17.3. Cache Eviction (ការលុបចេញពី Cache)

### 📌 និយមន័យ (Definition):

**Cache Eviction** គឺជាការលុប (remove) entries ពី cache នៅពេលដែលទិន្នន័យ ត្រូវបានធ្វើបច្ចុប្បន្នភាព (updated) ឬលុប (deleted) ដើម្បីធានាថា cache តែងតែមានភាពស្រប (consistent) ជាមួយ database។

```java
import org.springframework.cache.annotation.CacheEvict;
import org.springframework.cache.annotation.Caching;
import org.springframework.stereotype.Service;

@Service
public class ProductService {

    // Evict single entry by key
    @CacheEvict(value = "products", key = "#id")
    public void deleteProduct(Long id) {
        productRepository.deleteById(id);
        System.out.println("Product deleted and cache evicted for id: " + id);
    }

    // Evict all entries in cache
    @CacheEvict(value = "products", allEntries = true)
    public void clearAllProductCache() {
        System.out.println("All product cache cleared");
    }

    // Evict before method execution
    @CacheEvict(value = "products", key = "#id", beforeInvocation = true)
    public void updateProduct(Long id, ProductDto dto) {
        // If exception occurs, cache is still evicted
        productRepository.update(id, dto);
    }

    // Multiple cache evictions
    @Caching(evict = {
        @CacheEvict(value = "products", key = "#id"),
        @CacheEvict(value = "allProducts", allEntries = true)
    })
    public void deleteProductWithMultipleCaches(Long id) {
        productRepository.deleteById(id);
    }

    // Conditional eviction
    @CacheEvict(value = "products", key = "#id", condition = "#id > 0")
    public void conditionalEvict(Long id) {
        productRepository.deleteById(id);
    }

    // Update cache with @CachePut
    @CachePut(value = "products", key = "#result.id")
    public Product updateProduct(Product product) {
        return productRepository.save(product);
    }
}

// Scheduled cache eviction
@Component
public class ScheduledCacheEviction {

    @Autowired
    private CacheManager cacheManager;

    // Clear all caches every hour
    @Scheduled(fixedRate = 3600000)
    public void evictAllCaches() {
        for (String name : cacheManager.getCacheNames()) {
            cacheManager.getCache(name).clear();
            System.out.println("Cache cleared: " + name);
        }
    }

    // Clear specific cache at midnight
    @Scheduled(cron = "0 0 0 * * ?")
    public void evictUserCache() {
        Cache cache = cacheManager.getCache("users");
        if (cache != null) {
            cache.clear();
            System.out.println("User cache cleared at midnight");
        }
    }
}
```

## 17.4. Performance Monitoring (ការត្រួតពិនិត្យប្រសិទ្ធភាព)

### 📌 និយមន័យ (Definition):

**Performance Monitoring** គឺជាការតាមដាន (track) និងវាស់វែង (measure) metrics ដូចជា response time, throughput, error rate, resource usage ដើម្បីធានាថា កម្មវិធីដំណើរការបានល្អ។

### 🔹 Spring Boot Actuator:

```xml
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-actuator</artifactId>
</dependency>
<dependency>
    <groupId>io.micrometer</groupId>
    <artifactId>micrometer-registry-prometheus</artifactId>
</dependency>
```

### 🔹 Actuator Configuration:

```yaml
management:
  endpoints:
    web:
      exposure:
        include: health,info,metrics,prometheus
      base-path: /actuator
  endpoint:
    health:
      show-details: always
    metrics:
      enabled: true
  metrics:
    export:
      prometheus:
        enabled: true
    tags:
      application: myapp
```

### 🔹 Custom Metrics:

```properties
import io.micrometer.core.instrument.MeterRegistry;
import io.micrometer.core.instrument.Timer;
import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.stereotype.Component;
import javax.annotation.PostConstruct;
import java.util.concurrent.atomic.AtomicInteger;

@Component
public class CustomMetrics {

    @Autowired
    private MeterRegistry meterRegistry;

    private AtomicInteger activeUsers;
    private Timer requestTimer;

    @PostConstruct
    public void init() {
        // Counter
        meterRegistry.counter("api.calls.total", "endpoint", "/api/users");

        // Gauge
        activeUsers = meterRegistry.gauge("users.active", new AtomicInteger(0));

        // Timer
        requestTimer = Timer.builder("api.request.duration")
```

.description("Request processing time")

```text
            .register(meterRegistry);
    }

    public void incrementApiCalls(String endpoint) {
        meterRegistry.counter("api.calls", "endpoint", endpoint).increment();
    }

    public void recordRequestDuration(long durationMs) {
        requestTimer.record(durationMs, java.util.concurrent.TimeUnit.MILLISECONDS);
    }

    public void setActiveUsers(int count) {
        activeUsers.set(count);
    }

    public void recordError(String endpoint) {
        meterRegistry.counter("api.errors", "endpoint", endpoint).increment();
    }
}
```

## 17.5. Profiling (ការវិភាគប្រសិទ្ធភាព)

### 📌 និយមន័យ (Definition):

**Profiling** គឺជាការវិភាគ (analysis) នៃការប្រើប្រាស់ CPU, memory, threads របស់កម្មវិធីដើម្បីកំណត់អត្តសញ្ញាណ bottlenecks និងផ្នែកដែលត្រូវការកែលម្អ។

### 🔹 Java Profiling Tools:

- **JProfiler** – Commercial profiler with rich features

- **YourKit** – Java profiling for memory and CPU

- **VisualVM** – Free, built into JDK

- **Async Profiler** – Low overhead sampling profiler

- **Spring Boot Actuator** – Built-in metrics

### 🔹 JVM Arguments for Profiling:

```bash
# Enable JMX for remote monitoring
```

-Dcom.sun.management.jmxremote

```properties
-Dcom.sun.management.jmxremote.port=9010
-Dcom.sun.management.jmxremote.authenticate=false
-Dcom.sun.management.jmxremote.ssl=false

# Enable GC logging
-Xlog:gc*:file=gc.log:time,uptime:filecount=5,filesize=10M

# Heap dump on OOM
-XX:+HeapDumpOnOutOfMemoryError
-XX:HeapDumpPath=/var/log/myapp/heapdump.hprof

# Print GC details
-XX:+PrintGCDetails
-XX:+PrintGCTimeStamps

# Profiling with async-profiler
-agentpath:/path/to/libasyncProfiler.so=start,event=cpu,file=profile.html
```

## 17.6. Async Programming (ការសរសេរកម្មវិធីមិនសមកាលកម្ម)

### 📌 និយមន័យ (Definition):

**Asynchronous Programming** អនុញ្ញាតឱ្យកម្មវិធីអនុវត្តប្រតិបត្តិការ (operations) ដោយមិនរារាំង (non-blocking) thread ដើម្បីបង្កើន throughput និងការឆ្លើយតប (responsiveness)។

### 🔹 Enable Async:

```java
import org.springframework.context.annotation.Configuration;
import org.springframework.scheduling.annotation.EnableAsync;

@Configuration
@EnableAsync
public class AsyncConfig {

    @Bean(name = "taskExecutor")
    public Executor taskExecutor() {
        ThreadPoolTaskExecutor executor = new ThreadPoolTaskExecutor();
        executor.setCorePoolSize(5);
        executor.setMaxPoolSize(10);
        executor.setQueueCapacity(100);
        executor.setThreadNamePrefix("async-");
        executor.initialize();
        return executor;
    }
}
```

### 🔹 Using @Async:

```java
import org.springframework.scheduling.annotation.Async;
import org.springframework.stereotype.Service;
import java.util.concurrent.CompletableFuture;

@Service
public class EmailService {

    // Fire and forget
    @Async
    public void sendEmail(String to, String subject, String body) {
        System.out.println("Sending email to " + to + " in thread: " + Thread.currentThread().getName());
        // Simulate email sending
        try { Thread.sleep(1000); } catch (InterruptedException e) {}
        System.out.println("Email sent to " + to);
    }

    // Return CompletableFuture
    @Async
    public CompletableFuture<String> sendEmailAsync(String to, String subject, String body) {
        System.out.println("Sending email async to " + to);
        try { Thread.sleep(1000); } catch (InterruptedException e) {}
        return CompletableFuture.completedFuture("Email sent to " + to);
    }
}
```

## 17.7. Scheduling Tasks (ការកំណត់ពេលកិច្ចការ)

### 📌 និយមន័យ (Definition):

**Scheduled Tasks** គឺជាកិច្ចការដែលត្រូវបានប្រតិបត្តិដោយស្វ័យប្រវត្តិ នៅពេលវេលាកំណត់ (fixed time) ឬ interval (periodic)។ Spring Boot ផ្តល់@Scheduled annotation សម្រាប់សម្រួលដល់ការកំណត់ពេល។

### 🔹 Enable Scheduling:

```java
import org.springframework.context.annotation.Configuration;
import org.springframework.scheduling.annotation.EnableScheduling;

@Configuration
@EnableScheduling
public class SchedulingConfig {
    // Scheduling enabled
}
```

### 🔹 Scheduling Examples:

```java
import org.springframework.scheduling.annotation.Scheduled;
import org.springframework.stereotype.Component;
import java.time.LocalDateTime;

@Component
public class ScheduledTasks {

    private static final Logger log = LoggerFactory.getLogger(ScheduledTasks.class);

    // Fixed delay (milliseconds) between the end of last execution and start of next
    @Scheduled(fixedDelay = 5000)
    public void reportCurrentTime() {
        log.info("Current time: " + LocalDateTime.now());
    }

    // Fixed rate (milliseconds) - independent of execution time
    @Scheduled(fixedRate = 10000)
    public void processQueue() {
        log.info("Processing queue items...");
    }

    // Initial delay before first execution
    @Scheduled(initialDelay = 30000, fixedRate = 60000)
    public void warmUpCache() {
        log.info("Warming up cache...");
    }

    // Cron expression (second, minute, hour, day of month, month, day of week)
    // Run at 00:00 every day
    @Scheduled(cron = "0 0 0 * * ?")
    public void dailyCleanup() {
        log.info("Running daily cleanup job");
    }

    // Run every Monday at 9:00 AM
    @Scheduled(cron = "0 0 9 * * MON")
    public void weeklyReport() {
        log.info("Generating weekly report");
    }

    // Run every 5 minutes
    @Scheduled(cron = "0 */5 * * * ?")
    public void everyFiveMinutes() {
        log.info("Running every 5 minutes");
    }
}
```

### 💡 Cron Expression Reference:

| Field | Range | Example |
| --- | --- | --- |
| Second | 0-59 | 0 * * * * ? |
| Minute | 0-59 | 0 0 * * * ? |
| Hour | 0-23 | 0 0 0 * * ? |
| Day of Month | 1-31 | 0 0 0 1 * ? |
| Month | 1-12 or JAN-DEC | 0 0 0 ? JAN ? |
| Day of Week | 1-7 or MON-SUN | 0 0 9 ? * MON |

### 📊 Performance Optimization Checklist:

### ✅ Use caching for frequently accessed data

### ✅ Implement async processing for long-running tasks

### ✅ Configure proper database connection pool size

### ✅ Use pagination for large result sets

### ✅ Implement rate limiting for API endpoints

### ✅ Use connection pooling for HTTP clients

### ✅ Compress responses (Gzip)

### ✅ Use CDN for static resources

### ✅ Monitor JVM memory and GC behavior

### ✅ Use index in database queries

### 📚 សង្ខេបមេរៀនទី១៧ (Module 17 Summary)

នៅក្នុងមេរៀននេះ អ្នកបានរៀនអំពី Caching & Performance នៅក្នុង Spring Boot៖

- **Spring Cache** – @Cacheable, @CacheEvict, @CachePut annotations for declarative caching

- **Redis Integration** – In-memory data store, various data structures, TTL support

- **Cache Eviction** – Remove stale cache entries, scheduled eviction, conditional eviction

- **Performance Monitoring** – Actuator endpoints, custom metrics, Prometheus integration

- **Profiling** – JVM profiling tools, GC logging, heap dump analysis

- **Async Programming** – @Async, CompletableFuture, non-blocking operations

- **Scheduling Tasks** – @Scheduled, cron expressions, fixed rate/delay, dynamic scheduling

# មេរៀនទី១៨: Docker & Deployment (ដុកឃឺ និងការដាក់ពង្រាយ)

### 📖 សេចក្តីផ្តើម (Introduction):
Docker និង Deployment គឺជាផ្នែកសំខាន់ក្នុងការនាំយកកម្មវិធី Spring Boot ទៅដំណើរការក្នុងបរិស្ថានផលិតកម្ម (production)។ មេរៀននេះនឹងបង្រៀនអ្នកពី Introduction to Docker, Dockerizing Spring Boot App, Docker Compose, Environment Variables, CI/CD Basics, GitHub Actions, Deploy to VPS, Deploy to Render, Deploy to Railway, Deploy to AWS, និង Nginx Reverse Proxy។

## 18.1. Introduction to Docker

### 📌 និយមន័យ (Definition):

**Docker** គឺជា platform សម្រាប់អភិវឌ្ឍ, ដឹកជញ្ជូន (ship), និងដំណើរការ (run) applications ក្នុង containers។ Container គឺជា lightweight, portable unit ដែលផ្ទុក application និង dependencies ទាំងអស់របស់វា។

### 🔹 Docker vs Virtual Machine:

| លក្ខណៈ (Feature) | Docker Container | Virtual Machine |
| --- | --- | --- |
| OS | Shares host OS kernel | Full OS per VM |
| Startup Time | Milliseconds | Minutes |
| Size | MBs | GBs |
| Performance | Near native | Overhead |

### 🔹 Basic Docker Commands:

```bash
# Pull an image
```

docker pull openjdk:17-jdk-alpine

```bash
# List images
```

docker images

```bash
# Run a container
```

docker run -d -p 8080:8080 --name myapp myapp:latest

```bash
# List running containers
```

docker ps

```bash
# Stop a container
```

docker stop myapp

```bash
# View logs
```

docker logs myapp

```bash
# Build an image
```

docker build -t myapp:latest .

## 18.2. Dockerizing Spring Boot App

### 📌 ការបង្កើត Docker Image សម្រាប់ Spring Boot:

### 🔹 Dockerfile:

FROM openjdk:17-jdk-alpine

WORKDIR /app

COPY target/*.jar app.jar

EXPOSE 8080

ENTRYPOINT ["java", "-jar", "app.jar"]

### 🔹 Build and Run Commands:

```bash
# Build the JAR file
```

mvn clean package

```bash
# Build Docker image
```

docker build -t springboot-app:latest .

```bash
# Run the container
```

docker run -d -p 8080:8080 --name springboot-app springboot-app:latest

## 18.3. Docker Compose

### 📌 និយមន័យ (Definition):

**Docker Compose** គឺជាឧបករណ៍សម្រាប់កំណត់ (define) និងដំណើរការ (run) multi-container Docker applications។

### 🔹 docker-compose.yml:

```text
version: '3.8'
services:
postgres:
image: postgres:15
environment:
POSTGRES_DB: myapp
POSTGRES_USER: myuser
POSTGRES_PASSWORD: mypassword
ports:
```

- "5432:5432"

```text
redis:
image: redis:7-alpine
ports:
```

- "6379:6379"

```text
springboot-app:
build: .
ports:
```

- "8080:8080"

```text
depends_on:
```

- postgres

- redis

### 🔹 Docker Compose Commands:

```bash
# Start all services
```

docker-compose up -d

```bash
# Stop all services
```

docker-compose down

```bash
# View logs
```

docker-compose logs -f

## 18.4. Environment Variables

### 📌 ការប្រើប្រាស់ Environment Variables:

### 🔹 application.yml with Placeholders:

```yaml
spring:
datasource:
url: ${DB_URL:jdbc:postgresql://localhost:5432/myapp}
username: ${DB_USERNAME:myuser}
password: ${DB_PASSWORD:mypassword}
redis:
host: ${REDIS_HOST:localhost}
port: ${REDIS_PORT:6379}
```

### 🔹 Accessing Environment Variables in Code:

```java
import org.springframework.beans.factory.annotation.Value;
import org.springframework.stereotype.Component;

@Component
public class EnvConfig {
@Value("${APP_NAME:Default App}")
private String appName;
@Value("${DB_USERNAME}")
private String dbUsername;
public String getAppName() { return appName; }
public String getDbUsername() { return dbUsername; }
}
```

## 18.5. CI/CD Basics

### 📌 និយមន័យ (Definition):

**CI/CD (Continuous Integration/Continuous Deployment)** គឺជាការអនុវត្ត (practice) នៃការ automate build, test, និង deployment។

### 🔹 CI/CD Pipeline Stages:

1. **Build** – Compile code, run tests

2. **Package** – Create JAR/Docker image

3. **Test** – Run integration tests

4. **Deploy** – Deploy to staging/production

5. **Monitor** – Health checks, logs, alerts

## 18.6. GitHub Actions

### 📌 GitHub Actions CI/CD Pipeline:

```text
name: CI/CD Pipeline
on:
push:
branches: [ main ]
jobs:
build:
runs-on: ubuntu-latest
steps:
```

- uses: actions/checkout@v3

- name: Set up JDK 17

```text
uses: actions/setup-java@v3
with:
java-version: '17'
```

- name: Build with Maven

```java
run: mvn clean package -DskipTests
```

## 18.7. Deploy to VPS

### 📌 ជំហានដាក់ពង្រាយទៅកាន់ VPS:

```bash
# Connect to VPS
```

ssh root@your-server-ip

```bash
# Install Docker
curl -fsSL https://get.docker.com -o get-docker.sh
```

sudo sh get-docker.sh

```bash
# Clone repository
git clone https://github.com/yourusername/your-app.git
cd your-app
# Start application
```

docker-compose up -d

## 18.8. Deploy to Render

### 📌 Render Deployment Steps:

1. Create account at [render.com](https://render.com/)

2. Click "New +" → "Web Service"

3. Connect GitHub repository

4. Build Command: mvn clean package

5. Start Command: java -jar target/*.jar

6. Click "Create Web Service"

## 18.9. Deploy to Railway

### 📌 Railway Deployment Steps:

```bash
# Install Railway CLI
```

npm install -g @railway/cli

```bash
# Login
```

railway login

```bash
# Initialize project
```

railway init

```bash
# Deploy
```

railway up

```bash
# Open dashboard
```

railway open

## 18.10. Deploy to AWS

### 📌 AWS Elastic Beanstalk Deployment:

```bash
# Install EB CLI
```

pip install awsebcli

```bash
# Initialize EB application
```

eb init -p java-17 my-app --region us-east-1

```bash
# Create environment
```

eb create my-app-env

```bash
# Deploy application
```

eb deploy

```bash
# Open in browser
```

eb open

## 18.11. Nginx Reverse Proxy

### 📌 និយមន័យ (Definition):

**Nginx Reverse Proxy** គឺជា server ដែលទទួល requests ពី clients, បញ្ជូនពួកវាទៅកាន់ backend servers (Spring Boot), ហើយត្រឡប់ response វិញ។

### 🔹 nginx.conf:

```text
events {
worker_connections 1024;
}
http {
upstream springboot {
server springboot-app:8080;
}
server {
listen 80;
server_name your-domain.com;
location / {
proxy_pass http://springboot;
proxy_set_header Host $host;
proxy_set_header X-Real-IP $remote_addr;
}
}
}
```

### 💡 Nginx Commands:

- sudo nginx -t – Test configuration

- sudo systemctl reload nginx – Reload configuration

- sudo systemctl restart nginx – Restart Nginx

### 📊 Deployment Platforms Comparison

| Platform | Free Tier | Ease of Use |
| --- | --- | --- |
| Render | ✅ Yes | Very Easy |
| Railway | ✅ Yes | Very Easy |
| AWS EB | ❌ No | Moderate |
| VPS | ❌ No | Complex |

### 📚 សង្ខេបមេរៀនទី១៨ (Module 18 Summary)

នៅក្នុងមេរៀននេះ អ្នកបានរៀនអំពី Docker & Deployment សម្រាប់ Spring Boot៖

- **Introduction to Docker** – Containers vs VMs, basic Docker commands

- **Dockerizing Spring Boot** – Dockerfile, building images, running containers

- **Docker Compose** – Multi-container setup (app, database, redis)

- **Environment Variables** – Configuration with placeholders, @Value annotation

- **CI/CD Basics** – Continuous Integration/Continuous Deployment pipeline stages

- **GitHub Actions** – Automated build and test workflows

- **Deploy to VPS** – SSH, Docker installation, docker-compose on server

- **Deploy to Render** – Simple platform with GitHub integration

- **Deploy to Railway** – CLI-based deployment

- **Deploy to AWS** – Elastic Beanstalk CLI

- **Nginx Reverse Proxy** – Load balancing, proxy configuration

# មេរៀនទី១៩: Advanced Spring Boot (Spring Boot កម្រិតខ្ពស់)

### 📖 សេចក្តីផ្តើម (Introduction):
Advanced Spring Boot គ្របដណ្តប់លើលក្ខណៈពិសេសកម្រិតខ្ពស់ដែលធ្វើឱ្យ Spring Boot កាន់តែមានអានុភាព។ មេរៀននេះនឹងបង្រៀនអ្នកពី Custom Starter, AOP (Aspect Oriented Programming), Reflection, Event Listener, Custom Annotation, Spring Batch, Spring Scheduler, Reactive Programming, និង WebFlux។

## 19.1. Custom Starter (Starter ផ្ទាល់ខ្លួន)

### 📌 និយមន័យ (Definition):

**Custom Starter** គឺជា Spring Boot starter ដែលអ្នកបង្កើតដោយខ្លួនឯង ដើម្បីប្រមូលផ្តុំ (bundle) dependencies និង auto-configuration សម្រាប់មុខងារជាក់លាក់ណាមួយ។

### 🔹 Project Structure:

my-spring-boot-starter/

```text
├── pom.xml
├── src/
├── main/
├── java/
└── com/example/starter/
├── MyAutoConfiguration.java
├── MyService.java
└── MyProperties.java
└── resources/
└── META-INF/
└── spring/
└── org.springframework.boot.autoconfigure.AutoConfiguration.imports
```

### 🔹 Auto-configuration Class:

```java
import org.springframework.boot.autoconfigure.condition.ConditionalOnClass;
import org.springframework.boot.autoconfigure.condition.ConditionalOnMissingBean;
import org.springframework.boot.context.properties.EnableConfigurationProperties;
import org.springframework.context.annotation.Bean;
import org.springframework.context.annotation.Configuration;

@Configuration
@ConditionalOnClass(MyService.class)
@EnableConfigurationProperties(MyProperties.class)
public class MyAutoConfiguration {
@Bean
@ConditionalOnMissingBean
public MyService myService(MyProperties properties) {
return new MyService(properties);
}
}
```

### 🔹 Properties Class:

```java
import org.springframework.boot.context.properties.ConfigurationProperties;

@ConfigurationProperties(prefix = "my.service")
public class MyProperties {
private String name = "default";
private int timeout = 5000;
// Getters and Setters
}
```

### 🔹 Service Class:

```properties
public class MyService {
private final MyProperties properties;
public MyService(MyProperties properties) {
this.properties = properties;
}
public void doSomething() {
System.out.println("Service: " + properties.getName());
}
}
```

## 19.2. AOP (Aspect Oriented Programming)

### 📌 និយមន័យ (Definition):

**AOP (Aspect-Oriented Programming)** គឺជា programming paradigm ដែលអនុញ្ញាតឱ្យអ្នក បំបែក (separate) cross-cutting concerns (logging, security, transaction) ពី business logic។

### 🔹 Maven Dependency:

```xml
<dependency>
<groupId>org.springframework.boot</groupId>
<artifactId>spring-boot-starter-aop</artifactId>
</dependency>
```

### 🔹 Aspect Example (Logging):

```java
import org.aspectj.lang.JoinPoint;
import org.aspectj.lang.ProceedingJoinPoint;
import org.aspectj.lang.annotation.*;
import org.springframework.stereotype.Component;

@Aspect
@Component
public class LoggingAspect {
@Before("execution(* com.example..*.*(..))")
public void logBefore(JoinPoint joinPoint) {
System.out.println("Before method: " + joinPoint.getSignature().getName());
}

@AfterReturning(pointcut = "execution(* com.example..*.*(..))", returning = "result")
public void logAfterReturning(JoinPoint joinPoint, Object result) {
System.out.println("Method returned: " + result);
}

@Around("@annotation(com.example.annotation.LogExecutionTime)")
public Object logExecutionTime(ProceedingJoinPoint joinPoint) throws Throwable {
long start = System.currentTimeMillis();
Object result = joinPoint.proceed();
long duration = System.currentTimeMillis() - start;
System.out.println("Execution time: " + duration + "ms");
return result;
}
}
```

### 🔹 Custom Annotation for AOP:

```java
import java.lang.annotation.*;

@Target(ElementType.METHOD)
@Retention(RetentionPolicy.RUNTIME)
public @interface LogExecutionTime {
String value() default "";
}
```

## 19.3. Reflection

### 📌 និយមន័យ (Definition):

**Reflection** គឺជា feature ក្នុង Java ដែលអនុញ្ញាតឱ្យកម្មវិធីពិនិត្យ (inspect) និងកែប្រែ (modify) behavior របស់ classes, methods, fields នៅពេលដំណើរការ (runtime)។

```java
public class ReflectionExample {
public static void inspectClass(Object obj) throws Exception {
// Get class information
Class<?> clazz = obj.getClass();
System.out.println("Class name: " + clazz.getName());

// Get all fields
Field[] fields = clazz.getDeclaredFields();
for (Field field : fields) {
System.out.println("Field: " + field.getName());
}

// Get all methods
Method[] methods = clazz.getDeclaredMethods();
for (Method method : methods) {
System.out.println("Method: " + method.getName());
}

// Invoke method dynamically
Method method = clazz.getMethod("setName", String.class);
method.invoke(obj, "New Name");
}
}
```

## 19.4. Event Listener

### 📌 និយមន័យ (Definition):

**Event Listener** គឺជាយន្តការដែលអនុញ្ញាតឱ្យ components ទំនាក់ទំនងគ្នា តាមរយៈ events (publish-subscribe pattern)។ Spring ផ្តល់ ApplicationEventPublisherនិង @EventListener annotation។

```properties
// Custom Event
public class UserCreatedEvent extends ApplicationEvent {
private final Long userId;
private final String email;
public UserCreatedEvent(Object source, Long userId, String email) {
super(source);
this.userId = userId;
this.email = email;
}
// Getters
}

// Event Publisher
@Service
public class UserService {
@Autowired
private ApplicationEventPublisher eventPublisher;
public User createUser(UserDto dto) {
User user = userRepository.save(new User(dto));
eventPublisher.publishEvent(new UserCreatedEvent(this, user.getId(), user.getEmail()));
return user;
}
}

// Event Listener
@Component
public class UserEventListener {
@EventListener
public void handleUserCreated(UserCreatedEvent event) {
System.out.println("User created: " + event.getUserId());
// Send welcome email
}
@EventListener(condition = "#event.userId > 100")
public void handleLargeUserId(UserCreatedEvent event) {
System.out.println("Special handling for user ID > 100");
}
}
```

## 19.5. Custom Annotation

### 📌 និយមន័យ (Definition):

**Custom Annotation** អនុញ្ញាតឱ្យអ្នកបង្កើត annotations ផ្ទាល់ខ្លួន ដើម្បីបន្ថែម metadata ទៅកូដ និងដំណើរការវាតាមរយៈ AOP ឬ Reflection។

```java
// Create custom annotation
@Target(ElementType.METHOD)
@Retention(RetentionPolicy.RUNTIME)
public @interface RequirePermission {
String value();
String[] roles() default {};
}

// Use the annotation
@RestController
public class AdminController {
@RequirePermission(value = "DELETE_USER", roles = {"ADMIN"})
@DeleteMapping("/users/")
public void deleteUser(@PathVariable Long id) {
userService.delete(id);
}
}

// Aspect to process annotation
@Aspect
@Component
public class PermissionAspect {
@Before("@annotation(requirePermission)")
public void checkPermission(JoinPoint joinPoint, RequirePermission requirePermission) {
String permission = requirePermission.value();
String[] roles = requirePermission.roles();
// Check if current user has required permission
if (!hasPermission(permission, roles)) {
throw new SecurityException("Access denied");
}
}
}
```

## 19.6. Spring Batch

### 📌 និយមន័យ (Definition):

**Spring Batch** គឺជា lightweight framework សម្រាប់ batch processing (processing large volumes of data)។ វាផ្តល់ features ដូចជា read, process, write, retry, skip, chunk-based processing។

### 🔹 Maven Dependency:

```xml
<dependency>
<groupId>org.springframework.boot</groupId>
<artifactId>spring-boot-starter-batch</artifactId>
</dependency>
@Configuration
@EnableBatchProcessing
public class BatchConfig {
@Bean
public ItemReader<User> reader() {
return new FlatFileItemReaderBuilder<User>()
```

.name("userItemReader")

.resource(new ClassPathResource("users.csv"))

.delimited().names("id", "name", "email")

```text
.fieldSetMapper(new BeanWrapperFieldSetMapper<>() {{
setTargetType(User.class);
}})
.build();
}

@Bean
public ItemProcessor<User, User> processor() {
return user -> {
user.setName(user.getName().toUpperCase());
return user;
};
}

@Bean
public ItemWriter<User> writer() {
return users -> {
userRepository.saveAll(users);
};
}
}
```

## 19.7. Spring Scheduler

### 📌 និយមន័យ (Definition):

**Spring Scheduler** អនុញ្ញាតឱ្យអ្នកកំណត់ពេល (schedule) tasks ដើម្បីដំណើរការនៅពេលវេលាកំណត់ ឬ interval ទៀងទាត់។

```java
@Configuration
@EnableScheduling
public class SchedulerConfig {
@Bean
public TaskScheduler taskScheduler() {
ThreadPoolTaskScheduler scheduler = new ThreadPoolTaskScheduler();
scheduler.setPoolSize(10);
scheduler.setThreadNamePrefix("scheduled-");
return scheduler;
}
}

@Component
public class ScheduledTasks {
@Scheduled(fixedRate = 5000)
public void fixedRateTask() {
System.out.println("Running every 5 seconds");
}

@Scheduled(fixedDelay = 10000, initialDelay = 30000)
public void fixedDelayTask() {
System.out.println("Runs 10 seconds after previous execution");
}

@Scheduled(cron = "0 0 2 * * ?")
public void cronTask() {
System.out.println("Runs at 2 AM every day");
}
}
```

## 19.8. Reactive Programming

### 📌 និយមន័យ (Definition):

**Reactive Programming** គឺជា programming paradigm ដែលផ្តោតលើ asynchronous data streams និង propagation of change។ វាអនុញ្ញាតឱ្យកម្មវិធីមានប្រសិទ្ធភាពខ្ពស់ (non-blocking) និងអាចពង្រីកបាន (scalable)។

```java
import reactor.core.publisher.Flux;
import reactor.core.publisher.Mono;

@Service
public class ReactiveService {
// Mono: 0 or 1 element
public Mono<User> getUserById(Long id) {
return Mono.justOrEmpty(userRepository.findById(id));
}

// Flux: 0 to N elements
public Flux<User> getAllUsers() {
return Flux.fromIterable(userRepository.findAll());
}

// Reactive operators
public Flux<User> getActiveUsers() {
return getAllUsers()
```

.filter(User::isActive)

```text
.map(user -> {
user.setName(user.getName().toUpperCase());
return user;
})
.sort(Comparator.comparing(User::getName));
}
}
```

## 19.9. WebFlux (Spring WebFlux)

### 📌 និយមន័យ (Definition):

**Spring WebFlux** គឺជា reactive web framework ដែលប្រើ Project Reactor សម្រាប់ building non-blocking, asynchronous web applications។ វាគាំទ្រ functional endpoints, WebClient, និង reactive WebSocket។

### 🔹 Maven Dependency:

```xml
<dependency>
<groupId>org.springframework.boot</groupId>
<artifactId>spring-boot-starter-webflux</artifactId>
</dependency>
```

### 🔹 Reactive REST Controller:

```java
@RestController
@RequestMapping("/api/users")
public class UserReactiveController {
@Autowired
private UserReactiveService userService;

@GetMapping
public Flux<User> getAllUsers() {
return userService.getAllUsers();
}

@GetMapping("/")
public Mono<User> getUserById(@PathVariable Long id) {
return userService.getUserById(id);
}

@PostMapping
public Mono<User> createUser(@RequestBody User user) {
return userService.createUser(user);
}

@PutMapping("/")
public Mono<User> updateUser(@PathVariable Long id, @RequestBody User user) {
return userService.updateUser(id, user);
}

@DeleteMapping("/")
public Mono<Void> deleteUser(@PathVariable Long id) {
return userService.deleteUser(id);
}
}
```

### 🔹 WebClient (Reactive HTTP Client):

```properties
@Service
public class ExternalApiService {
private final WebClient webClient;

public ExternalApiService(WebClient.Builder webClientBuilder) {
this.webClient = webClientBuilder.baseUrl("https://api.example.com").build();
}

public Mono<User> fetchUser(Long id) {
return webClient.get()
.uri("/users/{id}", id)
```

.retrieve()

.bodyToMono(User.class)

.timeout(Duration.ofSeconds(5))

```text
.onErrorReturn(new User());
}

public Flux<Post> getPosts() {
return webClient.get()
```

.uri("/posts")

.retrieve()

```text
.bodyToFlux(Post.class);
}
}
```

### 🔹 Functional Endpoints (Router Functions):

```java
@Configuration
public class RouterConfig {
@Bean
public RouterFunction<ServerResponse> routes(UserHandler handler) {
return RouterFunctions.route()
```

.GET("/api/users", handler::getAllUsers)

```text
.GET("/api/users/{id}", handler::getUserById)
```

.POST("/api/users", handler::createUser)

```java
.PUT("/api/users/{id}", handler::updateUser)
.DELETE("/api/users/{id}", handler::deleteUser)
.build();
}
}

@Component
public class UserHandler {
@Autowired
private UserReactiveService userService;

public Mono<ServerResponse> getAllUsers(ServerRequest request) {
return ServerResponse.ok()
.body(userService.getAllUsers(), User.class);
}
}
```

### 💡 MVC vs WebFlux:

| Spring MVC | Spring WebFlux |
| --- | --- |
| Servlet API (Blocking) | Reactive Streams (Non-blocking) |
| Traditional threading model | Event loop (Netty) |
| Suitable for I/O bound | Suitable for I/O bound |
| Returns Object/List | Returns Mono/Flux |

### 📚 សង្ខេបមេរៀនទី១៩ (Module 19 Summary)

នៅក្នុងមេរៀននេះ អ្នកបានរៀនអំពី Advanced Spring Boot៖

- **Custom Starter** – Create reusable auto-configuration modules

- **AOP (Aspect Oriented Programming)** – Separate cross-cutting concerns (logging, security, transactions)

- **Reflection** – Inspect and modify code at runtime

- **Event Listener** – Publish and subscribe to application events

- **Custom Annotation** – Create annotations with custom behavior

- **Spring Batch** – Process large volumes of data (Chunk-based processing)

- **Spring Scheduler** – Schedule tasks with fixed rate/delay or cron expressions

- **Reactive Programming** – Non-blocking, asynchronous data streams (Mono/Flux)

- **WebFlux** – Reactive web framework, WebClient, functional endpoints

# មេរៀនទី២០: Real-World Projects (គម្រោងជាក់ស្តែង)

### 📖 សេចក្តីផ្តើម (Introduction):
មេរៀននេះនឹងណែនាំអ្នកអំពីគម្រោងជាក់ស្តែងដែលអ្នកអាចបង្កើតដោយប្រើ Spring Boot ដើម្បីអនុវត្តចំណេះដឹងទាំងអស់ដែលអ្នកបានរៀន។

## 20.1. Authentication System (ប្រព័ន្ធផ្ទៀងផ្ទាត់អត្តសញ្ញាណ)

### 📌 សេចក្តីសង្ខេប (Overview):

ប្រព័ន្ធ Authentication រួមបញ្ចូលការចុះឈ្មោះ (register), ចូលប្រើ (login), ការផ្ទៀងផ្ទាត់ JWT, Role-based Authorization, និងការគ្រប់គ្រងអ្នកប្រើប្រាស់។

### 🔹 API Endpoints:

```http
POST /api/auth/register - Register new user
POST /api/auth/login - Login user
POST /api/auth/logout - Logout user
POST /api/auth/refresh - Refresh JWT token
GET /api/auth/verify/<token> - Verify email
POST /api/auth/forgot-password - Send reset email
POST /api/auth/reset-password - Reset password
GET /api/users/me - Get current user profile
PUT /api/users/me - Update profile
GET /api/admin/users - Get all users (ADMIN only)
```

## 20.2. E-commerce API (API សម្រាប់ហាងលក់ទំនិញអនឡាញ)

### 📌 សេចក្តីសង្ខេប (Overview):

E-commerce API រួមបញ្ចូលការគ្រប់គ្រងផលិតផល (Products), កន្ត្រកទំនិញ (Cart), ការបញ្ជាទិញ (Orders), ការទូទាត់ (Payments), និងការពិនិត្យ (Reviews)។

### 🔹 API Endpoints:

```http
# Products
GET /api/products - Get all products
GET /api/products/<id> - Get product by ID
POST /api/products - Create product (ADMIN)
PUT /api/products/<id> - Update product (ADMIN)
DELETE /api/products/<id> - Delete product (ADMIN)
GET /api/products/search?q=keyword - Search products
GET /api/products/category/<id> - Products by category

# Cart
GET /api/cart - Get current user cart
POST /api/cart/items - Add item to cart
PUT /api/cart/items/<id> - Update cart item
DELETE /api/cart/items/<id> - Remove item from cart
DELETE /api/cart/clear - Clear cart

# Orders
POST /api/orders - Create order from cart
GET /api/orders - Get user orders
GET /api/orders/<id> - Get order details
PUT /api/orders/<id>/status - Update order status (ADMIN)
POST /api/orders/<id>/cancel - Cancel order
```

## 20.3. POS Management System (ប្រព័ន្ធគ្រប់គ្រងការលក់)

### 📌 សេចក្តីសង្ខេប (Overview):

POS (Point of Sale) Management System សម្រាប់គ្រប់គ្រងការលក់រាយ (retail sales), ស្តុកទំនិញ (inventory), អតិថិជន (customers), និងរបាយការណ៍ (reports)។

### 🔹 API Endpoints:

```http
# Sales
POST /api/sales - Create sale transaction
GET /api/sales - Get all sales
GET /api/sales/<id> - Get sale details
POST /api/sales/<id>/refund - Process refund

# Inventory
POST /api/inventory/stock-in - Add stock
POST /api/inventory/stock-out- Remove stock
GET /api/inventory/low-stock - Get low stock products

# Reports
GET /api/reports/daily - Daily sales report
GET /api/reports/monthly - Monthly sales report
GET /api/reports/top-products - Best selling products
```

## 20.4. Blog API (API សម្រាប់ប្លក់)

### 📌 សេចក្តីសង្ខេប (Overview):

Blog API រួមបញ្ចូលការគ្រប់គ្រងការប្រកាស (Posts), ប្រភេទ (Categories), ស្លាក (Tags), មតិយោបល់ (Comments), និងការចុះឈ្មោះអ្នកប្រើប្រាស់ (Users)។

### 🔹 API Endpoints:

```http
# Posts
GET /api/posts - Get all posts (paginated)
GET /api/posts/<slug> - Get post by slug
POST /api/posts - Create post (AUTHOR/ADMIN)
PUT /api/posts/<id> - Update post
DELETE /api/posts/<id> - Delete post
GET /api/posts/search?q=keyword - Search posts
GET /api/posts/category/<slug> - Posts by category
GET /api/posts/tag/<slug> - Posts by tag

# Comments
GET /api/posts/<id>/comments - Get post comments
POST /api/posts/<id>/comments - Add comment
PUT /api/comments/<id> - Update comment
DELETE /api/comments/<id> - Delete comment
```

## 20.5. School Management System (ប្រព័ន្ធគ្រប់គ្រងសាលារៀន)

### 📌 សេចក្តីសង្ខេប (Overview):

ប្រព័ន្ធគ្រប់គ្រងសាលារៀនសម្រាប់គ្រប់គ្រងសិស្ស (Students), គ្រូបង្រៀន (Teachers), ថ្នាក់រៀន (Classes), មុខវិជ្ជា (Subjects), ពិន្ទុ (Grades), និងកាលវិភាគ (Schedules)។

### 🔹 API Endpoints:

```http
# Students
GET /api/students - Get all students
POST /api/students - Enroll student
PUT /api/students/<id> - Update student info
GET /api/students/<id>/grades - Get student grades
GET /api/students/<id>/attendance - Get attendance record

# Grades
POST /api/grades - Enter grade (TEACHER)
GET /api/grades/class/<id> - Get class grades
GET /api/grades/student/<id> - Get student report card
```

## 20.6. Banking API (API សម្រាប់ធនាគារ)

### 📌 សេចក្តីសង្ខេប (Overview):

Banking API សម្រាប់គ្រប់គ្រងគណនី (Accounts), ប្រតិបត្តិការ (Transactions), ការផ្ទេរប្រាក់ (Transfers), និងសម្រង់ប្រវត្តិ (Statements)។

### 🔹 API Endpoints:

```http
# Accounts
POST /api/accounts - Create account
GET /api/accounts/<id> - Get account details
GET /api/accounts/<id>/balance - Get balance

# Transactions
POST /api/transactions/deposit - Deposit money
POST /api/transactions/withdraw - Withdraw money
POST /api/transactions/transfer - Transfer between accounts
GET /api/transactions/account/<id> - Get transaction history
```

## 20.7. Inventory System (ប្រព័ន្ធគ្រប់គ្រងស្តុក)

### 📌 សេចក្តីសង្ខេប (Overview):

Inventory System សម្រាប់គ្រប់គ្រងស្តុកទំនិញ, អ្នកផ្គត់ផ្គង់ (Suppliers), ការបញ្ជាទិញ (Purchase Orders), និងការចេញវិក្កយបត្រ (Invoices)។

### 🔹 API Endpoints:

```http
# Products
POST /api/products - Add product
PUT /api/products/<id> - Update product
GET /api/products/low-stock - Get low stock products

# Stock Movements
POST /api/stock/in - Receive stock
POST /api/stock/out - Dispatch stock
GET /api/stock/movements - Get stock movement history

# Suppliers
GET /api/suppliers - Get all suppliers
POST /api/suppliers - Add supplier
```

## 20.8. Chat Application (កម្មវិធីជជែក)

### 📌 សេចក្តីសង្ខេប (Overview):

Chat Application ប្រើ WebSocket និង STOMP សម្រាប់ real-time messaging, ការបង្កើតបន្ទប់ជជែក (Chat Rooms), និងការផ្ញើសារឯកជន (Private Messages)។

### 🔹 API Endpoints:

```bash
# WebSocket Endpoints
```

/ws/chat - WebSocket connection endpoint

/app/chat.send - Send message to room

/app/chat.private - Send private message

/topic/rooms/<id> - Subscribe to room messages

/user/queue/messages - Subscribe to private messages

```http
# REST Endpoints
GET /api/rooms - Get available chat rooms
POST /api/rooms - Create chat room
GET /api/rooms/<id>/messages - Get message history
```

## 20.9. Booking System (ប្រព័ន្ធកក់ទុក)

### 📌 សេចក្តីសង្ខេប (Overview):

Booking System សម្រាប់គ្រប់គ្រងការកក់សណ្ឋាគារ (Hotel), សំបុត្រយន្តហោះ (Flight), ឬសេវាកម្មផ្សេងៗ (Services)។

### 🔹 API Endpoints:

```http
# Bookings
GET /api/available - Check availability
POST /api/bookings - Create booking
GET /api/bookings/user - Get user bookings
GET /api/bookings/<id> - Get booking details
DELETE /api/bookings/<id> - Cancel booking

# Resources
GET /api/resources - Get available resources
GET /api/resources/<id>/calendar - Get resource calendar
```

## 20.10. Social Media Backend (Backend សម្រាប់បណ្តាញសង្គម)

### 📌 សេចក្តីសង្ខេប (Overview):

Social Media Backend រួមបញ្ចូលការបង្កើតការប្រកាស (Posts), ការតាមដាន (Follow), ការចូលចិត្ត (Likes), មតិយោបល់ (Comments), និងការផ្ញើសារ (Messages)។

### 🔹 API Endpoints:

```http
# Posts
POST /api/posts - Create post
GET /api/feed - Get user feed
GET /api/posts/<id> - Get post
DELETE /api/posts/<id> - Delete post
POST /api/posts/<id>/like - Like post
DELETE /api/posts/<id>/like - Unlike post
POST /api/posts/<id>/comment - Add comment

# Users
GET /api/users/<id> - Get user profile
PUT /api/users/profile - Update profile
POST /api/users/<id>/follow - Follow user
DELETE /api/users/<id>/follow - Unfollow user
GET /api/users/<id>/followers - Get followers

# Notifications
GET /api/notifications - Get user notifications
PUT /api/notifications/<id>/read - Mark as read
```

### 📊 Project Complexity Comparison

| Project | Difficulty | Key Technologies |
| --- | --- | --- |
| Authentication System | ⭐️⭐️ | Spring Security, JWT |
| Blog API | ⭐️⭐️ | JPA, Thymeleaf |
| Chat Application | ⭐️⭐️⭐️ | WebSocket, STOMP |
| POS System | ⭐️⭐️⭐️ | JPA, Reports |
| E-commerce API | ⭐️⭐️⭐️⭐️ | JPA, Payment Integration |
| School Management | ⭐️⭐️⭐️⭐️ | JPA, Complex Relationships |
| Social Media Backend | ⭐️⭐️⭐️⭐️⭐️ | WebSocket, Caching, Redis |

### 📚 សង្ខេបមេរៀនទី២០ (Module 20 Summary)

នៅក្នុងមេរៀននេះ អ្នកបានរៀនអំពី Real-World Projects ដែលអ្នកអាចបង្កើតដោយប្រើ Spring Boot៖

- **Authentication System** – JWT, Spring Security, Role-based access

- **E-commerce API** – Products, Cart, Orders, Payments, Reviews

- **POS Management System** – Sales, Inventory, Customers, Reports

- **Blog API** – Posts, Categories, Tags, Comments, Search

- **School Management System** – Students, Teachers, Grades, Attendance

- **Banking API** – Accounts, Transactions, Transfers, Statements

- **Inventory System** – Stock, Suppliers, Purchase Orders, Valuation

- **Chat Application** – WebSocket, STOMP, Real-time messaging

- **Booking System** – Availability, Reservations, Calendar

- **Social Media Backend** – Posts, Follow, Feed, Notifications, Messaging

# មេរៀនទី២១: Best Practices & Clean Code (ការអនុវត្តល្អ និងកូដស្អាត)

### 📖 សេចក្តីផ្តើម (Introduction):
Best Practices និង Clean Code គឺជាផ្នែកសំខាន់ក្នុងការអភិវឌ្ឍន៍កម្មវិធីដែលអាចថែទាំបាន (maintainable), អាចពង្រីកបាន (scalable), និងមានគុណភាពខ្ពស់ (high quality)។ មេរៀននេះនឹងបង្រៀនអ្នកពី Layered Architecture, DTO Pattern, Service Pattern, Repository Pattern, SOLID Principles, Clean Code, API Security Best Practices, Environment Configuration, Logging Best Practices, និង Production Optimization។

## 21.1. Layered Architecture (ស្ថាបត្យកម្មជាស្រទាប់)

### 📌 និយមន័យ (Definition):

**Layered Architecture** គឺជាការបែងចែកកម្មវិធីជាស្រទាប់ជាច្រើន (layers) ដែលស្រទាប់នីមួយៗមានទំនួលខុសត្រូវជាក់លាក់ (separation of concerns)។

```text
┌─────────────────────────────────────────────────────────────┐
│ Presentation Layer │
│ (Controllers - REST APIs) │
│ @RestController, @RequestMapping │
├─────────────────────────────────────────────────────────────┤
│ Business Layer │
│ (Services - Business Logic) │
│ @Service, @Transactional │
├─────────────────────────────────────────────────────────────┤
│ Persistence Layer │
│ (Repositories - Data Access) │
│ @Repository, JpaRepository, CrudRepository │
├─────────────────────────────────────────────────────────────┤
│ Database Layer │
│ (MySQL, PostgreSQL, MongoDB, etc.) │
└─────────────────────────────────────────────────────────────┘
```

### 🔹 Layer Responsibilities:

- **Presentation Layer** – ទទួល HTTP requests, validate input, return responses

- **Business Layer (Service)** – ផ្ទុក business logic, transaction management

- **Persistence Layer (Repository)** – Database operations, CRUD

- **Database Layer** – Data storage

### 💡 Benefits:

- Separation of concerns – ស្រទាប់នីមួយៗផ្តោតលើមុខងារតែមួយ

- Testability – អាចធ្វើតេស្តស្រទាប់នីមួយៗដោយឡែក

- Maintainability – ងាយស្រួលកែប្រែ និងថែទាំ

- Reusability – អាចប្រើស្រទាប់ដូចគ្នាសម្រាប់គម្រោងផ្សេងៗ

## 21.2. DTO Pattern (Data Transfer Object)

### 📌 និយមន័យ (Definition):

**DTO (Data Transfer Object)** គឺជា object ដែលប្រើសម្រាប់ដឹកជញ្ជូនទិន្នន័យ រវាង layers ឬរវាង client និង server។ DTO មិនមាន business logic ទេ មានតែ fields, getters, setters, constructors ប៉ុណ្ណោះ។

```java
// Entity (JPA)
@Entity
public class User {
@Id
private Long id;
private String username;
private String password;
private String email;
private LocalDateTime createdAt;
private LocalDateTime updatedAt;
}

// Request DTO (for receiving data from client)
public class UserRequest {
@NotBlank
@Size(min = 3, max = 20)
private String username;
@NotBlank
@Email
private String email;
@NotBlank
@Size(min = 6)
private String password;
}

// Response DTO (for sending data to client)
public class UserResponse {
private Long id;
private String username;
private String email;
private LocalDateTime createdAt;
}
```

### 🔹 Why use DTO?

- Decouple internal entities from API contracts

- Hide sensitive data (e.g., password, internal IDs)

- Reduce payload size (only send required fields)

- Add validation annotations specific to API layer

- Version APIs without changing entities

## 21.3. Service Pattern

### 📌 និយមន័យ (Definition):

**Service Pattern** គឺជា design pattern ដែលប្រមូលផ្តុំ business logic ទាំងអស់នៅក្នុង service layer។ Controller គួរតែស្រាល (thin) — គ្រាន់តែហៅ service methods, validate input, និងប្រគល់ response វិញ។

```java
// Good: Thin Controller
@RestController
@RequestMapping("/api/users")
public class UserController {
@Autowired
private UserService userService;

@PostMapping
public ResponseEntity<UserResponse> createUser(@Valid @RequestBody UserRequest request) {
UserResponse response = userService.createUser(request);
return ResponseEntity.status(HttpStatus.CREATED).body(response);
}
}

// Service with Business Logic
@Service
@Transactional
public class UserService {
@Autowired
private UserRepository userRepository;

public UserResponse createUser(UserRequest request) {
// Business validation
if (userRepository.existsByEmail(request.getEmail())) {
throw new DuplicateResourceException("Email already exists");
}

// Map DTO to Entity
User user = new User();
user.setUsername(request.getUsername());
user.setEmail(request.getEmail());
user.setPassword(passwordEncoder.encode(request.getPassword()));

// Save to database
User saved = userRepository.save(user);

// Map Entity to Response DTO
return new UserResponse(saved.getId(), saved.getUsername(), saved.getEmail());
}
}
```

## 21.4. Repository Pattern

### 📌 និយមន័យ (Definition):

**Repository Pattern** គឺជា abstraction layer ដែលបំបែក business logic ពី data access logic។ Repository ទទួលខុសត្រូវលើ CRUD operations និង query ទៅកាន់ database។

```java
// Base Repository Interface
@Repository
public interface UserRepository extends JpaRepository<User, Long> {
// Derived query methods
Optional<User> findByEmail(String email);
boolean existsByEmail(String email);
List<User> findByAgeGreaterThan(int age, Sort sort);

// Custom query with JPQL
@Query("SELECT u FROM User u WHERE u.name LIKE %:keyword%")
List<User> searchByName(@Param("keyword") String keyword);

// Custom query with native SQL
@Query(value = "SELECT * FROM users WHERE active = true", nativeQuery = true)
List<User> findAllActiveUsers();
}
```

## 21.5. SOLID Principles

### 📌 និយមន័យ (Definition):

**SOLID** គឺជា 5 principles សំខាន់ៗក្នុង Object-Oriented Design ដែលជួយឱ្យកូដ មានភាពរលុង (loosely coupled), ងាយស្រួលក្នុងការថែទាំ, និងអាចពង្រីកបាន។

**S - Single Responsibility Principle (SRP)**

Class មួយគួរតែមាន reason តែមួយដើម្បីផ្លាស់ប្តូរ។

```text
UserService: user management only, EmailService: email sending only
```

**O - Open/Closed Principle (OCP)**

Classes គួរតែបើកចំហសម្រាប់ extension ប៉ុន្តែបិទសម្រាប់ modification។

Use interfaces and abstract classes

**L - Liskov Substitution Principle (LSP)**

Subtypes ត្រូវតែអាចជំនួស (substitutable) base types បាន។

**I - Interface Segregation Principle (ISP)**

Interfaces គួរតែតូច និងជាក់លាក់។

**D - Dependency Inversion Principle (DIP)**

High-level modules មិនគួរពឹងផ្អែកលើ low-level modules ទេ។

Use dependency injection

## 21.6. Clean Code (កូដស្អាត)

### 📌 គោលការណ៍ Clean Code:

**Meaningful Names**

ប្រើឈ្មោះដែលមានអត្ថន័យ។

**Small Methods**

Methods គួរតែតូច និងធ្វើការតែមួយមុខគត់។

**No Duplication (DRY)**

Don't Repeat Yourself — កុំសរសេរកូដដដែលៗ។

**Proper Indentation**

តម្រឹមកូដឱ្យបានត្រឹមត្រូវ។

**❌ Bad Code Example:**

```text
public void doSomething(List l) { ... }
int a = 5; int b = 10; int c = a + b;
```

### ✅ Clean Code Example:

```text
public void calculateTotalAmount(List<OrderItem> items) { ... }
int firstNumber = 5; int secondNumber = 10; int sum = firstNumber + secondNumber;
```

## 21.7. API Security Best Practices

### 📌 ការអនុវត្តល្អសម្រាប់សន្តិសុខ API:

- Always use **HTTPS** in production

- Implement **rate limiting** to prevent DDoS attacks

- Validate all inputs (**@Valid**, sanitize user input)

- Use **JWT** or **OAuth2** for authentication

- Implement **CORS** properly

- Hash passwords with **BCrypt**

- Use **environment variables** for secrets

- Implement **audit logs** for sensitive operations

- Use **CSRF protection** for state-changing operations

- Set **security headers**

```bash
# Security Headers Configuration
@Bean
public SecurityFilterChain filterChain(HttpSecurity http) throws Exception {
```

http

.headers(headers -> headers

.contentSecurityPolicy("default-src 'self'")

.and()

.frameOptions().deny()

)

.authorizeHttpRequests(auth -> auth

.requestMatchers("/api/public/**").permitAll()

.anyRequest().authenticated()

```text
);
return http.build();
}
```

## 21.8. Environment Configuration

### 📌 Profile-based Configuration:

```yaml
# application-dev.yml (Development)
server:
port: 8080
spring:
datasource:
url: jdbc:h2:mem:testdb
jpa:
show-sql: true

# application-prod.yml (Production)
server:
port: 8080
spring:
datasource:
url: ${DB_URL}
username: ${DB_USERNAME}
password: ${DB_PASSWORD}
```

### 🔹 Activate Profile:

```bash
# Command line
java -jar app.jar --spring.profiles.active=prod

# Environment variable
export SPRING_PROFILES_ACTIVE=prod
```

## 21.9. Logging Best Practices

### 📌 ការអនុវត្តល្អសម្រាប់ Logging:

- Use **SLF4J** + **Logback** (default)

- Use appropriate log levels: **ERROR, WARN, INFO, DEBUG, TRACE**

- Never log sensitive data (passwords, tokens, credit cards)

- Use **parameterized logging**

- Log exceptions with stack trace

- Include **correlation IDs** for distributed tracing

- Rotate log files to prevent disk space issues

```java
import org.slf4j.Logger;
import org.slf4j.LoggerFactory;

@RestController
public class UserController {
private static final Logger log = LoggerFactory.getLogger(UserController.class);

@GetMapping("/users/{id}")
public User getUser(@PathVariable Long id) {
log.info("Fetching user with id: {}", id);
try {
return userService.findById(id);
} catch (Exception e) {
log.error("Failed to fetch user with id: {}", id, e);
throw e;
}
}
}
```

## 21.10. Production Optimization

### 📌 ការបង្កើនប្រសិទ្ធភាពសម្រាប់បរិស្ថានផលិតកម្ម:

**JVM Optimization**

```bash
java -Xms512m -Xmx1024m -XX:+UseG1GC -jar app.jar
```

**Connection Pooling**

```properties
spring.datasource.hikari.maximum-pool-size=20
```

**Database Indexing**

```text
@Table(indexes = @Index(columnList = "email"))
```

**Caching Strategy**

```text
@Cacheable(value = "products")
```

**Gzip Compression**

```properties
server.compression.enabled=true
```

**Async Processing**

```text
@EnableAsync
```

### 📊 Production Checklist:

### ✅ Use production database (not H2)

### ✅ Disable debug logging (set to WARN/ERROR)

### ✅ Enable HTTPS with valid SSL certificate

### ✅ Set up health checks (Spring Boot Actuator)

### ✅ Configure log rotation and retention

### ✅ Set up monitoring and alerting

### ✅ Implement rate limiting

### ✅ Enable database connection pool

### ✅ Set appropriate JVM heap size

### ✅ Enable compression for responses

### 📚 សង្ខេបមេរៀនទី២១ (Module 21 Summary)

នៅក្នុងមេរៀននេះ អ្នកបានរៀនអំពី Best Practices & Clean Code សម្រាប់ Spring Boot៖

- **Layered Architecture** – Separation of concerns (Controller, Service, Repository)

- **DTO Pattern** – Decouple internal entities from API contracts

- **Service Pattern** – Business logic encapsulation, thin controllers

- **Repository Pattern** – Data access abstraction

- **SOLID Principles** – SRP, OCP, LSP, ISP, DIP for maintainable code

- **Clean Code** – Meaningful names, small methods, no duplication

- **API Security Best Practices** – HTTPS, rate limiting, input validation

- **Environment Configuration** – Profile-based configuration (dev, test, prod)

- **Logging Best Practices** – SLF4J, appropriate log levels

- **Production Optimization** – JVM tuning, connection pooling, caching

# មេរៀនទី២២: Final Capstone Project (គម្រោងបញ្ចប់)

### 📖 សេចក្តីផ្តើម (Introduction):
គម្រោងបញ្ចប់នេះនឹងប្រមូលផ្តុំចំណេះដឹងទាំងអស់ដែលអ្នកបានរៀនពីមេរៀនទី១ ដល់ទី២១ ដើម្បីបង្កើតកម្មវិធីពេញលេញ (Complete Application) ដែលត្រៀមសម្រាប់ដាក់ពង្រាយក្នុងបរិស្ថានផលិតកម្ម (Production-Ready)។ អ្នកនឹងបង្កើតប្រព័ន្ធ Full Authentication, Admin Dashboard, User Management, Payment Integration, File Upload, Docker Deployment, Cloud Deployment, Documentation, Testing, និង Production Release។

## 22.1. Full Authentication (ប្រព័ន្ធផ្ទៀងផ្ទាត់ពេញលេញ)

### 📌 សេចក្តីសង្ខេប (Overview):

ប្រព័ន្ធ Authentication ពេញលេញរួមបញ្ចូលនូវ JWT Authentication, Refresh Token, Email Verification, Forgot Password, Role-Based Authorization, និង Social Login (Google, Facebook)។

### 🔹 Features:

```text
User Registration with email verification
```

- JWT Authentication (Access Token + Refresh Token)

- Role-Based Access Control (USER, MANAGER, ADMIN)

- Password Reset functionality (send email with reset link)

- Social Login (Google OAuth2, Facebook OAuth2)

- Two-Factor Authentication (2FA) with QR code

- Session Management (device tracking, force logout)

### 🔹 API Endpoints:

```http
POST /api/auth/register - Register new user
POST /api/auth/login - Login with credentials
POST /api/auth/refresh - Refresh access token
POST /api/auth/logout - Logout user
GET /api/auth/verify/<token> - Verify email address
POST /api/auth/forgot-password - Request password reset
POST /api/auth/reset-password - Reset password with token
POST /api/auth/enable-2fa - Enable Two-Factor Authentication
POST /api/auth/verify-2fa - Verify 2FA code
GET /api/auth/oauth2/google - Google OAuth2 login
GET /api/auth/oauth2/facebook - Facebook OAuth2 login
```

## 22.2. Admin Dashboard (ផ្ទាំងគ្រប់គ្រងរដ្ឋបាល)

### 📌 សេចក្តីសង្ខេប (Overview):

Admin Dashboard ផ្តល់នូវចំណុចប្រទាក់ (interface) សម្រាប់អ្នកគ្រប់គ្រងដើម្បីមើល (view), វិភាគ (analyze), និងគ្រប់គ្រង (manage) កម្មវិធីទាំងមូល។

### 🔹 Features:

- Dashboard with key metrics (KPIs)

- Real-time analytics and charts

```text
User activity monitoring
```

- System health status

- Revenue and sales reports

- Audit logs viewer

- Backup and restore functionality

- System configuration management

### 🔹 API Endpoints:

```http
GET /api/admin/dashboard/stats - Get dashboard statistics
GET /api/admin/audit-logs - Get audit logs
GET /api/admin/system/health - System health check
POST /api/admin/backup - Create database backup
POST /api/admin/restore - Restore from backup
GET /api/admin/reports/sales - Sales report
GET /api/admin/reports/users - User statistics report
```

## 22.3. User Management (ការគ្រប់គ្រងអ្នកប្រើប្រាស់)

### 📌 សេចក្តីសង្ខេប (Overview):

ប្រព័ន្ធគ្រប់គ្រងអ្នកប្រើប្រាស់អនុញ្ញាតឱ្យអ្នកគ្រប់គ្រងធ្វើ CRUD operations លើអ្នកប្រើប្រាស់, កំណត់តួនាទី (roles), និងការអនុញ្ញាត (permissions)។

### 🔹 Features:

- List, search, filter, and paginate users

- Create, update, delete user accounts

- Assign and revoke roles/permissions

- Enable/disable user accounts

- View user activity history

- Bulk user import/export (CSV/Excel)

- Password reset for users (by admin)

### 🔹 API Endpoints:

```http
GET /api/admin/users - Get all users (paginated)
GET /api/admin/users/<id> - Get user details
POST /api/admin/users - Create new user
PUT /api/admin/users/<id> - Update user
DELETE /api/admin/users/<id> - Delete user
PUT /api/admin/users/<id>/disable - Disable user account
PUT /api/admin/users/<id>/enable - Enable user account
POST /api/admin/users/<id>/reset-password - Reset user password
GET /api/admin/users/export - Export users to CSV/Excel
POST /api/admin/users/import - Import users from CSV/Excel
```

## 22.4. Payment Integration (ការភ្ជាប់ប្រព័ន្ធទូទាត់)

### 📌 សេចក្តីសង្ខេប (Overview):

Payment Integration អនុញ្ញាតឱ្យអ្នកប្រើប្រាស់ធ្វើការទូទាត់តាមរយៈ credit card, digital wallets, និង payment gateways (Stripe, PayPal, Wing, ABA Payway)។

### 🔹 Features:

- Multiple payment methods (Credit Card, PayPal, Wing, ABA)

- Secure payment processing with encryption

- Payment webhook handling

- Transaction history and receipts

- Refund processing

- Subscription/recurring payments

- Invoice generation (PDF)

### 🔹 API Endpoints:

```http
POST /api/payments/create-intent - Create payment intent
POST /api/payments/confirm - Confirm payment
POST /api/payments/webhook - Payment gateway webhook
GET /api/payments/transactions - Get user transactions
GET /api/payments/transactions/<id> - Get transaction details
POST /api/payments/refund/<id> - Request refund
GET /api/payments/invoice/<id> - Download invoice PDF
```

### 💡 Payment Gateway Integration Steps:

1. Create account with payment provider (Stripe, PayPal, ABA)

2. Get API keys (publishable key, secret key)

3. Configure webhook endpoints

4. Implement payment intent creation

5. Handle payment confirmation webhook

6. Update order status after successful payment

## 22.5. File Upload (ការផ្ទុកឯកសារ)

### 📌 សេចក្តីសង្ខេប (Overview):

File Upload system សម្រាប់ផ្ទុកឯកសារដូចជា profile pictures, product images, documents, videos ជាមួយ validation, resizing, និង cloud storage integration។

### 🔹 Features:

- Single and multiple file upload

- File validation (size, type, dimensions)

- Image resizing and optimization

- Store files in local filesystem or cloud (AWS S3, Cloudinary)

- Generate thumbnails for images

- Secure file access with signed URLs

- File download with expiration

### 🔹 API Endpoints:

```http
POST /api/files/upload - Upload single file
POST /api/files/upload-multiple - Upload multiple files
GET /api/files/<id> - Get file metadata
GET /api/files/download/<id> - Download file
DELETE /api/files/<id> - Delete file
POST /api/files/upload/profile - Upload profile picture
```

## 22.6. Docker Deployment

### 📌 សេចក្តីសង្ខេប (Overview):

Containerize the application using Docker and Docker Compose for easy deployment and scaling.

### 🔹 Dockerfile:

FROM openjdk:17-jdk-alpine

WORKDIR /app

COPY target/*.jar app.jar

EXPOSE 8080

ENTRYPOINT ["java", "-jar", "app.jar"]

### 🔹 docker-compose.yml:

```yaml
version: '3.8'

services:
app:
build: .
ports:
```

- "8080:8080"

```text
environment:
```

- SPRING_PROFILES_ACTIVE=prod

```text
depends_on:
```

- postgres

- redis

```text
postgres:
image: postgres:15
environment:
```

- POSTGRES_DB=myapp

- POSTGRES_USER=myuser

- POSTGRES_PASSWORD=mypassword

```text
volumes:
```

- postgres_data:/var/lib/postgresql/data

```text
redis:
image: redis:7-alpine
ports:
```

- "6379:6379"

```text
volumes:
postgres_data:
```

### 🔹 Build and Run:

```bash
# Build JAR
```

mvn clean package

```bash
# Build and run with Docker Compose
```

docker-compose up -d --build

```bash
# View logs
```

docker-compose logs -f app

```bash
# Stop containers
```

docker-compose down

## 22.7. Cloud Deployment (ការដាក់ពង្រាយលើ Cloud)

### 📌 ជម្រើសសម្រាប់ដាក់ពង្រាយ (Deployment Options):

**Render.com (Recommended for Beginners)**

- Connect GitHub repository

- Auto-deploy on push

- Free tier available

- Built-in SSL

**Railway.app**

- Simple CLI deployment

- Easy environment variables

- Free credits for new users

**AWS Elastic Beanstalk**

- Full control over infrastructure

- Auto-scaling

- Load balancing included

- Pay-as-you-go pricing

**Google Cloud Run**

- Serverless container deployment

- Auto-scales to zero

- Pay per request

### 🔹 Deploy to Render (Step by Step):

1. Push code to GitHub repository

2. Create account at render.com

3. Click "New +" → "Web Service"

4. Connect GitHub repository

5. Configure build settings:

  - Build Command: mvn clean package

  - Start Command: java -jar target/*.jar

6. Add environment variables (DB_URL, JWT_SECRET, etc.)

7. Click "Create Web Service"

8. Application will be live at https://yourapp.onrender.com

## 22.8. Documentation (ឯកសារ)

### 📌 ប្រភេទនៃឯកសារ (Documentation Types):

**API Documentation (Swagger/OpenAPI)**

Use SpringDoc OpenAPI to auto-generate API documentation

```text
http://localhost:8080/swagger-ui.html
```

**README.md**

Project overview, setup instructions, dependencies

```text
User Manual
```

Guide for end-users

**Developer Guide**

How to set up development environment, contribute

```java
# Swagger/OpenAPI Configuration
@Configuration
public class OpenAPIConfig {
@Bean
public OpenAPI customOpenAPI() {
return new OpenAPI()
```

.info(new Info()

.title("Capstone Project API")

.version("1.0.0")

.description("Complete Spring Boot Application"))

.servers(List.of(

```text
new Server().url("https://yourapp.com").description("Production"),
new Server().url("http://localhost:8080").description("Development")
));
}
}
```

## 22.9. Testing (ការធ្វើតេស្ត)

### 📌 ប្រភេទនៃការធ្វើតេស្ត (Testing Types):

**Unit Testing**

Test individual components (services, utilities)

```text
@ExtendWith(MockitoExtension.class)
```

**Integration Testing**

Test how components work together

```text
@SpringBootTest
```

**API Testing**

Test REST endpoints with MockMvc

```text
@WebMvcTest
```

**Database Testing**

Test repository layer with TestContainers

```text
@DataJpaTest
```

**Security Testing**

Test authentication and authorization

**Performance Testing**

Load testing with JMeter or Gatling

### 🔹 Code Coverage Requirement:

```xml
# JaCoCo Configuration
<plugin>
<groupId>org.jacoco</groupId>
<artifactId>jacoco-maven-plugin</artifactId>
<version>0.8.11</version>
<executions>
<execution>
<goals>
<goal>prepare-agent</goal>
</goals>
</execution>
<execution>
<id>report</id>
<phase>test</phase>
<goals>
<goal>report</goal>
</goals>
</execution>
</executions>
</plugin>
```

## 22.10. Production Release (ការចេញផ្សាយទៅបរិស្ថានផលិតកម្ម)

### 📌 ជំហានសម្រាប់ Production Release:

1. Run all tests (unit, integration, API tests)

2. Build with Maven/Gradle (mvn clean package)

3. Run security scan (OWASP dependency check)

4. Build Docker image (docker build -t myapp:latest .)

5. Push to container registry (Docker Hub, AWS ECR, GCR)

6. Deploy to cloud platform (Render, Railway, AWS)

7. Run smoke tests to verify deployment

8. Set up monitoring and alerting

9. Configure backup and disaster recovery

10. Update documentation

### 🔹 Production Configuration Checklist:

```yaml
# application-prod.yml
server:
port: 8080
tomcat:
max-threads: 200
min-spare-threads: 10

spring:
datasource:
url: ${DB_URL}
username: ${DB_USERNAME}
password: ${DB_PASSWORD}
hikari:
maximum-pool-size: 20
minimum-idle: 5

logging:
level:
com.example: WARN

management:
endpoints:
web:
exposure:
include: health,info,metrics
```

**📋 Pre-Launch Checklist:**

### ✅ All tests passing

### ✅ Code coverage > 80%

### ✅ No security vulnerabilities

### ✅ Environment variables configured

### ✅ Database backup strategy in place

### ✅ SSL certificate installed

### ✅ Monitoring and alerting set up

### ✅ Documentation updated

### ✅ Load testing completed

### ✅ Rollback plan defined
