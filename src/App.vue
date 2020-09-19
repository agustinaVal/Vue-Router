<template>
	<div id="app">
		<div id="Nav-bar">
			<router-link to="/">Home</router-link> |
			<router-link :to="{ name: 'About' }">Sobre mi</router-link> |
			<router-link :to="{ name: 'Contacto' }">Contacto</router-link> |
			<router-link to="/post/1">Último post</router-link> |
		</div>
		<router-view />
	</div>
</template>


<style lang="scss">
#app {
	font-family: Avenir, Helvetica, Arial, sans-serif;
	-webkit-font-smoothing: antialiased;
	-moz-osx-font-smoothing: grayscale;
	text-align: center;
	color: #2c3e50;
	margin: 0px;
	padding: 0px;
	box-sizing: border-box;
}

#Nav-bar {
  background-color: black;
	padding: 30px;

	a {
		font-weight: bold;
		color:white;

		&.router-link-exact-active {
			color: #42b983;
		}
	}
}
</style>
