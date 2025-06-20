# Ex03 Time Table
## Date:24.04.2025

## AIM
To write a html webpage page to display your slot timetable.

## ALGORITHM
### STEP 1
Create a Django-admin Interface.

### STEP 2
Create a static folder and inert HTML code.

### STEP 3
Create a simple table using ```<table>``` tag in html.

### STEP 4
Add header row using ```<th>``` tag.

### STEP 5
Add your timetable using ```<td>``` tag.

### STEP 6
Execute the program using runserver command.

## PROGRAM
<DOCTYPE HTML>
    <html>
        <head>
            <title>Official Timetable</title>
            <style>
                :root {
                    --primary-color: #b3225a;
                    --secondary-color: #cae9ff;
                    --text-color: #222;
                    --bg-color: #f4f4f4;
                    --border-color: #111412;
                    --header-bg: #3d43f7;
                    --header-text: white;
                    --highlight-bg: #1c78f0;
                    --highlight-text: white;
                }
        
                body {
                    font-family: 'Poppins', sans-serif;
                    background: var(--bg-color);
                    color: var(--text-color);
                    padding: 30px;
                }
        
                .container {
                    max-width: 1000px;
                    margin: auto;
                    background: white;
                    padding: 40px;
                    border-radius: 10px;
                    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
                    border: 2px solid var(--border-color);
                }
        
                .header {
                    text-align: center;
                    margin-bottom: 10px;
                }
        
                .header img {
                    max-width: 500px;
                    height: auto;
                    display: block;
                    margin: 0 auto;
                }
        
                h1 {
                    font-size: 35px;
                    margin-top: 10px;
                    color: var(--primary-color);
                    letter-spacing: 1px;
                    font-weight: 600;
                }
        
                .info {
                    text-align: center;
                    font-size: 20px;
                    margin-bottom: 10px;
                    font-weight: 500;
                }
        
                table {
                    width: 100%;
                    border-collapse: collapse;
                    margin-bottom: 30px;
                }
        
                th, td {
                    border: 2px solid var(--border-color);
                    padding: 12px;
                    text-align: center;
                    font-size: 14px;
                }
        
                th {
                    background-color: var(--header-bg);
                    color: var(--header-text);
                    font-weight: 600;
                }
        
                td.day {
                    background-color: var(--highlight-bg);
                    color: var(--highlight-text);
                    font-weight: bold;
                }
        
                td.lunch {
                    background-color: var(--secondary-color);
                    font-weight: bold;
                }
        
                tr:nth-child(even) {
                    background-color: var(--secondary-color);
                }
        
                .subject-title {
                    font-size: 26px;
                    text-align: center;
                    font-weight: 600;
                    margin-bottom: 15px;
                    color: var(--primary-color);
                }
        
                .subject-table th {
                    background-color: var(--header-bg);
                    color: var(--header-text);
                }
            </style>
        </head>
        <body>
        
        <div class="container">
            <div class="header">
                <img src="logo.png" alt="Saveetha Logo">
                <h1>OFFICIAL TIMETABLE</h1>
            </div>
        
            <div class="info">
                <strong>Name:</strong>   HARIHARAN M  &nbsp; | &nbsp;
                <strong>Reg No:</strong> 24900770
            </div>
        
            <table>
                <thead>
                    <tr>
                        <th>DAY</th>
                        <th>8:00 - 10:00</th>
                        <th>10:00 - 12:00</th>
                        <th>12:00 - 1:00</th>
                        <th>1:00 - 3:00</th>
                        <th>3:00 - 5:00</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td class="day">MON</td>
                        <td>Machine learning</td>
                        <td></td>
                        <td class="lunch">LUNCH</td>
                        <td>Web App Dev</td>
                        <td></td>
                    </tr>
                    <tr>
                        <td class="day">TUES</td>
                        <td>Physics</td>
                        <td></td>
                        <td class="lunch">LUNCH</td>
                        <td></td>
                        <td>C programming</td>
                    </tr>
                    <tr>
                        <td class="day">WED</td>
                        <td></td>
                        <td>C programming</td>
                        <td class="lunch">LUNCH</td>
                        <td>Mentor Meet</td>
                        <td>IOT</td>
                    </tr>
                    <tr>
                        <td class="day">THURS</td>
                        <td>Physics</td>
                        <td>C programming</td>
                        <td class="lunch">LUNCH</td>
                        <td></td>
                        <td>Machine learning</td>
                    </tr>
                    <tr>
                        <td class="day">FRI</td>
                        <td>Physics</td>
                        <td></td>
                        <td class="lunch">LUNCH</td>
                        <td></td>
                        <td>Career Dev</td>
                    </tr>
                    <tr>
                        <td class="day">SAT</td>
                        <td></td>
                        <td>C programming</td>
                        <td class="lunch">LUNCH</td>
                        <td>IOT</td>
                        <td>Web App Dev</td>
                    </tr>
                </tbody>
            </table>
        
            <div class="subject-title">Subject Details</div>
            <table class="subject-table">
                <thead>
                    <tr>
                        <th>S.No</th>
                        <th>Subject Code</th>
                        <th>Subject Name</th>
                    </tr>
                </thead>
                <tbody>
                    <tr><td>1</td><td>19AI304</td><td>Fundamental of C programming</td></tr>
                    <tr><td>2</td><td>19AI414</td><td>Web Application Development</td></tr>
                    <tr><td>3</td><td>19CS420</td><td>Prototyping of IOT System</td></tr>
                    <tr><td>4</td><td>SH3214</td><td>Physics for Quantum Computing</td></tr>
                    <tr><td>5</td><td>19EY708</td><td>Career Development</td></tr>
                    <tr><td>6</td><td>19AI410</td><td>Introduction to machine learning</td></tr>
                </tbody>
            </table>
            <center>
                <footer>
                    @2025 Offical TimeTable. All rights reserved.
                </footer>
            </center>
        
        </div>
        
        </body>
        </html>
## OUTPUT
![alt text](<Screenshot 2025-04-24 142543.png>)

## RESULT
The program for creating slot timetable using basic HTML tags is executed successfully.
