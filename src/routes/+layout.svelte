<main class="layout-container">
	<nav class="navbar">
		<a href="/">home</a>
		<a href="/habits">habits</a>
	</nav>
	<slot />
</main>

<style>
	.layout-container {
		max-width: 1440px;
		width: 100%;
        height: 100vh;
		margin: 0 auto;
        padding: 0 1rem;
        background-color: blueviolet;
        position: relative;
	}
	:global(body) {
        --ui-grid-col-width: 103px;
        --ui-grid-card-height: 9.6vw;
		font-size: 16px;
        margin: 0;
        padding: 0;
        box-sizing: border-box;
	}
    .navbar {
        height: 10%;
    }
</style>
