# IOC Example – Spring + Maven

This is a small Java project to show how **Inversion of Control (IoC)** works using the Spring Framework.  
Instead of creating objects manually in code, we let Spring handle it through an XML configuration.  

Think of it like this:  
👉 You ask Spring for a `MessagePrinter`, and it gives you one that’s already wired up with either an `EmailMessageService` or an `SMSMessageService`.  

---


IOC-Example/
├── src/main/java/com/example/
│ ├── App.java # Main app – loads Spring and runs
│ ├── MessagePrinter.java # Class that prints messages
│ ├── MessageService.java # Interface for message services
│ ├── EmailMessageService.java # Sends messages by Email
│ ├── SMSMessageService.java # Sends messages by SMS
│
├── src/main/resources/
│ └── applicationContext.xml # Spring configuration (wires the beans)
│
├── src/test/java/com/example/
│ └── AppTest.java # Basic unit test
│
├── pom.xml # Maven build file
└── README.md # This file 🙂 
