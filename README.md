# backend
<?php
if (isset($_POST['submit'])) {
//form was submitted
$username=$_POST["username"];
$password=$_POST["password"];

if ($username == "kaks" && $password == "joan") {

   echo " User {$username} was successfully logged in";

}else{

$message = "There is some error";

}

}else{
 $username ="";
$message ="please log in:";
}
?>

<!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN"
   "http://www.w3.0rg/TR/html14/loose.dtd">
<html lang="en">
<head>
<title>Form</title>
</head>
<body>

<?php echo $message; ?><br />

     <form action="single.php"method="post">
Username: <input type="text" name="username" value="" /><br />
Password:<input type="password" name="password" value="" /><br />
<br />
<input type="submit" name="submit" value="Submit" />
</form>
</body>
</html>
