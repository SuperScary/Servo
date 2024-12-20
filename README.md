<img src="https://raw.githubusercontent.com/SuperScary/Servo/refs/heads/main/logos/Servo%20Mascot-transparent.png" width="250" style="display: block; margin: 0 auto"/>

# Servo Programming Language

**Servo** is a high-level, object-oriented programming language designed for modern software development. With an emphasis on simplicity, scalability, and efficiency, Servo offers robust features to empower developers to write clean, maintainable, and performant code. Servo is versatile, supporting applications ranging from web development to complex system architectures.

---

## Features

- **Object-Oriented Design**: Full support for encapsulation, inheritance, and polymorphism.
- **Strong Typing with Flexibility**: Combines static typing for safety and dynamic capabilities where needed.
- **Memory Safety**: Servo includes built-in safeguards against memory leaks and null-pointer dereferencing.
- **Concurrency Made Easy**: First-class support for concurrent programming with lightweight threads and asynchronous operations.
- **Cross-Platform Support**: Write code once and deploy it anywhere.
- **Modern Syntax**: Inspired by popular languages like Python, Swift, and Java, with an emphasis on readability and developer productivity.
- **Built-In Testing Framework**: Integrated tools for writing, running, and debugging unit tests.
- **Extensible Libraries**: A rich standard library and support for third-party package integrations.

---

## Example Code

Here’s a quick example of Servo’s syntax:

```servo
// A simple "Hello, World!" program in Servo
public class Greeter {
    // Property
    var greeting -> String;

    // Constructor
    public Greeter (String message) {
        this.greeting = message;
    }

    // Method
    public sayHello() -> Void {
        print(greeting);
    }
}

// Create an instance of Greeter
let greeter = new Greeter("Hello, World!");
greeter.sayHello();
```

---

## Getting Started

### Installation

1. Download the latest version of Servo from the [official website](https://servolang.com/downloads).
2. Install the CLI using the installer for your platform.
3. Verify the installation:
   ```bash
   servo --version
   ```

### Writing Your First Program

1. Create a new Servo file:
   ```bash
   touch main.svo
   ```
2. Add your code to `main.svo`.
3. Run the program:
   ```bash
   servo run main.svo
   ```

---

## Language Basics

### Variables and Types

Servo supports both type inference and explicit type declarations:

```servo
let inferredVar = 42;      // Type inferred as Int
let explicitVar -> String = "Hello";
```

### Classes and Objects

Servo uses a clean and modern approach to object-oriented programming:

```servo
private class Animal {
    private var name -> String;

    private Animal (String name) {
        this.name = name;
    }

    private speak() -> Void {
        print("\(name) makes a sound.");
    }
}

let dog = new Animal("Dog");
dog.speak();
```

### Asynchronous Programming

Servo makes asynchronous operations intuitive:

```servo
async fetchData() -> String {
    await delay(2); // Simulates a delay of 2 seconds
    return "Data fetched!";
}

let data = await fetchData();
print(data);
```

---

## Contributing

We welcome contributions to Servo! Whether you're fixing bugs, suggesting features, or enhancing documentation, we appreciate your input.

### How to Contribute

1. Fork the repository.
2. Create a feature branch:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes and push:
   ```bash
   git commit -m "Add your message here"
   git push origin feature-name
   ```
4. Open a pull request.

For detailed contribution guidelines, refer to `CONTRIBUTING.md`.

---

## Community and Support

- **Documentation**: Comprehensive docs are available at [Servo Docs](https://docs.servolang.com).
- **Community Forums**: Join discussions at [Servo Forums](https://forum.servolang.com).
- **Issue Tracker**: Report bugs or request features at [Servo GitHub Issues](https://github.com/ServoLang/Servo/issues).

---

## License

Servo is licensed under the MIT License. See `LICENSE.md` for more details.

---

Happy coding with Servo! 🚀
