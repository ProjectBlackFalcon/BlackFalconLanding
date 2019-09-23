<template>
	<div id="app">
		<img height=200 alt="Vue logo" src="./assets/bbf.svg" />
		<Prompt msg="Welcome to Your Vue.js + TypeScript App" />
	</div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import Prompt from "./components/Prompt.vue";

@Component({
	components: {
		Prompt
	}
})
export default class App extends Vue {}
</script>

<style>
html{
	background-color: #323232;
}
body{
	display: flex;
	align-items: center;
	height: 100%;
	width: 100%;
	position: absolute;
	justify-content: center;
}

#app {
	font-family: "Raleway";
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
	text-align: center;
	color: #2c3e50;
	margin-top: 60px;
}

@font-face {
    font-family: "Raleway Light";
    src: url("./assets/fonts/Raleway-Light.ttf");
}

@font-face {
    font-family: "Raleway";
    src: url("./assets/fonts/Raleway-Regular.ttf");
}


@font-face {
    font-family: "Raleway Light Italic";
    src: url("./assets/fonts/Raleway-LightItalic.ttf");
}

@font-face {
    font-family: "Raleway Bold";
    src: url("./assets/fonts/Raleway-Bold.ttf");
}

@font-face {
    font-family: "Raleway Bold Italic";
    src: url("./assets/fonts/Raleway-BoldItalic.ttf");
}

@font-face {
    font-family: "Raleway Black";
    src: url("./assets/fonts/Raleway-Black.ttf");
}

@font-face {
    font-family: "Raleway Black Italic";
    src: url("./assets/fonts/Raleway-BlackItalic.ttf");
}

@font-face {
    font-family: "Raleway Medium";
    src: url("./assets/fonts/Raleway-Medium.ttf");
}

@font-face {
    font-family: "Raleway Medium Italic";
    src: url("./assets/fonts/Raleway-MediumItalic.ttf");
}

@font-face {
    font-family: "Raleway Regular";
    src: url("./assets/fonts/Raleway-Regular.ttf");
}

@font-face {
    font-family: "Raleway Italic";
    src: url("./assets/fonts/Raleway-Italic.ttf");
}

</style>
