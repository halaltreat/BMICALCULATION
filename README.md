# BMICALCULATION
new update bmi calculation
 <script>function computeBMI() {
                // user inputs
                var height = Number(document.getElementById("height").value);
                var weight = Number(document.getElementById("weight").value);
             
                //Perform calculation
             if (weight > 0 || height > 0 )
                 {
                     var hicm = height*0.01;
                    var BMI =parseFloat(weight / (hicm*hicm)).toFixed(2);
                    document.getElementById("demo1").innerHTML = "Your BMI is : " +BMI;
                                      
                    if(BMI < 18.5){
                        document.getElementById("demo2").innerHTML = "That you are too thin";
                    }                 
                    if(BMI >= 18.5 && BMI <= 25){
                        document.getElementById("demo2").innerHTML = "That you are healthy";
                    }                   
                    if(BMI >= 25){
                        document.getElementById("demo2").innerHTML = "That you have overweight";
                    }
                 }
             else{
                 alert("Please fill in everything correctly")
             }
             }
         </script>
