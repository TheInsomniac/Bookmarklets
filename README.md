Bookmarklets
============

###qr.js:###
####QR Code from URL####

```javascript:(function(){if(document.getElementById){var x=document.body;var o=document.createElement('script');if(typeof(o)!='object') o=document.standardCreateElement('script');o.setAttribute('src','https://raw.github.com/TheInsomniac/Bookmarklets/master/qr.js');o.setAttribute('type','text/javascript');x.appendChild(o);}})();```

###asciToUnicode.js:###
####Convert Character to it's Unicode Equivalent####

```javascript:prompt(%27Your unicode hex code:%27, (prompt(%27Enter a unicode character, please:%27)).charCodeAt(0).toString(16) )%3B```

###contentEditable.js###
####HTML editor including live preview in the browser####

```data:text/html,<pre onkeyup="(function(d,t){d[t]('iframe')[0].contentDocument.body.innerHTML = d[t]('pre')[0].textContent;})(document,'getElementsByTagName')" style="width:100%;height:48%;white-space:pre-wrap;overflow:auto;" contenteditable></pre><iframe style="width:100%;height:48%">```

