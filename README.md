<?php

	if($_POST) {


	$sayi1 = $_POST["sayi1"];
	$sayi2 = $_POST["sayi2"];
	$islem = $_POST["islem"];

	if ($islem == "+") {
		echo $sayi1+$sayi2;
	}

	if ($islem == "-") {
		echo $sayi1-$sayi2;
	}

	if ($islem == "*") {
		echo $sayi1*$sayi2;
	}

	if ($islem == "/") {
		echo $sayi1/$sayi2;
	}

}
	
	
?>

<form action="" method="POST">
		<input type="number" name="sayi1" />
		<input type="number" name="sayi2" />
		<select name="islem">

		<option value="+">toplama</option>
		<option value="-">çıkartma</option>
		<option value="*">çarpma</option>
		<option value="/">bölme</option>
		

		</select>
		<input type="submit" value="hesapla" />
</form>


