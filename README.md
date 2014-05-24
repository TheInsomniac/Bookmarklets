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

###jQuerify.js###
####Add jQuery to the currently opened page for easy tinkering####

```javascript: (function(){var el=document.createElement('div'),b=document.getElementsByTagName('body')[0];otherlib=false,msg='';el.style.position='fixed';el.style.height='32px';el.style.width='220px';el.style.marginLeft='-110px';el.style.top='0';el.style.left='50%';el.style.padding='5px 10px';el.style.zIndex=1001;el.style.fontSize='12px';el.style.color='#222';el.style.backgroundColor='#f99';if(typeof%20jQuery!='undefined'){msg='This%20page%20already%20using%20jQuery%20v'+jQuery.fn.jquery;return%20showMsg();}else%20if(typeof%20$=='function'){otherlib=true;}%20function%20getScript(url,success){var%20script=document.createElement('script');script.src=url;var%20head=document.getElementsByTagName('head')[0],done=false;script.onload=script.onreadystatechange=function(){if(!done&&(!this.readyState||this.readyState=='loaded'||this.readyState=='complete')){done=true;success();script.onload=script.onreadystatechange=null;head.removeChild(script);}};head.appendChild(script);}%20getScript('http://code.jquery.com/jquery-latest.min.js',function(){if(typeof%20jQuery=='undefined'){msg='Sorry,%20but%20jQuery%20wasn\'t%20able%20to%20load';}else{msg='This%20page%20is%20now%20jQuerified%20with%20v'+jQuery.fn.jquery;if(otherlib){msg+='%20and%20noConflict().%20Use%20$jq(),%20not%20$().';}}%20return%20showMsg();});function%20showMsg(){el.innerHTML=msg;b.appendChild(el);window.setTimeout(function(){if(typeof%20jQuery=='undefined'){b.removeChild(el);}else{jQuery(el).fadeOut('slow',function(){jQuery(this).remove();});if(otherlib){$jq=jQuery.noConflict();}}},2500);}})();```

