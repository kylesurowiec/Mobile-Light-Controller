<html>
<head>
<meta charset="UTF-8" />
</head>

<?php
if (isset($_POST['LightON']))
{
echo "ON";
exec("sudo python /home/pi/lightOn.py");
}
if (isset($_POST['LightOFF']))
{
echo "OFF";
exec("sudo python /home/pi/lightOff.py");
}
?>

<form method="post">
<button class="btn" name="LightON">On</button>&nbsp;
<button class="btn" name="LightOFF">Off</button><br><br>
</form> 

</html>