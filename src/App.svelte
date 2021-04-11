<script lang='ts'>
	import Typewriter from 'svelte-typewriter'
	const githubRef = () => {
		var url =  'https://github.com/peepopoggers';
		window.open(url, '_blank');
	}
</script>
<main>
	<div class="intro">
		<!-- svelte-ignore a11y-img-redundant-alt -->
		<img src="/images/favicon.png" alt="Profile Picture" title=":D" style="border-radius: 50%; height:200px;">
		<Typewriter interval="50" cursor="true"><h1>My name is faken</h1></Typewriter>
		<div style="max-width: 500px; margin: 0 auto;">
			<p>I specialize in creating JavaScript Applications, mainly including front-end web projects using frameworks built with node.</p>
			<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=peepopoggers&layout=compact&theme=dracula" alt="Language Statistics" style="margin-top: 20px;">
		</div>
	</div>
	<div class="abilities">
		<h1>Skills and Abilities</h1>
		<p></p>
		<div class="container" style="margin-top:0px;">
			<div class="row">
				<div class="one-third column abil">
					<img src="/images/_ionicons_svg_logo-javascript.svg" alt="SVG Logo for Topic">
					<p class="nonorm f20">JavaScript</p>
					<p>I have sufficient experience with the JS Syntax to a high level. I have experience with all the standard programming features to satisfy a front-end project.</p>
				</div>
				<div class="one-third column abil">
					<img src="/images/_ionicons_svg_logo-nodejs.svg" alt="SVG Logo for Topic">
					<p class="nonorm f20">Frameworks</p>
					<p>I use frameworks such as svelte-js and vue-js to compliment my normal HTML, CSS and JavaScript capabilities. I have an understanding in how the frameworks function.</p>
				</div>
				<div class="one-third column abil">
					<img src="/images/_ionicons_svg_logo-css3.svg" alt="SVG Logo for Topic">
					<p class="nonorm f20">Design and Layout</p>
					<p>I love designing beautiful user interfaces that are geometrically correct and that are easy to navigate. I love designing front ends that will satisfy the users.</p>
				</div>
			  </div>
		</div>
	</div>
	<div class="proof">
		<div style="margin: 0 auto; max-width: 600px;">
			<h1 style="padding-top: 10px;">About me</h1>
			<p class="f20" style="padding: 0 10px 0 10px">
				I am a hobbyist developer that has worked with programming languages such as Python and Javascript for a while now.<br><br>
				I have started with high level of experience in python, and I have carried over my knowledge from its syntax into JS dev.<br><br>
				My past experience with teams isn't extensive, but I would be glad to show you what I am capable of.
			</p>
		</div>
		<div class='githubcontainer' on:click={() => githubRef()}>
			<img src="/images/_ionicons_svg_logo-github.svg" alt="SVG Logo for Topic" style="-webkit-filter: invert(100%); filter: invert(100%); height:200px;">
			<h1>Github</h1>
		</div>
	</div>
</main>

<style>
	main {
		text-align: center;
		max-width: none;
	}

	.intro {
		background-color: #141414; 
		padding: 40px 0 50px;
	}

	.abilities {
		padding: 10px 0 40px;
		background-color: #272727;
		display: flex;
  		flex-direction: column;
  		justify-content: center;
  		align-items: center;
	}

	.proof {
		padding: 10px 0 40px;
		animation: colorchange 20s linear 1s infinite;
      	-webkit-animation: colorchange 20s linear 0s infinite alternate;
    }

	.abil {
		padding: 30px 10px 30px 10px;
		background-color: #111111;
		border-radius: 8px;
		margin-bottom:10px;
	}

	.abil > img {
		-webkit-filter: invert(100%);
  		filter: invert(100%);
		height: 100px;
	}
	
	.nonorm {
		padding: 0px;
		margin: 0px;
	}

	.f20 {
		font-size: 20px;
		padding-bottom:20px;
	}

	.githubcontainer {
		padding:20px;
		border: 2px solid white;
		border-radius:8px;
		margin: 0 auto;
		width:250px;
	}

	.githubcontainer:hover {
		cursor: pointer;
		background-color: rgba(0, 0, 0, 0.3)
	}

	@keyframes colorchange
    {
      0%   {background: #e45050; color: white;}
      33%  {background: #2e802e; color: white;}
      66%  {background: #5b5bff; color: white;}
      100% {background: #ff4f4f; color: white;}
    }

    @-webkit-keyframes colorchange /* Safari and Chrome*/
    {
      0%   {background: #e45050; color: white;}
      33%  {background: #2e802e; color: white;}
      66%  {background: #5b5bff; color: white;}
      100% {background: #ff4f4f; color: white;}
    }

	@media (max-width: 640px) {
		
	}
</style>