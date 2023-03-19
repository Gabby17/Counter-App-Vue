<script setup>

</script>
<template>
    <div class="home">
        <h1>Welcome!👋</h1>
        <h1>Counter-App-Vue 🚀</h1>
        <ul class="list">
            <RouterLink to="/">
                <li>Home</li>
            </RouterLink>
            <RouterLink to="/about">
                <li>Documentation</li>
            </RouterLink>
            <RouterLink to="/counter">
                <li>Counter</li>
            </RouterLink>
            <RouterLink to="/more">
                <li>More</li>
            </RouterLink>
        </ul>
    </div>
</template>

<style scoped>
.home {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    height: 100vh;
    width: 40vw;
    padding: 3em;
    border: 0.5px solid transparent;
    border-right-color: #ffc700;
}

img {
    width: 80%;
    padding: 20px;
    border-radius: 100px;
}

@media (width < 770px) {
    .home {
        height: 30vh;
        border-bottom-color: #ffc700;
        border-right-color: #000000;
        width: 100%;
    }

    img {
        width: 40%;
    }
}

.list {
    display: flex;
    list-style: none;
    margin-block: 10px;
}

li {
    padding: 10px;
    margin-top: 14px;
    border: 1px solid #ffc700;
    margin-inline: 6px;
    border-radius: 8px;
    cursor: pointer;
    font-weight: lighter;
}

li:hover {
    border: 1px solid #ffffff;
}

</style>