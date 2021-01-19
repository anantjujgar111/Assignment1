# Assignment1
#Q1
        <script>  
    var arr=[0,-1,4];  
    var result=arr.sort(function compare(a,b)  
    {  
      return b-a;  
    });  
    document.writeln(result);  
    </script>  
    
    
    
    #Q2
    <!DOCTYPE html>
<html>
<body>
<script>
   var num= window.prompt("Enter your number: "); 
  // var num = 5;
   document.write("Number = "+num+"<br>");
   if(num % 2 == 0) {
      document.write('Number is even!');
   } else {
      document.write('Number is odd!');
   }
</script>
</body>
</html>
