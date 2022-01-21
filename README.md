# Web Page for Mathematical Calculations

## AIM:

To design a static website with validation to perform mathematical calculations in client side.

## DESIGN STEPS:

### Step 1:

Requirement collection

### Step 2:

Creating the layout using HTML and CSS.

### Step 3:

Write javascript to perform the calculations.

### Step 4:

Include regularexpression based input validation.

### Step 5:

Validate the layout in various browsers.

### Step 6:

Validate the HTML code.

### Step 6:

Publish the website in the given URL.

## PROGRAM :

--include your code--
~~~
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Mathematical Calculations</title>
  
  <style>
  * {
  box-sizing: border-box;
  font-family: Arial, Helvetica, sans-serif;
  }
  body {
  background-color:rgb(236, 201, 45);
  }
  .container {
  width: 1080px;
  margin-left: auto;
  margin-right: auto;
  }
  .content {
  display: block;
  width: 100%;
  background-color: #fffeac;
  min-height: 500px;
  margin-top: 150px;
  }

  h1{
    text-align: center;
    padding-top: 50px;
    color: rgb(36, 23, 23);
  }
  .formelement{
    text-align: center;
    font-size:xx-large;
    margin-top: 5px;
    margin-bottom: 5px;

  }
    </style>
  </head>
  <h1 style="text-align: center;">MATHEMATICAL CALCULATIONS</h1>
  <body><div class="container">
  <div class="content">
            <h1>VOLUME OF  A CYLINDER</h1>
            <form>
                <div class=formelement>
                    <lable for="bedit">Radius:</lable>
                    <input type="text" id="bedit" value=""/>Meters
                </div><br>
                <div class=formelement>
                    <lable for="aedit">Height:</lable>
                    <input type="text" id="aedit" value=""/>Meters
                </div><br>
                
                <div class=formelement>
                    <input type="button" value="CALCULATE VOLUME" id="calbutton1"/>
                </div>
                <div class=formelement>
                    <lable for="cedit">Volume:</lable>
                    <input type="text" id="cedit" readonly="0"/>Cubic Meters
                </div><br>
              
            </form>
        </div>
        <script type="text/javascript">
            var button;
            button=document.querySelector("#calbutton1");
            button.addEventListener("click",function(){
                var atext,btext,ctext;
                var aval,bval,cval;
                atext=document.querySelector("#aedit");
                btext=document.querySelector("#bedit");
                ctext=document.querySelector("#cedit");

                aval=parseInt(atext.value);
                bval=parseInt(btext.value);
                cval=22/7*aval*bval*bval;
                ctext.value=cval;
                ctext.value=cval;
            });
        </script>
        <div class="container">
        <div class="content">
            <h1>AREA OF A RECTANGLE</h1>
            <form>
                <div class="formelement">
                  <lable for="lengthedit">LENGTH:</lable>
                  <input type="text" id="lengthedit" value=" "/>Meters
                </div><br>
                <div class="formelement">
                  <lable for="breadthedit">BREADTH:</lable>
                  <input type="text" id="breadthedit" value=" "/>Meters
                </div><br>
                <div class="formelement">
                  <input type="button" value="CALCULATE AREA" id="calbutton2"/>
                </div><br>
                <div class="formelement">
                  <lable for="areaedit">AREA:</lable>
                  <input type="text" id="areaedit" readonly="0"/>Square Meters
                </div><br>
                <div class="formelement">
              
                </div><br>
                
            </form>
    
            </div>
        </div>
        <script type="text/javascript">
          var button;
          button=document.querySelector("#calbutton2");
          button.addEventListener("click",function(){
            
              var lengthtext,breadthtext,areatext;
              var aval,bval,cval;
    
              lengthtext=document.querySelector("#lengthedit");
              breadthtext=document.querySelector("#breadthedit");
              areatext=document.querySelector("#areaedit");
      
              aval=parseInt(lengthtext.value);
              bval=parseInt(breadthtext.value);
              cval=aval*bval
              areatext.value=cval;
        
      
          });
    
      </script> 
  </body>
</html>
~~~

## OUTPUT:

-- include your output screenshots ---
![OUTPUT](m1.png)
![output](m2.png)
![output](m3.png)

## Result:

Thus a website is designed to perform mathematical calculations in the client side.

## HTML CANVASING ASSIGNMENT:

### PROGRAM:
~~~
<!DOCTYPE html>
<html>
    <title>Canvas</title>
    <body>
        <h1 style="text-align: center;">Assignment</h1>
        <canvas id="mycanvas" width="600px" height="400px" style="border:2px solid #000000">
        </canvas>
        <script>
        var canvas=document.getElementById("mycanvas");
        var ctx=mycanvas.getContext("2d");
        ctx.moveTo(5,5);
        ctx.lineWidth= 6;
        ctx.lineTo(590,390);
        ctx.stroke();
        ctx.fillStyle= "#FF0000";
        ctx.fillRect(5,5,590,390);
        ctx.stroke();
        ctx.fillStyle= "#000000";
        ctx.font = "900 30px Arial";
        ctx.fillText("DANGER", 20, 370);
        </script>

        <canvas id="canvas" width="400px" height="400px" style="border:2px solid #000000">
        </canvas>
        <script>
            var canvas=document.getElementById("canvas");
            var ctx= canvas.getContext("2d");
            ctx.beginPath();
            ctx.arc(200,200,150,100,-1.5*Math.PI,true);
            ctx.strokeStyle="black";
            ctx.lineWidth= 4;
            ctx.fillStyle= "lightgreen";
            ctx.fill();
            ctx.stroke();
            ctx.beginPath();
            ctx.arc(160,160,20,25,-1.5*Math.PI,true);
            ctx.fillStyle="lightblue";
            ctx.fill();
            ctx.stroke();
            ctx.beginPath();
            ctx.arc(235,160,20,10,-1.5*Math.PI,true);
            ctx.fillStyle="lightblue";
            ctx.fill();
            ctx.stroke();
            ctx.beginPath();
            ctx.arc(200,195,122,1*Math.PI,2*Math.PI,true);
            ctx.strokeStyle="violet";
            ctx.lineWidth=4;
            ctx.stroke()
        </script>
    </body>
</html>
~~~

## OUTPUT:
![output](canvas.png)