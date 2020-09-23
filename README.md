<div align="center">

## Creating a Cellphone Game/Application


</div>

### Description

Learn how to create a game or application for your cellphone.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[R\. Kistner](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/r-kistner.md)
**Level**          |Beginner
**User Rating**    |4.4 (57 globes from 13 users)
**Compatibility**  |Java \(JDK 1\.2\)
**Category**       |[Miscellaneous](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/miscellaneous__2-57.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/r-kistner-creating-a-cellphone-game-application__2-3066/archive/master.zip)





### Source Code

<style type="text/css"> A { COLOR: blue; TEXT-DECORATION: none } A:active { COLOR: blue; TEXT-DECORATION: underline } A:link { COLOR: blue; TEXT-DECORATION: none } A:visited { COLOR: blue; TEXT-DECORATION: none } A:hover { COLOR: blue; TEXT-DECORATION: underline } BODY { FONT-FAMILY: 'Trebuchet MS', 'comic sans ms', cursive, 'sans serif', serif, monospace } .code { COLOR: black; TEXT-INDENT: 10px } .code .keyword { FONT-WEIGHT: bold; COLOR: #000080 } .code .string { COLOR: #990000 } .code .number { COLOR: #0000ff } .code .comment { COLOR: #008000 } </style>
<center><h1>Creating Cellphone Game or Application</h1></center>
<div align="right"><h3>by Ralf Kistner</h3></div>
<p>To create a game or application for your cellphone, you need the following:</p>
<ul>
<li>Jdk1.3 or higher (http://java.sun.com/j2se/1.4.1/download.html)</li>
<li>J2ME Wireless Toolkit (http://java.sun.com/products/j2mewtoolkit/download-2_0.html)</li>
<li>Any Java IDE or text editor</li>
<li>A java-compatible cellphone (optional)</li>
</ul>
<p><b>Note:</b> This is not a tutorial to teach you Java. You should be confident with Java before reading this tutorial.</p>
<h2>Getting started with J2ME</h2>
<p><b>Step 1: </b>In J2ME Wireless Toolkit, create a new project. Give the project any name you want. Make the class name <i>Main</i>. You don't need to change any of the settings.<br></p>
<p><b>Step 2: </b>Create [J2ME home dir]\apps\[project name]\src\Main.java with the following code:</p>
<p><pre><code class="code">
<span class="keyword">import</span> javax.microedition.midlet.MIDlet;
<span class="keyword">import</span> javax.microedition.lcdui.*;
<span class="keyword">public class</span> Main <span class="keyword">extends</span> MIDlet {
	<span class="keyword">private</span> Form mainForm;
	<span class="keyword">public</span> Main() {
		<span class="comment">//create a new Form with the specified title</span>
		mainForm = new Form(<span class="string">"Hello World"</span>);
		<span class="comment">//append a String to the form</span>
		mainForm.append(<span class="string">"Hello World!"</span>);
	}
	<span class="keyword">public void</span> startApp () {
		<span class="comment">//show the Form in the display area</span>
		Display.getDisplay(<span class="keyword">this</span>).setCurrent(mainForm);
	}
	<span class="keyword">public void</span> destroyApp(boolean b) { }
	<span class="keyword">public void</span> pauseApp() { }
}
</code></pre></p>
<p><b>Step 3: </b>In J2ME, build the project. If you don't get any errors, you can run your program. A frame with a picture of a cellphone should pop up. Click on the button under launch and you should see "Hello World!".</p>
<p>Congratulations! You've just created your own cellphone application!</p>
<p><b>Step 4: </b>To get it on your cellphone, you'll have to create a package (Project-> Package-> Create Package).
See your cellphone's manual for futher instructions on how to put it on your cellphone.</p>

