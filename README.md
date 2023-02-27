# form_reg
сделано на веселе под веселую музычку(особенно градиент).
некоторая часть гуглилась, ибо без этого никак, гуглился вопрос, перестраивал код под себя или же писал сам.
><!DOCTYPE html>
<html>
<head>
	<link rel="stylesheet" type="text/css" href="styles.css">
	<meta charset="utf-8">
	<meta name="viewport" content="width=device-width, initial-scale=1">
	<title></title>
	<style >

	</style>
</head>
<body>
	<section class="center-container">
		<div class="form">
			<div class="photo_text_logo">
			<img class="logo" src="img/Icon.svg" alt="icon">
			<p class="logo_text">COM<span>PANY</span></p>
			</div>
			<p class="under_logo_text">Login to you private dashboard</p>
			<div class="input_email">
				<p class="email_text_int">Email</p>
			</div>
			<div class="input_pass">
				<p class="pass_text_int">Password</p>
			</div>
			<div class="buttom">
				<p class="bottom_text">Sing in</p>
			</div>
			<div class="text_creat_or_reset">
				<a href="#" class="creat_or_reset">Creat account</a> or <a href="#" class="creat_or_reset">reset password</a>
			</div>
		</div>
	</section>
</body>
</html>
























*{ /*всегда ставить*/
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial;
}
/* градиент цветов*/
html, body {
  width: 100%;
  height:100%;
}

body {
    background: linear-gradient(-45deg, #ee7752, #e73c7e, #23a6d5, #23d5ab);
    background-size: 400% 400%;
    animation: gradient 15s ease infinite;
}

@keyframes gradient {
    0% {
        background-position: 0% 50%;
    }
    50% {
        background-position: 100% 50%;
    }
    100% {
        background-position: 0% 50%;
    }
}
.form{
	position: relative;
	background-color: #ffffff;
	width:550px;
	height: 450px;
	border-radius: 91px;
	background: linear-gradient(145deg, #e6e6e6, #ffffff);
	box-shadow:  5px 5px 53px #666666,
             -5px -5px 53px #ffffff;
    justify-content: space-around; /*все что внутри все по ширине*/
    align-items: center; /*все что внутри все по центру*/
    display: flex;
    flex-direction: column; /*все что внутри все в колонку*/

}
 /*штука что бы контейнер был поцентру*/
.center-container{
    width: 100%;
    height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }
.logo{
	width: 6em;
    height: 6em;
}
.logo_text{
	font-size: 50px;
}
.photo_text_logo{
	    display: flex;
    align-items: center;

}
.photo_text_logo span{
	font-weight: bold;

}
.input_email{
 box-sizing: border-box;
 width: 400px;
 height: 50px;
 padding: 10px;
 border: 2px solid #eee;
 box-shadow: 0 0 15px 4px rgba(0, 0, 0, 1.0);
 border-radius: 10px;

}
.input_pass{
box-sizing: border-box;
width: 400px;
height: 50px;
padding: 10px;
border: 2px solid #eee;
box-shadow: 0 0 15px 4px rgba(0, 0, 0, 1.0);
border-radius: 10px;
}
.bottom{

}
.under_logo_text{
	font-size: 20px;
	color: rgba(0,0,0,0.5)
}
.buttom{
	    display: inline-block;
    text-decoration: none;
    background-color: #eaeaea;
    color: #006089;
    border: 1px solid #006089;
    border-radius: 15px;
    font-size: 20px;
    padding: 8px 100px; 
    transition: all 0.6s ease;
}
.buttom:hover{
	text-decoration: none; 
    background-color: #006089;
    color: #ffeded;
    border-color: #006089;
}
.creat_or_reset{
	color: #5CBFDD;
}
