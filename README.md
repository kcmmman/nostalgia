<!DOCTYPE HTML>
<html>
    
<head>
    <title> nostalgia </title>

<!--Little CSS fade in -->
<style>
    
    body{
        
        margin-left: 650px;
        margin-top: 95px; 
        
    }
    

.top-left {
  position: absolute;
  top: 10px;
  left: 16px;
}
    
    .bottom-right {
  position: absolute;
  bottom: 10px;
 right: 16px;
}
    
    
     .top-right {
  position: absolute;
  top: 10px;
 right: 16px;
}
    
    
    
    
    
    img{
        height: 700px;
        
    }
    
    button{
        margin-top: 60px;
        margin-left:225px;
        background-color: ghostwhite;
        color: black;
    }
.fade-in{
  -webkit-animation: fade-in 2s ease;
  -moz-animation: fade-in ease-in-out 1s both;
  -ms-animation: fade-in ease-in-out 1s both;
  -o-animation: fade-in ease-in-out 1s both;
  animation: fade-in 1s ease;
  visibility: visible;
  -webkit-backface-visibility: hidden;
}

@-webkit-keyframes fade-in{0%{opacity:0;} 100%{opacity:1;}}
@-moz-keyframes fade-in{0%{opacity:0} 100%{opacity:1}}
@-o-keyframes fade-in{0%{opacity:0} 100%{opacity:1}}
@keyframes fade-in{0%{opacity:0} 100%{opacity:1}}

</style>
</head>


<body>
    
<div class="container">

  <div class="top-left">what if...</div>

</div>
    
<div class="container">

  <div class="bottom-right">going back..?</div>

</div>

    <div class="bottom-right">going back..?</div>
    
 <div class="container">
         
     <div class="top-right">
       
       <a href="memories%20page.html" target="_blank">memories</a>
       
     </div>
</div>
        
<!--We append on this div-->
<div id="banner-load"></div>

<!--Don't forget Jquery-->
<script type='text/javascript' src='http://ajax.googleapis.com/ajax/libs/jquery/1.8/jquery.min.js'></script>

<!--New images on load -->
<script>
//Add your images, we'll set the path in the next step
    var images = ['1.jpg', '2.jpg', '3.jpg', '4.jpg', '5.jpg', '6.jpg', '7.jpg', '8.jpg', '9.jpg', '10.jpg'];
    
//Build the img, then do a bit of maths to randomize load and append to a div. Add a touch off css to fade them badboys in all sexy like.
    $('<img class="fade-in" src="images/' + images[Math.floor(Math.random() * images.length)] + '">').appendTo('#banner-load');
</script>

 <button type="submit"  onClick="location.reload()">click</button>
    
</body>
</html>
