<!DOCTYPE html>
<!-- Created By Satyendra -->
<html lang="en" dir="ltr">
<head>
<meta charset="utf-8">
<title>ZOHO-ASSESSEMENT</title>
<link rel="stylesheet" href="zoho.css">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>
<h1><u>ZOHO-ASSESSEMENT</u></h1>
<div class="wrapper">
<div class="title-text">
<div class="title SignIn">
Sign In Form
</div>
<div class="title SignUp">
Sign Up Form
</div>
</div>
<div class="form-container">
<div class="slide-controls">
<input type="radio" name="slide" id="SignIn" checked>
<input type="radio" name="slide" id="SignUp">
<label for="SignIn" class="slide SignIn">Sign In</label>
<label for="SignUp" class="slide SignUp">Sign Up</label>
<div class="slider-tab"></div>
</div>
<div class="form-inner">
<form action="C:\Users\Satyendra Kumar\index.html" class="SignIn">
<div class="field">
<input type="text" placeholder="Email Address" required>
</div>
<div class="field">
<input type="password" placeholder="Password" required>
</div>
<div class="pass-link">
<a href="https://accounts.google.com/b/0/AddMailService">Forgot password?</a>
</div>
<div class="field btn">
<div class="btn-layer"></div>
<input type="submit" value="Login">
</div>
<div class="SignUp-link">
Not a member?<a href="#">Sign Up now</a>
</div>
</form>
<form action="" class="SignUp">
<div class="field">
<input type="text" placeholder="Email Address" required>
</div>
<div class="field">
<input type="password" placeholder="Password" required>
</div>
<div class="field">
<input type="password" placeholder="Confirm password" required>
</div>
<div class="field btn">
<div class="btn-layer"></div>
<input type="submit" value="SignUp">
</div>
</form>
</div>
</div>
</div>
<script>
const SignInText = document.querySelector(".title-text .SignIn");
const SignInForm = document.querySelector("form.SignIn");
const SignInBtn = document.querySelector("label.SignIn");
const SignUpBtn = document.querySelector("label.SignUp");
const SignUpLUink = document.querySelector("form .SignUp-link a");
SignUpBtn.onclick = (()=>{
SignInForm.style.marginLeft = "-50%";
SignInText.style.marginLeft = "-50%";
});
SignInBtn.onclick = (()=>{
SignInForm.style.marginLeft = "0%";
SignInText.style.marginLeft = "0%";
});
SignUpLink.onclick = (()=>{
SignUpBtn.click();
return false;
});
</script>
</body>
</html>



@import
url('https://fonts.googleapis.com/css?family=Poppins:400,500,600,700&display=swap');
*{
margin: 0;
padding: 0;
box-sizing: border-box;
font-family: 'Poppins', sans-serif;
}
html,body{
display: grid;
height: 100%;
width: 100%;
place-items: center;
background: -webkit-linear-gradient(left, #2eb2da, #4744e4);
}
h1{
text-align: center;
font-weight: 700;
font-family: Arial, Helvetica, sans-serif;
text-decoration: #b3b3b3;
}
::selection{
background: #2bbfec;
color: #fff;
}
.wrapper{
overflow: hidden;
max-width: 390px;
background: #fff;
padding: 30px;
border-radius: 5px;
box-shadow: 0px 15px 20px rgba(0,0,0,0.1);
}
.wrapper .title-text{
display: flex;
width: 200%;
}
.wrapper .title{
width: 50%;
font-size: 35px;
font-weight: 600;
text-align: center;
transition: all 0.6s cubic-bezier(0.68,-0.55,0.265,1.55);
}
.wrapper .slide-controls{
position: relative;
display: flex;
height: 50px;
width: 100%;
overflow: hidden;
margin: 30px 0 10px 0;
justify-content: space-between;
border: 1px solid lightgrey;
border-radius: 5px;
}
.slide-controls .slide{
height: 100%;
width: 100%;
color: #fff;
font-size: 18px;
font-weight: 500;
text-align: center;
line-height: 48px;
cursor: pointer;
z-index: 1;
transition: all 0.6s ease;
}
.slide-controls label.SignUp{
color: #000;
}
.slide-controls .slider-tab{
position: absolute;
height: 100%;
width: 50%;
left: 0;
z-index: 0;
border-radius: 5px;
background: -webkit-linear-gradient(left, #26c2dd, #6442fa);
transition: all 0.6s cubic-bezier(0.68,-0.55,0.265,1.55);
}
input[type="radio"]{
display: none;
}
#SignUp:checked ~ .slider-tab{
left: 50%;
}
#SignUp:checked ~ label.SignUp{
color: #fff;
cursor: default;
user-select: none;
}
#SignUp:checked ~ label.SignIn{
color: #000;
}
#SignIn:checked ~ label.SignUp{
color: #000;
}
#SignIn:checked ~ label.SignIn{
cursor: default;
user-select: none;
}
.wrapper .form-container{
width: 100%;
overflow: hidden;
}
.form-container .form-inner{
display: flex;
width: 200%;
}
.form-container .form-inner form{
width: 50%;
transition: all 0.6s cubic-bezier(0.68,-0.55,0.265,1.55);
}
.form-inner form .field{
height: 50px;
width: 100%;
margin-top: 20px;
}
.form-inner form .field input{
height: 100%;
width: 100%;
outline: none;
padding-left: 15px;
border-radius: 5px;
border: 1px solid lightgrey;
border-bottom-width: 2px;
font-size: 17px;
transition: all 0.3s ease;
}
.form-inner form .field input:focus{
border-color: #83a3fc;
/* box-shadow: inset 0 0 3px #fb6aae; */
}
.form-inner form .field input::placeholder{
color: #999;
transition: all 0.3s ease;
}
form .field input:focus::placeholder{
color: #b3b3b3;
}
.form-inner form .pass-link{
margin-top: 5px;
}
.form-inner form .SignUp-link{
text-align: center;
margin-top: 30px;
}
.form-inner form .pass-link a,
.form-inner form .SignUp-link a{
color: #4298fa;
text-decoration: none;
}
.form-inner form .pass-link a:hover,
.form-inner form .SignUp-link a:hover{
text-decoration: underline;
}
form .btn{
height: 50px;
width: 100%;
border-radius: 5px;
position: relative;
overflow: hidden;
}
form .btn .btn-layer{
height: 100%;
width: 300%;
position: absolute;
left: -100%;
background: -webkit-linear-gradient(right, #4aa5cf, #5032f5, #41b7d4, #4539f0);
border-radius: 5px;
transition: all 0.4s ease;;
}
form .btn:hover .btn-layer{
left: 0;
}
form .btn input[type="submit"]{
height: 100%;
width: 100%;
z-index: 1;
position: relative;
background: none;
border: none;
color: #fff;
padding-left: 0;
border-radius: 5px;
font-size: 20px;
font-weight: 500;
cursor: pointer;
}
