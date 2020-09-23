<div align="center">

## Banner Advertisement Rotator


</div>

### Description

This code lets you input up to 3 banners and it rotates through them without refreshing the page. If you want to cycle through more than 3 banners it is very easy to make this code work for as many banners as you want.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Todd Williams](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/todd-williams.md)
**Level**          |Beginner
**User Rating**    |4.6 (23 globes from 5 users)
**Compatibility**  |
**Category**       |[Miscellaneous](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/miscellaneous__2-57.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/todd-williams-banner-advertisement-rotator__2-2241/archive/master.zip)





### Source Code

```
<html>
<head>
<title>rotator</title>
<style type="text/css">
body {background:'#ffffff'; color:'#000000'}
</style>
<script language="javascript">
/*
          ###################################
          ###### Banner Ad Rotator 1.0 ######
          ######## By: Todd Williams ########
          ###################################
		   http://www.media1designs.com/
----------------------------------------------------------------
Notes:
1)	The HTML codes for the banners can not contain
	(")s because you can't have quotes inside of quotes.
	If you really want quotes you must put a (\) before
	each (") so the computer knows its not ending the first
	quote in wich the whole html code is contained in.
2)	You must have this top script in the <head> of your
	document.
3)	In order for the script to start working you must have
	rotate(1) in the onLoad attribute of the body.
	ie: <body bgcolor="red" onLoad="rotate(1)">
4)	The banner will be located wherever you place the
	<div id="BANNER"></div> tag. Anything inside the
	div tag will not show up.
------------------------------------------------------------------
*/
function rotate(i) {
  switch (i)
  {
	case 1:
		BANNER.innerHTML = "banner1 html code"; //Change
		setTimeout("rotate(2)", 15000);
	break;
	case 2:
		BANNER.innerHTML = "banner2 html code"; //Change
		setTimeout("rotate(3)", 15000);
	break;
	case 3:
		BANNER.innerHTML = "banner3 html code"; //Change
		setTimeout("rotate(1)", 15000);
	break;
	default:
		alert("Invalid Interval!");
  }
}
</script>
</head>
<body onLoad="rotate(1)">
<div id="BANNER"></div>
</body>
</html>
```

