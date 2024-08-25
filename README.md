<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~ 01. javascript notes 4 pros logo (01) ~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ readme.md of js-notes4-pros.org ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="center">
  <img src="./images/image001.jpeg"
  title="JavaScript Notes 4 Professionals logo"
  alt="JavaScript Notes 4 Professionals logo."
  style="border: 2px solid #000000; width:4in;" />

<!--{width="8.25in" height="11.663194444444445in"}-->

<h4>Contents</h4>
<p>See end of document.</p>

<h4>About</h4>

<p>Please feel free to share this PDF with anyone for free, latest 
version of this book can be downloaded from:</p>

<p><a href="https://goalkicker.com/JavaScriptBook">JS Notes 4 Pros</a></p>

<p>This <i>JavaScript® Notes for Professionals</i> book is compiled from 
<a href="https://archive.org/details/documentation-dump.7z">Stack Overflow</a>.</p>

<p><a href="https://archive.org/details/documentation-dump.7z">Documentation</a>, the
content is written by the beautiful people at Stack Overflow.</p>

<p>Text content is released under Creative Commons BY-SA, see credits at 
the end of this book whom contributed to the various chapters. Images 
may be copyright of their respective owners unless otherwise specified.</p>

<p>This is an unofficial free book created for educational purposes and 
is not affiliated with official JavaScript® group(s) or company(s) nor 
Stack Overflow. All trademarks and registered trademarks are the 
property of their respective company owners.</p>

<p>The information presented in this book is not guaranteed to be correct 
nor accurate, use at your own risk.</p>

<p>Please send feedback and corrections to &lbrack;web@petercv.com&rbrack;.</p>

<!--page 2-->

<h2 id="ch1">Chapter 1: Getting started with JavaScript</h2>

<h4>Version Release Date</h4>

1.  1997-06-01
2.  1998-06-01
3.  1998-12-01
<a href="http://www-archive.mozilla.org/js/language/ECMA-357.pdf">E4X</a> 2004-06-01<br>
<a href="http://www.ecma-international.org/publications/files/ECMA-ST-ARCH/ECMA-262%205th%20edition%20December%202009.pdf">5</a> 2009-12-01<br>
<a href="http://www.ecma-international.org/publications/files/ECMA-ST-ARCH/ECMA-262%205.1%20edition%20June%202011.pdf">5.1</a> 2011-06-01<br>
6.  2015-06-01
7.  2016-06-14
8.  2017-06-27
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ readme.md of js-notes4-pros.org ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch1-1">Section 1.1: Using console.log()</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h4>Introduction</h4>

<p>All modern web browsers, Node.js as well as almost every other 
JavaScript environments support writing messages to a console using a 
suite of logging methods. The most common of these methods is ().</p>

<p>In a browser environment, the () function is predominantly used for
debugging purposes.</p>

<h4>Getting Started</h4>

<p>Open up the JavaScript Console in your browser, type the following,
and press Enter:</p>

<pre>
console.log("Hello, World!");
</pre>

<p>This will log the following to the console:</p>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="left">
  <img src="./images/image002.jpg"
  title=""
  alt="."
  style="border: 2px solid #000000; width:3.89in;" />
</p>
<!--{width="3.8916666666666666in" height="1.4236111111111112in"}-->

<p>In the example above, the console.log() function prints Hello, World! to the console and returns <b>undefined</b>
(shown above in the console output window). This is because () has no 
explicit <i>return value</i>.</p>

<h4>Logging variables</h4>

<p>console.log() can be used to log variables of any kind; not only strings. Just pass
in the variable that you want to be displayed in the console, for example:</p>

<pre>
<b>var</b>foo = &quot;bar&quot;;
console.log(foo);
</pre>

<p>This will log the following to the console:</p>
<!-- page 2 -->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="left">
  <img src="./images/image003.jpg"
  title="foobar console example."
  alt="Example foobar console."
  style="border: 2px solid #000000; width:5.95in;" />
</p>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!-- {width="5.954861111111111in" height="1.4777777777777779in"}-->

<p>If you want to log two or more values, simply separate them with 
commas. Spaces will be automatically added between each argument 
during concatenation:</p>

<pre>
var thisVar = 'first value';
var thatVar = 'second value';
console.log("thisVar:", thisVar, "and thatVar:", thatVar);
</pre>

<p>This will log the following to the console:</p>
<!-- page 3 -->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="left">
  <img src="./images/image004.jpg"
  title="thisVar and thatVar"
  alt="thisVar and thatVar."
  style="border: 2px solid #000000; width:7.47in;" />
</p>
<!-- {width="7.477777777777778in" height="0.9729166666666667in"} -->

<h4>Placeholders</h4>

<p>You can use console.log() in combination with placeholders:</p>

<pre>
<b>var</b> greet = "Hello", who = "World";
console.log ("%s, %s!", greet, who);
</pre>

<p>This will log the following to the console:</p>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="left">
  <img src="./images/image005.jpg"
  title="greet Hello, World"
  alt="greet Hello, World."
  style="border: 2px solid #000000; width:7in;" />
</p>
<!--{width="6.990972222222222in" height="1.4868055555555555in"}-->

<h4>Logging Objects</h4>

<p>Below we see the result of logging an object. This is often useful for 
logging JSON responses from API calls.</p>

<pre>
console.log ( { 
  'Email': '', 
  'Groups': {}, 
  'Id': 33, 
  'IsHiddenInUI': <b>false</b>,
  'IsSiteAdmin': <b>false</b>, 
  'LoginName': 'i:0#.w|virtualdomain\\user2',
  'PrincipalType': 1, 
  'Title': 'user2' 
} );
</pre>

<!-- page 4 -->
<p>This will log the following to the console:</p>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="left">
  <img src="./images/image006.jpg"
  title=" "
  alt="."
  style="border: 2px solid #000000; width:6.73in;" />
<!--{width="6.738888888888889in" height="1.7208333333333334in"}-->

<h4>Logging HTML elements</h4>

<p>You have the ability to log any element which exists within the
<a href="https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction">
<i>DOM</i></a>. In this case we log the body element:</p>

<pre>
console.log(document.body);
</pre>

<p>This will log the following to the console:</p>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="left">
  <img src="./images/image007.jpg"
  title=" "
  alt="."
  style="border: 2px solid #000000; width:6.52in;" />
<!--{width="6.522222222222222in" height="2.3784722222222223in"}-->

<h4>End Note</h4>
<p>For more information on the capabilities of the console, see the 
Console topic.</p>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch1-2">Section 1.2: Using the DOM API</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p>DOM stands for <b>D</b>ocument <b>O</b>bject <b>M</b>odel. It is an
object-oriented representation of structured documents like XML and HTML.</p>

<p>Setting the textContent property of an Element is one way to output
text on a web page.</p>

<p>For example, consider the following HTML tag:</p>

<pre><b>&lt;p</b> id="paragraph"<b>&gt;&lt;/p&gt;</b></pre>

<p>To change its textContent property, we can run the following JavaScript:</p>

<!-- page 5 -->

<pre>document.getElementById("paragraph").textContent = "Hello, World";</pre>

<p>This will select the element that with the id paragraph and set its
text content to "Hello, World":</p>

<pre><b>&lt;p</b> id="paragraph"&gt;Hello, World<b>&lt;/p&gt;</b></pre>

<p><a href="http://jsbin.com/fuzijox/edit?html,js,console,output">(See also this demo)</a></p>
<p>You can also use JavaScript to create a new HTML element programmatically. For example, 
consider an HTML document with the following body:</p>

<pre><b>&lt;body&gt;</b>
  <b>&lt;h1&gt;</b>Adding an element<b>&lt;/h1&gt;</b>
<b>&lt;/body&gt;</b></pre>

<p>In our JavaScript, we create a new <b>&lt;p&gt;</b>tag with a textContent property of 
and add it at the end of the html body:</p>

<pre><b>var</b> element = document.createElement('p');
element.textContent = "Hello, World";
document.body.appendChild(element); //<i>add the newly created element to the DOM</i></pre>

<p>That will change your HTML body to the following:</p>

<pre>
<b>&lt;body&gt;</b>
  <b>&lt;h1&gt;</b>Adding an element<b>&lt;/h1&gt;</b>
  <b>&lt;p&gt;</b>Hello, World<b>&lt;/p&gt;</b>
<b>&lt;/body&gt;</b>
</pre>

<p>Note that in order to manipulate elements in the DOM using JavaScript,
the JavaScript code must be run <i>after</i> the relevant element has been
created in the document. This can be achieved by putting the
JavaScript <b>&lt;script&gt;</b> tags <i>after</i> all of your other 
<b>&lt;body&gt;</b> content. Alternatively, you can also use 
<a href="https://developer.mozilla.org/en-US/docs/Web/API/EventTarget/addEventListener">
an event listener</a> to listen to eg. <a href="https://developer.mozilla.org/en-US/docs/Web/API/GlobalEventHandlers/onload">
window's onload event</a>, adding your code to that event listener 
will delay running your code until after the whole content on your page has been loaded.</p>

<p>A third way to make sure all your DOM has been loaded, is 
<a href="https://stackoverflow.com/questions/779379/why-is-settimeoutfn-0-sometimes-useful">
to wrap the DOM manipulation code with a timeout function of 0 ms</a>. This way, this 
JavaScript code is re-queued at the end of the execution queue, which gives the browser 
a chance to finish doing some non-JavaScript things that have been waiting to finish 
before attending to this new piece of JavaScript.</p>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch1-3">Section 1.3: Using window.alert()</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p>The alert method displays a visual alert box on screen. The alert
method parameter is displayed to the user in <b>plain</b> text:</p>

<pre>window.alert(message);</pre>

<p>Because window is the global object, you can call also use the following shorthand:</p>

<pre>alert(message);</pre>

<p>So what does window.alert() do? Well, let's take the following example:</p>

<pre>alert('hello, world');</pre>

<!-- page 6 -->

<p>In Chrome, that would produce a pop-up like this:</p>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="left">
  <img src="./images/image008.png"
  title=" "
  alt="."
  style="border: 2px solid #000000; width:5.225in;" />
<!--{width="5.225in" height="2.3152777777777778in"}-->

<h4>Notes</h4>

<blockquote>
  The alert method is technically a property of window object, but since
  all window properties are automatically global variables, we can use
  alert as a global variable instead of as a property of window meaning
  you can directly use alert() intead of window.alert().
</blockquote>

<p>Unlike using console.log, alert acts as a modal prompt meaning that the code
calling alert will pause until the prompt is answered. Traditionally
this means that <i>no other JavaScript code will execute</i> until the
alert is dismissed:</p>

<pre>alert('Pause!');
console.log('Alert was dismissed');</pre>

<p>However the specification actually allows other event-triggered code
to continue to execute even though a modal dialog is still being
shown. In such implementations, it is possible for other code to run
while the modal dialog is being shown.</p>

<p>More information about usage of the alert method can be found in the
modals prompts topic.</p>

<p>The use of alerts is usually discouraged in favour of other methods
that do not block users from interacting with the page - in order to
create a better user experience. Nevertheless, it can be useful for
debugging.</p>

<p>Starting with Chrome 46.0, window.alert() is blocked inside an <b>&lt;iframe&gt;</b> 
<a href="https://developer.mozilla.org/en-US/docs/Web/API/Window/alert">
unless its sandbox attribute has the value allow-modal</a>.
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch1-4">Section 1.4: Using window.prompt()</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p>An easy way to get an input from a user is by using the () method.</p>

<h4>Syntax</h4>

<pre>prompt(text, &lbrack;<b>default</b>&rbrack;);</pre>

<ul>
  <li><b>text</b>: The text displayed in the prompt box.</li>
  <li><b>default</b>): A default value for the input field (optional).</li>
</ul>

<h4>Examples</h4>

<pre>
<b>var</b> age = prompt("How old are you?");
console.log(age); // <i>Prints the value inserted by the user</i>
</pre>
<!-- page 7 -->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="left">
  <img src="./images/image009.png"
  title=" "
  alt="."
  style="border: 2px solid #000000; width:4.603in;" />
<!--{width="4.603472222222222in" height="1.9548611111111112in"}-->

<p>If the user clicks the <b>OK</b> button, the input value is returned.
Otherwise, the method returns <b>null</b>.</p>

<p>The return value of prompt is always a string, unless the user clicks
<b>Cancel</b>, in which that case it returns <b>null</b>. Safari is an
exception in that when the user clicks Cancel, the function returns an
empty string. From there, you can convert the return value to another
type, such as an integer.</p>

<h4>Notes</h4>

<ul>
  <li>While the prompt box is displayed, the user is prevented from accessing 
    other parts of the page, since dialog boxes are modal windows.</li>
  <li>Starting with Chrome 46.0 this method is blocked inside an <b>&lt;iframe&gt;</b>
    unless its sandbox attribute has the value allow-modal.</li>
</ul>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch1-5">Section 1.5: Using window.confirm()</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p>The window.confirm() method displays a modal dialog with an optional message and two
buttons, OK and Cancel.</p>

<p>Now, let's take the following example:</p>

<pre>result = window.confirm(message);</pre>

<p>Here, <b>message</b> is the optional string to be displayed in the dialog
and <b>result</b> is a boolean value indicating whether OK or Cancel was
selected (true means OK).</p>

<p>window.confirm() is typically used to ask for user confirmation before doing a
dangerous operation like deleting something in a Control Panel:</p>

<pre><b>if</b> (window.confirm("Are you sure you want to delete this?")) { 
  deleteItem (itemId);
}</pre>

<p>The output of that code would look like this in the browser:</p>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="left">
  <img src="./images/image010.jpg"
  title=" "
  alt="."
  style="border: 2px solid #000000; width:4.603in;" />
<!--{width="4.603472222222222in" height="1.4597222222222221in"}-->

<p>If you need it for later use, you can simply store the result of the
user's interaction in a variable:</p>

<!-- page 8 -->

<pre><b>var</b> deleteConfirm = window.confirm("Are you sure you want to delete this?");</pre>

<h4>Notes</h4>

<ul>
  <li>The argument is optional and not required by the specification.</li>
  <li>Dialog boxes are modal windows - they prevent the user from accessing
    the rest of the program's interface until the dialog box is closed.
	For this reason, you should not overuse any function that creates a
	dialog box (or modal window). And regardless, there are very good reasons 
	to avoid using dialog boxes for confirmation.</li>
  <li>Starting with Chrome 46.0 this method is blocked inside an <b>&lt;iframe&gt;</b>
    unless its sandbox attribute has the value allow-modal.</li>
  <li>It is commonly accepted to call the confirm method with the window
    notation removed as the window object is always implicit. However, it
	is recommended to explicitly define the window object as expected
	behavior may change due to implementation at a lower scope level with
	similarly named methods.</li>
</ul>

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch1-6">Section 1.6: Using the DOM API (with graphical text: Canvas, SVG, or image file)</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h4>Using canvas elements</h4>

<p>HTML provides the canvas element for building raster-based images.</p>

<p>First build a canvas for holding image pixel information.</p>

<pre><b>var</b> canvas = document.createElement('canvas');
canvas.width = 500;
canvas.height = 250;</pre>

<p>Then select a context for the canvas, in this case two-dimensional:</p>

<pre><b>var</b> ctx=canvas.getContext ('2d');</pre>

<p>Then set properties related to the text:</p>

<pre>ctx.font = '30px Cursive';
ctx.fillText ("Hello world!", 50, 50);</pre>

<p>Then insert the canvas element into the page to take effect:</p>

<pre>document.body.appendChild(canvas);</pre>

<h4>Using SVG</h4>

<p>SVG is for building scalable vector-based graphics and can be used
within HTML.</p>

<p>First create an SVG element container with dimensions:</p>

<pre><b>var</b> svg=document.createElementNS('http://www.w3.org/2000/svg', 'svg');
svg.width = 500;
svg.height = 50;</pre>

<p>Then build a text element with the desired positioning and font
characteristics:</p>

<!-- page 9 -->

<pre><b>var</b> text = document.createElementNS('http://www.w3.org/2000/svg', 'text');
text.setAttribute('x', '0');
text.setAttribute('y', '50');
text.style.fontFamily = 'Times New Roman';
text.style.fontSize = '50';</pre>

<p>Then add the actual text to display to the textelement:</p>

<pre>text.textContent = 'Hello world!';</pre>

<p>Finally add the text element to our svg container and add the svg
container element to the HTML document:</p>

<pre>svg.appendChild(text);
document.body.appendChild(svg);</pre>

<h4>Image file</h4>

<p>If you already have an image file containing the desired text and have
it placed on a server, you can add the URL of the image and then add
the image to the document as follows:</p>

<pre><b>var</b> img = <b>new</b> Image ( );
img.src = 'https://i.ytimg.com/vi/zecueq-mo4M/maxresdefault.jpg';
document.body.appendChild(img);</pre>
<!-- page 10 -->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h2 id="ch2">Chapter 2: JavaScript Variables</h2>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p><b>variable_name &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;{Required} The name of the variable: used when calling it.</b></p>

<p>= &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<b>&lbrack;Optional&rbrack;</b> Assignment (defining the variable)</p>

<p>value &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp<b>{Required when using Assignment}</b> The value of a variable
<b>&lbrack;default: undefined&rbrack;</b></p>

<p>Variables are what make up most of JavaScript. These variables make up
things from numbers to objects, which are all over JavaScript to make
one's life much easier.</p>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch2-1">Section 2.1: Defining a Variable</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<pre><b>var</b> myVariable = "This is a variable!";</pre>

<p>This is an example of defining variables. This variable is called a
"string" because it has ASCII characters (A-Z, 0-9, !@#$, etc.)</p>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch2-2">Section 2.2: Using a Variable</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<pre><b>var</b> number1 = 5;
number1 = 3;</pre>

<p>Here, we defined a number called "number1" which was equal to 5. 
However, on the second line, we changed the value to 3. To show the 
value of a variable, we log it to the console or use window.alert():</p>

<pre>console.log(number1); // <i>3</i>
window.alert(number1); // <i>3</i></pre>

<p>To add, subtract, multiply, divide, etc., we do like so:</p>

<pre>number1 = number1 + 5; // <i>3 + 5 = 8</i>
number1 = number1 - 6; // <i>8 - 6 = 2</i>
<b>var</b> number2 = number1 &ast; 10; // <i>2 (times) 10 = 20</i>
<b>var</b> number3 = number2 / number1; // <i>20 (divided by) 2 = 10;</i></pre>

<p>We can also add strings which will concatenate them, or put them
together. For example:</p>

<pre><b>var</b> myString = "I am a " + "string!" ; // <i>"I am a string!"</i></pre>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch2-3">Section 2.3: Types of Variables</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<pre><b>var</b> myInteger = 12; // <i>32-bit number (from -2,147,483,648 to 2,147,483,647)</i>
<b>var</b> myLong = 9310141419482 ; // <i>64-bit number (from -9,223,372,036,854,775,808 to
  9,223,372,036,854,775,807)</i>
<b>var</b> myFloat = 5.5; // <i>32-bit floating-point number (decimal)</i>
<b>var</b> myDouble = 9310141419482.22; // <i>64-bit floating-point number</i>

<b>var</b> myBoolean = <b>true</b>; // <i>1-bit true/false (0 or 1)</i>
<b>var</b> myBoolean2 = <b>false</b>;

<b>var</b> myNotANumber = <b>NaN</b>;
<b>var</b> NaN_Example = 0 / 0 ; // <i>NaN: Division by Zero is not possible</i>

<b>var</b> notDefined; // <i>undefined: we didn&apos;t define it to anything yet</i>
window.alert(aRandomVariable); // <i>undefined</i>

<b>var</b> myNull=<b>null</b>; // <i>null</i>
<i>// etc...</i></pre>

<!-- page 11 -->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch2-4">Section 2.4: Arrays and Objects</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<pre><b>var</b> myArray=&lbrack;&rbrack;; // <i>empty array</i></pre>

<p>An array is a set of variables. For example:</p>

<pre><b>var</b> favoriteFruits = &lbrack;"apple", "orange", "strawberry"&rbrack;;
<b>var</b> carsInParkingLot = &lbrack;"Toyota", "Ferrari", "Lexus"&rbrack;;
<b>var</b> employees = &lbrack;"Billy", "Bob", "Joe"&rbrack;;
<b>var</b> primeNumbers = &lbrack;2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31&rbrack;;
<b>var</b> randomVariables = &lbrack;2, "any type works", <b>undefined</b>, <b>null</b>, <b>true</b>, 2.51&rbrack;;

myArray = &lbrack;"zero" , "one" , "two" &rbrack;;
window.alert ( myArray &lbrack;0&rbrack;); // <i>0 is the first element of an array</i>
                             // <i>in this case, the value would be "zero"</i>
myArray = &lbrack;"John Doe", "Billy"&rbrack;;
elementNumber = 1;

window.alert(myArray&lbrack;elementNumber&rbrack;); // <i>Billy</i></pre>

<p>An object is a group of values; unlike arrays, we can do something
better than them:</p>

<pre>myObject = {};
john = {firstname: "John", lastname: "Doe", fullname: "John Doe"};
billy = {
  firstname: "Billy",
  lastname: <b>undefined</b>,
  fullname: "Billy"
};
window.alert(john.fullname); // <i>John Doe</i>
window.alert(billy.firstname); // <i>Billy</i></pre>

<p>Rather than making an array &lbrack;"John Doe", "Billy"&rbrack; and calling myArray&lbrack;0&rbrack;, we
can just call john.fullname and billy.fullname.</p>

<!-- page 12 -->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h2 id="ch3">Chapter 3: Built-in Constants</h2>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch3-1">Section 3.1: null</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p><b>null</b> is used for representing the intentional absence of an object value and is a 
primitive value. Unlike <b>undefined</b>, it is not a property of the global object.</p>

<p>It is equal to <b>undefined</b> but not identical to it.</p>

<pre><b>null</b> == <b>undefined</b>; // true
<b>null</b> === <b>undefined</b>; // false</pre>

<p><b>CAREFUL</b>: The <b>typeof null</b> is 'object'.</p>

<pre><b>typeof null</b>; // 'object';
</pre>

<p>To properly check if a value is <b>null</b>, compare it with the strict equality operator.</p>

<pre>
<b>var</b> a = <b>null</b>;

a === <b>null</b>; // true</pre>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch3-2">Section 3.2: Testing for NaN using isNaN()</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<pre><b>window.isNaN</b></pre>  

<p>The global function () can be used to check if a certain value or
expression evaluates to <b>NaN</b>. This function (in short) first checks
if the value is a number, if not tries to convert it (*), and then
checks if the resulting value is <b>NaN</b>. For this reason, <b>this
testing method may cause confusion</b>.</p>

<p>(*) The "conversion" method is not that simple, see <a href="http://www.ecma-international.org/ecma-262/6.0/#sec-isnan-number">ECMA-262 18.2.3</a>
for a detailed explanation of the algorithm.</p>

<p>These examples will help you better understand the isNaN() behavior:</p>

<pre>isNaN(<b>NaN</b>);            // <i>true</i>
isNaN(1);             // <i>false: 1 is a number</i>
isNaN(-2e-4);         // <i>false: -2e-4 is a number (-0.0002) in scientific notation</i>
isNaN(<b>Infinity</b>);      // <i>false: Infinity is a number</i>
isNaN(<b>true</b>);          // <i>false: converted to 1, which is a number</i>
isNaN(<b>false</b>);         // <i>false: converted to 0, which is a number</i>
isNaN(<b>null</b>);          // <i>false: converted to 0, which is a number</i>
isNaN("");            // <i>false: converted to 0, which is a number</i>
isNaN("");            // <i>false: converted to 0, which is a number</i>
isNaN("45.3");        // <i>false: string representing a number, converted to 45.3</i>
isNaN("1.2e3");       // <i>false: string representing a number, converted to 1.2e3</i>
isNaN("Infinity");    // <i>false: string representing a number, converted to Infinity</i>
isNaN(<b>new</b> Date);      // <i>false: Date object, converted to milliseconds since epoch</i>
isNaN("10$");         // <i>true : conversion fails, the dollar sign is not a digit</i>
isNaN("hello");       // <i>true : conversion fails, no digits at all</i>
isNaN(<b>undefined</b>);     // <i>true : converted to NaN</i>
isNaN();              // <i>true : converted to NaN (implicitly undefined)</i>
isNaN(<b>function</b>(){}); // <i>true : conversion fails</i>
isNaN({});           // <i>true : conversion fails</i>
isNaN(&lbrack;1, 2&rbrack;);       // <i>true : converted to "1, 2", which can't be converted to a number</i></pre>

<!-- page 13 -->
<p>This last one is a bit tricky: checking if an Array is <b>NaN</b>. To do
the Number() constructor first converts the array to a string, then to
a number; this is the reason why isNaN(&lbrack;&rbrack) and isNaN (&lbrack;34&rbrack;), 
"1,2", and <b>true</b> respectively. In general, <b>an array is
considered NaN by () unless it only holds one element whose string
representation can be converted to a valid number</b>.</p>

<pre>Version ≥ 6
<b>Number.isNaN</b></pre>  

<p>In ECMAScript 6, the Number.isNaN() function has been implemented primarily to
avoid the problem of window.isNaN() of forcefully converting the parameter to a 
number.Number.isNaN(), indeed, <b>doesn't try to convert </b> the value to a number 
before testing. This also means that <b>only values of the type number, that
are also NaN, return true</b> (which basically means only )).</p>

<p>From <a href="http://www.ecma-international.org/ecma-262/6.0/#sec-number.isnan">
ECMA-262 20.1.2.4</a>:</p>

<blockquote>
<p>When the Number .isNaN is called with one argument number, the following steps are taken:</p>

1.  If Type(number) is not Number, return <b>false</b>.
2.  If number is <b>NaN</b>, return <b>true</b>.
3.  Otherwise, return <b>false</b>.
</blockquote>

<p>Some examples:</p>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="left">
  <img src="./images/image011.png"
  title="Examples; Number.isNaN"
  alt="Examples; Number.isNaN."
  style="border: 2px solid #000000; width:7.486in;" />
<!-- (./images/image011.png){width="7.486805555555556in" height="4.891666666666667in"} -->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch3-3">Section 3.3: NaN</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/NaN"><b>NaN</b></a> 
stands for "Not a Number." When a mathematical function or operation in JavaScript cannot return a specific 
number, it returns the value <b>NaN</b> instead.</p>

<!-- page 14 -->

<p>It is a property of the global object, and a reference to 
<a href="https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Number/NaN">
Number.NaN</a></p>

<pre>window.hasOwnProperty('NaN'); // <i>true</i>
<b>NaN</b>; // <i>NaN</i></pre>

<p>Perhaps confusingly, <b>NaN</b> is still considered a number.</p>

<pre><b>typeof</b> <b>NaN</b>; // <i>'number'</i></pre>

<p>Don&apos;t check for <b>NaN</b> using the equality operator. See isNaN instead.</p>

<pre><b>NaN</b> == <b>NaN</b>  // <i>false</i>
<b>NaN</b> === <b>NaN</b> // <i>false</i></pre>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch3-4">Section 3.4: undefined and null</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p>At first glance it may appear that <b>null</b> and <b>undefined</b> are
basically the same, however there are subtle but important
differences.</p>

<p><b>undefined</b> is the absence of a value in the compiler, because where
it should be a value, there hasn&apos;t been put one, like the case of an
unassigned variable.</p>

<ul>
  <li><b>undefined</b> is a global value that represents the absence of an
    assigned value.
	<ul>
	  <li><b>typeof</b> <b>undefined</b> === 'undefined'</li>
	</ul>
  </li>
  <li><b>null</b> is an object that indicates that a variable has been
    explicitly assigned "no value".
	<ul>
	  <li><b>typeof</b> <b>null</b> === 'object'</li>
	</ul>
  </li>
</ul>

<p>Setting a variable to <b>undefined</b> means the variable effectively
does not exist. Some processes, such as JSON serialization, may strip
<b>undefined</b> properties from objects. In contrast, <b>null</b>
properties indicate will be preserved so you can explicitly convey the
concept of an "empty" property.</p>

<p>The following evaluate to <b>undefined</b>:</p>

<ul>
  <li>A variable when it is declared but not assigned a value (i.e. defined)
    <ul>
	  <li><b>let</b> foo;<br>
	    console.log('is undefined?', foo === <b>undefined</b>);<br>
        // <i>is undefined? true</i>
	  </li>
	</ul>
  <li>Accessing the value of a property that doesn't exist
    <ul>
	  <li><b>let</b> foo = { a: 'a' };<br>
	    console.log('is undefined?', foo.b === <b>undefined</b>);<br>
        // <i>is undefined? true</i>
	  </li>
	</ul>
  <li>The return value of a function that doesn't return a value
    <ul>
	  <li><b>function</b> foo() { <b>return</b>; }<br>
        console.log('is undefined?', foo() === <b>undefined</b>);<br>
		// <i>is undefined? true</i>
      </li>
	</ul>
  <li>The value of a function argument that is declared but has been omitted
    from the function call
	<ul>
      <li><b>function</b> foo(param) {<br>
          console.log('is undefined?', param === <b>undefined</b>);<br>
		}<br>
        foo('a');<br>
        foo();<br>
        // <i>is undefined? false</i><br>
        // <i>is undefined? true</i><br>
	  </li>
	</ul>
  </li>
</ul>

<!-- page 15 -->
<p><b>undefined</b> is also a property of the global window object.</p>

<pre>// <i>Only in browsers</i>
console.log(window.<b>undefined</b>); // <i>undefined</i>
window.hasOwnProperty('undefined'); // <i>true</i></pre>

<h5>Version &lt; 5</h5>

<p>Before ECMAScript 5 you could actually change the value of the
window.<b>undefined</b> property to any other value potentially breaking everything.</p>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch3-5">Section 3.5: Infinity and -Infinity</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<pre>1 / 0; // <i>Infinity</i>
// <i>Wait! WHAAAT?</i></pre>

<p><b>Infinity</b> is a property of the global object (therefore a global
variable) that represents mathematical infinity. It is a reference to Number.POSITIVE_INFINITY</p>

<p>It is greater than any other value, and you can get it by dividing by
0 or by evaluating the expression of a number that's so big that
overflows. This actually means there is no division by 0 errors in
JavaScript, there is Infinity!</p>

<p>There is also <b>-Infinity</b> which is mathematical negative infinity, and it's lower 
than any other value.</p>

<p>To get <b>-Infinity</b> you negate <b>Infinity</b>, or get a reference to it in 
<b>Number.NEGATIVE_INFINITY</b>.

<pre>- <b>Infinity</b>; // <i>-Infinity</i></pre>

<p>Now let's have some fun with examples:</p>

<pre><b>Infinity</b> &gt; 123192310293;  // <i>true</i>
<b>-Infinity</b> &lt; -123192310293;  // <i>true</i>
1 / 0;  // <i>Infinity</i>
Math.pow(123123123, 9123192391023); // <i>Infinity</i>
Number.MAX_VALUE * 2;  // <i>Infinity</i>
23 / <b>Infinity;</b>  // <i>0</i>
<b>-Infinity;</b>  // <i>-Infinity</i>
<b>-Infinity</b> === Number.NEGATIVE_INFINITY;  // <i>true</i>
-0;  // <i>-0 , yes there is a negative 0 in the Language</i>
0 === -0;  // <i>true</i>
1 / -0;  // <i>-Infinity</i>
1 / 0 === 1 / -0;  // <i>false</i>
<b>Infinity + Infinity</b>  // <i>Infinity</i>

<b>var</b> a = 0, b = -0;

a === b;  // <i>true</i>
1 / a === 1 / b;  // <i>false</i>

// <i>Try your own!</i></pre>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch3-6">Section 3.6: Number constants</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!-- page 16 -->
<p>The Number constructor has some built in constants that can be useful</p>

<pre>Number.MAX_VALUE;  // <i>1.7976931348623157e+308</i>
Number.MAX_SAFE_INTEGER;  // <i>9007199254740991</i>
Number.MIN_VALUE;  // <i>5e-324</i>
Number.MIN_SAFE_INTEGER;  // <i>-9007199254740991</i>

Number.EPSILON; // <i>0.0000000000000002220446049250313</i>

Number.POSITIVE_INFINITY; // <i>Infinity</i>
Number.NEGATIVE_INFINITY;  // <i>-Infinity</i>

Number.<b>NaN</b>;  // <i>NaN</i></pre>

<p>In many cases the various operators in JavaScript will break with
values outside the range of (Number.MIN_SAFE_INTEGER,Number.MAX_SAFE_INTEGER)</p>

<p>Note that represents the different between one and the smallest Number
greater than one, and thus the smallest possible difference between
two different Number values. One reason to use this is due to the
nature of how numbers are stored by JavaScript see Check the equality
of two numbers.</p>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch3-7">Section 3.7: Operations that return NaN</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p>Mathematical operations on values other than numbers return NaN.</p>

<pre>"b" &ast; 3
"cde" - "e"
&lbrack;1, 2, 3&rbrack; &ast; 2</pre>

<p>An exception: Single-number arrays.</p>

<pre>&lbrack;2&rbrack; &ast; &lbrack;3&rbrack;  // <i>Returns 6</i></pre>

<p>Also, remember that the + operator concatenates strings.</p>

<pre>"a" + "b"  // <i>Returns "ab"</i></pre>

<p>Dividing zero by zero returns <b>NaN</b>.</p>

<pre>0 / 0  // <i>NaN</i></pre>

<p>Note: In mathematics generally (unlike in JavaScript programming),
dividing by zero is not possible.</p>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch3-8">Section 3.8: Math library functions that return NaN</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p>Generally, Math functions that are given non-numeric arguments will
return NaN.</p>

<pre>Math.floor("a")</pre>

<p>The square root of a negative number returns NaN, because does not
support <a href="https://en.wikipedia.org/wiki/Imaginary_number">imaginary</a> or
<a href="https://en.wikipedia.org/wiki/Complex_number">complex</a> numbers.</p>

<pre>Math.sqrt(-1)</pre>
<!-- page 17 -->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h2 id="ch4">Chapter 4: Comments</h2>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch4-1">Section 4.1: Using Comments</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p>To add annotations, hints, or exclude some code from being executed
JavaScript provides two ways of commenting code lines.</p>

<h4>Single line Comment //</h4>

<p>Everything after the // until the end of the line is excluded from execution.</p>

<pre>
<b>function</b> elementAt( event ) {
// <i>Gets the element from Event coordinates</i>
  <b>return</b> document.elementFromPoint(event.clientX, event.clientY);
}
&ast;// <i>TODO: write more cool stuff!</i>
</pre>

<h4>Multi-line Comment /&ast;&ast;/</h4>

<p>Everything between the opening /* and the closing */ is excluded
from execution, even if the opening and closing are on different
lines.</p>

<pre>
/*
   <i>Gets the element from Event coordinates.
   Use like:
     var clickedEl = someEl.addEventListener("click", elementAt, false);</i>
*/
<b>function</b> elementAt( event ) {
  <b>return</b> document.elementFromPoint(event.clientX, event.clientY);
}
/&ast; <i>TODO: write more useful comments!</i> */
</pre>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch4-2">Section 4.2: Using HTML comments in JavaScript (Bad practice)</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p>HTML comments (optionally preceded by whitespace) will cause code (on
the same line) to be ignored by the browser also, though this is
considered <b>bad practice</b>.</p>

<p>One-line comments with the HTML comment opening sequence (&lt;!-&dash;):

<p><b>Note:</b> the JavaScript interpreter ignores the closing characters of HTML comments (&dash;-&gt;) here.</p>

<pre>
&lt;!-- A single-line comment.
&lt;!-- --&gt; Identical to using `//` since
&lt;!-- --&gt; the closing '--&gt;' is ignored.
</pre>

<p>This technique can be observed in legacy code to hide JavaScript from
browsers that didn't support it:</p>

<pre>
<b>script</b> type="text/javascript" language="JavaScript"<b>&gt;</b>
&lt;!-&dash;
/* Arbitrary JavaScript code.
   Old browsers would treat
   it as HTML code. */
// --&gt;
&lt;/script&gt;
</pre>

<!-- page 18 -->
<p>An HTML closing comment can also be used in JavaScript (independent of
an opening comment) at the beginning of a line (optionally preceded by
whitespace) in which case it too causes the rest of the line to be
ignored:</p>

<pre>
&dash;-&gt; Unreachable JS code
</pre>

<p>These facts have also been exploited to allow a page to call itself
first as HTML and secondly as JavaScript. For example:</p>

<pre>
&lt;!-&dash;
 self.postMessage('reached JS "file"');
/*
&dash;-&gt;
<b>&lt;!DOCTYPE html&gt;</b>
<b>&lt;script&gt;</b>
var w1 = new Worker('#1');
w1.onmessage = function (e) {
  console.log(e.data); // 'reached JS "file"
};
<b>&lt;/script&gt;</b>
&lt;!-&dash;
*/
&dash;-&gt;
</pre>

<p>When run a HTML, all the multiline text between the &lt;!-&dash; and &dash;-&gt;
comments are ignored, so the JavaScript contained therein is ignored
when run as HTML.</p>

<p>As JavaScript, however, while the lines beginning with &lt;!-&dash; and &dash;-&gt;
are ignored, their effect is not to escape over <i>multiple</i>
lines, so the lines following them (e.g., self.postMessage(...) will not be ignored when
run as JavaScript, at least until they reach a <i>JavaScript</i> comment,
marked by /* and */. Such JavaScript comments are used in the above
example to ignore the remaining <i>HTML</i> text (until the &dash;-&gt; which is
also ignored as JavaScript).</p>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h2 id="ch5">Chapter 5: Console</h2>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!-- page 19 -->
<p>The information displayed by a <a href="https://developer.mozilla.org/en-US/docs/Tools/Web_Console">
debugging/web console</a> is made available through the multiple <a href="https://developer.mozilla.org/en-US/Add-ons/SDK/Tools/console">
methods of the console Javascript object</a> that can be consulted through property, the methods 
displayed are generally the following (taken from Chromium&apos;s output):

<ul>
  <li><a href="https://developer.mozilla.org/en-US/docs/Web/API/console/assert">assert</a></li>
  <li><a href="https://developer.mozilla.org/en-US/docs/Web/API/Console/clear">clear</a></li>
  <li><a href="https://developer.mozilla.org/en-US/docs/Web/API/Console/count">count</a></li>
  <li><a href="https://developer.mozilla.org/en-US/Add-ons/SDK/Tools/console#console.debug(...)">debug</a></li>
  <li><a href="https://developer.mozilla.org/en-US/docs/Web/API/Console/dir">dir</a></li>
  <li><a href="https://developer.mozilla.org/en-US/docs/Web/API/Console/dirxml">dirxml</a></li>
  <li><a href="https://developer.mozilla.org/en-US/docs/Web/API/Console/error">error</a></li>
  <li><a href="https://developer.mozilla.org/en-US/docs/Web/API/Console/group">group</a></li>
  <li><a href="https://developer.mozilla.org/en-US/docs/Web/API/Console/groupCollapsed">groupCollapsed</a></li>
  <li><a href="https://developer.mozilla.org/en-US/docs/Web/API/Console/groupEnd">groupEnd</a></li>
  <li><a href="https://developer.mozilla.org/en-US/docs/Web/API/Console/info">info</a></li>
  <li><a href="https://developer.mozilla.org/en-US/docs/Web/API/Console/log">log</a></li>
  <li>markTimeline</li>
  <li><a href="https://developer.mozilla.org/en-US/docs/Web/API/Console/profile">profile</a></li>
  <li><a href="https://developer.mozilla.org/en-US/docs/Web/API/Console/profileEnd">profileEnd</a></li>
  <li><a href="https://developer.mozilla.org/en-US/docs/Web/API/Console/table">table</a></li>
  <li><a href="https://developer.mozilla.org/en-US/docs/Web/API/Console/time">time</a></li>
  <li><a href="https://developer.mozilla.org/en-US/docs/Web/API/Console/timeEnd">timeEnd</a></li>
  <li><a href="https://developer.mozilla.org/en-US/docs/Web/API/Console/timeStamp">timeStamp</a></li>
  <li>timeline</li>
  <li>timelineEnd</li>
  <li><a href="https://developer.mozilla.org/en-US/docs/Web/API/Console/trace">trace</a></li>
  <li><a href="https://developer.mozilla.org/en-US/docs/Web/API/Console/warn">warn</a></li>
</ul>

<h4>Opening the Console</h4>

<p>In most current browsers, the JavaScript Console has been integrated
as a tab within Developer Tools. The shortcut keys listed below will
open Developer Tools, it might be necessary to switch to the right tab
after that.</p>

<h4>Chrome</h4>

<p>Opening the "Console" panel of Chrome's <b>DevTools</b>:</p>

<ul>
  <li>Windows / Linux: any of the following options.
    <ul>
      <li>Ctrl + Shift + J</li>
      <li>Ctrl + Shift + I , then click on the "Web Console" tab <b>or</b> press ESC to toggle the console on and off</li>
      <li>F12 , then click on the "Console" tab <b>or</b> press ESC to toggle the console on and off</li>
    </ul>
  </li>
  <li>Mac OS: Cmd + Opt + J</li>
</ul>

<h4>Firefox</h4>
<!-- page 20 -->
<p>Opening the "Console" panel in Firefox's <b>Developer Tools</b>:</p>

<ul>
  <li>Windows / Linux: any of the following options.
    <ul>
	  <li>Ctrl + Shift + K</li>
	  <li>Ctrl + Shift + I , then click on the "Web Console" tab <b>or</b> press ESC to toggle the console on and off</li>
	  <li>F12 , then click on the "Web Console" tab <b>or</b> press ESC to toggle the console on and off</li>
	</ul>
	</li>
  <li>Mac OS: Cmd + Opt + K</li>
</ul>

<h4>Edge and Internet Explorer</h4>

<p>Opening the "Console" panel in the <b>F12 Developer Tools</b>:</p>

<ul>
  <li>F12 , then click on the "Console" tab</li>
</ul>

<h4Safari</h4>

<p>Opening the "Console" panel in Safari's <b>Web Inspector</b> you must
first enable the develop menu in Safari&apos;s Preferences</p>

<!-- image goes here top of pg 21 -->

<p>Then you can either pick &quot;Develop-&gt;Show Error Console&quot; from the menus or press ⌘
&plus; Option &plus; C</p>

<h4>Opera</h4>

<p>Opening the "Console" in opera:</p>

<ul>
  <li>Ctrl + Shift + I ,then click on the "Console" tab</li>
</ul>

<h4>Compatibility</h4>

<p>When using or emulating Internet Explorer 8 or earlier versions (e.g.
through Compatibility View / Enterprise Mode) the console will
<b>only</b> be defined when the Developer Tools are active, so console.log ()
statements can cause an exception and prevent code from executing. To
mitigate this, you can check to see if the console is available before
you log:</p>

<pre>
<b>if</b> (<b>typeof</b> window.console !== &apos;undefined&apos)
{
  console.log(&quot;Hello World&quot;);
}
</pre>

<p>Or at the start of your script you can identify if the console is available and if not, define a null function to catch all of your
references and prevent exceptions.</p>

<!-- page 22 -->

<pre>
<b>if</b> (!window.console)
{
  console = {log: <b>function</b>() {}};
}
</pre>

<p>Note this second example will stop <b>all</b> console logs even if the developer window has been opened.</p>

<p>Using this second example will preclude use of other functions such as console.dir(obj) unless that is specifically added.</p>

<p>A browser&apos;s debugging console or <a href="https://developer.mozilla.org/en-US/docs/Tools/Web_Console">web console</a>
is generally used by developers to identify errors, understand flow of
execution, log data and for many other purpose at runtime. This
information is accessed through the <a href="https://developer.mozilla.org/en-US/docs/Web/API/Console">
console</a> object.</p>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch5-1">Section 5.1: Measuring time - console.time()</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p>console.time() can be used to measure how long a task in your code takes to run.</p>

<p>Calling <a href="https://developer.mozilla.org/en-US/docs/Web/API/Console/timeEnd">
console.time(&lbrack;label&rbrack;)</a> starts a new timer. When 
<a href="https://developer.mozilla.org/en-US/docs/Web/API/Console/time">
console.timeEnd(&lbrack;label&rbrack;) is called, the elapsed time, in milliseconds, Since
the original .time() call is calculated and logged. Because of this behavior, you can call 
.timeEnd() multiple times with the same label to log the elapsed time since the original .time()
call was made.</p>

<h4>Example 1:</h4>

<pre>
console.time(&apos;response in&apos;);

alert(&apos;Click to continue&apos;);
console.timeEnd(&apos;response in&apos;);

alert(&apos;One more time&apos;);
console.timeEnd(&apos;response in&apos;);
</pre>

<p>will output:</p>

<pre>
response <b>in</b>: 774.967ms
response <b>in</b>: 1402.199ms
</pre>

<h4>Example 2:</h4>

<pre>
<b>var</b> elms = document.getElementsByTagName(&apos;*&apos;); // <i>select all elements on the page</i>

console.time(&apos;Loop time&apos;);

<b>for</b>(<b>var</b> i = 0; i &lt; 5000; i ++ ) {
  <b>for</b> (<b>var</b> j = 0, length = elms.length; j &lt; length; j ++ ) { 
    // <i>nothing to do ...</i>
  }
} 
console.timeEnd(&apos;Loop time&apos;);
</pre>

<p>will output:</p>

<pre>
Loop time: 40.716ms
</pre>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch5-2">Section 5.2: Formatting console output</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!-- page 23 -->
<p>Many of the console&apos;s print methods can also handle C-like string
formatting, using % tokens:</p>

<pre>
console.log(&apos;%s has %d points&apos;,&apos;Sam&apos;,100);
</pre>

<p>Display Sam has 100 points.</p>

<p>The full list of format specifiers in JavaScript is:</p>

| <b>Specifier | Output</b>                             |
|---------|:-------------------------------------------:|
| %s | Formats the value as a string |
| %i or %d | Formats the value as an integer |
| %f | Formats the value as a floating point value |
| %o | Formats the value as an expandable DOM element |
| %O | Formats the value as an expandable JavaScript object |
| %c | Applies CSS style rules to the output string as specified by the second parameter |

<h4>Advanced styling</h4>

<p>When the CSS format specifier (%c) is placed at the left side of the
string, the print method will accept a second parameter with CSS rules
which allow fine-grained control over the formatting of that string:</p>

<pre>
console.log(&apos;%cHello world!&apos;, &apos;color: blue; font-size: xx-large&apos;);</p>
</pre>

<p>Displays:</p>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="left">
  <img src="./images/image013.jpg"
  title=" "
  alt="."
  style="border: 2px solid #000000; width:7.477in;" />
<!-- (./images/image013.jpg){width="7.477777777777778in" height="0.6666666666666666in"} -->

<p>It is possible to use multiple %c format specifiers:</p>

<ul>
  <li>any substring to the right of a %c has a corresponding parameter in
    the print method;</li>
  <li>this parameter may be an empty string, if there is no need to apply CSS 
    rules to that same substring;</li>
  <li>if two %c format specifiers are found, the 1st (encased in %c) and 2nd 
    substring will have their rules defined in the 2nd and 3rd parameter of the print
	method respectively.</li>
  <li>if three %c format specifiers are found, then the 1st, 2nd and 3rd substrings will 
    have their rules defined in the 2nd , 3rd and 4th parameter respectively, and so on&hellip;</li>
</ul>

<pre>
console.log("%cHello %cWorld%c!!", // <i>string to be printed</i>

"color: blue;", // <i>applies color formatting to the 1st substring</i>

&quot;font-size: xx-large;&quot;, // <i>applies font formatting to the 2nd substring</i>

&quot;/&ast; no CSS rule&ast;/&quot; // <i>does not apply any rule to the remaining substring</i>
);
</pre>

<p>Displays:</p>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="left">
  <img src="./images/image014.jpg"
  title=" "
  alt="."
  style="border: 2px solid #000000; width:7.477in;" />
<!-- (./images/image014.jpg){width="7.477777777777778in" height="0.6395833333333333in"} -->

**Using groups to indent output**

Output can be indented and enclosed in a collapsible group in the
debugging console with the following methods:

[groupCollapsed](https://developer.mozilla.org/en-US/docs/Web/API/Console/groupCollapsed):
creates a collapsed group of entries that can be expanded through the

  [console.groupCollapsed](https://developer.mozilla.org/en-US/docs/Web/API/Console/groupCollapsed)
  
  [console.group](https://developer.mozilla.org/en-US/docs/Web/API/Console/group)

disclosure button in order to reveal all the entries performed after
this method is invoked;

[Console group](https://developer.mozilla.org/en-US/docs/Web/API/Console/group):
creates an expanded group of entries that can be collapsed in order to
hide the entries after this method is invoked.

The indentation can be removed for posterior entries by using the
following method:

[console.groupEnd()](https://developer.mozilla.org/en-US/docs/Web/API/Console/groupEnd):
exits the current group, allowing newer entries to be printed in the
parent group after this method is invoked.

Groups can be cascaded to allow multiple indented output or
collapsible layers within each other:

  
  Collapsed group expanded =&gt;

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="left">
  <img src="./images/image015.jpg"
  title=" "
  alt="."
  style="border: 2px solid #000000; width:2.108in;" />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<img src="./images/image016.jpg"
  title=" "
  alt="."
  style="border: 2px solid #000000; width:2.081in;" />
<!-- ![](./images/image015.jpg){width="2.1083333333333334in" height="3.009027777777778in"} -->
<!-- ![](./images/image016.jpg){width="2.08125in" height="3.729861111111111in"} -->

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch5-3">Section 5.3: Printing to a browser&apos;s debugging console</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p>A browser&apos;s debugging console can be used in order to print simple
messages. This debugging or <a href="https://developer.mozilla.org/en-US/docs/Tools/Web_Console">web
console</a> can be directly opened in the browser (F12 key in most browsers 
see <i>Remarks</i> below for further information) and the log method of the
console JavaScript object can be invoked by typing the following:</p>

<pre>
console.log('My message');
</pre>

<p>Then, by pressing Enter, this will display "My message" in the debugging console.

<p>console.log() can be called with any number of arguments and variables available in
the current scope. Multiple arguments will be printed in one line with a small space between them.</p>

<pre>
<b>var</b> obj = {test: 1};
console.log(&lbrack;'string'&rbrack;, 1, obj, window);
</pre>

<p>The log method will display the following in the debugging console:</p>

<pre>
&lbrack;'string'&rbrack; 1 Object { test: 1 } Window { /* <i>truncated</i> */ }
</pre>

<p>Beside plain strings, console.log() can handle other types, like arrays, objects, dates, functions, etc.:</p>

<pre>
console.log(&lbrack;0, 3, 32, 'a string' &rbrack;);
console.log({key1: 'value', key2: 'another value'});
</pre>

<h4>Displays:</h4>

<pre>
Array &lbrack;0, 3, 32, 'a string'&rbrack;
Object { key1: 'value', key2: 'another value'}
</pre>

<p>Nested objects may be collapsed:</p>

<pre>
console.log({ key1: 'val', key2:
&lbrack;'one', 'two'&rbrack;, key3: { a: 1, b: 2 } });
</pre>

<h4>Displays:</h4>

<pre>
Object { key1: 'val', key2: Array &lbrack;2&rbrack;, key3: Object }
</pre>

<p>Certain types such as Date objects and **function**s may be displayed
differently:</p>

<pre>
console.log( **new** Date ( 0 ) );
console.log( **function** test(a, b) { **return** c; });


<h4>Displays:</h4>

<pre>
Wed Dec 31 1969 19:00:00 GMT &minus; 0500 (Eastern Standard Time)
**function** test (a , b) { **return** c;}

<h4>Other print methods</h4>

<p>In addition to the log method, modern browsers also support similar methods:</p>

<ul>
  <li><a href="https://developer.mozilla.org/es/docs/Web/API/Console/info">
    console.info</a> - small informative icon (ⓘ) appears on the left side of the printed
    string(s) or object(s).</li>
  <li><a href="a href="https://developer.mozilla.org/en-US/docs/Web/API/Console/warning">
    console.warn</a> - small warning icon (!) appears on the left side. In some browsers,
    the background of the log is yellow.</li>
  <li><a href="a href="https://developer.mozilla.org/en-US/docs/Web/API/Console/error">
    console.error</a> - small times icon (⊗) appears on the left side. In some browsers, 
	the background of the log is red.</li>
  <li><a href="https://developer.mozilla.org/en-US/docs/Web/API/Console/timeStamp">
    console.timeStamp</a> - outputs the current time and a specified string, but 
	is non-standard:</li>
</ul>

<back
<pre>
console.timeStamp('msg');
</pre>

<h4>Displays:</h4>

<pre>
00:00:00.001 msg
</pre>

<ul>
  <li><a href="https://developer.mozilla.org/en-US/docs/Web/API/Console/trace">
    console.trace</a> outputs the current stack trace or displays the same output as the
	log method if invoked in the global scope.</li>
</ul>
<!-- page 26 -->
<pre>
<b>function</b> sec () {
  first();
}
<b>function</b> first () {
  console.trace();
}
sec ();
</pre>

<h4>Displays:</h4>

<pre>
first
sec
(anonymous <b>function</b>)
</pre>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="left">
  <img src="./images/image017.jpg"
  title=" "
  alt="."
  style="border: 2px solid #000000; width:7.477in;" />
<!-- (./images/image017.jpg){width="7.477777777777778in" height="1.3243055555555556in"} -->

<p>The above image shows all the functions, with the exception of timeStamp, in Chrome version 56.</p>

<p>These methods behave similarly to the log method and in different
debugging consoles may render in different colors or formats.</p>

<p>In certain debuggers, the individual objects information can be
further expanded by clicking the printed text or a small triangle (►)
which refers to the respective object properties. These collapsing
object properties can be open or closed on log. See the for additional
information on this.</p>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch5-4">Section 5.4: Including a stack trace when logging console.trace()</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<pre>
<b>function</b> foo(){
  console.trace('My log statement');
}

foo();
</pre>

<h4>Will display this in the console:</h4>

<pre>
My log statement VM696:1
  foo            @ VM696:1
  (anonymous <b>function</b>) @ (program):1
</pre>

<p>Note: Where available it&apos;s also useful to know that the same stack
trace is accessible as a property of the Error object. This can be
useful for post-processing and gathering automated feedback.</p>

<pre>
<b>var</b> e = <b>new</b> Error ('foo');
console.log(e&period;stack);
</pre>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch5-5">Section 5.5: Tabulating values - console.table()</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
console.table 
 
  
In most environments, () can be used to display objects and arrays in
a tabular format.

**For example:**

console.table(&lbrack;&apos;Hello&apos;,&apos;world&apos;&rbrack;);
displays like:

*(index) value**

0 &quot;Hello&quot; 1 &quot;world&quot;
console.table({foo: &apos;bar&apos;, bar: &apos;baz&apos;});

displays like:

**(index) value**
&quot;foo&quot; &quot;bar&quot; &quot;bar&quot; &quot;baz&quot;
**var** personArr = &lbrack; { &quot;personId&quot;: 123, &quot;name&quot;: &quot;Jhon&quot;, &quot;city&quot;: &quot;Melbourne&quot;, &quot;phoneNo&quot;
: &quot;1234567890&quot;}, {&quot;personId&quot;: 124, &quot;name&quot;: &quot;Amelia&quot;, &quot;city&quot;: &quot;Sydney&quot;,
&quot;phoneNo&quot;: &quot;1234567890&quot; }, {
&quot;personId&quot;: 125,
&quot;name&quot;: &quot;Emily&quot;,
&quot;city&quot;: &quot;Perth&quot;,
&quot;phoneNo&quot;: &quot;1234567890&quot;},
{&quot;personId&quot;: 126,
&quot;name&quot;: &quot;Abraham&quot;,
&quot;city&quot;: &quot;Perth&quot;,
&quot;phoneNo&quot;: &quot;1234567890&quot;}
&rbrack;;
console.table(personArr, &lbrack;&apos;name&apos;, &apos;personId&apos;&rbrack;);

displays like:
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="left">
  <img src="./images/image018.jpg"
  title=" "
  alt="."
  style="border: 2px solid #000000; width:7.477in;" />
<!-- ![](./images/image018.jpg){width="7.477777777777778in" height="4.279166666666667in"} -->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch5-6">Section 5.6: Counting - console.count()</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
[console.count](https://developer.mozilla.org/en-US/docs/Web/API/Console/count)
[(&lbrack;](https://developer.mozilla.org/en-US/docs/Web/API/Console/count)
[obj](https://developer.mozilla.org/en-US/docs/Web/API/Console/count)

[&rbrack;)](https://developer.mozilla.org/en-US/docs/Web/API/Console/count)
places a counter on the object&apos;s value provided as argument. Each time
this method is invoked, the counter is increased (with the exception of the empty
string &apos;&apos;). A label together with a number is displayed in the
debugging console according to the following format:

&lbrack;label&rbrack;: X

label represents the value of the object passed as argument and X
represents the counter&apos;s value.

An object&apos;s value is always considered, even if variables are
provided as arguments:

**var** o1 = 1, o2 = &apos;2&apos;, o3 = &quot;&quot;;
console.count(o1);
console.count(o2);
console.count(o3);
console.count(1);
console.count(&apos;2&apos;);
console.count(&apos;&apos;);
Displays:1:12:1:11:22:2:1
Strings with numbers are converted to Number
objects: console.count(42.3);
console.count(Number(&apos;42.3&apos;));
console.count(&apos;42.3&apos;);
Displays:42.3:142.3:242.3:3
Functions point always to the global
Function object: console.count(console.constructor);
console.count(**function**(){});
console.count(Object);
**var** fn1 = **function** myfn ( ){};
console.count(fn1);
console.count(Number);
Displays:
&lbrack;object Function&rbrack;: 1 &lbrack;object Function&rbrack;: 2
&lbrack;object Function&rbrack;: 3 &lbrack;object Function&rbrack;: 4
&lbrack;object Function&rbrack;: 5 
Certain objects get specific counters associated to the type of object they refer to:

console.count(**undefined**);
console.count(document.Batman);
**var** obj;
console.count(obj);
console.count(Number(**undefined**));
console.count(**NaN**);
console.count(**NaN** &plus; 3);
console.count(1 /0);
console.count(String ( 1 /0));
console.count(window);
console.count(document);
console.count(console);
console.count(console.&lowbar;&lowbar;proto&lowbar;&lowbar;);
console.count(console.constructor
.**prototype**);
console.count(
console.&lowbar;&lowbar;proto&lowbar;&lowbar;.constructor.
**prototype**
);
console.count(Object.getPrototypeOf(console));
console.count(**null**);
Displays:
**undefined**:1
**undefined**:2
**undefined**:3
**NaN**:1
**NaN**:2
**NaN**:3
**Infinity**:1
**Infinity**:2
&lbrack;object Window&rbrack;:
1&lbrack;object HTMLDocument&rbrack;:
1&lbrack;object Object&rbrack;: 1
&lbrack;
object
Object
&rbrack;
:
2
&lbrack;
object
Object
&rbrack;
:
3
&lbrack;
object
Object
&rbrack;
:
4
&lbrack;
object
Object
&rbrack;
:

**null**
:
1
**Empty string or absence of argument**

If no argument is provided while **sequentially inputting the count
method in the debugging console**, an empty string is assumed as
parameter, i.e.:

console.count();
:1&gt; console.count(&apos;&apos;);
:2&gt; console.count(&quot;&quot;);
:3
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch5-7">Section 5.7: Clearing the console - console.clear()</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
 
You can clear the console window using the () method. This removes all
previously printed messages in the console and may print a message
like &quot;Console was cleared&quot; in some environments.
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch5-8">Section 5.8: Displaying objects and XML interactively console.dir(), console.dirxml()</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
displays an interactive list of the properties of the specified
JavaScript object. The output is

presented as a hierarchical listing with disclosure triangles that let
you see the contents of child objects.

**var** myObject = { &quot;foo&quot; : { &quot;bar&quot; : &quot;data&quot; } };

console.dir ( myObject );

displays:
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="left">
  <img src="./images/image019.jpg"
  title=" "
  alt="."
  style="border: 2px solid #000000; width:7.477in;" />
<!-- ![](./images/image019.jpg){width="7.477777777777778in" height="2.657638888888889in"} -->

prints an XML representation of the descendant elements of object if
possible, or the JavaScript representation if not. Calling () on HTML
and XML elements is equivalent to calling ().

**Example 1:**

console.dirxml ( document )
displays:
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="left">
  <img src="./images/image020.jpg"
  title=" "
  alt="."
  style="border: 2px solid #000000; width:7.477in;" />
<!-- ![](./images/image020.jpg){width="7.477777777777778in" height="1.6847222222222222in"} -->

**Example 2:**

console.log(document)

displays:
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="left">
  <img src="./images/image021.jpg"
  title=" "
  alt="."
  style="border: 2px solid #000000; width:7.477in;" />
<!-- ![](./images/image021.jpg){width="7.477777777777778in" height="1.8020833333333333in"} -->

**Example 3:**

**var** myObject = { &quot;foo&quot; : { &quot;bar&quot; : &quot;data&quot; } };

console.dirxml ( myObject );

displays:
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="left">
  <img src="./images/image022.jpg"
  title=" "
  alt="."
  style="border: 2px solid #000000; width:6.5in;" />
<!-- ![](./images/image022.jpg){width="6.504166666666666in" height="2.6486111111111112in"} -->

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch5-9">Section 5.9: Debugging with assertions - console.assert()</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

Writes an error message to the console if the assertion is **false**.
Otherwise, if the assertion is **true**, this does nothing.

console.assert ( &apos;one&apos; === 1 );

Multiple arguments can be provided after the assertionthese can be
strings or other objectsthat will only be printed if the assertion
is **false**:
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p align="left">
  <img src="./images/image024.jpg"
  title=" "
  alt="."
  style="border: 2px solid #000000; width:6.5in;" />
<!-- ![](./images/image024.jpg){width="6.46875in" height="1.2069444444444444in"} -->

[console.assert](https://developer.mozilla.org/en-US/docs/Web/API/console/assert)

does *not* throw an AssertionError (except in Node.js), meaning that
this method is incompatible with most testing frameworks and that code execution will not break on
a failed assertion.

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h2 id="ch6">Chapter 6: Datatypes in JavaScript</h2>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch6-1">Section 6.1: typeof</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

**typeof** is the &apos;official&apos; function that one uses to get the type
in JavaScript, however in certain cases it might yield some unexpected
results &hellip;

1.  **Strings**
**typeof** &quot;String&quot; or
**typeof** Date(2011,01,01)
&quot;string&quot;

2.  **Numbers**
**typeof** 42
&quot;number&quot;

3.  **Bool**
  **typeof** **true**
(valid values **true** and **false**)
&quot;boolean&quot;

4.  **Object**
  **typeof** {}
  **typeof** &lbrack;&rbrack;
  **typeof** **null**
  **typeof** /aaa/
or or or or
**typeof** Error()
&quot;object&quot;

5.  **Function**
**typeof** **function**(){}
&quot;function&quot;

6.  **Undefined**
**var** var1; **typeof** var1
&quot;undefined&quot;

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch6-2">Section 6.2: Finding an object&apos;s class</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

To find whether an object was constructed by a certain constructor or
one inheriting from it, you can use the

**instanceof**

command:
*//We want this function to take the sum of the numbers passed to it*

*//It can be called as sum(1, 2, 3) or sum(&lbrack;1, 2, 3&rbrack;) and should give
6*

**function**
sum ( &hellip; arguments ) { **if**
( arguments.

length === 1 )
{
**const** &lbrack; firstArg &rbrack; = arguments **if** ( firstArg **instanceof**

Array ) {

*//firstArg is something like &lbrack;1, 2, 3&rbrack;*

**return**

sum ( &hellip;
firstArg )

*//calls sum(1, 2, 3)* }
}
**return**
arguments.
reduce
( (a, b) =&gt; a &plus; b ) }

console.log ( sum ( 1 , 2 , 3 ) )

*//6*

console.log (
sum
(
&lbrack;
1
,
2
,
3
&rbrack;
)
)
*//6*
console.
log
(
sum
(
4
)
)
*//4*

Note that primitive values are not considered instances of any class:
console.
log
(
2
**instanceof**
Number
)
*//false*
console.
log
(
&apos;abc&apos;
**instanceof**
String
)
*//false*
console.
log
(
**true**
**instanceof**
Boolean
)
*//false*
console.log(Symbol
(
)
<b>instanceof</b>
Symbol
)

*//false*

Every value in JavaScript besides **null** and **undefined** also has
a constructor property storing the function that was used to construct
it. This even works with primitives.

*//Whereas instanceof also catches instances of subclasses, //using
obj.constructor does not* console.log(&lbrack;&rbrack; **instanceof** Object, &lbrack;&rbrack;
**instanceof** Array) *//true true* console.log(&lbrack;&rbrack;.constructor ===
Object, &lbrack;&rbrack;.constructor === Array) *//false true*

**function** isNumber(value) {

*//null.constructor and undefined.constructor throw an error when
accessed* **if** (value === **null** &vert;&vert; value === **undefined**)
**return** **false** **return** value.constructor === Number }
console.log(isNumber(**null**), isNumber(**undefined**)) *//false
false* console.log(isNumber(&apos;abc&apos;), isNumber(&lbrack;&rbrack;), isNumber(() =&gt;
1)) *//false false false* console.log(isNumber(0),
isNumber(Number(&apos;10.1&apos;)), isNumber(**NaN**)) *//true true true*

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch6-3">Section 6.3: Getting object type by constructor name</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

When one with **typeof** operator one gets type object it falls into
somewhat wast category&hellip;
In practice you might need to narrow it down to what sort of
&apos;object&apos; it actually is and one way to do it is to use
  Object     .   **prototype**   .   toString      .   call   (   yourObject
object constructor name to get what flavour of object it actually is:
)
1.  **String**
  Object     .   **prototype**    .   toString       .   call    (   &quot;String&quot;
)

&quot;&lbrack;object String&rbrack;&quot;

2.  **Number**
  Object       .   **prototype**       .   toString          .   call     (   42
)
&quot;&lbrack;object Number&rbrack;&quot;

3.  **Bool**
  Object       .   **prototype**      .   toString         .   call     (   **true**
)
&quot;&lbrack;object Boolean&rbrack;&quot;

4.  **Object**
  Object
  call
  call
  toString
  toString
  **prototype**
  **prototype**
  Object
  Object
&hellip;(()) or &hellip;({})
&quot;&lbrack;object Object&rbrack;&quot;

5.  **Function**
  Object     .   **prototype**    .   toString       .   call    (   **function**
(){})
&quot;&lbrack;object Function&rbrack;&quot;

6.  **Date**
  Object   .   **prototype**   .   toString    .   call   (   **new**     (   2015   ,   10   ,   21
                                                              Date                                
))

&quot;&lbrack;object Date&rbrack;&quot;

7.  **Regex**
  **new** RegExp
  call
  call
  toString
  toString
  **prototype**
  **prototype**
  Object
  Object
  */foo/*
&hellip;(()) or &hellip;();
&quot;&lbrack;object RegExp&rbrack;&quot;

8.  **Array**
  Object         .   **prototype**         .   toString           .   call
(&lbrack;&rbrack;);
&quot;&lbrack;object Array&rbrack;&quot;

9.  **Null**

  -
  Object       .   **prototype**      .   toString         .   call     (   **null**
    -  -    -

  -

);

&quot;&lbrack;object Null&rbrack;&quot;

10. **Undefined**

  -
  Object     .   **prototype**   .   toString       .   call    (   **undefined**
  -      -  

  -

);

&quot;&lbrack;object Undefined&rbrack;&quot;

11. **Error**

  
  Object      .   **prototype**     .   toString        .   call    (   Error
        -  

  

());

&quot;&lbrack;object Error&rbrack;&quot;

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h2 id="ch7">Chapter 7: Strings</h2>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch7-1">Section 7.1: Basic Info and String Concatenation</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

Strings in JavaScript can be enclosed in Single quotes &apos;hello&apos;,
Double quotes &quot;Hello&quot; and (from ES2015, ES6) in Template Literals
(*backticks*) \`hello\`.

**var** hello = &quot;Hello&quot;;
**var** world = &apos;world&apos;;
**var** helloW = \`Hello World\`;

*// ES2015 / ES6*
String
Strings can be created from other types using the () function.

**var** intString = String ( 32 );

*// &quot;32&quot;*

**var** booleanString = String ( **true** );

*// &quot;true&quot;* 

**var** nullString = String ( **null** );

*// &quot;null&quot;*
toString
Or, () can be used to convert Numbers, Booleans or Objects to Strings.

**var** intString = ( 5232 ) . toString ();

*// &quot;5232&quot;*

**var** booleanString = ( **false** ).toString();

*// &quot;false&quot;*

**var** objString = ( { } ) . toString ( );

*// &quot;&lbrack;object Object&rbrack;&quot;*

  
String                 .   fromCharCode
Strings also can be created by using method.
String
.
fromCharCode
(

104

,

101

,

108

,

108

,

111

)

*//&quot;hello&quot;*

Creating a String object using **new** keyword is allowed, but is not
recommended as it behaves like Objects unlike primitive strings.

**var**

objectString

=

**new**

String

(

&quot;Yes, I am a String object&quot;

)

;

**typeof**

objectString

;

*//&quot;object&quot;*

**typeof**

objectString.

valueOf

(

)

;

*//&quot;string&quot;*

**Concatenating Strings**

  
  concat
  

  

String concatenation can be done with the + concatenation operator, or
with the built-in () method on the String object prototype.

**var**

foo

=

&quot;Foo&quot;

;

**var**

bar

=

&quot;Bar&quot;

;

console.

log

(

foo

&plus;

bar

)

;

*// =&amp;quot;FooBar&quot;*

console.

log

(

foo

&plus;

&quot; &quot;

&plus;

bar

)

;

*// =&amp;quot;Foo Bar&quot;*

foo.

concat

(

bar

)

*// =&amp;quot;FooBar&quot;*

&quot;a&quot;

.

concat

(

&quot;b&quot;

,

&quot; &quot;

,

&quot;d&quot;

)

*// =&amp;quot;ab d&quot;*

Strings can be concatenated with non-string variables but will
type-convert the non-string variables into strings.

**var**

string

=

&quot;string&quot;

;

**var**

number

=

32

;

**var**

boolean

=

**true**

;

console.

log

(

string

&plus;

number

&plus;

boolean

)

;

*// &quot;string32true&quot;*

**String Templates**

Version ≥ 6

Strings can be created using template literals (*backticks*)
\`hello\`.

**var**

greeting

=

\`Hello\`

;

  
  variable
  

  

With template literals, you can do string interpolation using &dollar;{}
inside template literals:

**var**

place

=

\`World\`

;

**var**

greet

=

\`Hello &dollar;

{

place

}

!

\`

console.

log

(

greet

)

;

*// &quot;Hello World!&quot;*

You can use String.raw to get backslashes to be in the string without
modification.

\`a\\\\b\`

*// = a\\b*

String

.

raw

\`a\\\\b\`

*// = a\\\\b*

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch7-2">Section 7.2: Reverse String</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

The most &quot;popular&quot; way of reversing a string in JavaScript is the
following code fragment, which is quite common:

**function**

reverseString

(

str

)

{

**return**

str.

split

(

&apos;&apos;

)

.

reverse

(

)

.

join

(

&apos;&apos;

)

;

}

reverseString

(

&apos;string&apos;

)

;

*// &quot;gnirts&quot;*

However, this will work only so long as the string being reversed does
not contain surrogate pairs. Astral symbols, i.e. characters outside
of the basic multilingual plane, may be represented by two code units,
and will lead this naive technique to produce wrong results. Moreover,
characters with combining marks (e.g. diaeresis) will appear on the
logical &quot;next&quot; character instead of the original one it was combined
with.

&apos;?????.&apos;

.

split

(

&apos;&apos;

)

.

reverse

(

)

.

join

(

&apos;&apos;

)

;

*//fails*

While the method will work fine for most languages, a truly accurate,
encoding respecting algorithm for string reversal is slightly more
involved. One such implementation is a tiny library called
[Esrever](https://github.com/mathiasbynens/esrever), which uses
regular expressions for matching combining marks and surrogate pairs
in order to perform the reversing perfectly.
>
**Explanation**
>
**Section Explanation Result** str The input string &quot;string&quot;

  
  [String.**prototype**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/split)   
  - -
  [deliminator )](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/split)          

  

  
  [split](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/split)
  

  

  
  &quot;s&quot;     ,   &quot;t&quot;     ,   &quot;r&quot;     ,   &quot;i&quot;     ,   &quot;n&quot;     ,   &quot;g&quot;
            

  

Splits string str into an array. The
>
[.(](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/split)
>
parameter &quot;&quot; means to split between each &lbrack;&rbrack; character.

  
  [Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/reverse)   [.](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/reverse)   [**prototype**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/reverse)   [.](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/reverse)   [reverse](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/reverse)
   - - - -

  

  
  &quot;g&quot;     ,   &quot;n&quot;     ,   &quot;i&quot;     ,   &quot;r&quot;     ,   &quot;t&quot;     ,   &quot;s&quot;
            

  

Returns the array from the split string with

[()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/reverse)
&lbrack;&rbrack;

its elements in reverse order.
>
Joins the elements in the array together into

  -
  [**prototype**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/join)   [.](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/join)   [join](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/join)   [(](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/join)   [deliminator](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/join)
    -  

  -

[Array.](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/join)a
string. The &quot;&quot; parameter means an empty
>
&quot;gnirts&quot;

[)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/join)
deliminator (i.e., the elements of the array

are put right next to each other).
>
**Using spread operator**

Version ≥ 6

**function**

reverseString

(

str

)

{

**return**

&lbrack;

&hellip;

String

(

str

)

&rbrack;

.

reverse

(

)

.

join

(

&apos;&apos;

)

;

}

console.

log

(

reverseString

(

&apos;stackoverflow&apos;

)

)

;

*// &quot;wolfrevokcats&quot;*

console.

log

(

reverseString

(

1337

)

)

;

*// &quot;7331&quot;*

console.

log

(

reverseString

(

&lbrack;

1

,

2

,

3

&rbrack;

)

)

;

*// &quot;3,2,1&quot;*

**Custom**

**e**

**revers**

**(**

**)**

**function**

**function**

reverse

(

string

)

{

**var**

strRev

=

&quot;&quot;

;

**for**

(

**var**

i

=

string.

length

&minus;

1

;

i

&gt;=

0

;

i

\

)

{

strRev

+=

string

&lbrack;

i

&rbrack;

;

}

**return**

strRev

;

}

reverse

(

&quot;zebra&quot;

)

;

*// &quot;arbez&quot;*

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch7-3">Section 7.3: Comparing Strings Lexicographically</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

  
  [localeCompare](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/localeCompare)
  

  

To compare strings alphabetically, use
[()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/localeCompare).
This returns a negative value if the reference string is
lexicographically (alphabetically) before the compared string (the
parameter), a positive value if it comes afterwards, and a value of 0
if they are equal.

**var**

a

=

&quot;hello&quot;

;

**var**

b

=

&quot;world&quot;

;

console.

log

(

a&period;

localeCompare

(

b

)

)

;

*// -1*

  
  localeCompare
  

  

The \and &lt; operators can also be used to compare strings
lexicographically, but they cannot return a value of zero (this can be
tested with the == equality operator). As a result, a form of the ()
function can be written like so:

**function**

strcmp

(

a

,

b

)

{

**if**

(

a

===

b

)

{

**return**

0

;

}

**if**

(

a

&gt;

b

)

{

**return**

1

;

}

**return**

&minus;

1

;

}

console.

log

(

strcmp

(

&quot;hello&quot;

,

&quot;world&quot;

)

)

;

*// -1*

console.

log

(

strcmp

(

&quot;hello&quot;

,

&quot;hello&quot;

)

)

;

*// 0*

console.

log

(

strcmp

(

&quot;world&quot;

,

&quot;hello&quot;

)

)

;

*// 1*

This is especially useful when using a sorting function that compares
based on the sign of the return value (such as sort).

**var**

arr

=

&lbrack;

&quot;bananas&quot;

,

&quot;cranberries&quot;

,

&quot;apples&quot;

&rbrack;

;

arr.

sort

(

**function**

(

a

,

b

)

{

**return**

a&period;

localeCompare

(

b

)

;

}

)

;

console.

log

(

arr

)

;

*// &lbrack; &quot;apples&quot;, &quot;bananas&quot;, &quot;cranberries&quot; &rbrack;*

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch7-4">Section 7.4: Access character at index in string</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

  
  [charAt](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/charAt)
  

  

Use
[()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/charAt)
to get a character at the specified index in the string.

**var**

string

=

&quot;Hello, World!&quot;

;

console.

log

(

string.

charAt

(

4

)

)

;

*// &quot;o&quot;*

Alternatively, because strings can be treated like arrays, use the
index via [bracket
notation](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Property_Accessors).

**var**

string

=

&quot;Hello, World!&quot;

;

console.

log

(

string

&lbrack;

4

&rbrack;

)

;

*// &quot;o&quot;*

  
  [charCodeAt](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/charCodeAt)
  

  

To get the character code of the character at a specified index, use
[()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/charCodeAt).

**var**

string

=

&quot;Hello, World!&quot;

;

console.

log

(

string.

charCodeAt

(

4

)

)

;

*// 111*

Note that these methods are all getter methods (return a value).
Strings in JavaScript are immutable. In other words, none of them can
be used to set a character at a position in the string.

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch7-5">Section 7.5: Escaping quotes</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

If your string is enclosed (i.e.) in single quotes you need to escape
the inner literal quote with *backslash* \\

**var**

text

=

&apos;L

**&amp;amp;apos;**

albero means tree in Italian&apos;

;

console.

log

(

text

)

;

\\\\

&quot;L&apos;albero means tree in Italian&quot;

Same goes for double quotes:

**var**

text

=

&quot;I feel

**&amp;amp;quot;**

high

**&amp;amp;quot;**

&quot;

;

Special attention must be given to escaping quotes if you&apos;re storing
HTML representations within a String, since HTML strings make large
use of quotations i.e. in attributes:
>
**var** content = &quot;&lt;p class=**&amp;amp;quot;**special**&amp;amp;quot;**&gt;Hello
World!&lt;/p&gt;&quot;; *// valid String* **var** hello = &apos;&lt;p
class=&quot;special&quot;&gt;I**&amp;amp;apos;**d like to say &quot;Hi&quot;&lt;/p&gt;&apos;; *// valid
String*

  
  apos   ; (or &#  39   ;) as a single quote and &       quot   ; ( or &#  34
     -  - 

  

Quotes in HTML strings can also be represented using &;) as double
quotes.
>
**var** hi = &quot;&lt;p class=&apos;special&apos;&gt;I&apos;d like to say
&quot;Hi&quot;&lt;/p&gt;&quot;; *// valid String* **var** hello = &apos;&lt;p
class=&quot;special&quot;&gt;I&apos;d like to say &quot;Hi&quot;&lt;/p&gt;&apos;; *// valid
String*

  
  apos                ; and &                         quot
    

  

*Note:* The use of &; will not overwrite double quotes that browsers
can automatically place on

  
  **&lt;p**            **&gt;** being     **&lt;p**   =   &quot;special&quot;   **&gt;**,   quot
  class=special      made to          class                       using &   
  - -   -  

  

attribute quotes. For example ; can lead to

  
  **&lt;p**    =   &quot;&quot;special&quot;&quot;   **&gt;** where &amp;amp;quot;    **&lt;p**    =   &quot;special&quot;
  class                            will be              class          
  -    -  -

  

**&gt;**.

Version ≥ 6

If a string has &apos; and &quot; you may want to consider using template
literals (*also known as template strings in previous ES6 editions*),
which do not require you to escape &apos; and &quot;. These use backticks (\`)
instead of single or double quotes.

**var**

x

=

\`

&quot;Escaping &quot;

and

&apos; can become very annoying\`;

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch7-6">Section 7.6: Word Counter</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

  
  **&lt;textarea**
  

  

Say you have a **&gt;** and you want to retrieve info about the number
of:

Characters (total)

Characters (no spaces)

Words

Lines

**function**

wordCount

(

val

)

{

**var**

wom

=

val.

match

(

*/\\S+/g*

)

;

**return**

{

charactersNoSpaces

:

val.

replace

(

*/\\s+/g*

,

&apos;&apos;

)

.

length

,

characters

:

val.

length

,

words

:

wom

?

wom.

length

:

0

,

lines

:

val.

split

(

*/\\r&ast;\\n/*

)

.

length

}

;

}

*// Use like:*

wordCount

(

someMultilineText

)

.

words

;

*// (Number of words)*

[jsFiddle exampl]{.underline}

[e](http://jsfiddle.net/RokoCB/5nfay7d1/206/)

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch7-7">Section 7.7: Trim whitespace</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

  
  String               .   **prototype**                  .   trim
    -  -

  

To trim whitespace from the edges of a string, use :
>
&quot; some whitespaced string &quot;.trim(); *// &quot;some whitespaced string&quot;*
>
Many JavaScript engines, but [not Internet
Explorer](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/TrimLeft#Browser_compatibility),
have implemented non-standard trimLeft and trimRight methods. There is
a
[proposal](https://github.com/sebmarkbage/ecmascript-string-left-right-trim),
currently at Stage 1 of the process, for standardised trimStart and
trimEnd methods, aliased to trimLeft and trimRight for compatibility.

*// Stage 1 proposal*

&quot; this is me &quot;

.

trimStart

(

)

;

*// &quot;this is me &quot;*

&quot; this is me &quot;

.

trimEnd

(

)

;

*// &quot; this is me&quot;*

*// Non-standard methods, but currently implemented by most engines*

&quot; this is me &quot;

.

trimLeft

(

)

;

*// &quot;this is me &quot;*

&quot; this is me &quot;

.

trimRight

(

)

;

*// &quot; this is me&quot;*

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch7-8">Section 7.8: Splitting a string into an array</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

  
  split
  

  

Use . to go from strings to an array of the split substrings:

**var**

s

=

&quot;one, two, three, four, five&quot;

s&period;

split

(

&quot;, &quot;

)

;

*// &lbrack;&quot;one&quot;, &quot;two&quot;, &quot;three&quot;, &quot;four&quot;, &quot;five&quot;&rbrack;*

  
  join
  

  

Use the **array method** . to go back to a string:

s&period;

split

(

&quot;, &quot;

)

.

join

(

&quot;&amp;quot;

)

;

*// &quot;one\two\three\four\five&quot;*

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch7-9">Section 7.9: Strings are unicode</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

**All JavaScript strings are unicode!**

**var**

s

=

&quot;some

∆

≈

ƒ

unicode

¡

™

£

¢

¢

¢

&quot;

;

s&period;

charCodeAt

(

5

)

;

*// 8710*

There are no raw byte or binary strings in JavaScript. To effectively
handle binary data, use Typed Arrays.

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch7-10">Section 7.10: Detecting a string</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

To detect whether a parameter is a *primitive* string, use **typeof**:

**var**

aString

=

&quot;my string&quot;

;

**var**

anInt

=

5

;

**var**

anObj

=

{

}

;

**typeof**

aString

===

&quot;string&quot;

;

*// true*

**typeof**

anInt

===

&quot;string&quot;

;

*// false*

**typeof**

anObj

===

&quot;string&quot;

;

*// false*

  
  **new** String                      (   &quot;somestr&quot;
    

  

If you ever have a String object, via ), then the above will not work.
In this instance, we can use **instanceof**:

**var**

aStringObj

=

**new**

String

(

&quot;my string&quot;

)

;

aStringObj

**instanceof**

String

;

*// true*

To cover both instances, we can write a simple helper function:

**var**

isString

=

**function**

(

value

)

{

**return**

**typeof**

value

===

&quot;string&quot;

&vert;&vert;

value

**instanceof**

String

;

}

;

**var**

aString

=

&quot;Primitive String&quot;

;

**var**

aStringObj

=

**new**

String

(

&quot;String Object&quot;

)

;

isString

(

aString

)

;

*// true*

isString

(

aStringObj

)

;

*// true*

isString

(

{

}

)

;

*// false*

isString

(

5

)

;

*// false*

Or we can make use of toString function of Object. This can be useful
if we have to check for other types as well say in a switch statement,
as this method supports other datatypes as well just like **typeof**.
>
**var** pString = &quot;Primitive String&quot;;
>
**var** oString = **new** String(&quot;Object Form of String&quot;);
>
Object.**prototype**.toString.call(pString);*//&quot;&lbrack;object String&rbrack;&quot;*
>
Object.**prototype**.toString.call(oString);*//&quot;&lbrack;object String&rbrack;&quot;*
>
A more robust solution is to not *detect* a string at all, rather only
check for what functionality is required. For example:

**var**

aString

=

&quot;Primitive String&quot;

;

*// Generic check for a substring method*

**if**

(

aString.

substring

)

{

}

*// Explicit check for the String substring prototype method*

**if**

(

aString.

substring

===

String

.

**prototype**

.

substring

)

{

aString.

substring

(

0

,

)

;

}

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch7-11">Section 7.11: Substrings with slice</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

  
  slice
  

  

Use .() to extract substrings given two indices:

**var**

s

=

&quot;0123456789abcdefg&quot;

;

s&period;

slice

(

0

,

5

)

;

*// &quot;01234&quot;*

s&period;

slice

(

5

,

6

)

;

*// &quot;5&quot;*

Given one index, it will take from that index to the end of the
string:

s&period;

slice

(

10

)

;

*// &quot;abcdefg&quot;*

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch7-12">Section 7.12: Character code</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

The method charCodeAt retrieves the Unicode character code of a single
character: **var** charCode = &quot;µ&quot;.charCodeAt(); *// The character
code of the letter* µ *is 181*

To get the character code of a character in a string, the 0-based
position of the character is passed as a parameter to charCodeAt:

**var** charCode = &quot;ABCDE&quot;.charCodeAt(3); *// The character code of
&quot;D&quot; is 68*

Version ≥ 6

Some Unicode symbols don&apos;t fit in a single character, and instead
require two UTF-16 surrogate pairs to encode. This is the case of
character codes beyond 216 - 1 or 63553. These extended character
codes or *code point* values can be retrieved with codePointAt:

*// The Grinning Face Emoji has code point 128512 or 0x1F600*

**var**

codePoint

=

&quot;????&quot;

.

codePointAt

(

)

;

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch7-13">Section 7.13: String Representations of Numbers</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

JavaScript has native conversion from *Number* to its *String
representation* for any base from *2 to 36*.
>
The most common representation after *decimal (base 10)* is
*hexadecimal (base 16)*, but the contents of this section work for all
bases in the range.
>
In order to convert a *Number* from decimal (base 10) to its
hexadecimal (base 16) *String representation* the *toString* method
can be used with *radix 16*.

*// base 10 Number*

**var**

b10

=

12

;

*// base 16 String representation*

**var**

b16

=

b10.

toString

(

16

)

;

*// &quot;c&quot;*

If the number represented is an integer, the inverse operation for
this can be done with parseInt and the *radix 16* again

*// base 16 String representation*

**var**

b16

=

&apos;c&apos;

;

*// base 10 Number*

**var**

b10

=

parseInt

(

b16

,

16

)

;

*// 12*

To convert an arbitrary number (i.e. non-integer) from its *String
representation* into a *Number*, the operation must be split into two
parts; the integer part and the fraction part.

Version ≥ 6

**let**

b16

=

&apos;3.243f3e0370cdc&apos;

;

*// Split into integer and fraction parts*

**let**

&lbrack;

i16

,

f16

&rbrack;

=

b16.

split

(

&apos;.&apos;

)

;

*// Calculate base 10 integer part*

**let**

i10

=

parseInt

(

i16

,

16

)

;

*// 3*

*// Calculate the base 10 fraction part*

**let**

f10

=

parseInt

(

f16

,

16

)

/

Math

.

pow

(

16

,

f16.

length

)

;

*// 0.14158999999999988*

*// Put the base 10 parts together to find the Number*

**let**

b10

=

i10

&plus;

f10

;

*// 3.14159*

**Note 1:** Be careful as small errors may be in the result due to
differences in what is possible to be represented in different bases.
It may be desirable to perform some kind of rounding afterwards.
>
**Note 2:** Very long representations of numbers may also result in
errors due to the accuracy and maximum values of *Numbers* of the
environment the conversions are happening in.

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch7-14">Section 7.14: String Find and Replace Functions</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

To search for a string inside a string, there are several functions:

  
  [**indexOf**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/indexOf)   [**(**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/indexOf)   [**searchString**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/indexOf)   **[)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/indexOf)   [**lastIndexOf**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/lastIndexOf)   [**(**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/lastIndexOf)   [**searchString**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/lastIndexOf)
                                                                                                                                                                                                                                                                                                                                                    and**                                                                                                                                                                                                                                                                                                                                            
        

  

[**)**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/lastIndexOf)

  
  indexOf
  

  

() will return the index of the first occurrence of searchString in
the string. If searchString is not found, then -1 is returned.

**var**

string

=

&quot;Hello, World!&quot;

;

console.

log

(

string.

indexOf

(

&quot;o&quot;

)

)

;

*// 4*

console.

log

(

string.

indexOf

(

&quot;foo&quot;

)

)

;

*// -1*

  
  lastIndexOf
  

  

Similarly, () will return the index of the last occurrence of
searchstring or -1 if not found.

**var**

string

=

&quot;Hello, World!&quot;

;

console.

log

(

string.

lastIndexOf

(

&quot;o&quot;

)

)

;

*// 8*

console.

log

(

string.

lastIndexOf

(

&quot;foo&quot;

)

)

;

*// -1*

  
  [**includes**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/includes)   [**(**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/includes)   [**searchString**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/includes)   [**,**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/includes)   [**start**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/includes)
   -  - -

  

[**)**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/includes)

  
  includes
  

  

  
  indexOf
  

  

() will return a boolean that tells whether searchString exists in the
string, starting from index start (defaults to 0). This is better than
() if you simply need to test for existence of a substring.

**var**

string

=

&quot;Hello, World!&quot;

;

console.

log

(

string.

includes

(

&quot;Hello&quot;

)

)

;

*// true*

console.

log

(

string.

includes

(

&quot;foo&quot;

)

)

;

*// false*

  -
  [**replace**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/replace)   [**(**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/replace)   [**regexp**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/replace)   [**&vert;**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/replace)   [**substring**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/replace)   [**,**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/replace)   [**replacement**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/replace)   [**&vert;**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/replace)   [**replaceFunction**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/replace)
    - -   - - 

  -

[**)**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/replace)

  
  replace
  

  

() will return a string that has all occurrences of substrings
matching the
[RegExp](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/RegExp)
regexp or string substring with a string replacement or the returned
value of replaceFunction.
>
Note that this does not modify the string in place, but returns the
string with replacements.

**var**

string

=

&quot;Hello, World!&quot;

;

string

=

string.

replace

(

&quot;Hello&quot;

,

&quot;Bye&quot;

)

;

console.

log

(

string

)

;

*// &quot;Bye, World!&quot;*

string

=

string.

replace

(

*/W.{3}d/g*

,

&quot;Universe&quot;

)

;

console.

log

(

string

)

;

*// &quot;Bye, Universe!&quot;*

replaceFunction can be used for conditional replacements for regular
expression objects (i.e., with use with regexp). The parameters are in
the following order:

**Parameter Meaning**

match the substring that matches the entire regular expressiong g1,
g2, g3, &hellip; the matching groups in the regular expression offset the
offset of the match in the entire string string the entire string
>
Note that all parameters are optional.

**var**

string

=

&quot;heLlo, woRlD!&quot;

;

string

=

string.

replace

(

*/(&lbrack;a-zA-Z&rbrack;)(&lbrack;a-zA-Z&rbrack;+)/g*

,

**function**

(

match

,

g1

,

g2

)

{

**return**

g1.

toUpperCase

(

)

&plus;

g2.

toLowerCase

(

)

;

}

)

;

console.

log

(

string

)

;

*// &quot;Hello, World!&quot;*

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch7-15">Section 7.15: Find the index of a substring inside a string</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

  
  indexOf
  

  

The . method returns the index of a substring inside another string
(if exists, or -1 if otherwise)

&apos;Hellow World&apos;

.

indexOf

(

&apos;Wor&apos;

)

;

*// 7*

  
  indexOf
  

  

. also accepts an additional numeric argument that indicates on what
index should the function start looking

&quot;harr dee harr dee harr&quot;

.

indexOf

(

&quot;dee&quot;

,

10

)

;

*// 14*

  
  indexOf
  

  

You should note that . is case sensitive

&apos;Hellow World&apos;

.

indexOf

(

&apos;WOR&apos;

)

;

*// -1*

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch7-16">Section 7.16: String to Upper Case</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

String.prototype.toUpperCase():

console.

log

(

&apos;qwerty&apos;

.

toUpperCase

(

)

)

;

*// &apos;QWERTY&apos;*

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch7-17">Section 7.17: String to Lower Case</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

String.prototype.toLowerCase()

console.

log

(

&apos;QWERTY&apos;

.

toLowerCase

(

)

)

;

*// &apos;qwerty&apos;*

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch7-18">Section 7.18: Repeat a String</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

Version ≥ 6

This can be done using the
[.repeat()](http://www.ecma-international.org/ecma-262/6.0/#sec-string.prototype.repeat)
method:

&quot;abc&quot;

.

repeat

(

3

)

;

*// Returns &quot;abcabcabc&quot;*

&quot;abc&quot;

.

repeat

(

0

)

;

*// Returns &quot;&quot;*

&quot;abc&quot;

.

repeat

(

&minus;

1

)

;

*// Throws a RangeError*

Version

&lt;

6

In the general case, this should be done using a correct polyfill for
the ES6
[String.prototype.repeat()](http://www.ecma-international.org/ecma-262/6.0/#sec-string.prototype.repeat)
method.

Otherwise, the idiom

**new**

Array

(

n

&plus;

1

)

.

join

(

myString

)

can repeat

n

times the string

myString

:

**var**

myString

=

&quot;abc&quot;

;

**var**

n

=

3

;

**new**

Array

(

n

&plus;

1

)

.

join

(

myString

)

;

*// Returns &quot;abcabcabc&quot;*

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h2 id="ch8">Chapter 8: Date</h2>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

**Parameter Details**

value The number of milliseconds since 1 January 1970 00:00:00.000 UTC
(Unix epoch) dateAsString A date formatted as a string (see examples
for more information)

The year value of the date. Note that month must also be provided, or
the value will be interpreted

year as a number of milliseconds. Also note that values between 0 and
99 have special meaning. See the examples.

  
  11
  

  

The month, in the range 0-. Note that using values outside the specified
range for this and the

month following parameters will not result in an error, but rather
cause the resulting date to &quot;roll over&quot; to the next value. See the
examples.

  
  31
  

  

  
  23
  

  

  
  59
  

  

  
  59
  

  

  
  999
  

  

day Optional: The date, in the range 1-. hour Optional: The hour, in
the range 0-. minute Optional: The minute, in the range 0-. second
Optional: The second, in the range 0-. millisecond Optional: The
millisecond, in the range 0-.

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch8-1">Section 8.1: Create a new Date object</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

  
  Date
  

  

To create a new Date object use the () constructor:
>
**with no arguments**

  
  Date
  

  

() creates a Date instance containing the current time (up to
milliseconds) and date.
>
**with one integer argument**

  
  Date
  

  

  -
  **new** Date                (   749019369738
    -

  -

\(m\) creates a Date instance containing the time and date
corresponding to the Epoch time (1 January, 1970 UTC) plus m
milliseconds. Example: ) gives the date *Sun, 26 Sep 1993 04:56:09
GMT*.
>
**with a string argument**

  
  Date   (   dateString   ) returns the Date object that results after      Date   .   parse
                          parsing dateString with                                      
        -

  

.

**with two or more integer arguments**

  
  Date       (   i1    ,   i2      ,   i3      ,   i4      ,   i5      ,   i6
  -  -  -  -  -  -  -

  

) reads the arguments as year, month, day, hours, minutes, seconds,

  
  **new** Date                                (     2017
   - 

  

milliseconds and instantiates the corresponding Dateobject. Note that
the month is 0-indexed in JavaScript, so 0 means January and 11 means
December. Example: , 5, 1) gives *June 1st, 2017*.
>
**Exploring dates**
>
Note that these examples were generated on a browser in the Central
Time Zone of the US, during Daylight Time,

  
  Date       .   **prototype**            .   toISOString
  -  -  -

  

as evidenced by the code. Where comparison with UTC was instructive,
() was used to show the date and time in UTC (the Z in the formatted
string denotes UTC).
>
*// Creates a Date object with the current date and time from the //
user&apos;s browser* **var** now = **new** Date(); now.toString() ===
&apos;Mon Apr 11 2016 16:10:41 GMT-0500 (Central Daylight Time)&apos; *//
true*
>
*// well, at the time of this writing, anyway*
>
*// Creates a Date object at the Unix Epoch (i.e.,
&apos;1970-01-01T00:00:00.000Z&apos;)* **var** epoch = **new** Date(0);
epoch.toISOString() === &apos;1970-01-01T00:00:00.000Z&apos; *// true*
>
*// Creates a Date object with the date and time 2,012 milliseconds //
after the Unix Epoch (i.e., &apos;1970-01-01T00:00:02.012Z&apos;).* **var** ms
= **new** Date(2012); date2012.toISOString() ===
&apos;1970-01-01T00:00:02.012Z&apos; *// true*
>
*// Creates a Date object with the first day of February of the year
2012 // in the local timezone.* **var** one = **new** Date(2012, 1);
one.toString() === &apos;Wed Feb 01 2012 00:00:00 GMT-0600 (Central
Standard Time)&apos; *// true*
>
*// Creates a Date object with the first day of the year 2012 in the
local // timezone. // (Months are zero-based)* **var** zero = **new**
Date(2012, 0); zero.toString() === &apos;Sun Jan 01 2012 00:00:00 GMT-0600
(Central Standard Time)&apos; *// true*
>
*// Creates a Date object with the first day of the year 2012, in
UTC.* **var** utc = **new** Date(Date.UTC(2012, 0)); utc.toString()
=== &apos;Sat Dec 31 2011 18:00:00 GMT-0600 (Central Standard Time)&apos;
>
*// true* utc.toISOString() === &apos;2012-01-01T00:00:00.000Z&apos;
>
*// true*
>
*// Parses a string into a Date object (ISO 8601 format added in
ECMAScript 5.1) // Implementations should assumed UTC because of ISO
8601 format and Z designation* **var** iso = **new**
Date(&apos;2012-01-01T00:00:00.000Z&apos;); iso.toISOString() ===
&apos;2012-01-01T00:00:00.000Z&apos; *// true*
>
*// Parses a string into a Date object (RFC in JavaScript 1.0)*
**var** local = **new** Date(&apos;Sun, 01 Jan 2012 00:00:00 -0600&apos;);
local.toString() === &apos;Sun Jan 01 2012 00:00:00 GMT-0600 (Central
Standard Time)&apos; *// true*
>
*// Parses a string in no particular format, most of the time. Note
that parsing*
>
*// logic in these cases is very implementation-dependent, and
therefore can vary // across browsers and versions.*
>
**var** anything = **new** Date(&apos;11/12/2012&apos;); anything.toString()
=== &apos;Mon Nov 12 2012 00:00:00 GMT-0600 (Central Standard Time)&apos; *//
true, in Chrome 49 64-bit on Windows 10 in the en-US locale. Other
versions in // other locales may get a different result.*
>
*// Rolls values outside of a specified range to the next value.*
>
**var** rollover = **new** Date(2012, 12, 32, 25, 62, 62, 1023);
rollover.toString() === &apos;Sat Feb 02 2013 02:03:03 GMT-0600 (Central
Standard Time)&apos; *// true; note that the month rolled over to Feb;
first the month rolled over to*
>
*// Jan based on the month 12 (11 being December), then again because
of the day 32 // (January having 31 days).*

*// Special dates for years in the range 0-99*

**var**

special1

=

**new**

Date

(

12

,

0

)

;

special1.

toString

(

)

===

&apos;Mon Jan 01 1912 00:00:00 GMT-0600 (Central Standard Time)\`

// true

// If you actually wanted to set the year to the year 12 CE, you&apos;

d need to use the

*// setFullYear() method:*

special1.

setFullYear

(

12

)

;

special1.

toString

(

)

===

&apos;Sun Jan 01 12 00:00:00 GMT-0600 (Central Standard Time)\`

// true

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch8-2">Section 8.2: Convert to a string format</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

**Convert to String**

**var**

date1

=

**new**

Date

(

)

;

date1.

toString

(

)

;

Returns: &quot;Fri Apr 15 2016 07:48:48 GMT-0400 (Eastern Daylight Time)&quot;

**Convert to Time String**

**var**

date1

=

**new**

Date

(

)

;

date1.

toTimeString

(

)

;

Returns: &quot;07:48:48 GMT-0400 (Eastern Daylight Time)&quot;

**Convert to Date String**

**var**

date1

=

**new**

Date

(

)

;

date1.

toDateString

(

)

;

Returns: &quot;Thu Apr 14 2016&quot;

**Convert to UTC String**

**var**

date1

=

**new**

Date

(

)

;

date1.

toUTCString

(

)

;

Returns: &quot;Fri, 15 Apr 2016 11:48:48 GMT&quot;

**Convert to ISO String**

**var**

date1

=

**new**

Date

(

)

;

date1.

toISOString

(

)

;

Returns: &quot;2016-04-14T23:49:08.596Z&quot;

**Convert to GMT String**

**var**

date1

=

**new**

Date

(

)

;

date1.

toGMTString

(

)

;

Returns: &quot;Thu, 14 Apr 2016 23:49:08 GMT&quot;

This function has been marked as deprecated so some browsers may not
support it in the future. It is suggested to use toUTCString()
instead.

**Convert to Locale Date String**

**var**

date1

=

**new**

Date

(

)

;

date1.

toLocaleDateString

(

)

;

Returns: &quot;4/14/2016&quot;

This function returns a locale sensitive date string based upon the
user&apos;s location by default.

date1.

toLocaleDateString

(

&lbrack;

locales

&lbrack;

,

options

&rbrack;

&rbrack;

)

can be used to provide specific locales but is browser implementation
specific. For example,

date1.

toLocaleDateString

(

&lbrack;

&quot;zh&quot;

,

&quot;en-US&quot;

&rbrack;

)

;

would attempt to print the string in the Chinese locale using United
States English as a fallback. The options parameter can be used to
provide specific formatting. For example:

**var** options = { weekday: &apos;long&apos;, year: &apos;numeric&apos;, month:
&apos;long&apos;, day: &apos;numeric&apos; }; date1.toLocaleDateString(&lbrack;&rbrack;, options);
would result in

&quot;Thursday, April 14, 2016&quot;.

See [the
MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date/toLocaleDateString#Example:_Checking_for_support_for_locales_and_options_arguments)
for more details.

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch8-3">Section 8.3: Creating a Date from UTC</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

By default, a Date object is created as local time. This is not always
desirable, for example when communicating a date between a server and
a client that do not reside in the same timezone. In this scenario,
one doesn&apos;t want to worry about timezones at all until the date needs
to be displayed in local time, if that is even required at all.

**The problem**

In this problem we want to communicate a specific date (day, month,
year) with someone in a different timezone. The first implementation
naively uses local times, which results in wrong results. The second
implementation uses UTC dates to avoid timezones where they are not
needed.

**Naive approach with WRONG results**

**function**

formatDate

(

dayOfWeek

,

day

,

month

,

year

)

{

**var**

daysOfWeek

=

&lbrack;

&quot;Sun&quot;

,

&quot;Mon&quot;

,

&quot;Tue&quot;

,

&quot;Wed&quot;

,

&quot;Thu&quot;

,

&quot;Fri&quot;

,

&quot;Sat&quot;

&rbrack;

;

**var**

months

=

&lbrack;

&quot;Jan&quot;

,

&quot;Feb&quot;

,

&quot;Mar&quot;

,

&quot;Apr&quot;

,

&quot;May&quot;

,

&quot;Jun&quot;

,

&quot;Jul&quot;

,

&quot;Aug&quot;

,

&quot;Sep&quot;

,

&quot;Oct&quot;

,

&quot;Nov&quot;

,

&quot;Dec&quot;

&rbrack;

;

**return**

daysOfWeek

&lbrack;

dayOfWeek

&rbrack;

&plus;

&quot; &quot;

&plus;

months

&lbrack;

month

&rbrack;

&plus;

&quot; &quot;

&plus;

day

&plus;

&quot; &quot;

&plus;

year

;

}

*//Foo lives in a country with timezone GMT + 1*

**var**

birthday

=

**new**

Date

(

2000

,

0

,

1

)

;

console.

log

(

&quot;Foo was born on: &quot;

&plus;

formatDate

(

birthday.

getDay

(

)

,

birthday.

getDate

(

)

,

birthday.

getMonth

(

)

,

birthday.

getFullYear

(

)

)

)

;

sendToBar

(

birthday.

getTime

(

)

)

;

Sample output:

Foo was born on: Sat Jan 1 2000

*//Meanwhile somewhere else&hellip;*

*//Bar lives in a country with timezone GMT - 1*

**var**

birthday

=

**new**

Date

(

receiveFromFoo

(

)

)

;

console.

log

(

&quot;Foo was born on: &quot;

&plus;

formatDate

(

birthday.

getDay

(

)

,

birthday.

getDate

(

)

,

birthday.

getMonth

(

)

,

birthday.

getFullYear

(

)

)

)

;

Sample output:

Foo was born on: Fri Dec 31 1999

And thus, Bar would always believe Foo was born on the last day of
1999.
>
**Correct approach**

**function**

formatDate

(

dayOfWeek

,

day

,

month

,

year

)

{

**var**

daysOfWeek

=

&lbrack;

&quot;Sun&quot;

,

&quot;Mon&quot;

,

&quot;Tue&quot;

,

&quot;Wed&quot;

,

&quot;Thu&quot;

,

&quot;Fri&quot;

,

&quot;Sat&quot;

&rbrack;

;

**var**

months

=

&lbrack;

&quot;Jan&quot;

,

&quot;Feb&quot;

,

&quot;Mar&quot;

,

&quot;Apr&quot;

,

&quot;May&quot;

,

&quot;Jun&quot;

,

&quot;Jul&quot;

,

&quot;Aug&quot;

,

&quot;Sep&quot;

,

&quot;Oct&quot;

,

&quot;Nov&quot;

,

&quot;Dec&quot;

&rbrack;

;

**return**

daysOfWeek

&lbrack;

dayOfWeek

&rbrack;

&plus;

&quot; &quot;

&plus;

months

&lbrack;

month

&rbrack;

&plus;

&quot; &quot;

&plus;

day

&plus;

&quot; &quot;

&plus;

year

;

}

*//Foo lives in a country with timezone GMT + 1*

**var**

birthday

=

**new**

Date

(

Date

.

UTC

(

2000

,

0

,

1

)

)

;

console.

log

(

&quot;Foo was born on: &quot;

&plus;

formatDate

(

birthday.

getUTCDay

(

)

,

birthday.

getUTCDate

(

)

,

birthday.

getUTCMonth

(

)

,

birthday.

getUTCFullYear

(

)

)

)

;

sendToBar

(

birthday.

getTime

(

)

)

;

Sample output:

Foo was born on: Sat Jan 1 2000

*//Meanwhile somewhere else&hellip;*

*//Bar lives in a country with timezone GMT - 1*

**var**

birthday

=

**new**

Date

(

receiveFromFoo

(

)

)

;

console.

log

(

&quot;Foo was born on: &quot;

&plus;

formatDate

(

birthday.

getUTCDay

(

)

,

birthday.

getUTCDate

(

)

,

birthday.

getUTCMonth

(

)

,

birthday.

getUTCFullYear

(

)

)

)

;

Sample output:

Foo was born on: Sat Jan 1 2000

**Creating a Date from UTC**

  
  Date                    .     UTC               (     &hellip;
   -  - 

  

If one wants to create a Date object based on UTC or GMT, the ) method
can be used. It uses the same arguments as the longest Date
constructor. This method will return a number representing the time
that has passed since January 1, 1970, 00:00:00 UTC.

console.

log

(

Date

.

UTC

(

2000

,

0

,

31

,

12

)

)

;

Sample output:

949320000000

**var**

utcDate

=

**new**

Date

(

Date

.

UTC

(

2000

,

0

,

31

,

12

)

)

;

console.

log

(

utcDate

)

;

Sample output:

Mon Jan 31 2000 13:00:00 GMT+0100 (West-Europa (standaardtijd))

Unsurprisingly, the difference between UTC time and local time is, in
fact, the timezone offset converted to milliseconds.

**var**

utcDate

=

**new**

Date

(

Date

.

UTC

(

2000

,

0

,

31

,

12

)

)

;

**var**

localDate

=

**new**

Date

(

2000

,

0

,

31

,

12

)

;

console.

log

(

localDate

&minus;

utcDate

===

utcDate.

getTimezoneOffset

(

)

&ast;

60

&ast;

1000

)

;

Sample output:

**true**

**Changing a Date object**

  
  setDate         (   &hellip;   ) and       setFullYear              (   &hellip;
      -  

  

All Date object modifiers, such as ) have an equivalent takes an
argument in
>
UTC time rather than in local time.

**var**

date

=

**new**

Date

(

)

;

date.

setUTCFullYear

(

2000

,

0

,

31

)

;

date.

setUTCHours

(

12

,

0

,

0

,

0

)

;

console.

log

(

date

)

;

Sample output:

Mon Jan 31 2000 13:00:00 GMT+0100 (West-Europa (standaardtijd))

  -
  setUTCMonth                     (), .       setUTCDate
    

  -

The other UTC-specific modifiers are .() (for the day of the month),

  
  setUTCMinutes    (), . setUTCSeconds    () and .  setUTCMilliseconds
  - - -  

  

.().

**Avoiding ambiguity with getTime() and setTime()**
>
Where the methods above are required to differentiate between
ambiguity in dates, it is usually easier to communicate a date as the
amount of time that has passed since January 1, 1970, 00:00:00 UTC.
This single number represents a single point in time, and can be
converted to local time whenever necessary.

**var**

date

=

**new**

Date

(

Date

.

UTC

(

2000

,

0

,

31

,

12

)

)

;

**var**

timestamp

=

date.

getTime

(

)

;

*//Alternatively*

**var**

timestamp2

=

Date

.

UTC

(

2000

,

0

,

31

,

12

)

;

console.

log

(

timestamp

===

timestamp2

)

;

Sample output:

**true**

*//And when constructing a date from it elsewhere&hellip;*

**var**

otherDate

=

**new**

Date

(

timestamp

)

;

*//Represented as a universal date*

console.

log

(

otherDate.

toUTCString

(

)

)

;

*//Represented as a local date*

console.

log

(

otherDate

)

;

Sample output:

Mon, 31 Jan 2000 12:00:00 GMT

Mon Jan 31 2000 13:00:00 GMT+0100 (West-Europa (standaardtijd))

/code&gt;

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h3 id="ch8-4">Section 8.4: Formatting a JavaScript date</h3>
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

**Formatting a JavaScript date in modern browsers**

  
  [Date](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date/toLocaleDateString)   [.](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date/toLocaleDateString)   [**prototype**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date/toLocaleDateString)   [.](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date/toLocaleDateString)   [toLocaleDateString](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date/toLocaleDateString)
   -  - -

  

In modern browsers (&ast;),
[()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date/toLocaleDateString)
allows you to define the formatting of a Date in a convenient manner.
>
It requires the following format :

dateObj.

toLocaleDateString

(

&lbrack;

locales

&lbrack;

,

options

&rbrack;

&rbrack;

)

The locales parameter should be a string with a BCP 47 language tag,
or an array of such strings.
>
The options parameter should be an object with some or all of the
following properties:
>
**localeMatcher** : possible values are &quot;lookup&quot; and &quot;best fit&quot;;
the default is &quot;best fit&quot; **timeZone** : the only value
implementations must recognize is &quot;UTC&quot;; the default is the
runtime&apos;s default time zone **hour12** :possible values are **true**
and **false**; the default is locale dependent **formatMatcher** :
possible values are &quot;basic&quot; and &quot;best fit&quot;; the default is &quot;best
fit&quot; **weekday** : possible values are &quot;narrow&quot;, &quot;short&quot; &
&quot;long&quot; **era** : possible values are &quot;narrow&quot;, &quot;short&quot; &
&quot;long&quot; **year** : possible values are &quot;numeric&quot; & &quot;2-digit&quot;
**month** : possible values are &quot;numeric&quot;, &quot;2-digit&quot;, &quot;narrow&quot;,
&quot;short&quot; & &quot;long&quot; **day** : possible values are &quot;numeric&quot; &
&quot;2-digit&quot; **hour** : possible values are &quot;numeric&quot; & &quot;2-digit&quot;
**minute** : possible values are &quot;numeric&quot; & &quot;2-digit&quot; **second**
: possible values are &quot;numeric&quot; & &quot;2-digit&quot; **timeZoneName** :
possible values are &quot;short&quot; & &quot;long&quot;
>
**How to use**

**var**

today

=

**new**

