<main class="layout-container">
    <nav>
        <a href="/">home</a>
        <a href="/habits">habits</a>
    </nav>
    <slot />
</main>

<style>
    .layout-container {
        max-width: 1440px;
        width: 100%;
        margin: 0 auto;
    }
</style>
