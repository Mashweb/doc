
---
title: "Demos"
linkTitle: "Demos"
weight: 30
menu:
  main:
    weight: 30
type: docs
---

{{% pageinfo %}}
This is a placeholder page that shows you how to use this template site.
{{% /pageinfo %}}


This section is where the user documentation for your project lives - all the information your users need to understand and successfully use your project. 

For large documentation sets we recommend adding content under the headings in this section, though if some or all of them don’t apply to your project feel free to remove them or add your own. You can see an example of a smaller Docsy documentation site in the [Docsy User Guide](https://docsy.dev/docs/), which lives in the [Docsy theme repo](https://github.com/google/docsy/tree/master/userguide) if you'd like to copy its docs section. 

Other content such as marketing material, case studies, and community updates should live in the [About](/about/) and [Community](/community/) pages.

Find out how to use the Docsy theme in the [Docsy User Guide](https://docsy.dev/docs/). You can learn more about how to organize your documentation (and how we organized this site) in [Organizing Your Content](https://docsy.dev/docs/best-practices/organizing-content/).


## Zen: A New Approach to Authoring the Web
### Web-Page Editing and Web App Development Based upon Direct Manipulation of the DOM and Visual Programming

Version 0.11.10<br />
by Tom Elam<br />
Elam & Associates<br />
Mysuru, India<br />
January 6, 2020

<div class="container">
  <div class="column-group">
    <div class="column docs-content">
      <div class="docs-section">
        <h2 id="Introduction">1. Introduction</h2>
        <p class="lead">This white paper presents a profoundly unique, personalized, and adaptive approach
	    to the creation of web experiences&mdash;a radically new approach usable by a very broad class of people.
	    It links to live prototypes of web-page-editor interfaces to demonstrate that it could be possible
	    for end users to build their own web pages from scratch and decide every detail
	    of their web pages' look and structure simply, easily, and quickly, without any prior learning.
	    The possibilities go far beyond just editing web pages, which this paper also intends to show.
	    The code name for this approach and its implementation (under development) is <em>Zen</em>.
	    The unique selling point (USP) of Zen will be in-context, instant-feedback, <em>full-featured</em> editing
	    of website or web app structure, function, and styling.
	    In particular, Zen will make it easy for users to create any kind of valid HTML structure in web pages
	    without getting into the complexity or distraction of code
	    and will make it easy for them to create basic-level <em>programs</em> using visual-programming
	    principles adopted from successful visual-programming languages for children.
	    Most importantly, all this "development" and its <em>deployment</em> can be continuous,
	    carried on by a <em>website's users</em> of all levels of experience.
	    Since, with Zen, deploying and sharing a new application could be as simple
	    as clicking a <em>Share</em> or <em>Deploy</em> button,
	    self-organizing user communities might develop altogether novel applications.
	</p>
	
	<p>
	    A deliverable of the Zen project will be an example Zen-based
	    web application framework<sup><a href="#1">1</a></sup> comprising the Zen
	    client-side JavaScript library, aka <em>Core Zen</em>, and a liberally licensed server-side framework
	    (possibly Ruby on Rails) augmented with code to store and serve the web pages created and modified by Zen.
	    Even though Core Zen will only have to be loaded once to create an unlimited number of web pages
	    with unique URLs, a strong effort will be made to keep the "time-to-interact" (TTI)
	    delay introduced by Core Zen down to 2&ndash;3 seconds, so that Zen's potential application
	    can be as broad as possible.
	    (TTI is the time it takes from the start of a web page
	    load until the time when the user is comfortable interacting with the web page.)
	    Potentially many other implementations of Zen could be developed
	    to incorporate and integrate Core Zen into
	    web content management systems, wikis, website builders, web frameworks, web portals,
	    web development tools for editing, testing, and debugging code,
	    and integrated development environments (IDEs) for web development.
	    Web services such as Google's Accelerated Mobile Pages (AMP)<sup><a href="#2">2</a></sup>
	    and Google Hosted Libraries<sup><a href="#3">3</a></sup> could broaden Zen's potential.
	</p>

	<p>
	    Many user-programmed systems for customizing websites are described in the book
	    <em>No Code Required: Giving Users Tools to Transform the Web</em>
	    <sup><a href="#4">4</a></sup> but no system for <em>creating</em> web apps.
	    With Zen, many kinds of web apps will be created as simply as are the applications
	    written by children in specially designed visual programming languages.
	    (Specific references to these child-oriented systems are provided later in this paper.)
	</p>

	<p>
	    Though many of the problems of creating end-user programming environments
	    have been overcome to some degree or other,
	    there is one obstacle to it that still has no embeddable (library-based) solution&mdash;as
	    opposed to a framework-based solution.
	    That is a problem that arises from the stateless nature of the Web.
	    To illustrate, we take an example of a typical program that asks a user's name
	    and greets him accordingly:
<pre>
<code>		    
    PRINT "What is your name?"
    INPUT "(Enter your name.)", $name
    PRINT
    PRINT "Hello, "; $name; ", how are you today?"
</code>
</pre>
            The flow of this program is obvious, but even such a simple program must be written on
            a platform that hides complexity:
            it must be halted, waiting for a response.
            This is true no matter what the programming platform is.
            For desktop applications, the operating system provides system calls, a scheduler,
            and library functions that
	    allow program flow to mirror the thread or process of the program, as in the example.
            For web apps there is no underlying operating system to support the halting and restarting
            of the program.
            However, some languages, such as Scheme, support <em>continuations</em>,<sup><a href="#5">5</a></sup>
            which allow programs written in that language to be halted and restarted using
            <em>language-level</em> mechanisms (as opposed to operating-styem system calls and library functions).
            Zen will utilize continuations to simplify the end-user's programming tasks.
	</p>
	
	<p>
	    <div style="display:inline-block; float:right; width:300px;">
		<figure>
		    <a href="http://www.youtube.com/watch?feature=player_embedded&v=3c3Rt6QbHDw#t=12m9s
			     " target="_blank">
			<img style="float:right" src="http://img.youtube.com/vi/3c3Rt6QbHDw/0.jpg" 
			     alt="www.digial-archaelogy.org demo of Nexus" width="240" height="180" border="10">
		    </a><br />
		    <figcaption>
			<small>Figure 1. Demonstration of the editing function of the first web browser.
			    Click to open.</small>
		    </figcaption>
		</figure>
	    </div>
	    Why Zen's new approach is desirable and how it is anticipated to work are the subjects of this whole paper,
	    but a brief video from the Digital Archaeology project<a href="#1"><sup>1</sup></a>
	    showing the operation of the first web browser can provide some background context.
	    The video shows the operation of the first web browser, called Nexus, crafted by the inventor
	    of the World Wide Web himself, Sir Tim Berners-Lee.
	    Twelve minutes and nine seconds into the video, Nexus's editing function is demonstrated (Figure 1).
	    Thus, from the very beginning, Berners-Lee
	    intended the web browser to enable easy collaborative authoring.
	    However, as he himself says, "It didn't really take off that
	    way."<sup><a href="#2">2</a>,
		<a href="#3">3</a>,
		<a href="#4">4</a>
	    </sup>
	</p>

	<p>Now, a quarter of a century later,
	    the position of the A-grade web
	    browsers<sup><a href="#5">5</a>,
		<a href="#6">6</a>,
		<a href="#7">7</a>,
		<a href="#8">8</a>
	    </sup>
	    as the central applications for online sharing seems unshakeable.
	    Yet till today, not one A-grade web browser has full-fledged web-authoring capabilities.
	    (We shall discuss the browser features <em>contentEditable</em> and <em>designMode</em> later,
	    since these do not, without external programming, constitute web-authoring capabilities.)
	    The direct descendents of Berners-Lee's early web-page editing application
	    are visual web-page editors in three broad categories:
	    <ol>
		<li>
		    In-browser rich-text editors.
		    These are web-page-embedded, JavaScript-based, WYSIWYG web-page editors
		    that convert HTML textarea fields or other HTML elements into editor instances.
		    TinyMCE and CKeditor are typical examples.
	</li>
		<li>
		    Standalone WYSIWYG web-page editors that operate on web-page source
		    and show a preview of the resultant web page.
		    Source can be HTML or markup to be translated into HTML.
		</li>
		<li>
		    WYSIWYM semantic web-page editors.
		    Examples of this type of editor are WYMEditor, RDFaCE, BlueprintUI, PageDown, and Showdown.
		    (The author needs to further investigate these editors.)
		    Source can be HTML or markup that can be translated into HTML.
		</li>
	    </ol>
	    Apart from editors that only edit web pages, there are other tools and applications
	    for developing web experiences:
	    <ol>
		<li>
		    online web development tools for testing and debugging code
		    (e.g. JSFiddle.net, CodePen.io, jsbin.com, etc.),
		</li>
		<li>
		    web-developer's tools and "augmented-browsing software"<sup><a href="#9">9</a>,
		    <a href="#10">10</a></sup>
		    (e.g. Firebug for Firefox, Developer Tools for Chrome, Developer Tools for Safari,
		    Greasemonkey, Tampermonkey, Chickenfoot, X-Ray Goggles, etc.),
		</li>
		<li>
		    integrated development environments (IDEs) that build websites,
		</li>
		<li>
		    web content management systems (web CMSs or simply WCMSs),
		</li>
		<li>
		    website builders,
		</li>
		<li>
		    web frameworks, and
		</li>
		<li>
		    web portals.
		</li>
	    </ol>
	</p>

	<h3 id="Contents"><strong>Contents</strong></h3>
	<p>
	    <ol>
		<li><a href="#Introduction">Introduction</a></li>
		<li><a href="#WYSIWYG_Critique">Critique of current WYSIWYG web-page composers</a></li>
		<li><a href="#WYSIWYM_Critique">Critique of current WYSIWYM web-page composers</a></li>
		<li><a href="#Values">Values</a></li>
		<li><a href="#Principles">Principles</a></li>
		<li><a href="#Practices">Practices</a></li>
		<li><a href="#Questions_Ideas">Initial Questions and Ideas for Zen Development</a></li>
		<li><a href="#Diving">Diving Deeper: Zen According to <em>The Elements of User Experience</em></a></li>
		<li><a href="#Name">Encapsulating the Zen Concept in a Domain Name</a></li>
		<li><a href="#Study">For Further Study</a></li>
		<li><a href="#Notes">Notes</a></li>
	    </ol>
	</p>
      </div>
      
      <div class="docs-section">
        <h2 id="WYSIWYG_Critique">2. Critique of current WYSIWYG web-page composers</h2>
        <p>All the well-known WYSIWYG web-page composers, whether standalone or embedded,
	    treat web-page composition like word-processing&mdash;that is, like a layout
	    or 2-D-drawing  problem&mdash;rather than as an organizational
	    (structured, semantic, dynamic-design) problem.
	    Typically visual web-page composers are designed
	    merely to provide a gentle approach to HTML editing,
	    leaving out important aspects like styling based upon semantic meaning;
	    <code>div</code> and <code>span</code> elements; reactive widgets; and dynamic (AJAX-enabled) web pages.
	    They often sport a button to switch to an HTML-source view.
	    Their interfaces are reminiscent of IDEs or RAD tools provided by frameworks
	    used by web-developer frameworks.
	    Indeed, WYSIWYG web-page composers are sometimes included in IDEs.
	    The HTML they produce tends not to be "clean," in the sense that it contains	
	    excess pieces of HTML, and not well-behaved, as explained by Nick Santos.<sup><a href="#9">9</a></sup>
	    The HTML they produce gets dirtier and dirtier as the user makes more and more
	    changes to the web page.
	</p>

	<p>The main problem with web-page-embedded, JavaScript-based editors
	    is that the jobs they are tasked with are extremely difficult and not well supported by web browsers.
	    Piotrek Koszuliński, lead developer of CKEditor, has written
	    a detailed technical explanation<sup><a href="#10">10</a></sup>
	    of why the key browser feature supporting web-page editing&mdash;<code>contentEditable</code>&mdash;is
	    both flawed and indispensable.
	    Some of his points are:
	    <ol>
		<li>It is difficult to force every browser to use <code>&lt;strong&gt;</code> instead of
		    <code>&lt;b&gt;</code> for the <em>bold</em> command.</li>
		<li>It is difficult to force the <em>Enter</em> key to create new paragraphs instead of
		    <code>&lt;br&gt;</code> or <code>&lt;div&gt;</code>.</li>
		<li>Cleaning up pasted code is messy and imperfect.</li>
		<li>As of August, 2015, the selection systems of the Blink and WebKit web browser engines
		    had been broken for eight years.</li>
		<li>APIs and their implementations related to <code>contentEditable</code>
		    "are incomplete and/or inconsistent and buggy."</li>
		<li>Trying to avoid <code>contentEditable</code> uncovers many large difficulties in correctly
		    handling <em>composition events</em> (which allow multiple keystrokes to form an accented letter,
		    a complex Japanese character, or a letter with a diacritic)
		    without breaking editing on an iPad, the keystrokes for jumping over words,
		    shake-to-undo on the iPhone, spell checking, and screen readers.
		<li>Standardizing browser APIs to address all the above issues is an extremely difficult job.</li>
	    </ol>
	</p>

	<p>Nick Santos explains how HTML is not well behaved in WYSIWYG editors.
	    For example, he says, all the forms:
	    <small><pre>&lt;strong&gt;&lt;em&gt;Baggins&lt;/em&gt;&lt;/strong&gt;<br>&lt;em&gt;&lt;strong&gt;Baggins&lt;/strong&gt;&lt;/em&gt;<br>&lt;em&gt;&lt;strong&gt;Bagg&lt;/strong&gt;&lt;strong&gt;ins&lt;/strong&gt;&lt;/em&gt;<br>&lt;em&gt;&lt;strong&gt;Bagg&lt;/strong&gt;&lt;/em&gt;&lt;strong&gt;&lt;em&gt;ins&lt;/em&gt;&lt;/strong&gt;</pre></small>
	    should be treated the same by the WYSIWYG editor.
	    An edit to any of these forms should be treated the same,
	    but, as he says, "For many ContentEditable implementations on the web,
	    some invisible character or empty span tag may slip into the HTML,
	    so that two ContentEditable elements behave totally differently (even though they look the same)."
	</p>
	
	<p>
	    According to Dan Dascalescu,<sup><a href="#11">11</a></sup> in a survey of about 60 in-browser,
	    WYSIWYG editors, only one editor could paste images directly from the clipboard.
	</p>

	<p>Here are screenshots of a few of the many composers in this class,
	    leaving aside the composers tied to heavyweight integrated
	    development environments:
	    <div>
		<figure>
		    <img src="{{site.url}}/images/bluegriffon1_6_french.jpg" alt="BlueGriffon" width="680" height="499"
			 onclick="window.open('{{site.url}}/images/bluegriffon1_6_french.jpg', '_blank');" />
		    <figcaption>
			<small>Figure 2. BlueGriffon. Click to expand in a new window.</small>
		    </figcaption>
		</figure>
	    </div>
	    <div>
		<figure>
		    <img src="{{site.url}}/images/ckeditor.jpg" alt="CKeditor" width="680" height="382"
			 onclick="window.open('{{site.url}}/images/ckeditor.jpg', '_blank');" />
		    <figcaption>
			<small>Figure 3. CKeditor (web-page-embedded). Click to expand in a new window.</small>
		    </figcaption>
		</figure>
	    </div>
	    <div>
		<figure>
		    <img src="{{site.url}}/images/kompozer.png" alt="KompoZer" width="680" height="510"
			 onclick="window.open('{{site.url}}/images/kompozer.png', '_blank');" />
		    <figcaption>
			<small>Figure 4. KompoZer (discontinued). Click to expand in a new window.</small>
		    </figcaption>
		</figure>
	    </div>
	    <div>
		<figure>
		    <img src="{{site.url}}/images/maqetta.png" alt="Maqetta" width="680" height="486"
			 onclick="window.open('{{site.url}}/images/maqetta.png', '_blank');" />
		    <figcaption>
			<small>Figure 5. Maqetta (inactive as of May 2013). Click to expand in a new window.</small>
		    </figcaption>
		</figure>
	    </div>
	    <div>
		<figure>
		    <img src="{{site.url}}/images/tinymce.jpg" alt="TinyMCE" width="680" height="221"
			 onclick="window.open('{{site.url}}/images/tinymce.jpg', '_blank');" />
		    <figcaption>
			<small>Figure 6. TinyMCE (web-page-embedded). Click to expand in a new window.</small>
		    </figcaption>
		</figure>
	    </div>
	</p>

	<div style="margin: 0px 50px 50px; padding:10px; background-color:lightgray;">
	    <h3>Aside</h3>
	    <small>
		Maqetta, although its development is inactive, provides an
		interesting and unique approach to WYSIWYG
		web-page composition, in that it
		<ol>
		    <li>
			supports composition with OpenAjax widgets,
		    </li>
		    <li>
			"allows User Experience Designers (UXD) to perform drag/drop assembly of live UI mockups,"
		    </li>
		    <li>
			includes "deep support for CSS styling (the application includes
			a full CSS parser/modeler),"
		    </li>
		    <li>
			includes "a mechanism for organizing a UI prototype into a series of 'application states'
			(aka 'screens' or 'panels') which allows a UI designer to define interactivity without
			programming," and
		    </li>
		    <li>
			has a code base with "a toolkit-independent architecture that allows for plugging in
			arbitrary widget libraries and CSS themes."
		    </li>
		</ol>
	    </small>
	</div>

      <div class="docs-section">
	<h2 id="WYSIWYM_Critique">3. Critique of current WYSIWYM web-page composers</h2>

	<p><em>[This section is to be expanded to cover a representative set of WYSIWYM composers.]</em>
	</p>
	
	<p>WYMeditor is the best-known WYSIWYM web-page composer.
	    <div>
		<figure>
		    <img src="{{site.url}}/images/WYMeditor.png" alt="WYMeditor" width="680" height="170"
			 onclick="window.open('{{site.url}}/images/WYMeditor.png', '_blank');" />
		    <figcaption>
			<small>Figure 6. WYMeditor. Click to expand in a new window.</small>
		    </figcaption>
		</figure>
	    </div>
	    WYMeditor is tricky to set up and cannot be embedded in a web page.
	    According to the Wikipedia article on WYMeditor,<sup><a href="#12">9</a></sup>
	    "One downside of WYMeditor is that it cannot be used to include JavaScript in the content it edits.
	    Changing this would require eliminating WYMeditor's use of the innerHtml property."
	    Thus, WYMeditor won't work with reactive widgets.
	</p>
      </div>

      <div class="docs-section">
	<h2 id="Values">4. Values</h2>

	<p>The values driving Zen's development are:
	    <ol>
		<li>The creation of novel, beautiful,
		    well-formatted, semantic HTML and CSS should be dead simple.
		</li>
		<li>Amateur web authors should be able to create virtually any kind of page structure
		    and style.
		</li>
		<li>The interface should have a virtually zero learning curve, and zero should really mean zero.
		    Well-known interface metaphors and gestures must be leveraged to the hilt.
		    The "principle of least surprise" should be followed.
		</li>
		<li>The interface for manipulating and creating semantic and presentation structure
		    should not be cluttered with details that could be hidden until needed;
		    the user should be able to drill down to these details.
		    The interface should present two modes:
		    one mode to hide purely structural details so that semantic details can be addressed,
		    and another mode to hide semantic details so that the look and feel of a web page can be addressed.
		</li>
		<li>Meta organization, like the creation of themes, templates, or partials,
		    should not be precluded by the structure of Zen's low-level tools.
		    The creation of these should be empowered, if not directly implemented, by the low-level tools.
		</li>
	    </ol>
	</p>
      </div>

      <div class="docs-section">
        <h2 id="Principles">5. Principles</h2>
        <p class="lead">As pointed out by David Ungar (who pioneered
	    the type of prototypal object system that JavaScript uses),
	    from values arise principles and from principles arise
	    practices.<sup><a href="#13">13</a>, <a href="#14">14</a></sup>
	    We have just explored the <em>values</em> behind the Zen system.
	    Now let's explore the <em>principles</em> of the Zen system.
	    Zen will complement the approach of Lively Kernel,<sup><a href="#15">15</a>, <a href="#16">16</a></sup>
	    which shares Zen's principles 1&ndash;3 as listed below.
	    How much, if any, of Lively Kernel's code it will borrow is yet to be determined.
	    Note, in particular, the following principle 11 of Zen that is different than
	    the principles of Lively Kernel:
	    <ol>
		<li>It will run in any <em>browser</em> without a download and without installation.
		    (Sometime in the future an attempt might be made to make it work in mobile browsers.)
		</li>
		<li>It will be a composition environment, a GUI builder.
		</li>
		<li>It will store its apps as web pages, even new versions of itself.
		</li>
		<li>It will use only the DOM's interfaces and APIs<sup><a href="#17">17</a>, <a href="#18">18</a></sup>
		    for the composition of web pages and web GUIs
		    by element <em>insertion</em>, <em>manipulation</em>, <em>editing</em>,
		    and <em>deletion</em>&mdash;
		    as opposed to <em>drawing</em> objects using SVG or Canvas operations.
		</li>
		<li>Zen will not provide IDEs, but instead will
		    allow objects in its compositions to be inspected and edited
		    via a Squeak<sup><a href="#19">19</a></sup>-like object inspector.
		    Zen will allow its simple programs to be inspected and edited
		    in a normally hidden visual programming environment, using
		    HTML elements like DIV to model nodes in the program's abstract syntax tree
		    (AST).<sup><a href="#20">20</a></sup>
		    Zen will enable these program nodes or blocks to be copied, pasted, and rearranged,
		    just like the normally visible parts of a Zen web page.
		</li>
		<li>It will enable its users to easily compose sequential programs, that is,
		    programs that can wait for external, asynchronous events such as user input or I/O.
		    This will be accomplished by instantiating <em>true continuations</em>
		    in an interpretter running on top of JavaScript in the web browser. (See below.)
		</li>
		<li>It will exist as a library that can be loaded into any web page to provide
		    the page with Zen's capabilities,
		    although caution will be required to ensure compatibility.
		</li>
		<li>It will <em>complement</em>, <em>augment</em>, and <em>interact</em>
		    with existing web-page editors and website builders, not replace them.
		</li>
		<li>It will allow the Zen-editing of a web page to be locked,
		    leaving intact the form and behavior it built inside the web page.
		</li>
		<li>Zen will not add more than 1&ndash;3 seconds to the TTI (time to interact)
		    for a web page.
		</li>
		<li>Zen will not follow Lively Kernel's principle
		    of implementing a scene graph.<sup><a href="#15">15</a></sup>
		    Instead, it will honor the CSS2 visual formatting model<sup><a href="#21">21</a></sup>
		    in its modeling of a document in a web browser.
		    Zen will not be able use SVG or Canvas graphics for the creation of objects,
		    except where particular Zen-composed apps borrow the pertinent capabilities
		    from other software systems.
		</li>
	    </ol>
	</p>
      </div>

      <div class="docs-section">
	<h2 id="Practices">6. Practices</h2>
	  
	<h3>Zen vs. current WYSIWYG and WYSIWYM web-page composers</h3>

	<p>We have explored the <em>values</em> and <em>principles</em> behind the creation of the Zen system.
	    Now let's explore some of the <em>practices</em> to be followed in Zen's creation.
	</p>

	<p>Present-day WYSIWYG and WYSIWYM web-page composers immediately confront the user with
	    web-page structure details, requiring the user to prematurely optimize his web page.
	    With these composers, the web-page under construction is dominated by
	    a pallette of HTML elements with which the user can "paint" a web page.
	    Some of these composers offer the user a view of the web page
	    that is strewn with icons representing HTML elements.
	</p>

	<p>Zen will take a different approach.
	    In Zen, HTML elements making up the web page will represent themselves at the top-level view,
	    with all the obscurity of detail that implies, but when Zen's <em>node browser</em> is open,
	    Zen will be show a view of the web page with all borders and margins styled in such a way
	    that, to the extent possible, all <em>block boxes</em>, <em>inline boxes</em>,
	    and <em>inline-block boxes</em><sup><a href="#21">21</a></sup> are visible (Figure 7).
	    <div>
		<figure>
		    <img src="{{site.url}}/images/node-browser-cropped.png" 
			 alt="Node-Browser Prototype" width="643" height="345"
			 onclick="window.open('/zen/experiments/NodeLists/node-browser.html', '_blank');" />
		    <figcaption>
			<small>Figure 7. Screenshot of a node-browser prototype.
			    Click to open the live demo in a new window.</small>
		    </figcaption>
		</figure>
	    </div>
	</p>
	
	<p>
	    (Other display styles besides <em>block</em>, <em>inline</em>, and <em>inline-block</em>
	    will be modeled by Zen in a subsequent release.)
	    Zen will provide whatever kinds of object-browsers are necessary to unobscure details
	    of the page-as-an-object.
	    Although the details have not yet been worked out, hope and inspiration are provided by the
	    <a href="https://developer.mozilla.org/en/docs/Tools/3D_View" target="_blank">3D View tool</a>,
	    and by the
	    <a href="https://addons.mozilla.org/en-US/firefox/addon/tilt/" target="_blank">Tilt 3D add-on</a>,
	    for the Firefox browser (Figure 8).

	    <div>
		<figure>
		    <img src="https://developer.mozilla.org/en-US/docs/Tools/3D_View/3dview.png"
			 alt="3D View for Firefox 46 Developer Tools" width="1000" height="350"
			 onclick="window.open('https://developer.mozilla.org/en-US/docs/Tools/3D_View/3dview.png', '_blank');" />
		    <img src="https://wiki.mozilla.org/images/5/5f/Tilt.png"
			 alt="Tilt 3D Add-on for Firefox" width="640" height="390"
			 onclick="window.open('https://wiki.mozilla.org/images/5/5f/Tilt.png', '_blank');" />
		    <figcaption>
			<small>Figure 8. Screenshots of the Fireox 3D View tool for
			    Firefox versions prior to Firefox 47 and
			    the Tilt 3D Add-on for Firefox.
			    (These screenshots are not meant to represent the paradigm that Zen will use.)
			    Click each to expand it in a new window.</small>
		    </figcaption>
		</figure>
	    </div>

	</p>

	<p>The user will be able to select any node that can be the target of a mouse event.
	    In node-selection mode, passing the mouse pointer over nodes will highlight them one at a time (Figure 9).
	    <div>
		<figure>
		    <img src="{{site.url}}/images/layout-manipulator.gif" 
			 alt="Layout-Manipulator Prototype" width="720" height="516"
			 onclick="window.open('{{site.url}}/experiments/NodeLists/blocks+inlines.html', '_blank');" />
		    <figcaption>
			<small>Figure 9. Layout-manipulator prototype.
			    Click to open the live demo in a new window.</small>
		    </figcaption>
		</figure>
	    </div>
	</p>
	
	<p>When the user wants to add an HTML element to his web page,
	    Zen will first present a choice of block, inline, and inline-block box types,
	    because in Zen's paradighm, the visual behavior of a box is mainly determined
	    by its display sytle, not by HTML tag type.
	    This is demonstrated by the <a href="www.w3schools.com">w3schools.com's</a>
	    "Tryit Editor" page for converting <code>&lt;li&gt;</code> HTML elements into a
	    <a href="http://www.w3schools.com/css/tryit.asp?filename=trycss_navbar_horizontal">horizontal
		navigation bar</a>.
	    Using Zen's paradigm, with virtually zero learning, the user could intuitively mock up a web page
	    using only <em>block</em>, <em>inline</em>, and <em>inline-block</em> boxes,
	    and convert it piece by piece into semantic markup.
	    Or he could set the HTML element tag of each element immediately when adding
	    it to the web page.
	</p>

	<p>Zen will allow the user to inspect and manipulate these boxes in a way pioneered and developed by
	    Smalltalk and Smalltalk variants, using inspectors and browsers to inspect live web-page objects.
	    For a relatively gentle introduction to Smalltalk-style inspectors and browsers,
	    see Cincom Smalltalk's tutorials (Figures 10 and 11).
	    The specific HTML tag of an HTML element will be a detail to be drilled down to
	    rather than a primary detail of interest.
	    <div>
		<figure>
		    <a href="http://www.youtube.com/watch?feature=player_embedded&v=N55hT-abBaA" target="_blank">
			<img src="http://img.youtube.com/vi/N55hT-abBaA/0.jpg" 
			     alt="Cincom Smalltalk Inspector Tool overview tutorial" width="720" height="480" border="10" /></a>
		    <figcaption>
			<small>Figure 10. Cincom Smalltalk Inspector Tool overview tutorial video.
			    Click to open in a new window.</small>
		    </figcaption>
		</figure>

		<figure>
		    <a href="http://www.youtube.com/watch?feature=player_embedded&v=8Y9vOGSEm14" target="_blank">
			<img src="http://img.youtube.com/vi/8Y9vOGSEm14/0.jpg" 
			     alt="Cincom Smalltalk System Browser tutorial" width="720" height="480" border="10" /></a>
		    <figcaption>
			<small>Figure 11. Cincom Smalltalk System Browser tutorial video.
			    Click to open in a new window.</small>
		    </figcaption>
		</figure>
	    </div>
	    In addition to formal inspectors and browsers, Zen will allow simple operations like stretching
	    the width or height of an HTML element by grabbing an element's edge or corner and moving
	    the mouse.
	</p>

	<p>Zen will take an embedded, instant-feedback, hybrid WYSIWYM-WYSIWYG (not "pure" WYSIWYG) approach
	    to pull the authoring of novel, Semantic-Web applications
	    out of the exclusive province of programmer-specialists and put it into the hands of
	    amateurs and dilettantes (in the original, non-pejorative sense of the words).
	    The Zen project will primarily focus upon working with
	    the "purest" web technologies&mdash;HTML and CSS&mdash;rather than backend technologies
	    like web servers and web frameworks, because the back-end web framework or web server is opaque
	    to JavaScript running in the web page.
	    That is, the JavaScript running in the page has no way to affect the operation
	    of the back end unless specific arrangements have been made for it.
	    Zen will work by providing updates to web-page source in some format.
	    Where web-page source is persisted and how it is used to generate the web page
	    Zen is embedded in will not be the concern of Zen,
	    though a reference implementation for that will be developed along with Zen.
	</p>

	<p>In spite of these strict limitations, Zen as a building block for web servers
	    and web frameworks is anticipated to be a game-changing addition to present-day
	    website and web-app techniques.
	    In some cases, Zen might even be developed to itself reflect changes
	    to content, structure, and style back to sources, using a bit of code on the back end
	    (i.e. on the web server).
	    Perhaps, for example, in WebDAV-enabled websites&mdash;Zen
	    could relatively easily be leveraged to rewrite web-page source, including stylesheets.
	    On the other hand, using Zen only as a low-level, embedded, solid building block, it should be possible
	    to augment web frameworks of many types to achieve a new, higher level
	    of interactivity and customization in web applications.
	</p>

	<p>None of the well-known WYSIWYG and WYSIWYM page editors directly support
	    the creation of web applications.
	    The most radical aspect of Zen will be that it will allow simple, sequential
	    programs to be created and edited using a block representation of the program's
	    abstract syntax tree (AST),<sup><a href="#20">20</a></sup>
	    where blocks can be moved around using the same
	    user interface Zen will provide for moving web page elements, with minimal modifications.
	    Zen will accomplish this unusual feat by implementing a version of Scheme language
	    in JavaScript, along with <em>true continuations</em>,<sup><a href="#22">22</a></sup>
	    various supporting functions written in JavaScript, and some resources like icons.
	    The author has already used such continuations to string together JavaScript event
	    handlers to create a small sequential program without resorting to callbacks,
	    continuatinon-passing style, promises, or state machines.
	    Scratch and Snap! (formerly called BYOB) <em>[citations to be added]</em>
	    demonstrate that even young children
	    can program using a cleverly designed visual programming language (Figure 12).
	    <div style="margin-left:20px; display:inline-block;">
		<figure>
		    <img align="right" src="{{site.url}}/images/snap.png" width="720" height="371"
			 alt="Snap! Visual Programming Language"
			 onclick="window.open('{{site.url}}/images/snap.png', '_blank');" />
		    <figcaption>
			<small>Figure 12. The Snap! visual programming language.
			    Click to open in a new window.</small>
		    </figcaption>
		</figure>
	    </div>
	</p>
	
        <h3>Zen vs. Website Builders</h3>
        <p>It is important to characterize and visualize how Zen will be different from
	    "website builders" and WCMSs like Wix.com and Weebly.com.
	    In contrast to such WCMSs, which prescribe construction methods at the level of
	    business type, templates, plugins, modules, fonts, etc.,
	    Zen will give the user ultimate control of detail at the element/node/NodeList level of web pages.
	    Zen will allow a DOM node to be grabbed and "dragged" to different positions
	    in its containing NodeList because this is the simplest metaphor for that operation.
	    Drag-and-drop is a classic feature of direct-manipulation interfaces (DMIs)
	    and this metaphor of "moving" an HTML element or node is so compelling that we have to look at the code
	    to see that the element has not moved in terms of x and y coordianates, but rather in terms
	    of its cardinal position in a NodeList.
	    Zen will allow a DOM node to be "cut and pasted" to any valid position in the DOM&mdash;an
	    interaction between multiple NodeLists.
	    An HTML element's style has four possible, well-supported values for its <em>display</em> property:
	    <em>block</em>, <em>inline</em>, <em>inline-block</em>, and <em>none</em>.
	    Live demo code to implement GUIs to rearrange element positions in the NodeLists
	    of the first three of these display styles is located on the author's GitHub Pages
	    <a href="/zen/experiments/NodeLists/block.html">here</a>,
	    <a href="/zen/experiments/layouts/blocks+inlines.html">here</a>, and
	    <a href="/zen/experiments/NodeLists/inline.html">here</a>.
	    (Right-click on the links to open the pages in new tabs or windows.)
	    The method of sliding elements in these prototype GUIs was partly inspired by the 15 Puzzle
	    and JavaScript-based implementations of the 15 Puzzle.
	    There are <a href="/zen/experiments/NodeLists/15-puzzle.html">notes</a>
	    about some of these implementations on this website.
	    Below is a screen capture of Jamie Wong's AI-based
	    automated 15-Puzzle solver, which is written solely in JavaScript, HTML, and CSS
	    (Figure 13).
	    <div style="margin-left:20px; display:inline-block;">
		<figure>
		    <img align="right" src="{{site.url}}/images/15-puzzle.gif" alt="Jamie Wong's 15-Puzzle Solver">
		    <figcaption>
			<small>Figure 13. Jamie Wong's 15-Puzzle solver.</small>
		    </figcaption>
		</figure>
	    </div>
	</p>

	<p>
	    Presently, the customization of templates, plugins, and modules for website builders and web CMSs
	    and the creation of novel comment systems, forums, wikis, and presently unimagined
	    communication systems are far outside the bounds of casual web authorship.
	</p>

        <h3>Concessions to Usability</h3>
	<p>Some concessions to manipulability are necessary so that Zen can successfully edit all webpages.
	    When HTML elements are grabbed 
	    Zen should temporarily apply suitable styles to HTML elements like high-contrast borders
	    to make them visible during element selection.
	    When the display-style property of an HTML element is <em>none</em>,
	    Zen should make it possible for users to temporarily set it to another value so the element can be seen.
	    Likewise, wherever desired,
	    Zen should employ similar tactics to make all elements visible and manipulable,
	    whether they are too small; too big; too transparent; or animated.
	    Zen should employ intuitive, adaptive, custom cursors with contrast and distinctive patterns
	    that show up with whatever colors are behind them.
	    The animations in Figures 14 and 15 are actual screen recordings of rough-prototype GUIs
	    for rearranging NodeLists that contain just <em>blocks</em> or just <em>inlines</em>, respectively:
	    <div>
		<figure>
		    <img src="{{site.url}}/images/block-demo.gif"
			 alt="Block-Manipulator Prototype" width="188" height="564"
			 onclick="window.open('/zen/experiments/NodeLists/block.html', '_blank');" />
		    <figcaption>
			<small>Figure 14. Block-manipulator prototype.
			    Click to open the live demo in a new window.</small>
		    </figcaption>
		</figure>
		<figure>
		    <img src="{{site.url}}/images/inline-demo.gif"
			 alt="Inline-Manipulator Prototype" width="720" height="304"
			 onclick="window.open('/zen/experiments/NodeLists/inline.html', '_blank');" />
		    <figcaption>
			<small>Figure 15. Inline-manipulator prototype.
			    Click to open the live demo in a new window.</small>
		    </figcaption>
		</figure>
	    </div>
	    (The operations of the <em>inline-blocks</em> and <em>inlines</em> demo-GUIs look identical,
	    so just one is shown.)
	    Zen's drag-and-drop and cut-and-paste by themselves would get overly tedious and repetitive,
	    but eventually compound operations could be automated using Zen's visual programming environment
	    and leveraged by support and readymade functions
	    provided by a highly networked community built for Zen programmers and users.
	</p>

	<h3>Scope of the Issues Zen Will Address</h3>
        <p><em>[This section needs a complete overhaul. Possibly the spectrum analogy should be taken out.]</em></p>

	<p>We must determine the scope of the issues Zen will address, which appears to be huge.
	    Zen is meant to offer a uniquely democratizing way of creating web experiences
	    by avoiding code and instead allowing a Zen user a way to directly manipulate every parameter of his
	    web page to which a metaphor can be applied: block elements can be resized
	    by grabbing their edges; block, inline, and inline-block elements can be grabbed
	    and rearranged; etc.
	    Every time the user changes an aspect of style via Zen,
	    Zen will optionally apply the change to the memory-resident stylesheet
	    holding the previous value of that style or to a new memory-resident stylesheet
	    specific to the element selected for the style.
	    Other options, such as applying the change to a selector chosen or created by Zen, will be offered
	    (to be determined).
	</p>

        <p>
	    This approach is unique in its direct change at the canvas level and in its propagation of changes
	    backward to page source.
	    (See, however, <a href="https://gingkoapp.com/hybrid-dom-editors.html">Hybrid HTML/DOM Editors</a>.)
	    Nowdays the creation of web experiences is managed by a galaxy of software packages
	    and services, JavaScript libraries, and CSS libraries,
	    but by viewing this galaxy through the prism of the question
	    "What level of detail does the package or service address,"
	    each package and service can be tentatively placed somewhere along a spectrum.
	    <em>[An image is to be included here.]</em>
	    At one end of the spectrum, users or developers deal directly with HTML, CSS, and images,
	    crafting the details of web pages individually,
	    with no further abstraction or intermediation.
	    At the other end of the spectrum, users or developers have at their disposal
	    many abstractions and are coaxed or prodded into dealing with higher-level
	    concerns like minimization of web assets, quick development,
	    responsive design, patterns, standards, metaphors, and affordances.
	    There are problems with this oversimplification, of course, and some packages
	    and services should appear more as a blob
	    rather than as a single point on the spectrum,
	    but the metaphor of a spectrum enables us to filter an unmanageably long list of
	    web technologies so we can concentrate on comparing like with like.
	    Towards one end of the spectrum (the brass-tacks end) is an enormous set of front-end
	    (JavaScript and CSS libraries and toolkits) and back-end (web servers with CGI capabilities),
	    purely for hand-coded website creation, serving, and management,
	    including the management of website-triggered ancilary services like email and payments.
	    Let us call this the "Red End" of the web software and services spectrum.
	    It allows the web developer complete control of his website
	    at the expense of getting his hands very dirty.
	    Right at the Red End, he directly controls every character
	    of his every web page and, if applicable, every table and query
	    definition in his back-end database.
	    A developer working slightly removed from the extreme Red End
	    probably engages with templates, themes, and skins.
	    He might also use plugins.
	    Anywhere close to the Red End or right at the Red End,
	    the developer might use a content management system (CMS)
	    or blog software to create a database-driven dynamic website
	    or a static website (such as Moveable Type used to generate).
	</p>

	<p>The Red End originally comprised just text editors, web servers, and web browsers
	    and was designed and built to use a stateless protocol for transporting hypertext documents.
	    The web was later retrofitted with mobile scripting languages Java and JavaScript
	    to create a platform for distributed applications.
	    Web servers eventually developed sufficiently to support collaborative authoring applications.
	    One cycle of development was thus completed, bringing the web back around
	    to Berner-Lee's original dream of collaborative authoring, but
	    Berners-Lee's original vision of a simple, easy, collaborative authoring tool for everyone
	    lost out to the current ad hoc<sup><a href="#23">23</a></sup> proliferation of non-standard,
	    anonymous, front-end tools.<sup><a href="#24">24</a></sup>
	    These anonymous tools typically do not offer web-technology dilettantes and web power-users
	    the facility to add nested structure to HTML; to add JavaScript-backed widgets like
	    AngularJS, Dojo, ExtJS, jQuery UI, or web-component widgets; to add web forms;
	    to develop CSS class hierarchies and frameworks; or even to collaborate in a structured way.
	    The Red End for nontechnical people can usually only
	    create flat, static layouts of single pages,
	    not complicated, dynamic structures, and it often emphasizes
	    a code view of web pages (raw HTML and CSS) as much as a WYSIWYG view of pages.
	    Thus the Red End for nontechnical people is not very powerful and often is hard to use.
	    Meanwhile, on the back end, control of the web frameworks is mostly left up to
	    programmer-specialists.
	</p>

        <p>Nowdays many web applications are built inside walled gardens.
	    Even IDEs like Eclipse, IntelliJ IDEA, NetBeans are in at least a small sense walled gardens
	    because they impose their own formatting upon source-code files.
	    Many amateur and professional developers do web development using
	    rigid software web application servers that sell for hundreds of thousands of dollars,
	    such as IBM WebSphere Application Server and Red Hat JBoss.
	    Developers who use such application servers often deal with rigidly defined software modules
	    rather than more basic APIs like RDBMS queries and JavaScript library APIs.
	    Nowdays most online collaboration by nontechnical people does not involve
	    the restructuring of web pages or websites.
	    Instead, it only involves the insertion of data, such as blog or forum posts,
	    into databases, to be queried later.
	    This is a very strict limitation.
	    Let us call web application servers and web services the "Violet End"
	    of the web-development level-of-detail spectrum.
	    It is imminently possible to imagine highly flexible, desktop-app-inspired
	    table, form, query, and report design being built into the Violet End,
	    but such capabilities are not common.
	    Nontechnical people are offered very few simple ways to <em>program</em> websites.
	    The latest and greatest "web experience management" software and services promise
	    to bundle all that is needed to handle ... <em>[to be filled in later]</em>.
	    Given the vastness of the field and the inconceivability of a way to integrate all such facilities,
	    they end up with only the appeal of preserved and prepackaged frozen meals.
	    Furthermore, although there are hundreds or thousands of useful web services that can be tapped,
	    very often for free, specialist programming is necessary to use them.
	</p>

	<p>
	    There are many difficulties or problems in implementing simple ideas on the Web
	    due to complexities at the Red End and the leaky abstractions at the Violet End.
	    First we shall list just a few of those problems&mdash;not in a very systematic way,
	    but almost like a small collection
	    of anecdotes. After creating an initial small list of problems, we shall take an initial, inadequate stab
	    at listing a set of "solutions". After this first, inadequate attempt,
	    we shall delineate the method we are adopting
	    to conquer them with a set of technologies I have loosely been calling "Zen".
	    Finally, we shall attempt to discover a systematic way of cataloging problems with the Web experience
	    so that functional specifications can be created for software layers and modules
	    to improve the Web experience systematically.
	</p>

        <p>
	    <strong>Problem #1: Paucity of means for nontechnical people to author Web documents and websites.</strong>
	    One of the biggest problems or shortcomings of current web browsers is their lack of authoring
	    facilities.
	</p>

	<p>
	    <strong>Problem #2: No utility for Web copy/cut/paste/mashup.</strong>
	    To effectively manage the tremendous load of linked information raining down on him, the Web user
	    should have a robust <em>utility</em> for managing hypermedia in the native environment in which he
	    encounters that hypermedia&mdash;the Web environment. A utility built upon the Web can have features that a
	    desktop utility cannot have, foremost of which are instantaneous change and ubiquitous access.
	    The Web user should have high-quality, proven Web user interface shortcuts most appropriate to manipulating
	    information from the Web&mdash;for example, the "Rich Interaction" patterns described in the Yahoo Design
	    Pattern Library&mdash;so he can quickly clip, mash together, and rearrange information from the Web.
	    This interface must interwork with any A-grade web browser.
	    Incomplete, specialized, "opinionated" services, such as EverNote and Instapaper, do not support the ad hoc
	    creation of drawers, panels, and dialogs, which are necessary to cut, paste,
	    transclude<sup><a href="#25">25</a></sup>,
	    organize, associate, link, tag, and hide blocks of information. This problem is inherently related to
	    <strong>Problem #1</strong>, but it is also
	    related to various Web standards, such as the X-Frame-Options standard.<sup><a href="#26">26</a></sup>
	</p>

	<p>
	    <strong>Problem #3: Limits to the ability to remember paths through the hypermedia sphere.</strong>
	    In 2016, decades after the invention of virtual memory, web browsers still can't get enough memory,
	    causing themselves and their host operating systems to malfunction, to crash, or to function poorly.
	    Never mind the waste of the Web user's time.
	    When the "too many tabs" problem forces the user to close tabs, or causes the browser to slow to a crawl,
	    or crashes the browser, the reminders to the user about how he discovered the Web pages he visited get lost.
	    This is a travesty because many of the user's research insights are won by a hard, painful, lengthy
	    search.<sup><a href="#27">27</a></sup> For now, the problem can only be somewhat ameliorated
	    by adopting rare, non-free tools, such as the Tabs Outliner plugin for the Chrome web
	    browser.<sup><a href="#28">28</a></sup>
	    The right juxtaposition, encapsulation, and highlighting of blocks of information would make
	    it unnecessary to keep open many browser tabs at once and would make it possible to record the user's path
	    through the hypermedia sphere. To make these kinds of arrangement easy,
	    a new <em>utility</em> is necessary.
	</p>

	<p>
	    <strong>Problem #4: Bookmark managers inbuilt to web browsers are inadequate for their main
		purpose.</strong>
	    They are too slow to respond to user input.
	    Furthermore, they do not have even the most basic, useful organizational utilities&mdash;
	    for example, an interface, such as the desktop's drag-and-drop interface for folders and files,
	    or automatic Web-page-content indexing and retrieval based upon content.
	    Many web services that analyze websites could be proxied automatically by the Web browser:
	    services such as Alexa.com (formerly providing free information), the WHOIS service,
	    and Yahoo's free web service that provides semantic analysis of a website and provides a description of that
	    website.<sup><a href="#29">29</a></sup>
	    Inbuilt bookmark managers are tied to a particular web browser, which forces dependency upon the
	    user&mdash;not a good thing.
	</p>

	<p>
	    <strong>Problem #5: Lack of personal ownership of bookmarks.</strong> Web services such as Xmarks,
	    which archive a user's bookmarks, force the user to give up
	    ultimate responsibility for his own bookmarks and put the bookmarks
	    into the hands of a company or organisation that could
	    go out of existence or suspend
	    services.<sup><a href="#30">30</a>, <a href="#31">31</a>, <a href="#32">32</a></sup>
	    Xmarks was even made unavailable for awhile in India by court order.<sup><a href="#33">33</a></sup>
	    In the last few years there has been panic<sup><a href="#34">34</a>, <a href="#35">35</a></sup> and
	    uncertainty<sup><a href="#36">36</a>, <a href="#37">37</a></sup>
	    surrounding the spate of security breaches by web services that have revealed clients' sensitive data,
	    such as usernames, passwords, and credit-card
	    credentials.<sup><a href="#38">38</a>, <a href="#39">39</a></sup>
	    There should be a utility to make a Web user's bookmarks
	    available <em>offline</em> and/or on the user's <em>own</em> website.
	</p>

	<p>
	    <strong>Problem #6: There is no universally available bookmark file facility.</strong> Online collaboration
	    is not supported by good integration of bookmark files with the OS desktop.
	    For example, on a Mac, dragging a URL from Safari's address bar
	    to the desktop creates a file with type "webloc" that MS Windows does not understand by default.
	    It is possible to create a file with type "url" that Windows, Mac, and Ubuntu all understand, but this is
	    not currently happening.
	</p>
      </div>

      <div class="docs-section">
	<h2 id="Questions_Ideas">7. Initial Questions and Ideas for Zen Development</h2>

	<p>Now we shall make our first foray into describing Zen.
	    How do we propose to solve the problems listed in "Introduction"? Which of the following do we want
	    to focus upon?
	</p>

	<ol>
	    <li>A Lego-like construction kit, basically for building a Website (or web page) from scratch? Such a
		construction kit would concentrate upon a tall stack of capabilities based upon a narrow, "opinionated"
		trunk of foundational technologies. Examples of the foundational technologies could be a CSS framework
		like Bootstrap or Foundation,
		a CSS grid system like 960 Grid System, a CSS framework oriented to working with web components,
		components from customelements.io or webcomponents.org, and widgets from ExtJS or the Dojo Toolkit.
	    </li>

	    <li>A tool kit for creating or modifying web pages? Such a tool kit would concentrate upon the broadest
		possible comprehension of different kinds of web components in the broadest meaning of the
		term&mdash;including JavaScript-based widgets. Such a tool kit could not reasonably be made
		to comprehend attached JavaScript, but could understand the protocols of JavaScript-based widget
		libraries to intervene in and interact with
		the lifecycle of widgets. Such a tool kit could not reasonably comprehend other JavaScript,
		but could leave that JavaScript untouched. Such a tool kit could not reasonably be able to add useful,
		arbitrary JavaScript to a web page, but could add a very broad class of visually programmed functions
		as described later in this white paper.
	    </li>
	</ol>

	<p>Whichever path we choose&mdash;the creation of an isolated silo of technology
	    or the utility belt of tools&mdash;there are
	    some data-wrangling capabilities it seems Web users should be getting for free, but aren't.
	    These could be part of a Zen Manifesto:
	</p>

	<ol>
	    <li>Simple copying, cutting, and pasting of text, images, HTML components, and widgets should be possible.
		It should be possible to save various versions of these copied or cut items in a repertoire of
		patterns&mdash;with or without the text and images, with or without style
		classes, with or without style overrides. It should be possible to add parameters to the patterns so
		they can be used to easiy add to the Web. The patterns should be stored in a version control system
		that makes branching of versions very easy, as Git<sup><a href="#40">40</a></sup> does.
	    </li>

	    <li>The Web user should have the ability to create spreadsheets
		(like Google Sheets<sup><a href="#41">41</a></sup>
		via simple drag-and-drop. It should be possible to drag and drop whole cells, rows, and tables without
		even double-clicking and swiping the mouse pointer across words. These spreadsheets should be able
		to include images.
	    </li>
	</ol>
      </div>

      <div class="docs-section">
      <h2 id="Diving">8. Diving Deeper: Zen According to <em>The Elements of User Experience</em></h2>

      <p>Jesse James Garrett, who coined the term AJAX, wrote an influential book entitled
	  <em>The Elements of User Experience</em><sup><a href="#42">42</a></sup>,
	  which will serve to inform the strategy for the development of Zen.
	  (The acronym AJAX refers to a set of Web technologies
	  that enable the Web to be used as a remote software interface and employing
	  JavaScript and asynchronous HTTP requests.)
	  Garrett's elements are summarized in a chart<sup><a href="#43">43</a></sup>.
	  The "Surface Plane" described in that book corresponds roughly to the concerns of the Red End;
	  the "Strategy Plane" to the concerns of the Violet End.
      </p>

      <h3>User Needs for a "Zen Website"</h3>
      <p>There is a very specific set of user needs that a "Zen website" could uniquely fulfil.
	  At least some of these are:
      </p>

      <ol>
	  <li>A Web CMS that eschews text-based "code" in favor of a direct manipulation interface (DMI).
	  </li>

	  <li>A Web CMS that excels in the management of intermeshed or intertwined trees and meshes of data of many
	      types: Document Object Models (DOMs, including shadow DOMs),
	      including at least nodes implementing the HTMLElement, Attr, and Text interfaces;
	      CSS classes; and
	      link trees and meshes.
	      See "DOM Standard",<sup><a href="#44">44</a></sup>
	      published by the WHATWG community.
	  </li>

	  <li>A Web CMS (or WCMS) that can nest web components and widgets with no arbitrary limit.
	  </li>

	  <li>An easy way to consume and perhaps even interrelate Web schema.
	      (See schema.org.<sup><a href="#45">45</a></sup>)
	  </li>
      </ol>

      <h3>Site Objectives of a "Zen Website"</h3>

      <p>If there is a site objective, then there must be a website. If that website has a tight focus,
	  it must be oriented toward a particular segment of its entire potential user population (that is,
	  anyone who comes to the website). My initial attempt to segment users was this:
	  <ol>
	      <li>Users who are only fluent in the most basic Web-application constructs: URLs (or URIs), browsers,
		  windows, links, and maybe simple, clear buttons.
	      </li>
	      
	      <li>Users who are fluent in most of the basic, modern user interface patterns used in modern Web
		  applications like those described in the Yahoo Design Pattern Library<sup><a href="#46">46</a></sup>,
		  such as Top Navigation, Accordion, Breadcrumbs, Tabs, Navigation Bar, Calendar Picker,
		  Collapse Transition, Expand Transition, Slide Transition, and Drag and Drop.
	      </li>
	      
	      <li>Users with enough prior experience and intelligence to quickly adopt new methods of interaction with
		  computers, such as a Windows user who can adapt to an Apple laptop computer, or a user who can learn
		  about dragging and dropping URLs into a web browser or a images from the web browser to the desktop.
	      </li>
	      
	      <li>Users who can productively use a complex, specialized Web application such as a Web-page design
		  application, an application for photo manipulation, a paint application, an application for technical
		  analysis of financial data&mdash;an application that typically cannot be learned in less than an hour.
		  Some of the barriers to learning such an application more quickly are jargon, densely packed user
		  interface elements, and domain-specific knowledge.
	      </li>
	      
	      <li>A bit of reflection and research determined that I need to seek out experts' Web user segmentation.
		  That quickly turned up the topic of "web analytics user segmentation", where there is much good
		  information available for free. However, "levels of Web user ability" is a topic I have not explored
		  much at all.
		  It appears there is some very good guidance in the blog entry
		  <a href="https://www.w3.org/blog/2013/08/enabling-new-types-of-web-user/">
		      "Enabling new types of web user experiences"</a>.
		  A key insight in that post is that currently the dominant model of how web apps should be experienced
		  is that they should be "web ports" of iPhone apps. The author of the post believes that is aiming far
		  too low in aspiration. He gives some examples of devices like doorknobs and toasters broadcasting
		  web services over Bluetooth or WiFi. Such ideas, while not directly providing much help to Zen
		  development, provide inspiration for the necessary lateral thinking.
	      </li>
	  </ol>
      </p>

      <p>Some Zen website use cases could be:
	  <ol>
	      <li>Organizing the user's own text collections as hypertext in order to manage relationships
		  between various pieces of information, particularly hypertext documents
	      </li>

	      <li>Creating a "notebook" or "log"
	      </li>

	      <li>Creating a Web app for further personal Web exploration and use
	      </li>

	      <li>Creating a website or Web app for creative or commercial use
	      </li>
	      
	      <li>Create any kind of webiste by doing the front-end design, the front-end programming,
		  and the backend programming
	      </li>
	  </ol>
	  In lieu of the last-mentioned use case, I would like to go as far as I can with certain key ideas:
	  <ol>
	      <li>Enable a very short and very simple edit-compile-debug-commit-backup-deploy cycle.
	      </li>

	      <li>Use continuations and block-oriented visual programming to enable front-end programming in the
		  simple, logical, linear style of programming for a non-event-driven environment, with operating system
		  constructs like "wait".
	      </li>

	      <li>Since it is unnatural and sometimes dangerous to edit a live interface, use a run-edit toggle.
	      </li>

	      <li>Use visual paradigms and patterns like sliding DIVs, temporary absolute positioning,
		  the web browser's Z axis, parallax, and drag-and-drop.
	      </li>
	  </ol>
      </p>
      </div>

      <div class="docs-section">
      <h2 id="Name">9. Encapsulating the Zen Concept in a Domain Name</h2>
      <p>How to convey the proper central concept behind the "Zen website"?
	  Is the central concept for the Zen website all about being "on the same page"?
	  Would a better encapsulation of the gestalt of Zen be "own the web" or "your web" or "my web"
	  or "mash the web"?
	  Possible catch phrases to encapsulate the gestalt of Zen are:
	  <ul>
	      <li>"Own the Web"</li>
	      <li>"On the same page"</li>
	      <li>"Mash the Web"</li>
	      <li>"Remix the Web"</li>
	  </ul>
	  The following domain names that could convey the Zen concept are or appear to be squatted upon:
	  <ul>
	      <li>otw.com ("Own the Web")</li>
	      <li>ownweb.com</li>
	      <li>pweb.com ("Personal Web")</li>
	      <li>cweb.com ("Collaborative Web")</li>
	      <li>meweb.com</li>
	      <li>otsp.com ("On the Same Page")</li>
	      <li>zenweb.com</li>
	      <li>zweb.com</li>
	  </ul>
	  The following domain names are for sale:
	  <ul>
	      <li>owntheweb.com</li>
	      <li>myownweb.com</li>
	      <li>nowweb.com</li>
	  </ul>
	  The following domain names might be for sale:
	  <ul>
	      <li>myweb.com (currently selling emoji collections)</li>
	      <li>newweb.com (no DNS address)</li>
	  </ul>
	  The following domain names seem somewhat less likely to be for sale at an affordable price:
	  <ul>
	      <li>osp.com ("On the Same Page", but currently in use to sell fiberoptic products
		  under the brand name OSP)</li>
	      <li>youweb.com (redirects to videomeet.pro)</li>
	      <li>yourweb.com (redirects to secureserver.net)</li>
	      <li>collabweb.com (in use and might be a competitor to Zen)</li>
	      <li>me.com (redirects to Apple's icloud.com)</li>
	  </ul>
	  The top-level domain (TLD) <code>me</code> could convey the personalization aspect of Zen.
      </p>
      </div>
      
      <div class="docs-section">
      <h2 id="Study">10. For Further Study</h2>

      <ul>
	  <li>GGG and the Semantic Web. (Very important. Could be greatly helped by Zen.)</li>
	  <li>Lively Kernel.</li>
	  <li>Context Oriented Programming.</li>
	  <li>ContextJS.</li>
	  <li>Morphic.</li>
	  <li>Morphic.js (Morphic for JavaScript).</li>
	  <li>doCOUNT, related to Morphic.</li>
	  <li>Snap! (formerly named BYOB), related to Squeak Smalltalk and Morphic.</li>
	  <li>The principle of Lively Kernel that it has no run/edit mode distinction, that is,
	      the whole environment is live all the time: the environment runs, the debugger, and the editor
	      all run at the same time.
	  </li>
	  <li>APIs for clipboard operations such as copy, cut and paste in web applications,
	      as described in "Clipboard API and events"<sup><a href="#47">47</a></sup> on w3.org.
	  </li>
	  <li>Publications of the Web Platform Working Group at w3.org.</li>
	  <li><a href="http://www.svproduct.com/defining-good/">"Defining Good," Silicon Valley Product Group</a></li>
	  <li><a href="http://www.infovis-wiki.net/index.php/Visual_Information-Seeking_Mantra">B. Schneiderman's "Visual Information-Seeking Mantra"</a></li>
	  <li><a href="www.mat.ucsb.edu/~g.legrady/academic/courses/11w259/schneiderman.pdf">"A Task by Data Type Taxonomy for Information Visualizations,' B. Schneiderman</a></li>
	  <li><a href="www.eecs.berkeley.edu/Pubs/TechRpts/2014/EECS-2014-161.pdf">"Programming by Manipulation for Layout", Technical Report</a></li>
	  <li><a href="https://en.wikipedia.org/wiki/Programming_by_example">"Programming by example", Wikipedia</a></li>
	  <li><a href="https://www.w3.org/TR/wai-aria/">The W3C's "Accessible Rich Internet Applications (WAI-ARIA) 1.0" recommendation</a></li>
      </ul>

      </div>

      <div class="docs-section">
      <h2 id="Notes">11. Notes</h2>

      <ol>
	  <li>Jim Boulton, Kalle Everland, Jesper Lycke, 2014,
	      <a id="1" href="http://digital-archaeology.org/the-nexus-browser/">
		  "The Nexus Browser"</a>, digital-archaeology.org,
	      retrieved August 22, 2016.
	  </li>
	  <li>Allen Cypher, Mira Dontcheva, Tessa Lau, editors, 
	  </li>
	  <li>Pallab Ghosh, April 30, 2013,
	      <a id="2" href="http://www.bbc.com/news/technology-22249490">
		  "Cern re-creating first web page to revere early ideals"</a>, BBC.com,
	      retrieved August 11, 2016.
	  </li>
	  <li>Scott Laningham, August 22, 2006,
	      <a id="3" href="http://www.ibm.com/developerworks/podcast/dwi/cm-int082206txt.html">
		  "developerWorks Interviews: Tim Berners-Lee"</a>, IBM.com,
	      retrieved July 8, 2016.
	  </li>
	  <li>Berners-Lee, Tim, and Mark Fischetti, 1999,
	      <a id="4" href="https://www.w3.org/People/Berners-Lee/Weaving/Overview.html">
		  <em>Weaving the Web:
		      The original design and ultimate destiny of the World Wide Web by its inventor</em></a>,
	      HarperSanFrancisco, San Francisco.
	  </li>
	  <li><a id="5" href="https://wiki.mozilla.org/Support/Browser_Support">
		  "Browser Support"</a>, Mozilla Wiki,
	      retrieved July 8, 2016.
	  </li>
	  <li><a id="6" href="https://github.com/yui/yui3/wiki/Graded-Browser-Support">
		  "Graded Browser Support"</a>, YUI3,
	      retrieved July 8, 2016.
	  </li>
	  <li><a id="7" href="https://jquerymobile.com/browser-support/1.4/">
		  "jQuery Mobile 1.4 Browser Support"</a>, jquerymobile.com,
	      retrieved July 8, 2016.
	  </li>
	  <li><a id="8" href="https://en.wikipedia.org/wiki/Comparison_of_web_browsers">
		  "Comparison of web browsers"</a>, Wikipedia,
	      retrieved July 8, 2016.
	  </li>
	  <li><a id="9" href="https://en.wikipedia.org/wiki/Augmented_browsing">
		  "Augmented browsing"</a>, Wikipedia,
	      retrieved November 26, 2016.
	  </li>
	  <li><a id="10" href="https://en.wikipedia.org/wiki/List_of_augmented_browsing_software">
		  "List of augmented browsing software"</a>, Wikipedia,
	      retrieved November 25, 2016.
	  </li>
	  <li>Rick Santos, May 14, 2014,
	      <a id="9" href="https://medium.engineering/why-contenteditable-is-terrible-122d8a40e480#.dw8d785j2">
		  "Why ContentEditable is Terrible&mdash;Or: How the Medium Editor Works"</a>, Medium Engineering,
	      retrieved September 11, 2016.
	  </li>
	  <li>Piotrek Koszuliński, August 13, 2015,
	      <a id="10" href="https://medium.com/content-uneditable/contenteditable-the-good-the-bad-and-the-ugly-261a38555e9c#.wczx4t3am">
		  "ContentEditable — The Good, the Bad and the Ugly"</a>, Medium, retrieved September 21, 2016.
	  </li>
	  <li>Dan Dascalescu, September 6, 2016,
	      <a id="11" href="https://github.com/iDoRecall/comparisons/blob/master/JavaScript-WYSIWYG-editors.md">
		  "Comparison of JavaScript WYSIWYG editors"</a>, Github, retrieved September 21, 2016.
	  </li>
	  <li><a id="12" href="https://en.wikipedia.org/wiki/WYMeditor">
		  "WYMeditor"</a>, Wikipedia,
	      retrieved August 31, 2016.
	  </li>
	  <li>David Ungar,
	      <a id="13" href="http://web.stanford.edu/class/ee380/Abstracts/090930.html">
		  abstract entitled "Self and self: whys and wherefores"</a>, Stanford.edu,
	      retrieved August 8, 2016.
	  </li>
	  <li>David Ungar, September 30, 2009,
	      <a id="14" href="https://youtu.be/3ka4KY7TMTU">
		  video entitled "Self and Self: Whys and Wherefores"</a>, YouTub.com,
	      retrieved August 8, 2016.
	  </li>
	  <li>Dan Ingalls,
	      <a id="15" href="https://youtu.be/QTJRwKOFddc">
		  "The Live Web. Drag 'n drop in the cloud"</a>, YouTube.com,
	      retrieved August 11, 2016.
	  </li>
	  <li><a id="16" href="http://lively-kernel.org/">
		  "Lively Kernel"</a>, lively-kernel.org,
	      retrieved August 11, 2016.
	  </li>
	  <li><a id="17" href="https://dom.spec.whatwg.org/">
		  "DOM&mdash;Living Standard"</a>, WHATWG.org,
	      retrieved August 11, 2016.
	  </li>
	  <li><a id="18" href="https://www.w3.org/DOM/faq.html">
		  "Document Object Model FAQ"</a>, w3c.org,
	      retrieved September 1, 2016.
	  </li>
	  <li><a id="19" href="http://wiki.squeak.org/squeak/2175">
		  "Inspector"</a>, Squeak.org,
	      retrieved October 10, 2016.
	  </li>
	  <li><a id="20" href="https://en.wikipedia.org/wiki/Abstract_syntax_tree">
		  "Abstract syntax tree"</a>, Wikipedia,
	      retrieved September 1, 2016.
	  </li>
	  <li><a id="21" href="https://www.w3.org/TR/CSS2/visuren.html#box-gen">
		  "Controlling box generation"</a>,
	      Section 9.2 of "Cascading Style Sheets Level 2 Revision 1 (CSS 2.1) Specification" W3C Recommendation,
	      retrieved September 1, 2016.
	  </li>
	  <li>David Madore, <a id="22" href="http://www.madore.org/~david/computers/callcc.html">
		  "A page about call/cc"</a>, www.madore.org,
	      retrieved September 1, 2016.
	  </li>
	  <li>Steve Wittens, <a id="23" href="http://acko.net/blog/shadow-dom/">
		  "Shadow DOM&mdash;SVG, CSS, React and Angular"</a>, Hackery, Math & Design,
	      retrieved July 8, 2016.
	  </li>
	  <li><a id="24" href="google.com/search?q=web+framework">
		  "web framework - Google Search"</a>, Google,
	      retrieved July 28, 2016.
	  </li>
	  <li><a id="25" href="https://en.wikipedia.org/wiki/Transclusion">
		  "Transclusion"</a>, Wikipedia,
	      retrieved July 12, 2016.
	  </li>
	  <li><a id="26" href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Frame-Options">
		  "X-Frame-Options"</a>, Mozilla Developer Network,
	      retrieved July 8, 2016.
	  </li>
	  <li><a id="27" href="google.com/search?q=chrome+memory+usage">
		  "chrome memory usage - Google Search"</a>, Google,
	      retrieved July 8, 2016.
	  </li>
	  <li><a id="28"
		 href="https://chrome.google.com/webstore/detail/tabs-outliner/eggkanocgddhmamlbiijnphhppkpkmkl?hl=en">
		  "Tabs Outliner - Chrome Web Store"</a>, Google,
	      retrieved July 8, 2016.
	  </li>
	  <li><a id="29" href="https://developer.yahoo.com/search/content/V2/contentAnalysis.html">
		  "Content Analysis Web Service"</a>, Yahoo! Developer Network,
	      retrieved October 8, 2016.
	  </li>
	  <li><a id="30" href="https://en.wikipedia.org/wiki/Xmarks_Sync#Company_history">
		  "Xmarks company history"</a>, Wikipedia,
	      retrieved July 8, 2016.
	  </li>
	  <li><a id="31" href="https://en.wikipedia.org/wiki/Category:Discontinued_Google_services">
		  "Wikipedia category: Discontinued Google services"</a>, Wikipedia,
	      retrieved July 8, 2016.
	  </li>
	  <li><a id="32" href="http://www.huffingtonpost.in/2016/04/14/discontinued-google-produ_n_9436180.html">
		  "6 Popular Google Products Which No Longer Exist"</a>, The Huffington Post,
	      retrieved July 8, 2016.
	  </li>
	  <li><a id="33" href="https://en.wikipedia.org/wiki/Xmarks_Sync#Xmarks_domain_blocked_in_India">
		  "Xmarks domain blocked in India"</a>, Wikipedia,
	      retrieved July 8, 2016.
	  </li>
	  <li><a id="34" href="http://time.com/money/3528487/data-breach-identity-theft-jp-morgan-kmart-staples/">
		  "Data Breach Tracker: All the Major Companies That Have Been Hacked"</a>, Time,
	      retrieved July 8, 2016.
	  </li>
	  <li><a id="35"
		 href="http://www.cio.com/article/2872517/data-breach/6-biggest-business-security-risks-and-how-you-can-fight-back.html">
		  "6 Biggest Business Security Risks and How You Can Fight Back"</a>, CIO,
	      retrieved July 8, 2016.
	  </li>
	  <li><a id="36"
		 href="http://www.forbes.com/sites/kashmirhill/2014/08/05/huge-password-breach-shady-antics/#2cf211434769">
		  "Firm That Exposed Breach Of 'Billion Passwords' Quickly Offered $120 Service
		  To Find Out If You're Affected"</a>, Forbes,
	      retrieved July 8, 2016.
	  </li>
	  <li><a id="37" href="http://krebsonsecurity.com/2016/05/how-the-pwnedlist-got-pwned/">
		  "How the Pwnedlist Got Pwned"</a>, KrebsonSecurity,
	      retrieved July 8, 2016.
	  </li>
	  <li><a id="38"
		 href="http://www.nytimes.com/2014/08/06/technology/russian-gang-said-to-amass-more-than-a-billion-stolen-internet-credentials.html?_r=0">
		  "Russian Hackers Amass Over a Billion Internet Passwords"</a>, The New York Times,
		  retrieved July 8, 2016.
	  </li>
	  <li><a id="39" href="http://www.forbes.com/sites/moneybuilder/2015/01/13/the-big-data-breaches-of-2014/#a5d08f53a48f">
		  "The Big Data Breaches of 2014"</a>, Forbes,
	      retrieved July 8, 2016.
	  </li>
	  <li><a id="40" href="https://git-scm.com/">
		  "Git"</a>, git-scm.com,
	      retrieved July 12, 2016.
	  </li>
	  <li><a id="41"
		 href="https://www.google.com/sheets/about/?gclid=CjwKEAjwqpK8BRD7ua-U0orrgkESJADlN3YBgbIrdrOIvuMfcqq7taN4Fy3v0WHTdXNLQHsVvpcmWxoCy57w_wcB">
		  "Google Sheets - create and edit spreadsheets online, for free"</a>, Google,
	      retrieved July 12, 2016.
	  </li>
	  <li>Jesse James Garrett, October 21, 2002,
	      <a id="42" href="http://www.jjg.net/elements/">
		  <em>The Elements of User Experience: User-Centered Design for the Web</em></a>,
	      New Riders Publishing, New York.
	  </li>
	  <li>Jesse James Garrett,
	      <a id="43" href="http://www.jjg.net/elements/pdf/elements.pdf">
		  "The Elements of User Experience"</a>, jjg.net,
	      retrieved September 1, 2016.
	  </li>
	  <li><a id="44" href="https://dom.spec.whatwg.org/">
		  "DOM Standard"</a>, WHATWG.org,
	      retrieved October 10, 2016.
	  </li>
	  <li><a id="45" href="http://schema.org/">
		  "Home - schema.org"</a>, schema.org,
	      retrieved October 10, 2016.
	  </li>
	  <li><a id="46" href="https://developer.yahoo.com/ypatterns/">
		  "Yahoo Design Pattern Library"</a>, developer.yahoo.com,
	      retrieved September 1, 2016.
	  </li>
	  <li><a id="47" href="https://www.w3.org/TR/clipboard-apis/">
		  "Clipboard API and events"</a>, w3.org,
	      retrieved September 1, 2016.
	  </li>
      </ol>
      
      </div>
      
      <div class="column">
	  <!-- Footer -->
      </div>
