# canvas_createImageData
createImageData创建图像数据

<pre>
<code>
for(var i = 0; i < canvas.height; i++){
	for(var j = 0; j < canvas.width; j++){
		var p = i*canvas.width + j;
		pixelData[p*4 + 0] = parseInt(Math.pow(Math.cos(Math.atan2(j-canvasWidth/2, i-canvasHeight/2)/2),2)*255);
		pixelData[p*4 + 1] = parseInt(Math.pow(Math.cos(Math.atan2(j-canvasWidth/2, i-canvasHeight/2)/2-2*Math.acos(-1)/3),2)*255);
		pixelData[p*4 + 2] = parseInt(Math.pow(Math.cos(Math.atan2(j-canvasWidth/2, i-canvasHeight/2)/2+2*Math.acos(-1)/3),2)*255);
		pixelData[p*4 + 3] = 255;
	}
}
</code>
</pre>