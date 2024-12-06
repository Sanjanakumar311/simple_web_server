# EX01 Developing a Simple Webserver

# Date:14/11/2024
# AIM:
To develop a simple webserver to serve html pages and display the configuration details of laptop.

# DESIGN STEPS:
## Step 1:
HTML content creation.

## Step 2:
Design of webserver workflow.

## Step 3:
Implementation using Python code.

## Step 4:
Serving the HTML pages.

## Step 5:
Testing the webserver.

# PROGRAM:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>laptop configuration</title>
</head>
<style>
    body{
        background-color:beige;
    }

    table{
        background-color:burlywood;
        border-collapse: collapse;
        box-shadow: 0;
        margin: 60px;
        text-align: center;
        color: black;
    }
    header{
        font-size: 420%;
        background-color: cornsilk;
    }

</style>
<body>
    <center>
        <header>
            MY LAPTOP CONFIGURATION
        </header>
    <table border="4px" width="600" height="400">
        <div class="heading">
        <tr style="font-size: x-large;">
            <th>S.NO</th>
            <th>COMPONENTS</th>
            <th>DETAILS</th>
        </tr>
        </div>
        <tr>
            <th>1</th>
            <th style="font-style: inherit;">PROCESSOR(CPU)</th>
            <td>13th Gen i5-1335U</td>
        </tr>
        <tr>
            <th>2</th>
            <th style="font-style: inherit;">MEMORY(RAM)</th>
            <td>16.0 GB</td>
        </tr>
        <tr>
            <th>3</th>
            <th style="font-style: inherit;">STORAGE</th>
            <td>512GB SSD</td>
        </tr>
        <tr>
            <th>4</th>
            <th style="font-style: inherit;">DISPLAY</th>
            <td>15.6-inch Full HD (1920x1080)</td>
        </tr>
        <tr>
            <th>5</th>
            <th style="font-style: inherit;">GRAPHICS(GPU)</th>
            <td>Integrated Intel UHD</td>
        </tr>
        <tr>
            <th>6</th>
            <th style="font-style: inherit;">BATTERY</th>
            <td>45 Wh, Up to 8 hours</td>
        </tr>
        <tr>
            <th>7</th>
            <th style="font-style: inherit;">OPERATING SYSTEM</th>
            <td>Windows 10 Home</td>
        </tr>

    </table>
    </center>
</body>
</html>

# OUTPUT:
![alt text](<Screenshot 2024-12-06 110243.png>)

![alt text](<Screenshot 2024-12-06 110323.png>)
# RESULT:
The program for implementing simple webserver is executed successfully.
