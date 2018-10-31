# GHM Front-End Docs 

## Cookie 

```
<script src="js/jquery.cookie.js"></script>
<script>
    $(document).ready(function() {
        if(!$.cookie('videoNext')){
            setTimeout(function(){
                $.cookie('videoNext', '1', {expires:7, path:'/'});
            }, 10000);
            // Price Button Timer: 20min
            delay = 60000 * 1200;
            setTimeout(function(){
                $(".buyNowButton").css("display", "block");

            }, delay);
        }
        else{
            $(".buyNowButton").css("display", "block");

        }
    })
</script>
```


## Ooyala CODE

### Basic Version
```
var playerParam = {
	autoplay: true,
	pcode: "xvYWgyOgX8LlAER8dMPTua1yO938",
	playerBrandingId: "38dd44cdbeca4132a08badd1e565fab6",
	skin: {
		config: '../otc_m.json'
	},
};
OO.ready(function() {
	window.pp = OO.Player.create("ooyalaplayer", "g5aHc3ZjE69Y_EVJfMWzsMYPgiCGe3kD", playerParam);
});
```
