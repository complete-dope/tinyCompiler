<!DOCTYPE html>
<html>
<head>
</head>
<body>
  <h1>LISP  to                 C</h1>
  <table>
    <tr>
      <th>LISP</th>
      <th>C</th>
    </tr>
    <tr>
      <td>2 + 2</td>
      <td>add(2, 2)</td>
    </tr>
    <tr>
      <td>4 - 2</td>
      <td>subtract(4, 2)</td>
    </tr>
    <tr>
      <td>2 + (4 - 2)</td>
      <td>add(2, subtract(4, 2))</td>
    </tr>
  </table>
  
  <p>Easy, right?</p>
  
  <h2>Parsing</h2>
  
  <p>Parsing involves two phases: Lexical Analysis and Syntactic Analysis.</p>
  
  <ol>
    <li>Lexical Analysis breaks down the code into tokens using a tokenizer or lexer. Tokens represent isolated syntax components like numbers, labels, operators, etc.</li>
    <li>Syntactic Analysis transforms the tokens into an Abstract Syntax Tree (AST), representing the syntax structure and relationships between elements.</li>
  </ol>
  
  <h2>Transformation</h2>
  
  <p>The transformation stage operates on the AST, modifying it either in the same language or translating it into a different language.</p>
  
  <h2>Traversal</h2>
  
  <p>Traversing the AST is essential for navigating through its nodes. The process typically follows a depth-first approach, visiting each node.</p>
  
  <h2>Visitors</h2>
  
  <p>The concept of visitors involves creating a "visitor" object with methods that accept different node types. This allows performing operations or analyses on specific nodes.</p>
  
  <h2>Code Generation</h2>
  
  <p>Code generation is the final phase, where the AST is converted back into code. This can involve reusing earlier tokens, printing nodes linearly, or recursively calling the code generator to print nested nodes. The goal is to produce a string of code.</p>
</body>
</html>
