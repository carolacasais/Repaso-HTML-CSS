# Revision de CCS3

Descripcion:
En este ejercicio vemos las características más destacadas de CSS.

#### Selectors

##### Change the color of all p elements to "red".
        <!DOCTYPE html>
        <html>
            <head>
                <style>
                    p{
                        color:red;
                    }
                </style>
            </head>
            <body>
                <h1>This is a Heading</h1>
                <p>This is a paragraph.</p>
                <p>This is another paragraph.</p>
            </body>
        </html>

##### Change the color of the element with id="para1", to "red".
        <!DOCTYPE html>
        <html>
            <head>
                <style>
                    #para1 {
                        color:red;
                    }
                    
                </style>
            </head>
            <body>
                <h1>This is a Heading</h1>
                <p id="para1">This is a paragraph.</p>
                <p>This is another paragraph.</p>
            </body>
        </html>

##### Change the color of all elements with the class "colortext", to "red".
        <!DOCTYPE html>
        <html>
            <head>
                <style>
                    .colortext {
                        color:red;
                    }
                </style>
            </head>
            <body>
                <h1>This is a Heading</h1>
                <p>This is a paragraph.</p>
                <p class="colortext">This is another paragraph.</p>
                <p class="colortext">This is also a paragraph.</p>
            </body>
        </html>

##### Change the color of all p and &lth1> elements, to "red". Group the selectors to minimize code.
        <!DOCTYPE html>
        <html>
            <head>
                <style>
                    h1, p {
                        color:red;
                    }
                </style>
            </head>
            <body>
                <h1>This is a Heading</h1>
                <h2>This is a smaller Heading</h2>
                <p>This is a paragraph.</p>
                <p>This is another paragraph.</p>
            </body>
        </html>

#### How to...

##### Add an external style sheet with the URL: "mystyle.css".
        <!DOCTYPE html>
        <html>
            <head>
                <link rel="stylesheet" href="mystyle.css">
            </head>
            <body>
                <h1>This is a Heading</h1>
                <p>This is a paragraph.</p>
                <p>This is another paragraph.</p>
            </body>
        </html>

##### Set "background-color: linen" for the page, using an internal style sheet.
        <!DOCTYPE html>
        <html>
            <head>
                <style>
                    body {
                        background-color: linen;
                    }
                </style>
            </head>
            <body>
                <h1>This is a Heading</h1>
                <p>This is a paragraph.</p>
                <p>This is another paragraph.</p>
            </body>
        </html>

##### Set "background-color: linen" for the page, using an inline style.
        <!DOCTYPE html>
        <html>
            <head>
            </head>
            <body>
                <body style="background-color: linen;">
                <h1>This is a Heading</h1>
                <p>This is a paragraph.</p>
                <p>This is another paragraph.</p>
            </body>
        </html>

##### Remove all styles, except the external style sheet "mystyle.css".
        <!DOCTYPE html>
        <html>
            <head>
                <link rel="stylesheet" href="mystyle.css">
            </head>
            <body>
                <h1>This is a Heading</h1>
                <p>This is a paragraph.</p>
                <p>This is another paragraph.</p>
            </body>
        </html>

#### Background

##### Set the background color for the page to "linen" and the background color for h1 to "lightblue".
        <!DOCTYPE html>
        <html>
            <head>
                <style>
                body {
                    background-color:linen;
                }
                h1 {
                    background-color:lightblue;
                }
                </style>
            </head>
            <body>
                <h1>This is a Heading</h1>
                <p>This is a paragraph.</p>
                <p>This is another paragraph.</p>
            </body>
        </html>

##### Set "paper.gif" as the background image of the page.
        <!DOCTYPE html>
        <html>
            <head>
                <style>
                body {
                    background-image: url("paper.gif");
                }
                </style>
            </head>
            <body>
                <h1>This is a Heading</h1>
                <p>This is a paragraph.</p>
                <p>This is another paragraph.</p>
            </body>
        </html>

##### Set "gradient_bg_vertical.png" as the background image of the page, and repeat it vertically only.
        <!DOCTYPE html>
        <html>
            <head>
                <style>
                body {
                    background-image: url("gradient_bg_vertical.png");
                    background-repeat: repeat-y;
                }
                </style>
            </head>
            <body>
                <h1>This is a Heading</h1>
                <p>This is a paragraph.</p>
                <p>This is another paragraph.</p>
            </body>
        </html>

##### Specify that the background image should be shown once, in the top right corner.
        <!DOCTYPE html>
        <html>
            <head>
                <style>
                body {
                    background-image: url("img_tree.png");
                    background-repeat: no-repeat;
                    background-position: top right;
                }
                </style>
            </head>
            <body>
                <h1>This is a Heading</h1>
                <p>This is a paragraph.</p>
                <p>This is another paragraph.</p>
            </body>
        </html>

##### Use the shorthand background property to set background image to "img_tree.png", show it once, in the top right corner.
        <!DOCTYPE html>
        <html>
            <head>
                <style>
                body {
                    background: url("img_tree.png") no-repeat top right;
                }
                </style>
            </head>
            <body>
                <h1>This is a Heading</h1>
                <p>This is a paragraph.</p>
                <p>This is another paragraph.</p>
            </body>
        </html>

#### Border

##### Set a "4px", "dotted" border for p.
        <!DOCTYPE html>
        <html>
            <head>
                <style>
                p {
                    border-style: dotted;
                    border-width: 4px;
                }
                </style>
            </head>
            <body>
                <h1>This is a Heading</h1>
                <p>This is a paragraph.</p>
            </body>
        </html>

##### Set the border color for p to "red".
        <!DOCTYPE html>
        <html>
            <head>
                <style>
                p {
                    border-style: dotted;
                    border-width: 4px;
                    border-color: red;
                }
                </style>
            </head>
            <body>
                <h1>This is a Heading</h1>
                <p>This is a paragraph.</p>
            </body>
        </html>

##### Change the 3 border properties, so that they only show the border on the top side.
        <!DOCTYPE html>
        <html>
            <head>
                <style>
                p {
                    border-top-style: dotted;
                    border-top-width: 4px;
                    border-top-color: red;
                }
                </style>
            </head>
            <body>
                <h1>This is a Heading</h1>
                <p>This is a paragraph.</p>
            </body>
        </html>

##### With the border property: Set the border for p to "10px", "solid" and "green".
        <!DOCTYPE html>
        <html>
            <head>
                <style>
                p {
                    border: 10px solid green;
                }
                </style>
            </head>
            <body>
                <h1>This is a Heading</h1>
                <p>This is a paragraph.</p>
            </body>
        </html>

#### Margin

##### Set the left margin of h1 to "20px".
        <!DOCTYPE html>
        <html>
            <head>
                <style>
                h1 {
                    background-color: lightblue;
                    margin-left:20px;
                }
                </style>
            </head>
            <body>
                <h1>This is a Heading</h1>
                <p>This is a paragraph.</p>
            </body>
        </html>

##### Set all margins for &lth1> to "25px".
        <!DOCTYPE html>
        <html>
            <head>
                <style>
                h1 {
                    background-color: lightblue;
                    margin: 25px
                }
                </style>
            </head>
            <body>
                <h1>This is a Heading</h1>
                <p>This is a paragraph.</p>
            </body>
        </html>

##### Use the margin property to set the top and bottom margins for h1 to "50px", and left and right margins to "25px".
        <!DOCTYPE html>
        <html>
            <head>
                <style>
                h1 {
                    background-color: lightblue;
                    margin: 50px, 25px;
                }
                </style>
            </head>
            <body>
                <h1>This is a Heading</h1>
                <p>This is a paragraph.</p>
            </body>
        </html>

##### Use the margin property to center align the &lth1> element. Use the margin property to set the top and bottom margins for &lth1> to "50px", and left and right margins to "25px".
        <!DOCTYPE html>
        <html>
            <head>
                <style>
                h1 {
                    background-color: lightblue;
                    width: 300px;
                    margin: auto;
                }
                </style>
            </head>
            <body>
                <h1>This is a Heading</h1>
                <p>This is a paragraph.</p>
            </body>
        </html>



#### Padding

##### Set the top padding of &ltp> to "30px".
        <!DOCTYPE html>
        <html>
            <head>
                <style>
                p {
                    background-color: lightblue;
                    padding-top: 30px;
                }
                </style>
            </head>
            <body>
                <h1>This is a Heading</h1>
                <p>This is a paragraph.</p>
            </body>
        </html>

##### Set all paddings for &ltp> to "50px".
        <!DOCTYPE html>
        <html>
            <head>
                <style>
                p {
                    background-color: lightblue;
                    padding: 50px;
                }
                </style>
            </head>
            <body>
                <h1>This is a Heading</h1>
                <p>This is a paragraph.</p>
            </body>
        </html>

##### Use the padding property to set the top and bottom paddings for &ltp> to "25px", and left and right paddings to "50px".
        <!DOCTYPE html>
        <html>
            <head>
                <style>
                p {
                    background-color: lightblue;
                    padding: 25px 50px;
                }
                </style>
            </head>
            <body>
                <h1>This is a Heading</h1>
                <p>This is a paragraph.</p>
            </body>
        </html>

#### Height/Width

##### Set the height of &lth1> to "100px".
        <!DOCTYPE html>
        <html>
            <head>
                <style>
                h1 {
                    background-color: lightblue;
                    height: 100px;
                }
                </style>
            </head>
            <body>
                <h1>This is a Heading</h1>
                <p>This is a paragraph.</p>
            </body>
        </html>

##### Set the width of &lth1> to "50%".
        <!DOCTYPE html>
    <html>
        <head>
            <style>
            h1 {
                background-color: lightblue;
                width: 50%;
            }
            </style>
        </head>
        <body>
            <h1>This is a Heading</h1>
            <p>This is a paragraph.</p>
        </body>
    </html>

#### Box Model

##### Set the width of the div to "200px".
        <!DOCTYPE html>
    <html>
        <head>
            <style>
            div {
                background-color: lightblue;
                width: 200px;
            }
            </style>
        </head>
        <body>
            <div>Lorem ipsum dolor sit amet, consectetur adipiscing elit, 
            sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</div>
        </body>
    </html>

##### Set the padding of the div to "25px".
        <!DOCTYPE html>
        <html>
            <head>
                <style>
                div {
                    background-color: lightblue;
                    width: 200px;
                    padding: 25px;
                }
                </style>
            </head>
            <body>
                <div>Lorem ipsum dolor sit amet, consectetur adipiscing elit, 
            s   ed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</div>
            </body>
        </html>

##### Set the border of the div to "25px solid navy".
        <!DOCTYPE html>
        <html>
            <head>
                <style>
                div {
                    background-color: lightblue;
                    width: 200px;
                    padding: 25px;
                    border: 25px solid navy;
                }
                </style>
            </head>
            <body>
                <div>Lorem ipsum dolor sit amet, consectetur adipiscing elit, 
                sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</div>
            </body>
        </html>

##### Set the margin of the div to "25px".
        <!DOCTYPE html>
        <html>
            <head>
                <style>
                div {
                    background-color: lightblue;
                    width: 200px;
                    padding: 25px;
                    border: 25px solid navy;
                    margin: 25px;
                }
                </style>
            </head>
            <body>
                <div>Lorem ipsum dolor sit amet, consectetur adipiscing elit, 
                sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</div>
            </body>
        </html>


#### Outline

##### Set a "solid", "5px" outline for p.
        <!DOCTYPE html>
    <html>
        <head>
            <style>
            p {
                outline-style: solid;
                outline-width: 5px;
            }
            </style>
        </head>
        <body>
            <h1>This is a Heading</h1>
            <p>This is a paragraph.</p>
        </body>
    </html>

##### Set the outline color for p to "green".
        <!DOCTYPE html>
    <html>
        <head>
            <style>
            p {
                outline-style: solid;
                outline-width: 4px;
                outline-color: green;
            }
            </style>
        </head>
        <body>
            <h1>This is a Heading</h1>
            <p>This is a paragraph.</p>
        </body>
    </html>

##### With the outline property: Set the outline for p to "red", "dotted" and "10px".
        <!DOCTYPE html>
    <html>
        <head>
            <style>
            p {
                outline: red dotted 10px;
            }
            </style>
        </head>
        <body>
            <h1>This is a Heading</h1>
            <p>This is a paragraph.</p>
        </body>
    </html>



#### Text

##### Set the text color for the page to "red", and the text color for &lth1> to "blue".
        <!DOCTYPE html>
    <html>
        <head>
            <style>
            body {
                color: red;
            }
            h1 {
                color: blue;
            }
            </style>
        </head>
        <body>
            <h1>This is a Heading</h1>
            <p>This is a paragraph.</p>
        </body>
    </html>

##### Center align the &lth1> element.
        <!DOCTYPE html>
            <html>
                <head>
                    <style>
                    h1 {
                        text-align: center;
                    }
                    </style>
                </head>
                <body>
                    <h1>This is a Heading</h1>
                    <p>This is a paragraph.</p>
                    <p>This is another paragraph.</p>
                </body>
            </html>

##### Remove the underline from the link.
        <!DOCTYPE html>
            <html>
                <head>
                    <style>
                    a {
                        text-decoration: none;
                    }
                    </style>
                </head>
                <body>
                    <h1>This is a Heading</h1>
                    <p>This is a paragraph.</p>
                    <p><a href="css_text.asp">CSS text tutorial</a></p>
                </body>
            </html>

##### Style text in &lth1> to uppercase letters, and text in &ltp> to capitalized letters.
        <!DOCTYPE html>
            <html>
                <head>
                    <style>
                    h1 {
                        text-transform: uppercase;
                    }
                    p {
                        text-transform: capitalize;
                    }
                    </style>
                </head>
                <body>
                    <h1>This is a Heading</h1>
                    <p>This is a paragraph.</p>
                    <p>This is another paragraph.</p>
                </body>
            </html>

##### Indent the first line of the &ltp> element with 20px.
        <!DOCTYPE html>
            <html>
                <head>
                    <style>
                    p {
                        text-indent: 20px;
                    }
                    </style>
                </head>
                <body>
                    <h1>This is a Heading</h1>
                    <p> Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor 
                        incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud
                        exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure 
                        dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
                        Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit 
                        anim id est laborum </p>
                </body>
            </html>


#### Font

##### Set the font family for the page to "Courier New", and the font family for &lth1> to "Verdana".
        <!DOCTYPE html>
            <html>
                <head>
                    <style>
                    body {
                        font-family: 'Courier New';
                    }
                    h1 {
                        font-family: Verdana;
                    }
                    </style>
                </head>
                <body>
                    <h1>This is a Heading</h1>
                    <p>This is a paragraph.</p>
                    <p>This is another paragraph.</p>
                </body>
            </html>

##### Show p elements as "italic" text.
        <!DOCTYPE html>
            <html>
                <head>
                    <style>
                    p {
                        font-style: italic;
                    }
                    </style>
                </head>
                <body>
                    <h1>This is a Heading</h1>
                    <p>This is a paragraph.</p>
                    <p>This is another paragraph.</p>
                </body>
            </html>

##### Set the font size for the page to "20px", and the font size for &lth1> to "3em".
        <!DOCTYPE html>
            <html>
                <head>
                    <style>
                    body{
                        font-size: 20px;
                    }
                    h1{
                        font-size: 3em;
                    }
                    </style>
                </head>
                <body>
                    <h1>This is a Heading</h1>
                    <p>This is a paragraph.</p>
                    <p>This is another paragraph.</p>
                </body>
            </html>

##### Show &ltp> elements as "bold" text.
        <!DOCTYPE html>
            <html>
                <head>
                    <style>
                    p {
                        font-weight: bold;
                    }
                    </style>
                </head>
                <body>
                    <h1>This is a Heading</h1>
                    <p>This is a paragraph.</p>
                    <p>This is another paragraph.</p>
                </body>
            </html>

##### With the font property: Set the &ltp> to "italic", "20px" and "Verdana".
        <!DOCTYPE html>
            <html>
                <head>
                    <style>
                    p {
                        font: italic 20px Verdana;
                    }
                    </style>
                </head>
                <body>
                    <h1>This is a Heading</h1>
                    <p>This is a paragraph.</p>
                    <p>This is another paragraph.</p>
                </body>
            </html>



#### Links

##### Set the color for links to "green".
        <!DOCTYPE html>
            <html>
                <head>
                    <style>
                    a {
                        color: green;
                    }
                    </style>
                </head>
                <body>
                    <h1>This is a Heading</h1>
                    <p>This is a paragraph.</p>
                    <p><a href="https://www.w3schools.com">W3Schools.com</a></p>
                </body>
            </html>

##### Set the color for unvisited links to "red", and the color for visited links "blue".
        <!DOCTYPE html>
            <html>
                <head>
                    <style>
                        /* unvisited link */
                        a:link {
                            color: red;
                        }

                        /* visited link */
                        a:visited {
                            color: blue;
                        }

                        /* mouse over link */
                        a:hover {
                            color: black;
                        }
                        
                        /* selected link */
                        a:active{
                            color: green;
                        }

                    </style>
                </head>
                <body>
                    <h1>This is a Heading</h1>
                    <p>This is a paragraph.</p>
                    <p><a href="https://www.w3schools.com">W3Schools.com</a></p>
                </body>
            </html>

##### Remove underlines for visited and unvisited links, and specify "underline" for the hover and active link states.
        <!DOCTYPE html>
            <html>
                <head>
                    <style>
                        /* unvisited link */
                        a:link {
                            text-decoration: none;
                        }

                        /* visited link */
                        a:visited {
                            text-decoration: none;
                        }

                        /* mouse over link */
                        a:hover {
                            text-decoration: underline;
                        }
                        
                        /* selected link */
                        a:active{
                            text-decoration: underline;
                        }

                    </style>
                </head>
                <body>
                    <h1>This is a Heading</h1>
                    <p>This is a paragraph.</p>
                    <p><a href="https://www.w3schools.com">W3Schools.com</a></p>
                </body>
            </html>

##### Set the background color for visited and unvisited links to "lightblue", and the background color for the hover and active link states to "yellow".
        <!DOCTYPE html>
            <html>
                <head>
                    <style>
                        /* unvisited link */
                        a:link {
                            background-color: lightblue;
                        }

                        /* visited link */
                        a:visited {
                            background-color: lightblue;
                        }

                        /* mouse over link */
                        a:hover {
                            background-color: yellow;
                        }
                        
                        /* selected link */
                        a:active{
                            background-color: yellow;
                        }

                    </style>
                </head>
                <body>
                    <h1>This is a Heading</h1>
                    <p>This is a paragraph.</p>
                    <p><a href="https://www.w3schools.com">W3Schools.com</a></p>
                </body>
            </html>

#### List

##### Set the list style for unordered lists to "square", and the list style for ordered lists to "upper-roman".
        <!DOCTYPE html>
            <html>
                <head>
                    <style>
                        ul{
                            list-style-type: square;
                        }
                        ol {
                            list-style-type: upper-roman;
                        }
                    </style>
                </head>
                <body>
                    <p>This is an unordered list:</p>
                    <ul>
                        <li>Coffee</li>
                        <li>Tea</li>
                        <li>Coca Cola</li>
                    </ul>

                    <p>This is an ordered list:</p>
                    <ol>
                        <li>Coffee</li>
                        <li>Tea</li>
                        <li>Coca Cola</li>
                    </ol>
                </body>
            </html>

##### Set the image "sqpurple.gif" as the list item marker for the unordered list.
        <!DOCTYPE html>
            <html>
                <head>
                    <style>
                        ul{
                            list-style-image: url("sqpurple.gif");
                        }
                        
                    </style>
                </head>
                <body>
                    <p>This is an unordered list:</p>
                    <ul>
                        <li>Coffee</li>
                        <li>Tea</li>
                        <li>Coca Cola</li>
                    </ul>

                </body>
            </html>

##### With the list-style property: Set the unordered list marker to "img_marker.png", with a backup style of "circle", and display the markers inside the content flow.
        <!DOCTYPE html>
            <html>
                <head>
                    <style>
                        ul{
                            list-style: circle inside url('img_marker.png');
                        }
                        
                    </style>
                </head>
                <body>
                    <p>This is an unordered list:</p>
                    <ul>
                        <li>Coffee</li>
                        <li>Tea</li>
                        <li>Coca Cola</li>
                    </ul>

                </body>
            </html>

##### Remove the bullets/markers from the list items.
        <!DOCTYPE html>
            <html>
                <head>
                    <style>
                        ul{
                            list-style-type: none;
                        }
                        
                    </style>
                </head>
                <body>
                    <p>This is an unordered list:</p>
                    <ul>
                        <li>Coffee</li>
                        <li>Tea</li>
                        <li>Coca Cola</li>
                    </ul>

                </body>
            </html>

#### Tables

##### Set the border to "2px solid green" for table, th and td elements.
        <!DOCTYPE html>
            <html>
                <head>
                    <style>
                        table, th, td {
                            border: 2px solid green;
                        }
                    </style>
                </head>
                <body>
                    <table>
                        <tr>
                            <th>Firstname</th>
                            <th>Lastname</th>
                        </tr>
                        <tr>
                            <td>Peter</td>
                            <td>Griffin</td>
                        </tr>
                        <tr>
                            <td>Lois</td>
                            <td>Griffin</td>
                        </tr>
                    </table>
                </body>

            </html>

##### Collapse the table borders into a single border.
        <!DOCTYPE html>
            <html>
                <head>
                    <style>
                        table {
                            border-collapse: collapse;
                        }
                        table, th, td {
                            border: 1px solid black;
                        }
                    </style>
                </head>
                <body>
                    <table>
                        <tr>
                            <th>Firstname</th>
                            <th>Lastname</th>
                        </tr>
                        <tr>
                            <td>Peter</td>
                            <td>Griffin</td>
                        </tr>
                        <tr>
                            <td>Lois</td>
                            <td>Griffin</td>
                        </tr>
                    </table>
                </body>

            </html>

##### Set the width of the table to "100%".
        <!DOCTYPE html>
            <html>
                <head>
                    <style>
                        table {
                            width: 100%;
                        }
                        table, th, td {
                            border: 1px solid black;
                        }
                    </style>
                </head>
                <body>
                    <table>
                        <tr>
                            <th>Firstname</th>
                            <th>Lastname</th>
                        </tr>
                        <tr>
                            <td>Peter</td>
                            <td>Griffin</td>
                        </tr>
                        <tr>
                            <td>Lois</td>
                            <td>Griffin</td>
                        </tr>
                    </table>
                </body>

            </html>

##### Set the text alignment in td elements to "right".
        <!DOCTYPE html>
            <html>
                <head>
                    <style>
                        table, th, td {
                            border: 1px solid black;
                        }
                        td {
                            text-align: right;
                        }
                    </style>
                </head>
                <body>
                    <table>
                        <tr>
                            <th>Firstname</th>
                            <th>Lastname</th>
                        </tr>
                        <tr>
                            <td>Peter</td>
                            <td>Griffin</td>
                        </tr>
                        <tr>
                            <td>Lois</td>
                            <td>Griffin</td>
                        </tr>
                    </table>
                </body>

            </html>

##### Set the padding in &ltth> elements to "15px".
        <!DOCTYPE html>
            <html>
                <head>
                    <style>
                        table, th, td {
                            border: 1px solid black;
                        }
                        th {
                            padding: 15px;
                        }
                    </style>
                </head>
                <body>
                    <table>
                        <tr>
                            <th>Firstname</th>
                            <th>Lastname</th>
                        </tr>
                        <tr>
                            <td>Peter</td>
                            <td>Griffin</td>
                        </tr>
                        <tr>
                            <td>Lois</td>
                            <td>Griffin</td>
                        </tr>
                    </table>
                </body>

            </html>

##### Set the background color of &ltth> elements to "lightblue".
        <!DOCTYPE html>
            <html>
                <head>
                    <style>
                        table, th, td {
                            border: 1px solid black;
                        }
                        th {
                            background-color: lightblue;
                        }
                    </style>
                </head>
                <body>
                    <table>
                        <tr>
                            <th>Firstname</th>
                            <th>Lastname</th>
                        </tr>
                        <tr>
                            <td>Peter</td>
                            <td>Griffin</td>
                        </tr>
                        <tr>
                            <td>Lois</td>
                            <td>Griffin</td>
                        </tr>
                    </table>
                </body>

            </html>




#### Display/visibility

##### Hide the &lth1> element. It should still take up the same space as before.
        <!DOCTYPE html>
            <html>
                <head>
                    <style>
                        h1 {
                            visibility: hidden;
                        }
                    </style>
                </head>
                <body>
                    <h1>This is a Heading</h1>
                    <p>This is a paragraph.</p>
                    <p>This is another paragraph.</p>
                </body>
            </html>

##### Hide the h1 element. It should not take up any space.
        <!DOCTYPE html>
            <html>
                <head>
                    <style>
                        h1 {
                            display: none;
                        }
                    </style>
                </head>
                <body>
                    <h1>This is a Heading</h1>
                    <p>This is a paragraph.</p>
                    <p>This is another paragraph.</p>
                </body>
            </html>

##### Display the list items as inline elements.
        <!DOCTYPE html>
            <html>
                <head>
                    <style>
                        li {
                            display: inline;
                        }
                    </style>
                </head>
                <body>
                    <h1>This is a heading</h1>
                    <ul>
                        <li>Apple</li>
                        <li>Orange</li>
                        <li>Pear</li>
                    </ul>
                </body>
            </html>

##### Display the strong elements as block elements.
        <!DOCTYPE html>
            <html>
                <head>
                    <style>
                        strong {
                            display: block;
                        }
                    </style>

                </head>
                <body>
                    <h1>This is a heading</h1>
                    <p>This is a <strong>paragraph</strong> with some words more <strong> important </strong> than others. </p>
                    <p>This is another paragraph.</p>
                </body>

            </html>

#### Positioning

##### Position the &lth1> element to always be 50px from the top, and 50px from the right, relative to the window/frame edges.
        <!DOCTYPE html>
            <html>
                <head>
                    <style>
                        h1 {
                            position: fixed;
                            top: 50px;
                            right: 50px;
                            color: red;
                        }
                    </style>
                </head>
                <body>
                    <h1>This is a Heading</h1>
                    <p>This is a paragraph</p>
                    <p>This is another paragraph</p>
                </body>
            </html>

##### Position the h1 element 20px left, and 30px down, relative to its normal position.
        <!DOCTYPE html>
            <html>
                <head>
                    <style>
                        h1 {
                            position: relative;
                            top: 30px;
                            left: -20px;
                            color: red;
                        }
                    </style>
                </head>
                <body>
                    <h1>This is a Heading</h1>
                    <p>This is a paragraph</p>
                    <p>This is another paragraph</p>
                </body>
            </html>

##### Position the h1 element 50px from the left, and 100px from the top, relative to the HTML page.
        <!DOCTYPE html>
            <html>
                <head>
                    <style>
                        h1 {
                            position: absolute;
                            top: 100px;
                            left: 50px;
                            color: red;
                        }
                    </style>
                </head>
                <body>
                    <h1>This is a Heading</h1>
                    <p>This is a paragraph</p>
                    <p>This is another paragraph</p>
                </body>
            </html>

##### Position the img element behind the text.
        <!DOCTYPE html>
            <html>
                <head>
                    <style>
                        img {
                            position: absolute;
                            top: 0px;
                            left: 0px;
                        }
                    </style>
                </head>
                <body>
                    <h1>This is a Heading</h1>
                    <p>This is a paragraph</p>
                    <p>This is another paragraph</p>
                    <img src="smiley.gif" width="100" height="140">
                </body>
            </html>

##### Position the element with the "topleft" class 30px from the left, and 15px from the top, relative to its container.
        <!DOCTYPE html>
            <html>
            <head>
            <style>
            .container {
                position: relative;
            }

            .topleft {
                position: absolute;
                left: 30px;
                top: 15px;
                font-size: 18px;
            }

            img {
                width: 100%;
                height: auto;
                opacity: 0.3;
            }
            </style>
            </head>
            <body>

            <div class="container">
            <img src="img_5terre.jpg" alt="Cinque Terre" width="1000" height="300">
            <div class="topleft">Top Left</div>
            </div>


            </body>
            </html>

#### Overflow

##### Add a scrollbar to the div element.
        <!DOCTYPE html>
            <html>
            <head>
            <style>
                div {
                background-color: #eee;
                width: 200px;
                height: 70px;
                border: 1px dotted black;
                overflow: scroll;
            }
            </style>
            </head>
            <body>  

            <div>
            <p>In my younger and more vulnerable years my father gave me some advice that I've been turning over in my mind ever since.</p>
            <p>'Whenever you feel like criticizing anyone,' he told me, 'just remember that all the people in this world haven't had the advantages that you've had.'</p>
            </div>

            </body>
            </html>

##### Specify that the overflowing text in the &ltdiv> element should not be visible, not even with scrolling.
        <!DOCTYPE html>
            <html>
            <head>
            <style>
                div {
                background-color:lightblue;
                width: 200px;
                height: 200px;
                overflow: hidden;
            }
            </style>
            </head>
            <body>  

            <div>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
                incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud 
                exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure 
                dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. 
                Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit 
                anim id est laborum. </div>

            </body>
            </html>

##### Add a horizontal scrollbar to div.
        <!DOCTYPE html>
            <html>
            <head>
            <style>
                div {
                background-color:#eee;
                width: 150px;
                height: 70px;
                border: 1pz dotted black;
                white-space: nowrap;
                overflow-x:scroll;
            }
            </style>
            </head>
            <body>  

            <div><p>In my younger and more vulnerable years my father gave me some
            advice that I've been turning over in my mind ever since.</p> </div>

            </body>
            </html>

#### Align

##### Center align the div element using margins.
        <!DOCTYPE html>
            <html>
            <head>
            <style>
                div {
                margin-left: auto;
                margin-right: auto;
                width: 300px;
                background-color: #b0e0e6;
            }
            </style>
            </head>
            <body>  

            <div><p>In my younger and more vulnerable years my father gave me some
            advice tha#b0e0e6t I've been turning over in my mind ever since.</p> 
            <p>'Whenever you feel like criticizing anyone,' he told me, 'just remember 
                that all the people in this world haven't had the advantages that you've had.'</p> 
            </div>

            </body>
            </html>

##### Position the &ltdiv> element all the way to the right using absolute positioning.
        Example:
            <!DOCTYPE html>
            <html>
            <head>
            <style>
                div {
                position: absolute;
                right: 0px;
                width: 300px;
                background-color: #b0e0e6;
            }
            </style>
            </head>
            <body>  

            <div><p>In my younger and more vulnerable years my father gave me some
            advice tha#b0e0e6t I've been turning over in my mind ever since.</p> 
            <p>'Whenever you feel like criticizing anyone,' he told me, 'just remember 
                that all the people in this world haven't had the advantages that you've had.'</p> 
            </div>

            </body>
            </html>

#### Combinators

##### Change the color of all p elements, that are descendants of %ltdiv> elements, to "red".
        <!DOCTYPE html>
            <html>
            <head>
            <style>
            div p {
                color: red;
            }
            </style>
            </head>
            <body>

            <div>
                <p>This is a paragraph inside a div element.</p>
                <p>This is another paragraph inside a div element.</p>
                <span><p>This a paragraph inside a span element, inside a div element.</p></span>
            </div>

            <p>This is a paragraph, not inside a div element.</p>
            <p>This is another paragraph, not inside a div element.</p>

            </body>
            </html>

##### Change the color of all p elements, that are immediate children of div elements, to "red".
        <!DOCTYPE html>
            <html>
            <head>
            <style>
            div > p {
                color: red;
            }
            </style>
            </head>
            <body>

            <div>
                <p>This is a paragraph inside a div element.</p>
                <p>This is another paragraph inside a div element.</p>
                <span><p>This a paragraph inside a span element, inside a div element.</p></span>
            </div>

            <p>This is a paragraph, not inside a div element.</p>
            <p>This is another paragraph, not inside a div element.</p>

            </body>
            </html>

##### Change the color of p elements, that are the adjacent (immediately following) sibling of a div element, to "red".
        <!DOCTYPE html>
            <html>
            <head>
            <style>
            div + p {
                color: red;
            }
            </style>
            </head>
            <body>

            <div>
                <p>This is a paragraph inside a div element.</p>
                <p>This is another paragraph inside a div element.</p>
                <span><p>This a paragraph inside a span element, inside a div element.</p></span>
            </div>

            <p>This is a paragraph, not inside a div element.</p>
            <p>This is another paragraph, not inside a div element.</p>

            </body>
            </html>

##### Change the color of p elements, that are the siblings of a div element, to "red".
        <!DOCTYPE html>
            <html>
            <head>
            <style>
            div ~ p {
                color: red;
            }
            </style>
            </head>
            <body>

            <div>
                <p>This is a paragraph inside a div element.</p>
                <p>This is another paragraph inside a div element.</p>
                <span><p>This a paragraph inside a span element, inside a div element.</p></span>
            </div>

            <p>This is a paragraph, not inside a div element.</p>
            <p>This is another paragraph, not inside a div element.</p>

            </body>
            </html>

#### Pseudo-classes

##### Set the background color for visited and unvisited links to "lightblue", and the background color for the hover and active link states to "yellow".
        <!DOCTYPE html>
            <html>
                <head>
                    <style>
                        /* unvisited link */
                        a:link {
                            background-color: lightblue;
                        }

                        /* visited link */
                        a:visited {
                            background-color: lightblue;
                        }

                        /* mouse over link */
                        a:hover {
                            background-color: yellow;
                        }
                        
                        /* selected link */
                        a:active{
                            background-color: yellow;
                        }

                    </style>
                </head>
                <body>
                    <h1>This is a Heading</h1>
                    <p>This is a paragraph.</p>
                    <p><a href="https://www.w3schools.com">W3Schools.com</a></p>
                </body>
            </html>

##### Change the background color, when a user hovers over p elements, with the class "highlight", to "lightblue".
        <!DOCTYPE html>
            <html>
            <head>
            <style>
            p.highlight:hover {
            background-color: lightblue;
            }
            </style>
            </head>         
            <body>

            <h1>This is a Heading</h1>
            <p>This is a paragraph.</p>
            <p class="highlight">This is another paragraph.</p>

            </body>
            </html>

##### Set the background color of &ltp> elements, that are the first child of any element, to "lightblue".
        <!DOCTYPE html>
            <html>
            <head>
            <style>
            p:first-child {
                background-color: lightblue;
            }
            </style>
            </head>
            <body>

            <p>This is a paragraph.</p>
            <p>This is also a paragraph</p>

            </body>
            </html>

##### Set the background color of input elements that are in focus (clicked or active), to "lightblue".
        <!DOCTYPE html>
            <html>
            <head>
            <style>
            input:focus {
                background-color: lightblue;
            }
            </style>
            </head>
            <body>

            <form action="/action_page.php" method="get">
            First name: <input type="text" name="fname"><br>
            Last name: <input type="text" name="lname"><br>
            <input type="submit" value="Submit">
            </form>

            </body>
            </html> 

#### Pseudo-elements



#### Opacity

#### Attribute Selectors

#### Rounded Corners

#### Border Images

#### Backgrounds

#### Colors

#### Gradients

#### Shadow Effects

#### Text Effects

#### Web Fonts

#### 2D Transforms

#### 3D Transforms

#### Transitions

#### Animations

