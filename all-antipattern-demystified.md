# All antipatterns demystified     
### Architects are abstractionists with significant experience in the majority of key technologies.
I deleted duplicates and categorize them again with alternative name.   
may be some of them be in [Code smells]() but don't worry we investigate them later.      
___________
## Architect anti-patterns.     


1:::::Jumble: mix vertical and horizontal design together

2:::::Cover your Assets: not good documentation or not using diagram well to describe   

3:::::Swiss Army Knifes : design architect for multi or general porpose(all possible use of class).    

4:::::Warm bodies(Brook law):One out of 20 programmers... produces 20 times the software compared to an average programmer.(NOT ALL PROGRAMMERS).       

5:::::The Grand Old Duke Of York(Abstraction vs Implimentation) :Experts report that only 1 in 5 software developers is able to define good abstractions On hearing this, a practicing software architect retorted, "It's more like 1 out of 50.".     

6:::::Architecture by Implication:Management of risk in follow-on system development is often overlooked due to overconfidence and recent system successes.Reliance on previous experience, which may differ in critical areas.         



7:::::Bikeshedding (Death by Planning): wasting your time with non-important debate or sessions (Giving disproportionate weight to trivial 
issues).  

8:::::Fear of adding class : you can't seprate or extract concerns in new files.     

9:::::Management by Numbers (Management by objectives): relience on numbers, rather more solution or result.     

10:::::Useless class (Poltergeists): using OOP too where it can be handled by a function.     

___________
## Organizational anti-patterns.     

11:::::Analysis paralysis: Devoting disproportionate effort to the analysis phase of a project.     

12:::::Cash cow: A profitable legacy product that often leads to complacency about new products.     

13:::::Bleeding edge(The Shiny Toy )(Wolf Ticket): Operating with cutting-edge technologies that are still untested or unstable leading to cost overruns, 
under-performance or delayed delivery.     

14:::::**Peter principle**: Continually promoting otherwise well-performing employees up to their level of incompetence, where they remain 
indefinitely.     

15:::::Design by committee: The result of having many contributors to a design, but no unifying vision.     

16:::::**Escalation of commitment**: Failing to revoke a decision when it proves wrong.     

17:::::**Management by perkele**: Authoritarian style of management with no tolerance of dissent(iranian bosses).     

18:::::Matrix Management: Unfocused organizational structure that results in divided loyalties and lack of direction.     

19:::::Micromanagement: Ineffectiveness from excessive observation, supervision, or other hands-on involvement from management.     

20:::::Moral hazard: Insulating a decision-maker from the consequences of his or her decision.     

21:::::Seagull management: Management in which managers only interact with employees when a problem arises, when they "fly in, make a lot of 
noise, dump on everyone, do not solve the problem, then fly out".     

22:::::Mushroom management: Keeping employees uninformed and misinformed (kept in the dark and fed manure).     

23:::::Stovepipe or Silos: A structure that supports mostly up-down flow of data but inhibits cross organizational communication.     

24:::::Vendor lock-in: Making a system excessively dependent on an externally supplied component.     

25:::::**Typecasting**: Locking successful employees into overly safe, narrowly defined, predictable roles based on their past successes rather 
than their potential.     

___________
## Project management anti-patterns.     
26::::: Walking Through a Minefield:When software is released before it is ready,

27:::::The Fast Beats Right:  alleges that it is always better to just get something done, Fast_Beats_Right_Dec_2014regardless of quality, than 
to invest any effort into doing the job right.    

28:::::Cart before the horse: Focusing too many resources on a stage of a project out of its sequence.     

29:::::Death march: Everyone knows that the project is going to be a disaster – except the CEO. However, the truth remains hidden and the project 
is artificially kept alive until the Day Zero finally comes ("Big Bang"). Alternative definition: Employees are pressured to work late nights and weekends on a project with an unreasonable deadline..   

30:::::Groupthink: During groupthink, members of the group avoid promoting viewpoints outside the comfort zone of consensus thinking.     

31:::::Smoke and mirrors: Demonstrating how unimplemented functions will appear.     

32:::::**Ninety-ninety rule**: Tendency to underestimate the amount of time to complete a project when it is "nearly done".     

33:::::Software bloat: Allowing successive versions of a system to demand ever more resources.     

34:::::Waterfall model: An older method of software development that inadequately deals with unanticipated change.     

35:::::**Overengineering**: Spending resources making a project more robust and complex than is needed.     

36:::::**Scope creep**(Feature Creep): Uncontrolled changes or continuous growth in a project's scope, or adding new features to the project 
after the original requirements have been drafted and accepted (also known as requirement creep and feature creep).     

37:::::**Brooks's law**: Adding more resources to a project to increase velocity, when the project is already slowed by coordination 
overhead.     
___________

## Analysis anti-patterns

38:::::Bystander apathy: When a requirement or design decision is wrong, but the people who notice this do nothing because it affects a larger 
number of people or The phenomenon in which people are less likely to or do not offer help to a person in need when others are present.     

___________
## Software design anti-patterns.    
39::::: Waterfail(waterfall):Waterfall, or Waterfail, is a rigid software development life cycle methodology that moves all activity through a 
series of stages, such as Gather Requirements, Design, Develop, Test, Deliver, Maintain.    

40::::: The Flags Over Objects: anti-pattern occurs when behavior is written outside of an object by inspecting flags (such as status codes), 
rather than within the object itself. This violates the Tell, Don’t Ask principle.     

41:::::**Abstraction inversion**(Inner-platform effect): Not exposing implemented functionality required by users, so that they re-implement it using higher level 
functions.     

42:::::Copy Folder Versioning:  a software development anti-pattern in which source code is updated by simply making copies of the folder.    

43:::::Ambiguous viewpoint: Presenting a model (usually Object-oriented analysis and design (OOAD)) without specifying its viewpoint.there are 
three viewpoints: **The business viewpoint** (the information that is domain specific and matters to the end user), the **specification viewpoint** (which defines the exposed interface elements of a class), and the **implementation viewpoint** (which deals with the actual internal implementation of the class).        

44:::::Big ball of mud: A system with no recognizable structure.     

45:::::**Database-as-IPC**: Using a database as the message queue for routine interprocess communication where a much more lightweight mechanism 
would be suitable.     

46:::::Gold plating: Continuing to work on a task or project well past the point at which extra effort is adding value(it can also mean developing features that were not originally requested by the customer.).     

47:::::**Inner-platform effect**: A system so customizable as to become a poor replica of the software development platform(Greenspun's tenth 
rule).     

48:::::**Input kludge**: Failing to specify and implement the handling of possibly invalid input(lack of validator).     

49:::::Interface bloat: Making an interface so powerful that it is extremely difficult to implement.     

50:::::Magic pushbutton: Coding implementation logic directly within interface code(submit button in form), without using abstraction.     

51:::::Race hazard: Failing to see the consequence of different orders of events.     

52:::::Stovepipe system: A barely maintainable assemblage of ill-related components.     

53::::: Frankencode : refers to code that was never designed to work together, being pulled into a single application and held together with duct 
tape, baling wire, and maybe some Adapter design pattern usage.(like Stovepipe)    

54::::: The Duct Tape Coder:  is someone who is able to cobble together software that solves the immediate problem, but without any concern for 
the code’s quality or maintainability.    

55::::: straw man :“architecture astronaut” who spends endless amounts of time on design but never actually delivers any software.    

___________
## Object-oriented design anti-patterns.     

56:::::Iceberg Class: you encapsulate tooooo much

57:::::Anemic Domain Model: The use of domain model without any business logic. The domain model's objects cannot guarantee their correctness at 
any moment, because their validation and mutation logic is placed somewhere outside (most likely in multiple places).    

58:::::**BaseBean**: Inheriting functionality from a utility class rather than delegating to it.     

59:::::Call super: Requiring subclasses to call a superclass's overridden method.     

60:::::Circle-ellipse problem(Square–rectangle problem)(Person prisoner): Subtyping variable-types on the basis of value-subtypes.     

61:::::Circular dependency: Introducing unnecessary direct or indirect mutual dependencies between objects or software modules.     

62:::::Constant interface: Using interfaces to define constants.     

63:::::God object(the blob): Concentrating too many functions in a single part of the design (class).     

64:::::**Object cesspool**: Reusing objects whose state does not conform to the (possibly implicit) contract for re-use.     

65:::::**Object orgy**: Failing to properly encapsulate objects permitting unrestricted access to their internals.     

66:::::Poltergeists: Objects whose sole purpose is to pass information to another object.     

67:::::Sequential coupling(water fall): A class that requires its methods to be called in a particular order.     

68:::::Yo-yo problem: A structure (e.g., of inheritance) that is hard to understand due to excessive fragmentation.     

69:::::Hurry up and wait: One or more asynchronous events triggered in the constructor of an object.     

___________
## Programming anti-patterns.     

70:::::Accidental complexity(Architecture by Implication): Introducing unnecessary complexity into a solution.     

71:::::Action at a distance: Unexpected interaction between widely separated parts of a system.     

72:::::Blind faith: Lack of checking of (a) the correctness of a bug fix or (b) the result of a subroutine.     

73:::::Boat anchor: Retaining a part of a system that no longer has any use.     

74:::::Busy spin(waiting): Consuming CPU while waiting for something to happen, usually by repeated checking instead of messaging.     

75:::::Caching failure: Forgetting to reset an error flag when an error has been corrected.     

76:::::Broken Windows : Small problems, left uncorrected, signal a lack of care about the state of things.     

77:::::**Cargo cult programming** (the Calendar Coder): Using patterns and methods without understanding why.     

78:::::**Coding by exception**(spagetti , Lasagna , n season pizza , ...): Adding new code to handle each special case as it is recognized.     

79:::::**Design pattern**: The use of patterns has itself been called an anti-pattern, a sign that a system is not employing enough 
abstraction.     

80:::::Error hiding: Catching an error message before it can be shown to the user and either showing nothing or showing a meaningless 
message.     

81:::::Hard code: Embedding assumptions about the environment of a system in its implementation.     

82:::::Lava flow: Retaining undesirable (redundant or low-quality) code because removing it is too expensive or has unpredictable 
consequences.     

83:::::Loop-switch sequence: Encoding a set of sequential steps using a switch within a loop statement.     

84:::::Magic numbers: Including unexplained numbers in algorithms.     

85:::::Magic strings: Including literal strings in code, for comparisons, as event types etc.

86:::::Soft code: Storing business logic in configuration files rather than source code.     

87:::::**Repeating yourself**: Writing code which contains repetitive patterns and substrings over again; avoid with once and only once 
(abstraction principle).     

88:::::Spaghetti code: Programs whose structure is barely comprehensible, especially because of misuse of code structures.     

89:::::Lasagna code: Programs whose structure consists of too many layers of inheritance.     

90:::::**Shooting the messenger**: Throwing exceptions from the scope of a plugin or subscriber in response to legitimate input, especially when this causes the outer scope to fail.     

91:::::Shotgun surgery: Developer adds features to an application codebase which span a multiplicity of implementors or implementations in a 
single change.     

___________
## Methodological anti-patterns.     

92:::::Copy and paste programming(Found on Internet): Copying (and modifying) existing code rather than creating generic solutions.     

93:::::**Every fool their own tool**: Failing to use proper software development principles when creating tools to facilitate the software 
development process itself.     

94:::::Golden hammer: Assuming that a favorite solution is universally applicable (See: Silver Bullet).     

95:::::Improbability factor: Assuming that it is improbable that a known error will occur.     

96:::::Not Invented Here (NIH) syndrome: The tendency towards reinventing the wheel (Failing to adopt an existing, adequate solution).     

97:::::**Invented here**: The tendency towards dismissing any innovation or less than trivial solution originating from inside the organization, usually because of lack of confidence in the staff.     

98:::::Premature optimization: Coding early-on for perceived efficiency, sacrificing good design, maintainability, and sometimes even real-world 
efficiency.     

99:::::Programming by permutation (or "programming by accident"): Trying to approach a solution by successively modifying the code to see if it 
works.     

100:::::Reinventing the wheel: Failing to adopt an existing, adequate solution.     

101:::::Reinventing the square wheel: Failing to adopt an existing solution and instead adopting a custom solution which performs much worse than 
the existing one.     

102:::::Silver bullet: Assuming that a favorite technical solution can solve a larger process or problem.     

103:::::Tester Driven Development: Software projects in which new requirements are specified in bug reports.     

104:::::Assumption Driven Programming: refers to the developer practice of assuming all users are like them. The best way to avoid falling into this trap is to interact with users as much as possible.   
___________

## Configuration management anti-patterns.     

105:::::Dependency hell: Problems with versions of required products.     

106:::::DLL hell: Inadequate management of dynamic-link libraries (DLLs), specifically on Microsoft Windows.     

107:::::Extension conflict: Problems with different extensions to pre-Mac OS X versions of the Mac OS attempting to patch the same parts of the 
operating system.     

108:::::JAR hell: Overutilization of the multiple JAR files, usually causing versioning and location problems because of misunderstanding of the Java class loading model.     



# Solution     
base on above anti patterns , we can avoid them by follow this this major principles:  

#### 1- Get technical depth and breadth about tools and how they work
get familar and expert about your os, tools,goals of project,concepts you use,software methodology, advantage and disadvantage of them.    
ability to **trade off** them together , it's need your brain has enough cache to store all of them     
it can be reach by exprience ,reading awesomes source codes,be practical with design patterns, try and error.      

#### 2- seprate concerns for god's sake     
seprate variable meaning , method , class , module, package , responsibility.   
don't encapsulate or expose interface or abstract too much or too a few.     

#### 3- [use clean code](https://gist.github.com/Arshiamidos/8474c210e072fed50b9747863b3e6619)      

#### 4- think past , now , future (time situation effect) of project. more important increamentaly but not too much or too a few     
it's like you are building a metro with stations and rails like [mini metro](https://play.google.com/store/apps/details?id=nz.co.codepoint.minimetro&hl=en).      
it's better to write test for backward(time) compatibility.    

#### 5- think all side of project or tech,with micro ,macro or mega magnifier simultaneously(place situation effect) .     
e.g use [codecity](https://wettel.github.io/codecity.html) for browseing project's density.     

#### 6 - repair your code as soon as possilbe you can , before it's too late [Leblanc Law : later equals never](https://gist.github.com/Arshiamidos/8474c210e072fed50b9747863b3e6619).    

#### 7 - don't trust user input, validate first and then apply.    

## links     
https://en.wikibooks.org/wiki/Introduction_to_Software_Engineering/Architecture/Anti-Patterns       
https://wiki.c2.com/?AntiPattern       
https://sourcemaking.com/antipatterns       
https://deviq.com/antipatterns/   
