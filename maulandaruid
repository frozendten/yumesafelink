var wpsafelink = "http://maulandaru.id/?go=";
var domain = ["mega.nz","mir.cr","mirrorace.com","mirrored.to","drive.google.com","solidfiles.com","solidfiles.com","1fichier.com","wdfiles.ru","racaty.com","anonfiles.com","sendit.cloud",];
var exclude_domain = ["",];
var els = document.getElementsByTagName("a"); 
for(var i = 0, l = els.length; i < l; i++) {	
	var el = els[i]; 
	var li = el.href;
	li = li.replace("https://", "");
	li = li.replace("http://", "");
	li = li.replace("www.", "");
	li = li.split("/")[0];
	
	if( exclude_domain.length > 0 ) {
		var exists = false;
		for(var d=0; d < exclude_domain.length; d++){
			if(li == exclude_domain[d]){
				exists = true;
			}
		}
		if( !exists ) {
			el.href = wpsafelink + btoa(el.href);
		}
	} else {
		for(var d=0; d < domain.length; d++){
			if(li == domain[d]){
				el.href = wpsafelink + btoa(el.href);
			}
		}
	}
}
