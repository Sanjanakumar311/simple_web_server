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
```python
from http.server import HTTPServer,BaseHTTPRequestHandler
content = """
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>laptop configuration</title>
</head>
<style>
    body{
        background-color: azure;
    }
    header{
        background-color: azure;
        color: rgb(53, 9, 156);
        padding: 20px 0;
        font-family: Georgia, 'Times New Roman', Times, serif;
    }
    table{
        background-color: beige;
        border-collapse: collapse;
        box-shadow: 0;
        margin: 20px;
        text-align: center;
    }

</style>
<body>
    <center>

        <header>
            <h1 style="font-size: 350%;">LAPTOP CONFIGURATION</h1>
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
            <th style="font-style: oblique;">PROCESSOR(CPU)</th>
            <td style="font-style: oblique;">13th Gen i5-1335U</td>
        </tr>
        <tr>
            <th>2</th>
            <th style="font-style: oblique;">MEMORY(RAM)</th>
            <td style="font-style: oblique;">16.0 GB</td>
        </tr>
        <tr>
            <th>3</th>
            <th style="font-style: oblique;">STORAGE</th>
            <td style="font-style: oblique;">512GB SSD</td>
        </tr>
        <tr>
            <th>4</th>
            <th style="font-style: oblique;">DISPLAY</th>
            <td style="font-style: oblique;">15.6-inch Full HD (1920x1080)</td>
        </tr>
        <tr>
            <th>5</th>
            <th style="font-style: oblique;">GRAPHICS(GPU)</th>
            <td style="font-style: oblique;">Integrated Intel UHD</td>
        </tr>
        <tr>
            <th>6</th>
            <th style="font-style: oblique;">BATTERY</th>
            <td style="font-style: oblique;">45 Wh, Up to 8 hours</td>
        </tr>
        <tr>
            <th>7</th>
            <th style="font-style: oblique;">OPERATING SYSTEM</th>
            <td style="font-style: oblique;">Windows 10 Home</td>
        </tr>
        <tr>
            <th>8</th>
            <th style="font-style: oblique;">WIFI</th>
            <td style="font-style: oblique;">Wi-Fi 5 (802.11ac)</td>
        </tr>
        <tr>
            <th>9</th>
            <th style="font-style: oblique;">PORTS</th>
            <td style="font-style: oblique;">2x USB-A, 1x USB-C, HDMI</td>
        </tr>
        <tr>
            <th>10</th>
            <th style="font-style: oblique;">KEYBOARD</th>
            <td style="font-style: oblique;">Standard, Non-backlit</td>
        </tr>

    </table>
    </center>
</body>
</html>
"""
class myhandler(BaseHTTPRequestHandler):
    def do_GET(self):
        print("request recieved")
        self.send_response(200)
        self.send_header('content-type','text/html;charset=utf-8')
        self.end_headers()
        self.wfile.write(content.encode())
server_address = ('',8000)
httpd = HTTPServer(server_address,myhandler)
print("my webserver is running...")
httpd.serve_forever()

```
# OUTPUT:

![Screenshot 2024-12-06 161830](https://github.com/user-attachments/assets/108dfea4-f5c6-45a5-81b6-f48294cc22b5)

![Screenshot 2024-12-06 161907](https://github.com/user-attachments/assets/440a522c-88a3-42d7-90cc-00b92b0c390a)

# RESULT:
The program for implementing simple webserver is executed successfully.
