public class JavaBasics {

    // Objects - Instances of Classes
    public class BankAccount {
        private double balance;

        public BankAccount() {
            balance = 0.0;
        }

        public void deposit(double amount) {
            balance += amount;
        }

        public void withdraw(double amount) {
            if (amount <= balance) {
                balance -= amount;
            }
        }

        public double getBalance() {
            return balance;
        }
    }

    // Creating and Storing Objects (Instantiation)
    public void createAndStoreObject() {
        BankAccount myAccount = new BankAccount();
    }

    // Calling a Void Method
    public void callVoidMethod() {
        BankAccount myAccount = new BankAccount();
        myAccount.deposit(100.0);
    }

    // Calling a Void Method with Parameters
    public void callVoidMethodWithParameters() {
        BankAccount myAccount = new BankAccount();
        myAccount.withdraw(50.0);
    }

    // Calling a Non-void Method
    public void callNonVoidMethod() {
        BankAccount myAccount = new BankAccount();
        double balance = myAccount.getBalance();
    }

    // String Objects - Concatenation, Literals, and More
    public void stringOperations() {
        String firstName = "John";
        String lastName = "Doe";
        String fullName = firstName + " " + lastName;
    }

    // String Methods
    public void stringMethods() {
        String fullName = "John Doe";
        int length = fullName.length();
        String upperCaseName = fullName.toUpperCase();
    }

    // Wrapper Classes - Integer and Double
    public void wrapperClasses() {
        Integer myInteger = new Integer(42);
        Double myDouble = new Double(3.14);
    }

    // Using the Math Class
    public void useMathClass() {
        double squareRoot = Math.sqrt(16);
        double power = Math.pow(2, 3);
    }
}
