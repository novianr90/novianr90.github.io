<template>
    <section id="portfolio">
        <h1>My Portfolio</h1>
        <div class="projects">
            <div class="project" v-for="project in projects" :key="project.id">
                <h3>{{ project.name }}</h3>
                <p>{{ project.description }}</p>
                <a :href="project.link" target="_blank">View Project</a>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'PortfolioSection',
    data() {
        return {
            projects: [
                {
                    id: 1,
                    name: 'Project 1',
                    description: 'This is the first project in my portfolio.',
                    link: 'https://example.com/project1'
                },
                {
                    id: 2,
                    name: 'Project 2',
                    description: 'This is the second project in my portfolio.',
                    link: 'https://example.com/project2'
                }
            ]
        };
    }
}
</script>

<style scoped>
.projects {
    display: flex;
    justify-content: space-around;
    padding: 2rem;
}

.project {
    width: 30%;
    padding: 1rem;
    background-color: #f9f9f9;
    border-radius: 8px;
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
}

.project h3 {
    margin-bottom: 1rem;
}

.project a {
    display: inline-block;
    margin-top: 1rem;
    color: #333;
    text-decoration: underline;
}
</style>
