# addHandler

function addHandler(element, event, func){
			try{
				element.addEventListener(event, func, false);
			}catch(e){
				element.attachEvent("on" + event, func);
			}
		}
