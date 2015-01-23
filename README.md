# addHandler

function addHandler(el, ev, func){
			try{
				el.addEventListener(ev, func, false);
			}catch(e){
				el.attachEvent("on" + ev, func);
			}
		}
