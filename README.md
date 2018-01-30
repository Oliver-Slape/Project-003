# Project-003
## Anagram Solver

### Task: 
### Design a system that will allow the player to enter up to 3 random letters. The system will return the best, largest, valid English word that can be made up of the 3 letters (Blanks/spaces are not allowed). For example: TCA should return CAT/ACT, OZR should return OR, ZZA should return A. Extension is adding more letters. 

<h1> User Stories <h1>
    <h3> As a user I want to be able to input 3 letters. <h3>
    <h3> As a user I want to be able to recieve feedback for incorecct entries. <h3>
    <h3> As a user I want to be able to view my letters at input. <h3>
    <h3> As a user I want the highest value word possible from my entry. <h3>
    <h3> As a user I want feedback to display my  highest value word. <h3>
    
# Flow Chart 
![FlowChart](https://github.com/Oliver-Slape/Project-003/blob/master/Flowchart.png)

<h1> Product Backlog <h1>
    <h3> High Level Function Requirements <h3>
        <h4> User can input 3 letters (no spaces/blanks) <h4>
        <h4> System can read and access dictionary or word file <h4>
        <h4> System has algorithm to make highest value word from user input <h4> 
        <h4> Return feedback to user for inputs and Highest value word <h4>
    <h3> High Level Non-Function Requirements <h3>
        <h4> Current development is pure console code based so no design is required <h4>

<h1> Sprint Backlog <h1>
    <h3> As a user I want to be able to input 3 letters. <h3>
    <h3> As a user I want to be able to recieve feedback for incorecct entries. <h3>
    <h3> As a user I want to be able to view my letters at input. <h3>
    <h3> As a user I want the highest value word possible from my entry. <h3>
    <h3> As a user I want feedback to display my  highest value word. <h3>
    
<h1> Design Documentation <h1>
  <h2> Process of Implememntation <h2>
    <h3>  <h3>
  <h2> IDE Used and Features <h2>
  
  # IDE 
![IDE](https://github.com/Oliver-Slape/Project-003/blob/master/IDE.fw.png)

   <h3> The IDE used was an online service called repl.it It is a colour coordinated IDE with Code hints And a complier with a console debug and input. Additionally, it allows for the upload of files into a project enabling a dictionary or wordlist to be added for this program. <h3>
  <h2> Debugging process <h2>
    <h3> The IDE used as stated above includes a debugging service. This made the Debugging a lot simpler as it pointed to where and why there were errors in the code. After it was just a matter of fixing this. This was done by commenting lines of code until the error removes and then editing that section of code line by line till it works. Because we used a compiler it scans the entire program before generating errors compared to interpreters than just break and output the error when met. This can make the debugging a little more difficult.<h3>
  <h2> Coding Standards <h2>
    <h3> With the use of an IDE that colour coordinates the text and code and numbers it makes the layout easier to see and allows for a uniform coding standard. Additionally there is an improved and detailed level of commenting in the project. Additionally, The use of correct naming of Variables, Functions and other naming techniques allowes for easy seperation between tasks. The use of lines, breaks and spacing allows for clean easy to read coding. <h3> 

``` C++    
    if(currentScore > lastScore){ // is currentScore greater than lastScore 
        best = w;// sets new line word to best if better 
        lastScore = currentScore; // sets lastScore to currentScore 
     } 
```

``` C++
   // Read from file
   ifstream fin(filename.c_str());  // default mode ios::in
   if (!fin) { // if not error and abort
      cout << "error: File Couldn't be Opened";
      abort();
   }
    string line; // current word on Dictionary
    
   while (fin >> line) {  // print till end of file
    
     if(anagram.length() >= line.length()){ //Checks Anagram length is greater or equal to Line length
       solution(anagram, line);
     }
    }
``` 

  <h2> Evaluation <h2>
    <h3> The use of a more intuitive IDE made the process of debugging and having a coding standard as well as it made typing the code faster with hints and auto finish. The extension needs to be completed and there is a minor error where the returned word does'nt use all 3 letters. For example: ZZA returns ZAP rather than A. <h3>
    <h2> Relationship between algorithm and code <h2>
    <h3> Because this program implements an algorithm the best paradigm to do this was procedural. This is because it carries out the program in computational steps, much like an algorithm. Because procedural works by calling function after function it works well with algorithms as we can write each step of the algorithm into a function and then execute them in order. <h3> 
    
    
