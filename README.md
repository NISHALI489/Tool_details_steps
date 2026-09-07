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



/*******************************************Davinci Configuration: (Dbc Import):Davinci Configuration: (Dbc Import):***************************************************/

Input file format: 
.dbc (Holds info like Network, ECU name, CAN Meaages, Signals)
Cdd  (Dignostic related infro specially SID, NRCs)
Fault matrix sheet  (DEM related faults, fault condition)

Import step:
•	For Davinci configurator Input file is .dpa (Davinci Project assist)
dpa -> Holds Module configuration ECU arxml path. 
Arxml : Autosar extension markup langage.

Step to opening Davinci Configurator Pro:
•	Go to project Stack check for .dpa exe file  right click on .dpa  
more option  a. BSW        For BSW
	b. ASW      For Appl

	Click on, I accept.
•	Once open go to Basic editor(holds all project related all modules).
•	Project  I/P Files  cdd, dbc (import)
•	View  option down consoles open option.
Another Way to open .dpa file.
•	Go to start search bar  type configurator  once open  file  import  +  select .dpa  open

•	After all configuration done  give on demand generator validation –> (for validation and generation module)(F8)  For validation.

•	After clicking validation and generation  in window left side  Deselect all  select which modules you changed based on Client Requirements  validate it  

•	Generate (F9)  generate arxml files  follow same for generation file (Deselect unchanged module) and generate

•	Down validation window  error show 

•	Parameter Description  left down properties window

•	If all configuration properties done  generate files in Gendata folder (with Updated date)

•	Import .dbc, cdd, files  Click on Project Input files  path for +mark dbc/cdd  arxml path  start flow/Update  click  after that it will update all configuration as per cdd/dbc files.

Davinci Congi and Dev:
1.	Set up Project
2.	Define Project setting
3.	Validation
4.	Start BSW configuration
5.	Design SWc
6.	Mappings
7.	Code generation
8.	Add Runnable code
9.	Compile, Link, And Test

Folder Structure:
Appl: GenData: After Configuration all module genearated output files.
Source: Source code
Config: 
a.	Appl_component: Put additional SWcType the davinci confi pro – read all .arxml files of this folder
b.	Autosar: Def files of data type (Platform type_AR4 arxml) is cenreally stored here.
Developers: All relevant project data for Dev Dev is located here
ECUc: contains created ECUc files, before you add input file, files are only place holder without content.
Internal Behavior: contain BSWmd files for all activated modules in the Dev D.
Mc Data: Used to store measurement and calibrate data.
Service component: Dev Config stored all generated service component prototype. 


/*************************************************************************************************************/
dBC  Data base file  System Architecture  Davanci Config  Configure parameter based on dBC reqs  once done validate and generate  based on configured container will generate separate arxml, with module will generate PB config, L config, config .c .h 6 files will generate  those gene rated arxml paths are available into ECUextract.arxml  that file  import into Davanci Developer Create SWC  in ECU exctract from configurator  in Developer can see the interfaces, Ports, Data Types  in Developer tool connects SWC, Port, Port Interfaces  Generate ARXL again  SWC.arxml will generate  SWC.arxml it holds SWC Runnable Port Interface Data Access that file again imprt to configurator  Now configurator has 
System.arxml+EcuExtract.arxml+EngineDisplaySWC.arxml+Com Configuration+OS Configuration 
RTE generator creates  Rte.c, Rte.h, Rte_EngineDisplaySWC.h, Rte_Type.

		
