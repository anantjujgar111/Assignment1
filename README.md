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



#Q3
<body>
<script>
 function rightTriangle(n) {
  for (var i = 0; i <= n; i++) {
    for (var j = n - 1; j >= i; j--) {
      document.write('*');
    }
    document.write('<br>');
  }
}
rightTriangle(5);
</script>
</body>
</html>







#Q4
<html>
<body>
<script type="text/javascript">
   newEmail = function (email) {
      var split = email.split("@");
      var split1 = split[0];
      var avg = split1.length / 2;
      split1 = split1.substring(0, (split1.length - avg));
      split2 = split[1];
      return split1 + "...@" + split2;
   };
   document.write(newEmail("@gmail.com"));
</script>
</body>
</html>
