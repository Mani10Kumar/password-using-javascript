# password-using-javascript
for week password ,good password ,strong password
<input onkeyup="abc()">

<h1 id="a">value</h1>
<h1 id="b">value's length</h1>
<h1 id="c">message</h1>


<script type="text/javascript">
	function abc()
	{
		a=document.querySelector("h1#a")
		b=document.querySelector("h1#b")
		c=document.querySelector("h1#c")

		input=document.querySelector("input")

		a.innerHTML=input.value
		b.innerHTML=input.value.length

		x=input.value.length
		color="black"
		bg="white"
		if(x==0)
		{
			c.innerHTML="enter something"
		}
		else if(x<4)
		{
			color="white"
			bg="red"
			c.innerHTML="weak data"
		}
		else if(x<10)
		{
			color="black"
			bg="yellow"
			c.innerHTML="good data"
		}
		else if(x>=10)
		{
			color="white"
			bg="green"
			c.innerHTML="strong data"
		}
		c.style.color=color
		c.style.background=bg


	}
</script>
