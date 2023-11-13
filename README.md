# PicoCTF Scavenger Hunt Walkthrough
A straightforward guide to tackle the PicoCTF Scavenger Hunt. Get step-by-step solutions to challenges, decode flags, and boost your cybersecurity know-how. Perfect for all skill levels.

## Overview
Points: 50
Category: Web Exploitation

## Description
Hint on the CTF Challenge: There is some interesting information hidden around this site http://mercury.picoctf.net:44070/. Can you find it?

## Hint
You should have enough hints to find the files, don't run a brute forcer.

## Getting Down To Business
When you click on the link provided, it leads you to a plain simple and boring website. 
To figure out where to start, you right click on the page to be able to view the page source. 

## The Page Source

<!doctype html>
<html>
  <head>
    <title>Scavenger Hunt</title>
    <link href="https://fonts.googleapis.com/css?family=Open+Sans|Roboto" rel="stylesheet">
    <link rel="stylesheet" type="text/css" href="mycss.css">
    <script type="application/javascript" src="myjs.js"></script>
  </head>

  <body>
    <div class="container">
      <header>
		<h1>Just some boring HTML</h1>
      </header>

      <button class="tablink" onclick="openTab('tabintro', this, '#222')" id="defaultOpen">How</button>
      <button class="tablink" onclick="openTab('tababout', this, '#222')">What</button>

      <div id="tabintro" class="tabcontent">
		<h3>How</h3>
		<p>How do you like my website?</p>
      </div>

      <div id="tababout" class="tabcontent">
		<h3>What</h3>
		<p>I used these to make this site: <br/>
		  HTML <br/>
		  CSS <br/>
		  JS (JavaScript)
		</p>
	<!-- Here's the first part of the flag: picoCTF{t -->
      </div>

    </div>

  </body>
</html>


