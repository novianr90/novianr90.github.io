<template>
    <header>
        <nav>
            <ul>
                <li><a href="#about">About</a></li>
                <li><a href="#portfolio">Portfolio</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>
</template>

<script>
export default {
    name: 'HeaderSection'
}
</script>

<style scoped>
header {
    background-color: #333;
    padding: 1rem;
}

nav ul {
    list-style: none;
    display: flex;
    justify-content: center;
}

nav ul li {
    margin: 0 1rem;
}

nav ul li a {
    color: white;
    text-decoration: none;
    font-size: 1.2rem;
}
</style>
