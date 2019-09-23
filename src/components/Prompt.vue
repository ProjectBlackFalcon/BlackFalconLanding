<template>
	<div class="prompt">
		<input contenteditable="true" placeholder="Enter your text here..."/>
		<button>Complete</button>
		<p>{{ msg }}</p>
	</div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class Prompt extends Vue {
	@Prop() private msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
input{
	background-color: #E6DAFF;
	color: #323232;
	border: none;
	border-radius: 2vw 2px 2px 2vw;
	padding: 10px 20px;
	font-size: 2vw;
	margin: 40px 0;
	outline: none;
	transition: ease .1s;
}
button{
	background: linear-gradient(45deg, #EF00FF, #AD00FF);
	border: solid 0px #EF00FF;
	border-radius: 2px;
	padding: 10px 20px;
	font-size: 2vw;
	margin: 40px 0;
	color: #E6DAFF;
	border-radius: 0 2vw 2vw 0;
	pointer-events:all;
	outline: none;
	transition: ease 0.3s;
}
button:hover{
	border: solid 5px #E6DAFF;
	transition: all .2s;
	padding: 5px 25px;
}
p {
	font-family: "Raleway Light Italic";
	font-size: 3vw;
	color: #E6DAFF;
}
</style>
