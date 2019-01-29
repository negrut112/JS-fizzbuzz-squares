# Fizzbuzz-squares
<p>I have used the HTML and JavaScript to make some squares, constraint by some rules that I will explain below.</p>
<p>You can see the live preview accessing:<a href="https://negrut112.github.io/JS-fizzbuzz-squares/">https://negrut112.github.io/JS-fizzbuzz-squares/</a><br>
<img src="https://i.imgur.com/If5XMoy.jpg">

## HTML
<p>I have used the HTML to define the area where I’m working defining the height, width and the border style:</p>
<p>&lt;canvas id=“myCanvas” height=“310” width=“500” style=“border: 1px solid black”&gt;&lt;/canvas&gt;</p>

## JavaScript

<p>Using a <b><i>if</i></b> condition, I generated 15 squares with 40px side length, arranged on diagonal of the canva.<br>
For each square I assigned a different color according to its divisibilty of a specific number.</p>
<p>To check this I ll give you an example: If we divide the 10th square by 2 we get 5 with 0 remainder, it means that 10 is divisible with 5, because the remainder is 0. For this we have a specfic color otherwise we would had another color.</p>

<pre><code>for(i=0;i&lt;15;i++){<br>
context.fillStyle=‘rgb(128, 128, 128,0.7)’;<br>
if(i%5 === 0 &amp;&amp; i%3 ===0){<br>
context.fillStyle=‘rgb(44, 255, 50,0.55)’;<br>
}else if(i%5 === 0){<br>
context.fillStyle=‘rgb(254, 255, 62, 0.5)’;<br>
}else if(i%3 ===0){<br>
context.fillStyle=‘rgb(0, 82, 251,0.5)’;<br>
}context.fillRect(400+i*-28,250+i*-17,40,40);<br>
}</pre></code>
