<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html>
<head>
<meta http-equiv="Content-Type" content="text/html; charset=UTF-8">	
<link rel="shortcut icon" href="http://imgur.com/CILKGax.png" >
<title>Điều tớ muốn nói</title> <!-- BẠN THAY ĐỔI TIÊU ĐỀ Ở ĐÂY-->
<link rel="stylesheet" href="css3/popup.css">
<link rel="stylesheet" href="css3/styles.css">
<link href='http://fonts.googleapis.com/css?family=Source+Sans+Pro&subset=latin,vietnamese' rel='stylesheet' type='text/css'>
<script type="text/javascript" src="http://code.jquery.com/jquery-1.6.min.js"></script>
<script type="text/javascript" src="jss/jquery.popup.js"></script>
<script src="jss/popup.js" type="text/javascript"></script>
<script src="jss/jquery-1.js" type="text/javascript"></script>
<script type="text/javascript" src="jss/jquery.js"></script>

<script type="text/javascript">

$(document).ready(function () {

	// if user clicked on button, the overlay layer or the dialogbox, close the dialog	
	$('a.btn-ok, #msb-nt').click(function () {		
		$('#dialog-overlay, #dialog-box').hide();		
		return false;
	});
	
	// if user resize the window, call the same function again
	// to make sure the overlay fills the screen and dialogbox aligned to center	
	$(window).resize(function () {
		

		if (!$('#dialog-box').is(':hidden')) popup();		
	});	
	
	
});

function popup(message) {
		
	var maskHeight = $(document).height();  
	var maskWidth = $(window).width();

	var dialogTop =  (maskHeight/3) - ($('#dialog-box').height());  
	var dialogLeft = (maskWidth/2) - ($('#dialog-box').width()/2); 
	$('#dialog-overlay').css({height:maskHeight, width:maskWidth}).show();
	$('#dialog-box').css({top:dialogTop, left:dialogLeft}).show();
	

	$('#dialog-message').html(message);
			
}

window.onbeforeunload = function (event) {
  var message = 'KHÔNG ĐƯỢC TẮT CÁI NÀY ĐI, TẮT ĐỒNG NGHĨA LÀ CHỊU LÀM VỢ CỦA TAO ĐÓ! ♥ =)) CÓ CHẮC TẮT KHÔNG? :3';
  if (typeof event == 'undefined') {
    event = window.event;
  }
  if (event) {
    event.returnValue = message;
  }
  return message;
}
</script>
		
<script language="javascript"> 
var kt=false
function move()
{
var x = Math.random()*500
var y = Math.random()*500
var left=x+'px'
var top=y+'px'
document.getElementById('lbNo').style.left=left
document.getElementById('lbNo').style.top=top
}
function dongy()
{
if(kt==false)
{

kt=true 
} 
else
{
}
}
</script>
<script src="jss/pace.min.js"></script>
  <link href="css3/dataurl.css" rel="stylesheet" />

</head>
	
<!-- ________________________________________ SỬA TRANG ĐẦU NGAY ĐÂY (1)______________________________________________________-->

<body onload="popup('<p>Tớ hỏi cái này, cậu phải trả lời thật lòng đó nghe chưa. Không trả lời thật lòng đánh bỏ mẹ mầy.</p></br>'); on()" onunload="s()">
<div id="bg"></div>
<div id="myModal" class="reveal-modal large">
    <div id="traloi">
	<!-- ___________________________________SỬA TRANG THỨ 3 NGAY ĐÂY (3)_______________________________________________-->
      <h1><center>NÓI GÌ ĐI</center></h1></br>
	  <p>TẠI SAO CẬU LẠI YÊU TỚ ? Nhập câu trả lời xuống bên dưới và bấm GỬI ĐI</br></br></p>
      <form id="f" name="f">
        <input id="form" name="txt" type="text" />

        <div>
          <input id="gui" onclick="Yeu();" type="button" value="Gửi đi" />
        </div>
      </form>
    </div>

    <div style="clear: both;"></div>

    <div id="divResult" style="text-align: center"></div>

    <div id="divResult2"></div>

    <div id="divResult3"></div>
<a class="close-reveal-modal">&#215;</a>
</div>
<script language="javascript"> 
    $(document).ready(function() {
        $('#msb-nt').click(function() {
                $('.music').slideToggle("fast");
                $('#bg').css('display','none');
        });
    });
</script>
<div id="dialog-overlay"></div>
<div id="dialog-box">
	<div class="dialog-content">
		<div id="dialog-message">
		</div>
		<div id="msb-nt">
		<a href="#">OK :D</a>
		</div>
	</div>
</div>
		
<div class="msg">
		<!-- ___________________________________________________SỬA TRANG THỨ 2 NGAY ĐÂY (2)________________________________________-->	
<h1> <?php if($_GET['em']==null) echo 'EM'; else echo $_GET['em']; ?> <b>CÓ YÊU TỚ KHÔNG ?</b></h1>
			
<h2><?php if($_GET['em']==null) echo 'EM'; else echo $_GET['em']; ?> MẦY MÀ TẮT CÁI NÀY ĐỒNG NGHĨA MẦY SẼ LÀM VỢ CỦA TAO. SUY NGHĨ ĐI !</br>
CÓ YÊU TAO KHÔNG ? TRẢ LỜI NHANH MẦY! ♥ =))</h2>

		
</div>
		
<center>
<div id="co"> 
<a href="#" data-reveal-id="myModal">CÓ! <?php if($_GET['em']==null) echo 'EM'; else echo $_GET['em']; ?> TỚ YÊU</a>
</div> 

<div id="lbNo" style="position:absolute; left: 700px; top: 300px;"> 
<input type="button" value="MẦY MƠ À" style="cursor:pointer;" onMouseMove="move()" > 
</div>
<div> <img src="http://imgur.com/i1LFl8j.png  "></div>
</center> 

<div class="music" style="display: none;">
<object width="1" height="1">  <param name="movie" value="http://www.nhaccuatui.com/m/UoqC0m8Rofjb" />  
<param name="quality" value="high" />  <param name="wmode" value="transparent" />  <param name="allowscriptaccess" value="always" /> 
<param name="allowfullscreen" value="true"/> <param name="flashvars" value="autostart=true" />  
<!-- ________________________________________THAY ĐỔI NHẠC Ở LINK BÊN DƯỚI_____________________________________-->
<embed src="http://www.nhaccuatui.com/m/G2Fil0oSQeHm" flashvars="target=blank&autostart=true" allowscriptaccess="always" allowfullscreen="true" quality="high" wmode="transparent" type="application/x-shockwave-flash" width="1" height="1"></embed></object>
</div>
<script type="text/javascript">
   $(document).ready(function(){
      $(document).bind("contextmenu",function(e){
        return false;
      });
    });
 </script>	
 <style>
 
 </style>
</body>
</html>
