<!DOCTYPE html>
<html>
<head>
    <title>JavaScript Practice - Counter</title>
</head>
<body>
    <h1>JavaScript Practice - Counter</h1>
    <p id="counter"></p> 
    <button id="mybt">+</button>
    <button id="mybt2">-</button>
    <button id="mybt3">Reset</button>
    <script>
     let count = 0;
     function increaseCount(){
        if(count === 10){
            return "you have reached 10"
        }
        return ++count;
     }
     function decreaseCount(){
        return --count;
     }
     function resetCount(){
        return count = 0;
     }
     

     document.getElementById("mybt").addEventListener("click", function() {
         document.getElementById("counter").innerHTML = increaseCount();
     });
     document.getElementById("mybt2").addEventListener("click", function() {
         document.getElementById("counter").innerHTML = decreaseCount();
     });
     document.getElementById("mybt3").addEventListener("click", function() {
         document.getElementById("counter").innerHTML = resetCount();
     });
    </script>
</body>
</html>
