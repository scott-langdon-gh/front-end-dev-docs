```javascript
        var item = $('#purchase-box li');
		item.hide();
		
		function recentlyBought() {
			counter = 0;
			var box = document.getElementById('purchase-box');
			var boxLength = box.children.length;
			
			function recentlyBoughtItemShow(num) {
				$(box.children[num]).show().delay(9000).fadeOut();	
			}
			function animatedPopUp() {
				$('.popup-box')
					.animate({
						bottom: -200,
					}, 10, function() {
						recentlyBoughtItemShow(counter);
						counter++;
						if (counter >= boxLength) {
							counter = 0;
						}
					})
					.animate({
						bottom: 50,
					}, 1000)
					.animate({
						bottom: 50,
					}, 2000)
					.animate({
						bottom: -200,
					}, 1000, function() {
						var delay_time = (Math.floor((Math.random() * ((12 - 5) + 1) + 5)) * 1000);
						setTimeout(function() {
							animatedPopUp()
						}, delay_time)
					})
			}
			animatedPopUp();
		}
		setTimeout(function() {
			recentlyBought()
		}, 4000);
```
