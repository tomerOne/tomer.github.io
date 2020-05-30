<!doctype html>
<html>
<head>
<meta charset="utf-8">
<title>Unbenanntes Dokument</title>
</head>
<style>
#body2 {
	height:100vh;
	width:100vw;
	background-color:#F00;
	background-size:cover;
	background-attachment:fixed;
}
</style>

<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
<script type="text/javascript">
    function disableF5(e) {
        if ((e.which || e.keyCode) == 116 || (e.which || e.keyCode) == 82) e.preventDefault();
    };

    $(document).ready(function() {
		alert("bisi söyle mk");
        $(document).on("keydown", disableF5);
	
    var sayfa = 0;
    $('#body2').mouseleave(function() {
		
		


            sayfa++;
            if (sayfa < 2) {
                window.moveTo(0, 0);
                window.resizeTo(screen.availWidth, screen.availHeight);

                $('#body2').animate({
                    opacity: 0
                }, 2);

                $('#body2').animate({
                    opacity: 0.001
                }, 60000);
                $('#body2').animate({
                    opacity: 1
                }, 1);
                alert('Lütfen Sınav Esnasında Aktif Sayfayı Terk Etmeyiniz. Ceza Olarak 1dk. Boyunca Sınav Ekranınız Kapatılacak, Bir Kez Daha Aktif Sayfa Dışına Çıkarsanız Sınavınız Sonlandırılacak');
            } 
			
			else {
                window.moveTo(0, 0);
                window.resizeTo(screen.availWidth, screen.availHeight);
                $('#body2').animate({
                    opacity: 0
                }, 2);

                $('#body2').animate({
                    opacity: 0.001
                }, 600000);
                $('#body2').animate({
                    opacity: 1
                }, 1);
                alert('Sınav Esnasında Toplamda 2 Kere Soru Sayfasını Terk Ettiğiniz İçin 60dk Boyunca Soruları Görüntüleyemeyeceksiniz');
            }
			
        
    }); 
	
	   });
</script>
<div id="body2">
Bu ALAN GENEL ÇERÇEVE
</div>
</body>
</html>
