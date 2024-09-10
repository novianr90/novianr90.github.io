<template>
    <section id="contact">
        <h1>Contact Me</h1>
        <form @submit.prevent="submitForm">
            <input type="text" v-model="name" placeholder="Your Name" required />
            <input type="email" v-model="email" placeholder="Your Email" required />
            <textarea v-model="message" placeholder="Your Message" required></textarea>
            <button type="submit">Send Message</button>
        </form>
    </section>
</template>

<script>
export default {
    name: 'ContactSection',
    data() {
        return {
            name: '',
            email: '',
            message: ''
        };
    },
    methods: {
        submitForm() {
            alert(`Message sent from ${this.name} (${this.email})`);
        }
    }
}
</script>

<style scoped>
form {
    display: flex;
    flex-direction: column;
    max-width: 400px;
    margin: 0 auto;
}

input,
textarea {
    margin: 0.5rem 0;
    padding: 0.5rem;
    border: 1px solid #ddd;
    border-radius: 4px;
}

button {
    padding: 0.5rem;
    background-color: #333;
    color: white;
    border: none;
    border-radius: 4px;
    cursor: pointer;
}

button:hover {
    background-color: #555;
}
</style>
