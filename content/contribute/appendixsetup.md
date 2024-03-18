+++
author = "Hugo Authors"
title = "Appendix"
date = "2024-03-18"
description = "Additional installation information for your laptop while creating a new pattern documentation"
tags = [
    "markdown",
    "text",
]
+++

Additional installation information for your laptop while creating a new pattern documentation


==== Node.js

In this guide, we'll be installing Node.js 18.

While you can install Node.js from the official packages, we strongly recommend that you use nvm (Node Version Manager) to manage your Node.js installation(s).
Follow the nvm installation instructions to set up nvm on your machine.

Once you've installed nvm, open a new terminal and install Node.js 18 using the following command:

 $ nvm install 18

You can switch to this version of Node.js at any time using the following command:

 $ nvm use 18

To make Node.js 10 the default in new terminals, type:

 $ nvm alias default 18

Now that you have Node.js installed, you can proceed with installing the Gulp CLI.

==== Gulp 

You'll need the Gulp command-line interface (CLI) to run the build.
The Gulp CLI package provides the `gulp` command which, in turn, executes the version of Gulp declared by the project.

You should install the Gulp CLI globally (which resolves to a location in your user directory if you're using nvm) using the following command:

 $ npm install -g gulp-cli

Verify the Gulp CLI is installed and on your PATH by running:

 $ gulp --version

Now that you have the prerequisites installed, you can fetch and build the UI project.

=== About the Solution Pattern Site Template

The template is available at: https://github.com/redhat-solution-patterns/solution-pattern-website-template.

This strategy benefits content writers by:

* Allowing for a simple projects creation flow: a couple of clicks and it's done;
* Providing, for free, a compatible look and feel with other https://redhat-solution-patterns.github.io/[existing solution patterns];
* Recommended high-level page structure, sections, and navigation menu, providing readers a similar experience across different solution patterns;
* Several documentation code samples that show useful features available;
* Allowing focus on what matters - the content. Using Asciidoc, there's no need to spend extra hours on CSS customization for page and text formatting.
* Bringing a ready-to-use deployment pipeline (https://github.com/redhat-solution-patterns/solution-pattern-website-template/blob/main/.github/workflows/docs.yml[GitHub action]) that builds and publishes the project website.

The solution pattern's template is derived from the https://github.com/redhat-scholars/courseware-template[Red Hat Scholars courseware template], with extra customization:

* UI: The pages are customized to represent the goals of the Red Hat Solution Pattern projects. The forked projects and changes are available at: https://github.com/redhat-scholars/course-ui[]
* Content recommendation: out-of-the-box configuration, content and structure that matches the target objectives of a solution pattern documentation. 

[#highlights]
=== Documentation components highlights 


Admonitions::
Use `NOTE`,`TIP`,`IMPORTANT`,`CAUTION` or `WARNING` to create nice admonition blocks.
+
[source,adoc]
-----
[NOTE] This is nice admonition block for a note.  
-----
+
More details on how to use: https://docs.asciidoctor.org/asciidoc/latest/blocks/admonitions/[AsciiDoctor Admonitions].


[NOTE]
Information below is part of https://redhat-scholars.github.io/build-course/rhs-build-course/index.html["Writing a RedHat scholar Course",window=_blank], by Red Hat Developers.

Copy-Pasteable Code::

To have your code/commands easily copied and pasted, you can use the special styling `.console-input` on the AsciiDoc source blocks. That should enables clipboard for the source block.
+
[source,adoc]
-----
[.console-input]
[source,adoc]
----
kubectl get pods
----
-----

+
The output result of the above code is:
+
[.console-input]
[source,adoc]
----
kubectl get pods
----

Console Output::
+
As you have commands that gets executed, you may wish to show the out of the command. Like adding special style source block for console input, you can add similar style like `.console-output` to the source block.
+
[source,adoc]
-----
[.console-input]
[source,adoc]
----
echo "Hello World!"
----
-----
+
The output result of the above code is:
+
[.console-output]
[source,bash]
----
Hello World!
----

Tabs::
+
Another resource you can use are *Tabs*. To do so, use the `[tabs]` macro as shown below:
+
[.console-input]
[source,adoc]
----
[tabs]
====
one::
+
--
--
two::
+
--
--
====
----
+
The output result of the above code is:
+
[tabs]
====
One::
+
--
[.console-input]
[source,bash]
----
echo Hello World!
----
--
Two::
+
--
[.console-output]
[source,bash]
----
Hello World!
----
--
====