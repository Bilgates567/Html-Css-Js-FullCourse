🌐 Comprehensive HTML Course Documentation
### 📚 Table of Contents
Introduction to HTML

Document Structure

Text Formatting

HTML Elements & Attributes

Links and Navigation

Images and Media

Lists

Tables

Forms

Semantic HTML

HTML5 APIs

Best Practices

Project Exercises

Resources

### 🧠 1. Introduction to HTML
What is HTML?
Definition: HyperText Markup Language

Purpose: Structures content for web browsers

Current Standard: HTML5 (released 2014)

Key Characteristics:
Uses tags (angle brackets) to mark up content

Platform-independent

Works with CSS (styling) and JavaScript (behavior)

Basic Workflow:
Create .html file

Write HTML code

Open in browser

### 🏗️ 2. Document Structure
Core Structure Template:
html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document Title</title>
</head>
<body>
    <!-- Visible content goes here -->
</body>
</html>
Essential Components:
Component	Purpose
<!DOCTYPE html>	Declares HTML5 document type
<html>	Root element containing all content
<head>	Contains metadata, links to resources
<body>	Holds all visible page content
Document Metadata:
html
<head>
    <!-- Character encoding -->
    <meta charset="UTF-8">
    
    <!-- Responsive viewport -->
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    
    <!-- Page description for SEO -->
    <meta name="description" content="Free HTML tutorial">
    
    <!-- CSS links -->
    <link rel="stylesheet" href="styles.css">
    
    <!-- JavaScript -->
    <script src="script.js" defer></script>
</head>
### ✍️ 3. Text Formatting
Heading Hierarchy:
html
<h1>Main Title</h1>  <!-- Only one per page -->
<h2>Section</h2>
<h3>Sub-section</h3>
<h4>Sub-sub-section</h4>
### Text Elements:
Element	Purpose	Example
<p>	Paragraph	<p>This is text.</p>
<strong>	Important text (bold)	<strong>Warning!</strong>
<em>	Emphasized text (italic)	<em>Please note</em>
<mark>	Highlighted text	<mark>Important</mark>
<small>	Side comments	<small>Terms apply</small>
<blockquote>	Block quotation	<blockquote cite="source">
Special Characters:
html
&copy;   <!-- © -->
&trade;  <!-- ™ -->
&nbsp;   <!-- Non-breaking space -->
&lt;     <!-- < -->
&gt;     <!-- > -->
🖼️ 6. Images and Media
Image Implementation:
html
<img src="image.jpg" 
     alt="Description of image"
     width="600"
     height="400"
     loading="lazy">
Attributes Explained:
Attribute	Purpose
src	Image file path (relative or absolute)
alt	Alternative text (required for accessibility)
width	Display width in pixels (optional)
loading	lazy delays loading until image is near viewport (performance boost)
### Responsive Images:
html
<picture>
    <source media="(min-width: 800px)" srcset="large.jpg">
    <source media="(min-width: 400px)" srcset="medium.jpg">
    <img src="small.jpg" alt="Responsive image">
</picture>
Video Embedding:
html
<video controls width="600" poster="preview.jpg">
    <source src="movie.mp4" type="video/mp4">
    <source src="movie.webm" type="video/webm">
    Your browser doesn't support HTML5 video.
</video>
Audio Embedding:
html
<audio controls>
    <source src="audio.mp3" type="audio/mpeg">
    Your browser doesn't support the audio element.
</audio>
### 📝 9. Forms
Complete Form Example:
html
<form action="/submit" method="POST" novalidate>
    <fieldset>
        <legend>Personal Information</legend>
        
        <label for="name">Full Name:</label>
        <input type="text" id="name" name="name" required minlength="3">
        
        <label for="email">Email:</label>
        <input type="email" id="email" name="email" required>
        
        <label for="password">Password:</label>
        <input type="password" id="password" name="password" required 
               pattern="(?=.*\d)(?=.*[a-z])(?=.*[A-Z]).{8,}">
    </fieldset>
    
    <button type="submit">Register</button>
    <button type="reset">Clear Form</button>
</form>
Form Validation Patterns:
Pattern	Matches
[A-Za-z]{3}	Exactly 3 letters
\d{3}-\d{3}-\d{4}	Phone: 123-456-7890
[^@]+@[^@]+\.[^@]+	Basic email format
(?=.*\d)(?=.*[a-z])(?=.*[A-Z]).{8,}	Password with 8+ chars, 1 uppercase, 1 lowercase, 1 number
🏆 13. Project Exercises
Beginner Projects:
Personal Profile Page

Requirements: Header, navigation, about section, contact form

Skills: Basic structure, text formatting, links

Recipe Page

Requirements: Ingredients list, preparation steps, images

Skills: Lists, images, text formatting

Intermediate Projects:
Product Landing Page

Requirements: Hero section, features grid, testimonial carousel

Skills: Semantic HTML, responsive images, sections

Technical Documentation

Requirements: Sidebar navigation, code samples, article sections

Skills: Page structure, accessibility

Advanced Projects:
Interactive Quiz Form

Requirements: Multiple question types, scoring system

Skills: Complex forms, input types

Portfolio with Filterable Gallery

Requirements: Project categories, modal details view

Skills: Semantic markup, accessibility

🔗 14. Resources
Official Documentation:
MDN HTML Reference

HTML Living Standard

Validation Tools:
W3C Validator

HTMLHint

Learning Platforms:
freeCodeCamp HTML

Codecademy HTML


