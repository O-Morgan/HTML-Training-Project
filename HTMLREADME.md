# HTML Web Page Training Project

To build this page I will be using inline style formatting which is considered outdated, but it's handy to use as a beginner to grasp some key fundamentals. CSS is now used to style pages which is much more effective with page layouts that are more responsive with mobile devices.    

When only using html, you are limited when it comes to the layout and format of the page. Without CSS I will need to insert all my objects inside tables, rows and columns.

So like I've mentioned already, using tables as layout containers has become a thing of the past but understanding tables is still important when working with tabular data. 

There'll still be many useful skill learnt from this, such as object insertion, text formatting, form development and basic styling. 

### What the end Product looks like using only html tables.  

![/workspace/HTML-Training-Project/html tables only image.png](<html tables only image.png>)





  
## The first thing is to create the basic html page structure 

The head tags are important instructions for the web browser, but anything between the head tags will not be displayed visually in the web browser.  

```html
<!DOCTYPE html>
<html>

<head>
<meta http-equiv="Content-Type" content="text/html; charset-utf-8" />
<title>Website Project</title>
</head>

<body>


    
</body>
</html>
```

### The website header

The website header is nested inside a table so that is the first thing to create, this is knows as the parent table and then we have an area to configure a table within, which is know as the nested table.

```html
<body>

<table width="100%" height="60" cellspacing="5" cellpadding="5" bgcolor="#000000">

    <tr>

        <td align="left">
            <!-- Add content inside the table cell here -->
        </td>

    </tr>

</table>
</body>
```

#### Now to add the nested header within the table

 The headers now complete, you can now see that theres a table nested within the parent table.   


```html
<body>
<table width="100%" height="60" cellspacing="5" cellpadding="5" bgcolor="#000000">

    <tr>

        <td align="left">
            <!-- Add content inside the table cell here -->
            <table width="547" border="0" align="center" cellpadding="1" cellspacing="1">
                <tr>
                    <td width="96"><font face="Verdana, Geneva, sans-serif" color="white"><h3>Home</h3></font></td>

                    <td width="113"><font face="Verdana, Geneva, sans-serif" color="white"><h3>About</h3></font></td>

                    <td width="128"><font face="Verdana, Geneva, sans-serif" color="white"><h3>Services</h3></font></td>

                    <td width="114"><font face="Verdana, Geneva, sans-serif" color="white"><h3>Clients</h3></font></td>

                    <td width="80"><font face="Verdana, Geneva, sans-serif" color="white"><h3>Contacts</h3></font></td>
                
                
                </tr>
            </table>
        </td>

    </tr>

</table>
</body>
```

## The Callout Area

In this section I'm going to configure the Callout Area below the header. This is also going to be contained within a table. Without using CSS, it is somewhat the only way we can style and layout the page. The callout area is only going to contain the business name and phone number to be contacted on.

To do this, we first create a primary table, then nest the details within a table inside the primary table, as we did before. You could consider the primary table as configuring the area, and the nested table as configuring the space within it. This way, you can display the information within a confined area and have some control over its position and layout.


```html
<table width="100%" height="150" border="0" cellspacing="5" cellpadding="5" bgcolor="#F0F0F0">
    <tr>
        <td align="center">
            <table width="708" border="0" cellpadding="1" cellspacing="1">
                <tr>
                    <td width="338" align="left">
                        <font face="Verdana, Geneva, sans-serif" color="black" size="5"><strong>MyBusiness</strong></font><br />
                        Website
                    </td> 
                    <td width="291" align="right">
                        <font face="Verdana, Geneva, sans-serif" color="black" size="5"><strong>Call Today</strong></font><br />
                        0121 do one
                    </td>
                </tr>
            </table>
        </td>
    </tr>
</table>
```

## Image Insertion

Again, to insert an image with text below it you have to insert multiple primary tables with a general area configuration setup, then you insert a nested table with more of a fine tuned configuration and associated image/text.

```html
<table width="100%" height="150" border="0" cellspacing="5" cellpadding="5" bgcolor="white">
    <tr>
        <td align="center">
            <table width="600" border="0" cellspacing="1" cellpadding="1">
                <tr>
                    <td align="center">
                        <img src="https://wallpapercave.com/wp/wp7199912.jpg" width="980" height="300" />
                    </td>
                </tr>
            </table>
        </td>
    </tr>
</table>

<table width="100%" height="150" border="0" cellspacing="5" cellpadding="5" bgcolor="white">
    <tr>
        <td height="72" align="center" valign="top">
            <table width="730" border="0" cellspacing="1" cellpadding="1">
                <tr>
                    <td width="726" align="center">
                        <font face="Verdana, Geneva, sans-serif" color="black" size="6">
                            This is my company website <br />
                            <strong>Dream. Plan. Create.</strong>
                        </font>
                    </td>
                </tr>
            </table>
        </td>
    </tr>
</table>
```

### Text Alignment Tips 

Text within HTML will appear next to the immediately written text, even if you have written it on another line and in a different place, i.e. directly or indirectly below the previous text. So, to get text to appear on the line below, you have to use a line break tag ```<br />```. Without it, the text will appear on the same line.

The ```<br />``` tag should be applied at the end of the text, but before the text you want to appear on a new line below.

If you want a spacing between words on the same line, it isn't as simple as just pressing the space bar as thats not recognised either. You have to use ```&nbsp;```. So, if you wanted four spaces, you would need to add it four times: ```&nbsp;&nbsp;&nbsp;&nbsp```.

For paragraph spacing, which will appear two lines below the last text, you have to use opening and closing ```<p>``` tags: ```<p>text here inside</p>```


## Contact Button Creation

The contact button creation is still a primary table with a nested table within. In this setup, the primary table forms the perimeter of the white box. Because the background of the website is white, it may not be visible. Then, I have configured the nested table to be orange, and the text is displayed within it.
```html
<!--Primary tabel the orange area -->
<table width="100%" height="75" border="0" cellspacing="5" cellpadding="5" bgcolor="white">
    <tr>
        <td height="72" align="center" valign="top">
            <!--The nested table within containing the text-->
            <table width="300" height="75" border="0" cellspacing="3" cellpadding="3" bgcolor="#FF9900">
                <tr>
                    <td width="301" align="center">
                        <font color="white" size="5" face="Verdana, Geneva, sans-serif">
                            <a href="#">Contact us Today</a><br />
                        </font>
                    </td>
                </tr>
            </table>
        </td>
    </tr>
</table>
```


### Submit Button Newsletter Registration 

This button is implemented as a post method, allowing you to submit information, such as your email address, for subscription to future newsletters. The backend hasn't been created yet, but the theory is that I would have a PHP action within this code or outside of it to validate the information before sending it to the backend. 

```html
 </td>
</tr>
<tr>
    <!--Straight into button creation for registration to receive the newsletter-->
    <td height="72" align="center" valign="top">
        <font color="black" size="2" face="Verdana, Geneva, sans-serif"><strong>Register for my Newsletter:</strong></font><br />

        <!--Send.php won't work as there's no backend configured-->
        <form name="contact" method="post" action="send.php">
            <input type="text" name="email" />
            <input type="submit" name="button" value="Submit" />
        </form>
    </td>
</tr>
</table>
```

## Entering Tabular Data

I have created and configured a primary table with nested tables, each consisting of three columns. In these nested tables, I've included headers and additional text. To make the subtext editable by users, I've used the ```contenteditable="true"``` attribute. The headers remain fixed. The last column contains an unordered list created with the ```<ul>``` and ```<li>``` tags. This example demonstrates different styles and layouts achievable using only HTML and tables."

```html
<table width="100%" height="236" border="0" cellspacing="5" cellpadding="5" bgcolor="white">
        <tr>
            <td height="72" align="center" valign="top">
                <table width="900" border="1" cellspacing="0" cellpadding="8" bgcolor="#CCCCCC">
                    <tr>
                        <td width="268">
                            <font face="Verdana, Geneva, sans-serif" color="black" size="3">
                                <strong><u>ABOUT US</u></strong>
                            </font>
                        </td>
                        <td width="268">
                            <font face="Verdana, Geneva, sans-serif" color="black" size="3">
                                <strong><u>OUR VISION</u></strong>
                            </font>
                        </td>
                        <td width="290">
                            <font face="Verdana, Geneva, sans-serif" color="black" size="3">
                                <strong><u>SERVICES</u></strong>
                            </font>
                        </td>
                    </tr>
                    <tr>
                        <td>
                            <font face="Verdana, Geneva, sans-serif" color="black" size="2" contenteditable="true">
                                Click here to add your own text and edit me. It's that easy. I'm just a paragraph of text.
                                Just click "Edit Text" or double-click me to make your changes to the font. Tell a story to let your users get to know you.
                            </font>
                        </td>
                        <td valign="top">
                            <font face="Verdana, Geneva, sans-serif" color="black" size="2" contenteditable="true">
                                I'm a paragraph. Click here to add your own text and edit me. It's easy.
                                Just click "Edit Text" or double-click me to add your own content and make changes to the font. I'm a great place for you to tell a story.
                            </font>
                        </td>
                        <td valign="top">
                            <font face="Verdana, Geneva, sans-serif" color="black" size="2" contenteditable="true">
                                <ul>
                                    <li>Strategy & Organization</li>
                                    <li>Corporate Development</li>
                                    <li>Globalization</li>
                                    <li>Operations Management</li>
                                    <li>Corporate Finance</li>
                                    <li>IT Management</li>
                                </ul>
                            </font>
                        </td>
                    </tr>
                </table>
            </td>
        </tr>
    </table>
```

## Inserting the footer

```html
<table width="100%" height="60" border="0" cellspacing="5" cellpadding="5" bgcolor="#000000">
         <tr>
            <td align="center">
                <font face="Verdana, Geneva, sans-serif" color="white">
            Home - About - Services - Clients - Contractor<br />
            <br />
            &copy; 2023 by Owen Morgan.</font>
            </td>
        </tr>
</table>                                                                        
</body>
</html>
```

### HTML website creation using only tables complete. 