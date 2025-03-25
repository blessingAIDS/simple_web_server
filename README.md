# EX01 Developing a Simple Webserver
# 24002843
# Date:25/3/25
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
~~~
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lenovo ThinkPad E16 Specifications</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            margin: 0;
            padding: 0;
        }
        header {
            background-color: #333;
            color: white;
            padding: 10px 0;
            text-align: center;
        }
        .container {
            width: 80%;
            margin: 20px auto;
            background-color: white;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            padding: 20px;
        }
        h1 {
            color: #333;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 20px;
        }
        table, th, td {
            border: 1px solid #ddd;
        }
        th, td {
            padding: 12px;
            text-align: left;
        }
        th {
            background-color: #f1f1f1;
        }
        td {
            background-color: #fafafa;
        }
        .footer {
            background-color: #333;
            color: white;
            padding: 10px 0;
            text-align: center;
            position: fixed;
            width: 100%;
            bottom: 0;
        }
        /* General Reset */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

/* Body Styling */
body {
    font-family: Arial, sans-serif;
    background-color: #f4f4f4;
    margin: 0;
    padding: 0;
}

/* Header Styling */
header {
    background-color: #333;
    color: white;
    padding: 20px 0;
    text-align: center;
}

/* Main Container */
.container {
    width: 80%;
    margin: 20px auto;
    background-color: white;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    padding: 20px;
}

/* Title Styling */
h1 {
    font-size: 2.5em;
    color: #fff;
}

h2 {
    font-size: 1.8em;
    color: #333;
    margin-bottom: 20px;
}

/* Table Styling */
table {
    width: 100%;
    border-collapse: collapse;
    margin-top: 20px;
}

th, td {
    padding: 12px;
    text-align: left;
    border: 1px solid #ddd;
}

/* Table Header Styling */
th {
    background-color: #f1f1f1;
    color: #333;
    font-weight: bold;
}

/* Table Data Row Styling */
td {
    background-color: #fafafa;
    color: #555;
}

/* Footer Styling */
.footer {
    background-color: #333;
    color: white;
    padding: 10px 0;
    text-align: center;
    position: fixed;
    width: 100%;
    bottom: 0;
}

/* Responsive Design */
@media (max-width: 768px) {
    .container {
        width: 90%;
    }

    th, td {
        font-size: 14px;
        padding: 8px;
    }

    h1 {
        font-size: 2em;
    }

    h2 {
        font-size: 1.6em;
    }
}

    </style>
</head>
<body>

<header>
    <h1  style="color: aqua;">Lenovo ThinkPad E16 Specifications</h1>
</header>

<div class="container">
    <h2 style="color: blue;">Key Specifications</h2>
    <table>
        <tr>
            <th style="color: burlywood;">Specification</th>
            <th style="color: blue;">Details</th>
        </tr>
        <tr>
            <td style="color: burlywood;">Model</td>
            <td style="color: blue;">Lenovo ThinkPad E16</td>
        </tr>
        <tr>
            <td style="color: burlywood;">Processor</td>
            <td style="color: blue;">Intel Core i5 or i7 (12th Gen)</td>
        </tr>
        <tr>
            <td style="color: burlywood;">Display</td>
            <td style="color: blue;">16.0" Full HD (1920 x 1200) IPS</td>
        </tr>
        <tr>
            <td style="color: burlywood;">Graphics</td>
            <td style="color: blue;">Intel Iris Xe Graphics</td>
        </tr>
        <tr>
            <td style="color: burlywood;">RAM</td>
            <td style="color: blue;">8GB / 16GB DDR4</td>
        </tr>
        <tr>
            <td><style="color: burlywood;">Storage</td>
            <td style="color: blue;">256GB / 512GB SSD</td>
        </tr>
        <tr>
            <td style="color: burlywood;">Battery</td>
            <td style="color: blue;">45Wh, up to 10 hours</td>
        </tr>
        <tr>
            <td style="color: burlywood;">Operating System</td>
            <td style="color: blue;">Windows 11 Pro</td>
        </tr>
        <tr>
            <td style="color: burlywood;" >Ports</td>
            <td style="color: blue;">2 x USB-A 3.2, 2 x USB-C 3.2, HDMI 2.0, RJ45 Ethernet, Audio Jack</td>
        </tr>
        <tr>
            <td style="color: burlywood;">Weight</td>
            <td style="color: blue;">1.70 kg (3.75 lbs)</td>
        </tr>
        <tr>
            <td style="color: burlywood;">Keyboard</td>
            <td style="color: blue;">Backlit Keyboard</td>
        </tr>
        <tr>
            <td style="color: burlywood;">Camera</td>
            <td style="color: blue;">720p HD Webcam</td>
        </tr>
        <tr>
            <td style="color: burlywood;">Color</td>
            <td style="color: blue;">Black</td>
        </tr>
    </table>
</div>

<div class="footer">
    <p>&copy; 2024 Lenovo. All Rights Reserved.</p>
</div>

</body>
</html>

~~~
# OUTPUT:
![Screenshot 2025-03-25 090941](https://github.com/user-attachments/assets/7bcaa6d1-3bbc-4e2b-8833-c7f8344ba75c)

![Screenshot 2025-03-25 091027](https://github.com/user-attachments/assets/b877cf4a-267a-412b-8772-acd6959d3c7c)


# RESULT:
The program for implementing simple webserver is executed successfully.
