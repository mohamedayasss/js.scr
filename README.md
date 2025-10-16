<!DOCTYPE html>
<html>
<head>
  <title>JavaScript Functions and Scope</title>
  <script>
    
    function addNumbers(x, y) {
      let sum = x + y;
      console.log("Addition:", sum);
    }
    addNumbers(10, 5);
    const multiply = function(a, b) {
      let product = a * b;
      console.log("Multiplication:", product);
    };
    multiply(4, 6);

    const subtract = (a, b) => {
      let result = a - b;
      console.log("Subtraction:", result);
    };
    subtract(20, 7);
    
    function divide(a, b) {
      if (b === 0) {
        return "Cannot divide by zero";
      }
      return a / b;
    }
    let divisionResult = divide(10, 2);
    console.log("Division Result:", divisionResult);

    let globalVar = "I am a Global Variable"; 

    function showScope() {
      let localVar = "I am a Local Variable"; 
      console.log(globalVar);
      console.log(localVar);  
    }

    showScope();
    console.log(globalVar);

  </script>
</head>
<body>
  <h2>JavaScript Functions and Scope Example</h2> 
</body>
</html>
