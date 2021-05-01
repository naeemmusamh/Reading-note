# BASIC MAP SETTINGS

Once you have included the Google Maps script in your page, you can use their maps object. It lets you display Google maps in your pages.

1. creating a map

The maps object is stored within an object called google. This creates scope for all Google objects.

To add a map to your page, you create a new map object using a constructor: Map ()The constructor is
part of the maps object, and it has two parameters:
• The element into which you want the map drawn
• A set of map options that control how it is displayed given using object literal notation

2. map options

The settings that control how the map should look are stored inside another JavaScript object called map options. It is created as an object literal before
you call the Map() constructor.
 In the JavaScript on the right, you can see that the map options object uses three pieces of data:
• Longitude and latitude of the center of the map
• The zoom level for the map
• The type of map data you want to show

3. zoom level

is typically set using a number between 0 and 16.

<img src="IMAGE/201/map.jpg">

# CHANGING CONTROLS

there is many type of control for map like :

1. zoom control :
Sets the zoom level of the map. It uses a slider "+/-" buttons

2. pan control :
Allows panning across the map

3. scale control
Shows the scale of the map

4. map type control
Switch map types

5. street view control
A Penman icon that can be dragged and dropped onto the map to show a street view

6. rotate control
Rotates maps that have oblique imagery

7. over view map control
A thumbnail showing a larger area, that reflects where the current map is within that wider area

A- google map with custom controls

APPEARANCE OF CONTROLS

To alter the appearance and position of map controls, you add to the map Options object.
1. To show or hide a control, the key is the name of the control, and the value is a Boolean
2. Each control has its own options object used to control its style and position. The word Options follows the control name
3. You can change the appearance of the zoom and map type controls.

# style a google map

To style the map you need to specify three things:
• feature Types: the map feature you want to style.
• element Types: the part of that feature you want to style.
• stylers: properties that allow you to adjust the color or visibility of items on the map.

<img src="IMAGE/201/map1.jpg">

# adding markers

Here you can see how to add a marker to a map. The map has been created, and its name is venueMap.

<img src="IMAGE/201/map2.jpg">

# order of execution

To find the source of an error, it helps to know how scripts are processed. The order in which statements are executed can be complex; some tasks cannot complete until another statement or function has been run.

# execution contexts

The JavaScript interpreter uses the concept of execution contexts. there is one global execution context; plus, each function creates a new new execution context they correspond to variable scope.

Every statement in a script lives in one of three execution contexts:
1. GLOBAL CONTEXT
Code that is in the script, but not in a function.
There is only one global context in any page.
2. FUNCTION CONTEXT
Code that is being run within a function.
Each function has its own function context.
3. EVAL CONTEXT
Text is executed like code in an internal function
called eva l {).

The first two execution contexts correspond with the notion of scope :
1. GLOBAL SCOPE
If a variable is declared outside a function, it can be used anywhere because it has global scope.
If you do not use the var keyword when creating a variable, it is placed in global scope.
2. FUNCTION-LEVEL SCOPE
When a variable is declared within a function, it can only be used within that function. This is because it has function-level scope.

# THE STACK

The javascript interpreter processes one line of code at a time. when a statement needs data from anther function.it stacks the new function on top the current task.

<img src="IMAGE/201/map3.jpg">

# EXECUTION CONTEXT & HOISTING

Each time a script enters a new execution context, there are two phases of activity:
1. PREPARE
• The new scope is created
• Variables, functions, and arguments are created
• The value of the this keyword is determined
2. EXECUTE
• Now it can assign values to variables
• Reference functions and run their code
• Execute statements

# UNDERSTANDING SCOPE

In the interpreter, each execution context has its own variables object. it holds the variables, functions, and parameters available within it. each execution context can also access its parent's variables object.

If a variable is not found in the variables object for the current execution context, it can look in the variables object of the parent execution context. But it is worth knowing that looking further up the stack can affect performance, so ideally you create variables inside the functions that use them.

# UNDERSTANDING ERRORS
If a JavaScript statement generates an error, then it throws an exception.
At that point, the interpreter stops and looks for exception-handling code.

# ERROR OBJECTS
Error objects can help you find where your mistakes are and browsers have tools to help you read them.

<img src="IMAGE/201/map4.jpg">