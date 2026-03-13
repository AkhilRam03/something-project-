# something-project-
/html 
<!DOCTYPE html>
<html>
<head>
  <title>Team Portfolio</title>
  <link rel="stylesheet" href="style.css"
</head>
<body>
  <header>
    <h1>Welcome to Our Team Portfolio</h1>
  </header>
  <section id="team">
    <h2>Meet the Team</h2>
    <div class="profile">
      <h3>Alice</h3>
      <p>Frontend Developer</p>
    </div>
    <div class="profile">
      <h3>Bob</h3>
      <p>UI/UX Designer</p>
    </div>
    <div class="profile">
      <h3>Charlie</h3>
      <p>JavaScript Developer</p>
    </div>
  </section>
  <footer>Contact us at: team@example.com</footer>
  <script src="script.js"> </script>
</body>
</html>

//Script.js
document.querySelectorAll('.profile').forEach(profile => {
    profile.addEventListener('mouseenter', () => {
      profile.style.backgroundColor = '#f0f0f0';
    });
    profile.addEventListener('mouseleave', () => {
      profile.style.backgroundColor = 'white';
    });
  });

//Style.css
class Calculator:
    def add(self, x, y):
        return x + y

    def subtract(self, x, y):
        return x - y

    def multiply(self, x, y):
        return x * y

    def divide(self, x, y):
        if y == 0:
            return "Error! Division by zero."
        return x / y


def main():
    calc = Calculator()

    while True:
        print("\n--- Calculator Menu ---")
        print("1. Addition")
        print("2. Subtraction")
        print("3. Multiplication")
        print("4. Division")
        print("5. Exit")

        choice = input("Enter your choice (1-5): ")

        if choice == '5':
            print("Exiting the calculator. Goodbye!")
            break

        if choice in ['1', '2', '3', '4']:
            try:
                num1 = float(input("Enter first number: "))
                num2 = float(input("Enter second number: "))
            except ValueError:
                print("Invalid input! Please enter numeric values.")
                continue

            if choice == '1':
                print("Result:", calc.add(num1, num2))
            elif choice == '2':
                print("Result:", calc.subtract(num1, num2))
            elif choice == '3':
                print("Result:", calc.multiply(num1, num2))
            elif choice == '4':
                print("Result:", calc.divide(num1, num2))
        else:
            print("Invalid choice! Please select a valid option.")


if __name__ == "__main__":
    main()
body { font-family: Arial, sans-serif; margin: 0; padding: 0; }
header { background-color: #4CAF50; color: white; padding: 20px; text-align: center; }
.profile { margin: 20px; padding: 10px; border: 1px solid #ddd; }
footer { text-align: center; padding: 10px; background: #f1f1f1; }
