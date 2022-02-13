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
