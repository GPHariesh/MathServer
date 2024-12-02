# Ex.05 Design a Website for Server Side Processing
## Date:02-12-24

## AIM:
 To design a website to calculate the power of a lamp filament in an incandescent bulb in the server side. 


## FORMULA:
P = I<sup>2</sup>R
<br> P --> Power (in watts)
<br> I --> Intensity
<br> R --> Resistance

## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Create python programs for views and urls to perform server side processing.

### Step 5:
Create a HTML file to implement form based input and output.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```<html>

<head>
    <meta charset='utf-8'>
    <meta http-equiv='X-UA-Compatible' content='IE=edge'>
    <title>Power calculator</title>
    <meta name='viewport' content='width=device-width, initial-scale=1'>
    <style type="text/css">
        body {
            background-color:darkseagreen;
        }
        
        .edge {
            display: flex;
            height: 100vh;
            width: 100%;    
            justify-content: center;
            align-items: center;
        }

       .formelt {
            color:black;
            text-align: center;
            margin-top: 7px;
            margin-bottom: 6px;
        }

        h1 {
            color:darkorange;
            text-align: center;
            padding-top: 20px;
        }
        input{
            margin: 5px;
            padding: 5px;
            border-radius: 5px;
            border: none;

        }
    </style>
</head>

<body>
    <center>
    <h2><b>HARIESH G.P. (24900267)</b></h2>
    </center>
    <div class="edge">
        <div class="box">
            </div>
            <div class="definition">

            <h1>POWER CALCULATION OF A LAMP</h1>
            
            <p>
               Power is the rate at which energy is transferred or converted. In the case of a lamp, it can be calculated using the formula:<br> <b>P = I² * R</b> where I is the intensity and R is the resistance.
            </p>
            </div>
            <form method="POST">
                {% csrf_token %}
                <div class="formelt">
                    Intensity: <input type="text" name="Intensity" value="{{I}}"></input>(in A)<br />
                </div>
                <div class="formelt">
                    Resistance: <input type="text" name="Resistance" value="{{R}}"></input>(in R)<br />
                </div>
                <div class="formelt">
                    <input type="submit" value="Calculate"></input><br />
                </div>
                <div class="formelt">
                    Power : <input type="text" name="Power" value="{{power}}"></input>watts<br />
                </div>
            </form>
        </div>
    </div>
</body>

</html>
```
            
        

     
   
            
            
                

## SERVER SIDE PROCESSING:

![alt text](<Screenshot 2024-12-02 223639.png>)
## HOMEPAGE:
![alt text](<Screenshot 2024-12-02 223624.png>)

## RESULT:
The program for performing server side processing is completed successfully.
