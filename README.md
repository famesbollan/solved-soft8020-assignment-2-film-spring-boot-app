Download Link: https://assignmentchef.com/product/solved-soft8020-assignment-2-film-spring-boot-app
<br>
You are to develop a website that stores information about directors and the films they have directed.

You may assume that a film has only one director.

<ul>

 <li>Any user can o view a list of the directors in the database in alphabetical order</li>

</ul>

(by surname) o select a director from the list to view that director’s films o view a list of the films in the database in chronological order showing all information you have about that film

<ul>

 <li>register by providing an email and password</li>

</ul>

<ul>

 <li>Authenticated users can o add a director to the database

  <ul>

   <li>no two directors can have the same name.</li>

   <li>apply sensible limitations to the name e.g. use</li>

  </ul></li>

</ul>

@Pattern and @Size

<ul>

 <li>add a film providing the film’s title, year of release and a director, which must be selected from a list provided.

  <ul>

   <li>Two films can have the same title. When a film is remade it often has the same name as the original.</li>

   <li>A film’s title cannot be left blank.</li>

   <li>The film’s year of release must be an integer between 1888 and the current year (which will not always be 2020).</li>

  </ul></li>

 <li>edit the title of a film

  <ul>

   <li>requires that the method’s signature created in the repository be annotated as @Transactional (facilitating rollback if necessary) and @Modifying.</li>

  </ul></li>

 <li>Administrators can o delete a film o delete a director along with their films</li>

</ul>

You must also provide

<ul>

 <li>Two REST API endpoints which you write yourself, to allow authenticated users to, o access (in json format) films released in a particular year

  <ul>

   <li>delete a director (and associated films) given their id</li>

  </ul></li>

 <li>An example of consuming these two APIs which requires another Spring project. Nothing fancy is needed here, just a second WebMVC project that has two controllers and two views. The controllers send authentication data to the REST APIs and present the result of the request in suitable format. No forms are needed.</li>

</ul>

<h1>Technical Notes</h1>

You will use <strong>WebMVC</strong> Spring Boot application.

Use an <strong>in-memory h2</strong> database to create an “out of the box” application. This database must be populated with sample data.

The application must be implemented using be implemented using <strong>JPA</strong>, making use of all that offers. This project essentially has two entities, a film and its director, along with users and their roles.

Use the <strong>Security</strong> module for authentication and authorisation.

I am not interested in visual styling – just make the web site well structured, readable, navigable, etc – although you should use some CSS. Credit any templates (CSS/HTML) if you use them.  I recommend the use of fragments to reduce the amount of code.

Forms must be validated using form binding and <strong>your own</strong> (not Spring or clientside) <strong>error messages </strong>should be displayed by the view if the user makes a mistake.

It must be possible to <strong>change</strong> <strong>the</strong> <strong>language</strong> of the website. User input must be validated with suitable (international) error messages. You do not have to translate content. I will accept subtle changes e.g. “Film Title” becoming “Film Title_FR” to indicate the language has changed to French.

You <strong>must</strong> use the following:




<ul>

 <li>Spring Boot</li>

 <li>Spring MVC</li>

 <li>Thymeleaf (not JSP)</li>

 <li>Spring Data JPA</li>

 <li>Spring Security</li>

 <li>H2 for an embedded database</li>

 <li>Maven</li>

</ul>

<strong>Unit tests are <em>not</em> required.</strong>

You may use <strong>Project Lombok</strong> to reduce boilerplate code.

Provide a <strong>brief document</strong> outlining the high-level design of your system (1 or 2 A4 pages) including but not limited to your database design and class diagrams and the beans which you used.


