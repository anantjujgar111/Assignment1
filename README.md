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




Q5
<!DOCTYPE html>
<html>
<title>Web Page Design</title>
<head>
<script>
function capitalize(str) {
   var splitStr = str.toLowerCase().split(' ');
   for (var i = 0; i < splitStr.length; i++) {
       // You do not need to check if i is larger than splitStr length, as your for does that for you
       // Assign it back to the array
       splitStr[i] = splitStr[i].charAt(0).toUpperCase() + splitStr[i].substring(1);     
   }
   // Directly return the joined string
   return splitStr.join(' '); 
}
document.write(capitalize("Hi From Skillsanta"));
</script>
</head>
<body>
</body>
</html>
        
        
        
Q6        
<script>
function truncate(str, no_words) {
    return str.split(" ").splice(0,no_words).join(" ");
}
console.log(truncate('The quick brown fox jumps over the lazy dog', 4));
</script>






Q7
function search_word(text, word){
    
    var x = 0, y=0;
   
    for (i=0;i< text.length;i++)
        {
        if(text[i] == word[0])
            {
            for(j=i;j< i+word.length;j++)
               {
                if(text[j]==word[j-i])
                  {
                    y++;
                  }
                if (y==word.length){
                    x++;
                }
            }
            y=0;
        }
    }
   return "'"+word+"' was found "+x+" times.";
}

console.log(search_word('where is skillsanta', 'is'));
console.log(search_word('ravi, bb, cc, dd, aa', 'ravi'));




Q8
var fibonacci_series = function (n) 
{
  if (n===1) 
  {
    return [0, 1];
  } 
  else 
  {
    var s = fibonacci_series(n - 1);
    s.push(s[s.length - 1] + s[s.length - 2]);
    return s;
  }
};

 console.log(fibonacci_series(8));
 

Q9
function cToF(celsius) 
{
  var cTemp = celsius;
  var cToFahr = cTemp * 9 / 5 + 32;
  var message = cTemp+'\xB0C is ' + cToFahr + ' \xB0F.';
    console.log(message);
}

function fToC(fahrenheit) 
{
  var fTemp = fahrenheit;
  var fToCel = (fTemp - 32) * 5 / 9;
  var message = fTemp+'\xB0F is ' + fToCel + '\xB0C.';
    console.log(message);
} 
cToF(60);
fToC(45);


