<script>
import PageHeader from './Lib/PageHeader.svelte';
import Hero from './Index/Hero.svelte';
import Main from './Index/Main.svelte';
import Sidebar from './Lib/Sidebar.svelte';
import PageFooter from './Lib/PageFooter.svelte';
</script>

<div class="grid">
	<div class="header">
		<PageHeader />
	</div>
	<div class="hero">
		<Hero />
	</div>
	<div class="main">
		<Main />
	</div>
	<div class="sidebar">
		<Sidebar />
	</div>
	<div class="footer">
		<PageFooter />
	</div>
</div>

<style>
.grid {
	display: grid;
	grid-template:
		"😄 😄 😄 😄" auto
		"🚀 🚀 🚀  ↕️" 500px
		" 🖼 🖼 🖼 ↕️" auto
		"👟 👟 👟 👟" auto /
		1fr 1fr 1fr 200px;
}
.header {
	grid-area: 😄;
}
.hero {
	grid-area: 🚀;
}
.sidebar {
	grid-area: ↕️;
}
.main {
	grid-area: 🖼;
}
.footer {
	grid-area: 👟;
}
</style>
