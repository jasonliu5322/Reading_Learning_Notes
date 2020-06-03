# Day 1

- From the Duckett HTML book:
    - Introduction p2-11
        -  1.When you connect to the web, you do so via an Internet Service Provider (ISP). You type a domain name or web address into your browser to visit a site; for example: google.com, bbc.co.uk, microsoft.com. 2.Your computer contacts a network of servers called Domain Name System (DNS) servers. These act like phone books; they tell your computer the IP address associated with the requested domain name. An IP address is a number of up to 12 digits separated by periods / full stops. Every device connected to the web has a unique IP address; it is like the phone number for that computer. 3.The unique number that the DNS server returns to your computer allows your browser to contact the web serverthat hosts the website you requested. A web server is a computer that is constantly connected to the web, and is set up especially to send web pages to users. 4.The web server then sends the page you requested back to your web browser.
          
    - HTML Chapter 1: “Structure” (pp.12-39)
        ```
        If you are working with a content management system, blogging platform, or e-commerce application, you will probably log into a special administration section of the website to control it. The tools provided in the administration sections of these sites usually allow you to edit parts of the page rather than the entire page, which means you will rarely see the <html>, <head>, or <body> elements.
        ```
    - HTML Chapter 8: “Extra Markup” (p.176-199)
        
        - Id attribute: Every HTML element can carry the id attribute. It is used to uniquely identify that element from other elements on the page. Its value should start with a letter or an underscore (not a number or any other character). It is important that no two elements on the same page have the same value for their id attributes (otherwise the value is no longer unique).
        The id attribute is known as **a global attribute** because it can be used on any element.
        
        - Class attribute: p184 example
         
        - Block Elements: 
           ```
           Some elements will always appear to start on a new line in the browser window. These are known as block level elements. Examples of block elements are <h1>, <p>, <ul>, and <li>.
           ```
        - Inline Elements:
           ```
           Some elements will always appear to continue on the same line as their neighbouring elements. These are known as inline elements. Examples of inline elements are <a>, <b>, <em>, and <img>.
           ```
        
        - Grouping text and elements in a block
            ```
            <div> element: p187 example
            The <div> element allows you to group a set of elements together in one block-level box.For example, you might create a <div> element to contain all of the elements for the header of your site (the logo and the navigation), or you might create a <div> element to contain comments from visitors. 
            ```
        - Grouping text and elements inline
            ```
            example p188
            The <span> element acts like an inline equivalent of the <div> element. It is used to either: 1. Contain a section of text where there is no other suitable element to differentiate it from its surrounding text 2. Contain a number of inline elements.
            ```
        - Iframes 
           ```
           example: p190
           <iframes>: An iframe is like a little window that has been cut into yourpage — and in that window you can see another page. The term iframe is an abbreviation of inline frame.One common use of iframes (that you may have seen on various websites) is to embed a Google Map into a page. The content of the iframe can be any html page (either located on the same server or anywhere else on the web).
           An iframe is created using the <iframe> element. There are a few attributes that you will need to know to use it: src, height, width, scrolling, frameborder, seamless.
         
         - Information about your pages
            ```
            <meta>: p191 example
            The <meta> element lives inside the <head> element and contains information about that web page. It is not visible to users but fulfills a number of purposes such as telling search engines about your page, who created it, and whether or not it is time sensitive. (If the page is time sensitive, it can be set to expire.) The <meta> element is an empty element so it does not have a closing tag. It uses attributes to carry the information.
            ```

    - HTML Chapter 17: “HTML5 Layout” (pp.428-451)
        ```
        <header>, <footer>, <nav>, <article>, <aside>，<section>, <hgroup>, <figure><figcaption>，<div>, <a>.
        ```
        example p444

    - HTML Chapter 18: “Process & Design” (pp.452-475)


- From the Duckett JS book:
    - Introduction
    - Chapter 1: “The ABC of Programming” (pp.11-52)
        - objects and properties
