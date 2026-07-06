/******************************************  Vector cast  ***********************************************/

Before explaning about the V-cast tool,
let's understand about the basics about testing how it works

There are two types of testing:
a. White box testing
b. Black box testing

a. White box testing: White box testing will be performed by developer, who is having coding knowledge. In this testing developer will check the
   internal behaviour.

b. Black box testing: The Tester will perform the Black box testing, here Tester will check for the only input and output.  

Unit test: It is the process of or test the quality of the code line by line, also check control flow, fills the gap between code flow control.

Static: After full code executation it will errors.
Dynamic: While code running at what line compiler will get error, it stop there running. 

////////////////////////////////////////////////   Vector cast ////////////////////////////////////////////////////
1: Open V-cast tool.
		however you open the v-cast tool one pop window will be open. There we have to create environment
		in Environment we have to add some attributes for our Unit test.
		While creating environment 
		1. Environment Name:
		2. Compiler: Vector CastMinGW
		3. Compilation Method: Traditional
		4. Build Type: Statement + Branch (For Code Coverage)
		5. Locate file: Source file + additional and supportive file reference
		6. UUT(Unit Under Test): Unit Which is under test
In window whole code divided into functions, there check the function based on function, right click and
add test case in that input value, expected values.

2. Based on function it covers percentage of code, where need to cover all 100% of code.
3. After that generate report(full report and Management report)
   1. Full Report: Contains About value change, time, task done percentage
   2. Management Report: Only code coverage
4. Once done regration report,
   1. batch file
   2. Environment file
   3. Test File
   
5. For large loop can't check for longer time so, (for, while loop) compound test there set value for 
   loop itration
   
6. code coverage = (No of line covered/Total no of code line) * 100%
		
		