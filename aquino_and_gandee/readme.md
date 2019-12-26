<!DOCTYPE html>
<html>
<head>
	<!--<title>Front-End Web Development: The Big Nerd Ranch Guide</title>-->
	<link href="https://github.com/skomja00/web/blob/master/github.css">
	<!--<link rel="stylesheet" href="stylesheets/styles.css">-->
	<!--<style>
		term {
			font-family: "Courier New", Courier, monospace;
		}
	</style>-->
</head>
<body>
    <!-- -------------------------------------------------------------------- -->
    <h1>
		Introduction
	</h1>
    Front-end web development is a very different animal from development for other platforms. Front-end technologies have no official developer documentation other than the technical specifications. Keep in mind: <u><i>The browser is a platform.</i></u>
    <!-- -------------------------------------------------------------------- -->
    <h1>
        Chapter 1 Setting Up Your Development Environment
    </h1>
    <h2>
        NetBeans Bundle
    </h2>
        <p>
            Aquino & Gandee use the Atom IDE. I am instead using NetBeans IDE 8.0.2 and Java SE Development Kit 8u191 as a development environment. This section is a collection of my own notes, references, and tips.
        </p>
    <ul>
		<li>
			<term>Node.js</term> (or simply "<term>Node</term>") lets you use programs written in JavaScript from the command line. Most front-end development tools are written for use with <term>Node.js</term>. It provides two command-line programs: 
			<ul>
				<li>
					The <term>node</term> program does the work of running programs written in JavaScript. 
				</li>
				<li>
					The Node Package Manager, <term>npm</term>, is needed for installing open-source development tools from the internet. <term>browser-sync</term> is a JavaScript tool that automatically reloads the browser when you save changes to your code. Install <term>browser-sync</term> using this command at the command line:<br>
					<code>npm install -g browser-sync</code><br>
					Navigate to you project directory, and run the following command to start <term>browser-sync</term>.<br>
					<code>browser-sync start --server --browser "Google Chrome" --files "stylesheets/*.css, *.html"</code>
				</li>
			</ul>
		</li>
		<li>
			Chrome has a really nice javaScript debugging environment. 
		</li>
		<li>
			Firefox may not be your favorite browser, Firefox provides better syntax error checking. When you you right click a page and "View Source", you’ll see syntax errors in red font. So, try using Firefox just until you are sure your HTML and CSS do not have any syntax errors in them. 
		</li>
        <li>NetBeans: To View your HTML page:
            <ul>
                <li>
                    Right click anywhere in the edit area and select "View". NetBeans will open up your index.html in a browser (showing "hello world"). Because you "Viewed" the page, you should see the file name and path in the address bar. 
                <li>
                    I like to View pages when I am working on my CSS, laying out my page, because it is a bit faster than running the page(discussed below).
                </li>
            </ul>
        <li> NetBeans: To Run Your Page: If your page needs the HTTP protocol (for example making AJAX calls), you need to have Apache serve up your web page. To do this, 
            <ul>
                <li>
					Right click anywhere in the editor pane and select Run (not View). The first time you run a page, there is a slight delay while NetBeans deploys your web application.
                </li>
                <li>
					Notice the difference in the URL – it shows localhost as your domain, not just the file name as before when you Viewed your page. 
                </li>
                <li>
					8080 is the port number that the web server uses to listen for web page requests. 
                </li>
            </ul>
        </li>
            <li>NetBeans:  Test That You Will Be Able To Write Web APIs. Later in this course, you will be writing Server Side code that responds to JavaScript requests from your web pages. We will use JSP pages for this. Test that your installation can run JSP pages, so that if there is a problem you have more time to fix it. 
                <ul>
                    <li>
						Right click on the "Web Pages" folder (in the project pane) and select New - JSP 
                    </li>
                    <li>
						You can accept the default file name of "newjsp". Double click newjsp to open it in the editor.
                    </li>
                    <li>
						Run the page by right clicking anywhere in the editor area and selecting Run. If you see newjsp.jsp in the browser’s address bar and “Hello World” displaying, then you have properly installed the NetBeans bundle and you will be able to write Web APIs later in the semester.  
                    </li>				
                </ul>
        </li>
    </ul>
    <!-- -------------------------------------------------------------------- -->
    <h1>
            Chapter 2 Setting Up Your First Project
    </h1>
    <h2>
            Setting Up Ottergram
    </h2>
    <p>There are no rules about how to structure or name your files and folders. However, projects follow some conventions used by many front-end developers.
    </p>
        <ul>
            <li>
				Your <code>index.html</code> file will hold your HTML code. 
            </li>
            <li>
				Your <code>stylesheets</code> folder will hold one or more files with styling information. Give your CSS files names that describe what part of the page or site they pertain to, such as <code>stylesheets/header.css</code> or <code>stylesheets/blog.css</code>. 
            </li>
        </ul>
	<p>Image tags are different from most other element in that they do not wrap other elements, but instead refer to a resource. When the brower encoutners an <code>img</code> tag, it draw the image to the page. This is know as a <i>replaced element</i>. Becuase they do not wrap content or other elements, they do no have a corresponding closing tag. Thie makes them <i>self-closing</i> tags (also known as <i>void</i> tags. You will sometimes see self-closing tags written with a slash before the right angle-bracket, like <code>img src="otter.jpg"/></code>.
    <!-- -------------------------------------------------------------------- -->
    <h1>
		HTML and CSS concepts courtesy of:
	</h1>
    <h2>
		Front-End Web Development: The Big Nerd Ranch Guide
	</h2>
		by Chris Aquino, Todd Gandee<br>
		Copyright © 2016 Big Nerd Ranch, LLC<br>
		<a href="http://www.informit.com/store/front-end-web-development-the-big-nerd-ranch-guide-9780134433943"
			alt"Big Nerd Book>
			http://www.informit.com/store/front-end-web-development-the-big-nerd-ranch-guide-9780134433943
		</a>
	<h2>
		Temple University CIS 3308: Web Application Development
	</h2>
		Sally Kyvernitis Temple University Faculty<br>
		<a href="http://cis-linux2.temple.edu/~sallyk/cis3308/index.php" alt="sallyk">
			http://cis-linux2.temple.edu/~sallyk/cis3308/index.php
		</a>
</body>
</html>
