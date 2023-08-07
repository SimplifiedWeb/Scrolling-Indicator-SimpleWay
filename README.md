# Scrolling-Indicator-SimpleWay
# The Main goal is to Understand The Logic How it is working.
# Open project code one side and this readme another side to better understand what I'm trying to say.

Check out Demo: https://simplifiedweb.github.io/Scrolling-Indicator-SimpleWay/
I developed this scrolling project let me explain you in simpler Explanation.

So Now I explain you how i develope this scrolling indicator,

So I'll explain you in a simple way what is this.

documentElement ---> Simple means our <html> element. and scrollHeight, clientHeight was its property.

clientHeight ----> Simply means only visible part of the user, no scrolling or anything only the visible part. 
		or more simply means the white visible part of the browser or window.

scrollHeight ---> Simply means the Total height of the content, total height it doesn't matter content is hidden or 
			overflowed, it gives total height.

scrollTop ---> It gives the position or value of scrolling from the Top to the were the user stop scrolling.

And The firstLine,
document.body.scrollTop ---> This line is for older version like Internet Explorer for compatibility purposes.
docuement.documentElement.scrollTop ---> This used in modern browsers. To Target The value of scrolling from the top to were the use stop scrolling.

So the second Line, 
document.documentElement.scrollHeight - document.documentElement.clientHeight;
it simply means total Height - viewport height. if it give negative value means (require Scrolling) or if it gives positive
 than it means (extra height is availabe, No scrolling or content is shorter less than the viewport height)

And the Last Line, 
(scroll/height)*100;
This line calculates the percentage of the page that has been scrolled.
Simply means, 
current scroll position from the top to were the user stop / total scrollabe height.
 And muliplies by 100 to get the percentage value simple.
  
 Hope This Explanation Helps. Happy Coading.
