# Spring IOCDemo 🚀

This is a basic demonstration of Spring IOC (Inversion of Control) using Java annotations. It includes a simple configuration to inject dependencies into a `Student` object. 💻

## Features ✨

- **Annotation-based Configuration**: Uses `@Configuration`, `@ComponentScan`, and `@Component` annotations to configure Spring beans. 🔧
- **Dependency Injection**: Demonstrates setter-based dependency injection using the `@Value` annotation. 🤖
- **Spring Core and Context**: Utilizes the Spring core and context modules for managing beans and the application context. 🌱

## Structure 📂

### 1. **Configuration Class** 📝
- The `SpringConfigurationFile` class is marked with `@Configuration` and `@ComponentScan` annotations. 
- It specifies the base package (`com.entity`) for component scanning to detect Spring beans. 📦

### 2. **Main Controller** 🕹️
- The `Controller` class uses `AnnotationConfigApplicationContext` to load the configuration and retrieve the `Student` bean from the Spring container. 
- Prints the `Student` object to demonstrate the dependency injection. 💬

### 3. **Student Bean** 🏫
- The `Student` class is annotated with `@Component` to define it as a Spring-managed bean. 
- Uses the `@Value` annotation to inject values for its fields (`Sid` and `Sname`). 🎓

### 4. **Maven Dependencies** 📡
- Includes the required Spring dependencies (`spring-core` and `spring-context`) in the `pom.xml`. ⚙️

## Example Output 💻
The application will print the `Student` object with its `Sid` and `Sname` values:

Output :- Student [Sid=211, Sname=Omkar]


## How It Works 🔍
1. The Spring framework scans the `com.entity` package for components. 🔍
2. The `Student` bean is detected and initialized with the specified `@Value` properties. ⚡
3. The `Controller` retrieves the bean from the Spring container and displays its details. 🖥️

## Requirements ✅
- Java 8 or higher ☕
- Maven for dependency management 📦
- Spring Core and Spring Context libraries (version 6.0.17) 🌿

This code demonstrates the basics of Spring IOC and Dependency Injection, useful for understanding the fundamentals of Spring's annotation-based configuration. 🎯
