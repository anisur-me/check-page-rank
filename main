<!doctype html>
<html lang="en-US">
<head>
  <meta http-equiv="Content-Type" content="text/html;charset=utf-8">
  <title>Page Rank</title>
  <meta name="author" content="Anisur">
  <link rel="shortcut icon" href="">
  <link rel="icon" href="">
  <link rel="stylesheet" type="text/css" media="all" href="styles.css">
  <script type="text/javascript" src="http://ajax.googleapis.com/ajax/libs/jquery/1.9.1/jquery.min.js"></script>
  <link href='http://fonts.googleapis.com/css?family=Indie+Flower' rel='stylesheet' type='text/css'>
  <link href='http://fonts.googleapis.com/css?family=Chewy' rel='stylesheet' type='text/css'>
  
</head>

<body>

 <div id="wrap">
	
  
    <h1><span>Find Page Rank</span></h1>
    

	<div id="content">
	<div class="out">
				<?php
	if(isset($_POST['submit'])){
	if($_POST['captcha']==$_POST['rand'])
	{
include("php/pagerank.php");
$pagerank = get_google_page_rank($_POST['s']);
if($pagerank!="")
echo "<h1>Page Rank of ".$_POST['s']."  is <span style='color:red'> " . $pagerank . "</span></h1>\n";
else
echo "<h1>Page Rank of ".$_POST['s']."  is <span style='color:red'> 0 </span></h1>\n";

   }
   else
   echo "<h1><span style='color:red'> Invalid captcha </span></h1>\n";
}
?>
</div>

	<form action="" method="post" class="inputform">
	<input type="text" name="captcha" placeholder="Enter the code" class="captcha_form"><span style="background:url(images/back.gif);width:450px;height:200px;padding:10px;color:#CCC;margin-left:5px;font-size:20px;font-width:700;font-family: 'Chewy', cursive;"><?php echo $rand=rand() ;?></span><br>
	<input type="hidden" name="rand" class="inputfield" value='<?php echo $rand;?>'>
	<input type="text" name="s" class="inputfield" >
	<input type="submit" name="submit" class="submitbutton"  value="Check Domain">
	</form>
     </div>
 </div> 
</body>
</html>
