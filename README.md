# floating-share-button
This include jQuery,FontAwesome,bootstrap 4 CDN

#Add Following code to your code
###HTML CODE
<div class="floating-social">
		<div class="floating1 bg-success text-center">
			<i class="fa fa-share-alt"></i>
		</div>
		<div class="floating2 text-center">
			<i class="fa fa-facebook"></i>
		</div>
		<div class="floating3 text-center">
			<i class="fa fa-twitter"></i>
		</div>
		<div class="floating4 text-center">
			<i class="fa fa-whatsapp"></i>
		</div>
</div>


###jQuery Code

$(document).ready(function(){
		$(".floating1").click(function(){
			$(".floating2").slideToggle(100,"linear",function(){
				$(".floating3").slideToggle(100,"linear",function(){
					$(".floating4").slideToggle(100,"linear");
				});
			});
		});
	});
	
	###CSS Code
	.floating-social{position:fixed;bottom:180px;left:20px}.floating1{height:50px;width:50px;padding-top:13px;box-shadow:0 0 10px #000;position:fixed;bottom:30px;left:20px;border-radius:50%;margin-top:20px}.floating2{height:50px;width:50px;padding-top:13px;box-shadow:0 0 10px #000;position:fixed;bottom:80px;left:20px;border-radius:50%;margin-top:20px;background-color:#4267b2}.floating3{height:50px;width:50px;padding-top:13px;box-shadow:0 0 10px #000;position:fixed;bottom:130px;left:20px;border-radius:50%;margin-top:20px;background-color:#1da1f2}.floating4{height:50px;width:50px;padding-top:13px;box-shadow:0 0 10px #000;position:fixed;bottom:180px;left:20px;border-radius:50%;margin-top:20px;background-color:#25d366}.floating1 i,.floating2 i,.floating3 i,.floating4 i{font-size:20px;color:#fff}.floating2,.floating3,.floating4{display:none;cursor:pointer}.floating2:hover,.floating3:hover,.floating4:hover{z-index:1000;border:1px dashed #fff;transform:scale(1.5)}
