# HTML Web Page Project Training 

To build this page I will be using inline style formatting which is considered outdated, but it's handy to use as a beginner to grasp some key fundamentals. CSS is now used to style pages which is much more effective with page layouts that are more responsive with mobile devices.    

When only using html, you are limited when it comes to the layout and format of the page. Without CSS I will need to insert all my objects inside tables, rows and columns.

So like I've mentioned already, using tables as layout containers has become a thing of the past but understanding tables is still important when working with tabular data. 

There'll still be many useful skill learnt from this, such as object insertion, text formatting, form development and basic styling. 

  
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

#### Now to add the nested header witin the table

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
                    <td width="338" align="left"><font face="Verdana, Geneva, sans-serif" color="black" size="5"><strong>MyBusiness</strong> <br />
                    Website</td> 

                    <td width="291" align="right"><font face="Verdana, Geneva, sans-serif" color="black" size="5"><strong>Call Today</strong> <br />
                        0121 do one</td>

                </tr>

</table>
```