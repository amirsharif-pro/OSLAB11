# OSLAB11
امیرحسین شریف نژاد
<br>
<hr>
1.
https://stackoverflow.com/questions/68105211/how-to-send-a-message-to-telegram-with-ajax
<br>
I have a form that sends a text to the Telegram robot via Ajax. But the problem is that if the text is written in several lines, when the text is sent, the text is sent in one line, The code I wrote is as follows:<br>

$.ajax({
    type: "POST",
    dataType: "text",
    data: 'sendmessage=' + token + '&chat_id=' + lines[i] + '&text=' + document.getElementById("text").value,
    url: "https://ss.ir/apps/tele/aa.php",
    success: function(result) {
      document.getElementById("loading").style.display = 'none';
      var res = JSON.parse(result);
      if (res.ok == true) {
}}<br>
Does anyone know what the solution to this problem is?<br>
