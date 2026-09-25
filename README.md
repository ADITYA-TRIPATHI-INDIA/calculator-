<!DOCTYPE html>

<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Math Solver | Grade 7-10</title>
  
  <link rel="stylesheet" href="style.css">
</head>

<body>
  
  <header>
    <h1>📘 Math Solver</h1>
    <p>Grade 7 - Grade 10 Mathematics</p>
  </header>
  
  <nav>
    <button onclick="showSection('home')">Home</button>
    <button onclick="showSection('grade7')">Grade 7</button>
    <button onclick="showSection('grade8')">Grade 8</button>
    <button onclick="showSection('grade9')">Grade 9</button>
    <button onclick="showSection('grade10')">Grade 10</button>
  </nav>
  
  <main>
    
    <!-- HOME -->
    
    <section id="home" class="page">
      
      <h2>Welcome!</h2>
      
      <p>
        This application contains different Math Solvers for
        Grade 7 to Grade 10 students.
      </p>
      
      <div class="cards">
        
        <div class="card">
          <h3>🧮 Calculator</h3>
          <p>Perform basic calculations.</p>
        </div>
        
        <div class="card">
          <h3>📏 GCF & LCM</h3>
          <p>Find the Greatest Common Factor and Least Common Multiple.</p>
        </div>
        
        <div class="card">
          <h3>📐 Algebra</h3>
          <p>Solve algebraic expressions.</p>
        </div>
        
        <div class="card">
          <h3>📈 Quadratic</h3>
          <p>Solve quadratic equations instantly.</p>
        </div>
        
        <div class="card">
          <h3>📊 Polynomial</h3>
          <p>Create polynomial expressions.</p>
        </div>
        
        <div class="card">
          <h3>📐 Trigonometry</h3>
          <p>Find Sin, Cos and Tan.</p>
        </div>
        
      </div>
      
    </section>
    
    <!-- GRADE 7 -->
    
    <section id="grade7" class="page hidden">
      
      <h2>Grade 7 Mathematics</h2>
      
      <!-- BASIC CALCULATOR -->
      
      <div class="calculator">
        
        <h3>🧮 Basic Calculator</h3>
        
        <input type="number" id="num1" placeholder="First Number">
        
        <select id="operator">
          <option value="+">+</option>
          <option value="-">-</option>
          <option value="*">×</option>
          <option value="/">÷</option>
        </select>
        
        <input type="number" id="num2" placeholder="Second Number">
        
        <button onclick="calculateBasic()">
          Calculate
        </button>
        
        <h3 id="basicResult">Answer:</h3>
        
      </div>
      
      <hr>
      
      <!-- GCF -->
      
      <div class="calculator">
        
        <h3>📏 GCF Calculator</h3>
        
        <input type="number" id="gcf1" placeholder="First Number">
        
        <input type="number" id="gcf2" placeholder="Second Number">
        
        <button onclick="calculateGCF()">
          Find GCF
        </button>
        
        <h3 id="gcfResult">Answer:</h3>
        
      </div>
      
      <hr>
      
      <!-- LCM -->
      
      <div class="calculator">
        
        <h3>📐 LCM Calculator</h3>
        
        <input type="number" id="lcm1" placeholder="First Number">
        
        <input type="number" id="lcm2" placeholder="Second Number">
        
        <button onclick="calculateLCM()">
          Find LCM
        </button>
        
        <h3 id="lcmResult">Answer:</h3>
        
      </div>
      
    </section><!-- ========================= -->
    <!-- GRADE 8 -->
    <!-- ========================= -->
    
    <section id="grade8" class="page hidden">
      
      <h2>Grade 8 Mathematics</h2>
      
      <div class="calculator">
        
        <h3>📐 Algebraic Expression</h3>
        
        <input type="number" id="algA" placeholder="Value of a">
        
        <input type="number" id="algB" placeholder="Value of b">
        
        <button onclick="solveAlgebra()">
          Solve a + b
        </button>
        
        <h3 id="algebraResult">
          Answer:
        </h3>
        
      </div>
      
      <hr>
      
      <div class="calculator">
        
        <h3>√ Square Root Calculator</h3>
        
        <input type="number" id="sqrtNum" placeholder="Enter Number">
        
        <button onclick="calculateSquareRoot()">
          Calculate
        </button>
        
        <h3 id="sqrtResult">
          Answer:
        </h3>
        
      </div>
      
      <hr>
      
      <div class="calculator">
        
        <h3>Power Calculator</h3>
        
        <input type="number" id="base" placeholder="Base">
        
        <input type="number" id="exponent" placeholder="Exponent">
        
        <button onclick="calculatePower()">
          Calculate
        </button>
        
        <h3 id="powerResult">
          Answer:
        </h3>
        
      </div>
      
    </section>
    
    <!-- ========================= -->
    <!-- GRADE 9 -->
    <!-- ========================= -->
    
    <section id="grade9" class="page hidden">
      
      <h2>Grade 9 Mathematics</h2>
      
      <div class="calculator">
        
        <h3>📊 Polynomial Calculator</h3>
        
        <input type="number" id="polyA" placeholder="Coefficient a">
        
        <input type="number" id="polyB" placeholder="Coefficient b">
        
        <input type="number" id="polyC" placeholder="Coefficient c">
        
        <button onclick="calculatePolynomial()">
          Create Polynomial
        </button>
        
        <h3 id="polyResult">
          Answer:
        </h3>
        
      </div>
      
      <hr>
      
      <div class="calculator">
        
        <h3>📈 Quadratic Equation Solver</h3>
        
        <input type="number" id="qa" placeholder="a">
        
        <input type="number" id="qb" placeholder="b">
        
        <input type="number" id="qc" placeholder="c">
        
        <button onclick="solveQuadratic()">
          Solve
        </button>
        
        <h3 id="quadResult">
          Answer:
        </h3>
        
      </div>
      
    </section><!-- ========================= -->
    <!-- GRADE 10 -->
    <!-- ========================= -->
    
    <section id="grade10" class="page hidden">
      
      <h2>Grade 10 Mathematics</h2>
      
      <!-- TRIGONOMETRY -->
      
      <div class="calculator">
        
        <h3>📐 Trigonometry Calculator</h3>
        
        <input type="number" id="angle" placeholder="Enter Angle">
        
        <select id="trigFunction">
          <option value="sin">sin</option>
          <option value="cos">cos</option>
          <option value="tan">tan</option>
        </select>
        
        <button onclick="calculateTrig()">
          Calculate
        </button>
        
        <h3 id="trigResult">
          Answer:
        </h3>
        
      </div>
      
      <hr>
      
      <!-- GEOMETRY -->
      
      <div class="calculator">
        
        <h3>📏 Rectangle Area Calculator</h3>
        
        <input type="number" id="length" placeholder="Length">
        
        <input type="number" id="width" placeholder="Width">
        
        <button onclick="calculateArea()">
          Calculate Area
        </button>
        
        <h3 id="areaResult">
          Answer:
        </h3>
        
      </div>
      
      <hr>
      
      <!-- CIRCLE -->
      
      <div class="calculator">
        
        <h3>⭕ Circle Calculator</h3>
        
        <input type="number" id="radius" placeholder="Radius">
        
        <button onclick="calculateCircle()">
          Calculate
        </button>
        
        <h3 id="circleResult">
          Area:
        </h3>
        
      </div>
      
    </section>
    
  </main>
  
  <footer>
    
    <p>
      © 2026 Math Solver | Grade 7–10
    </p>
    
  </footer>
  
  <script src="script.js"></script>
  
</body>

</html><html>

<head>
  <link rel="stylesheet" href="style.css">
</head>

<body>
  <div class="calculator">
    <div id="display">0</div>
    <div class="buttons">
      <button onclick="clearDisplay()">C</button>
      <button onclick="appendOperator('÷')">÷</button>
      <button onclick="appendNumber('7')">7</button>
      <button onclick="appendNumber('8')">8</button>
      <button onclick="appendNumber('9')">9</button>
      <button onclick="appendOperator('×')">×</button>
      <button onclick="appendNumber('4')">4</button>
      <button onclick="appendNumber('5')">5</button>
      <button onclick="appendNumber('6')">6</button>
      <button onclick="appendOperator('-')">-</button>
      <button onclick="appendNumber('1')">1</button>
      <button onclick="appendNumber('2')">2</button>
      <button onclick="appendNumber('3')">3</button>
      <button onclick="appendOperator('+')">+</button>
      <button onclick="appendNumber('0')">0</button>
      <button onclick="calculate()">=</button>
    </div>
  </div>
  <script src="script.js"></script>
</body>

</html>
