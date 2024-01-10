<template>
    <div class="skill-container">
        <div class="row">
            <div class="col-12 col-md-6 left-col">
                <router-link to="/" class="btn back-btn"><i class="fas fa-angle-left"></i> Back to Home</router-link>
                <img src="https://i.postimg.cc/c4Y3sc1q/D85-ADA04-101-D-40-F4-9521-EFE0957-CFCAE.jpg" alt="Diego Allies" class="hero-image">
            </div>
            <div class="col-12 col-md-6 right-col">
                <h1 class="skills-title">Skills</h1>
                <div class="skill-entry" v-for="skill in skills" :key="skill.name">
                    <div class="skill-name">{{ skill.name }}</div>
                    <div class="progress">
                        <div class="progress-bar" :style="{width: skill.level}"></div>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <Footer />
    </template>
    
    <script>
    import Footer from '@/components/Footer.vue';
    
    export default {
        components: {
            Footer
        },
        data() {
            return {
                skills: [
                    { name: 'JavaScript', level: '85%' },
                    { name: 'Vue.js', level: '90%' },
                    { name: 'Angular', level: '75%' },
                    { name: 'Next.js', level: '80%' },
                    { name: 'Node.js', level: '80%' },
                    { name: 'MongoDB', level: '80%' },
                    { name: 'Firebase', level: '70%' },
                    { name: 'HTML', level: '95%' },
                    { name: 'CSS/SASS', level: '95%' },
                    { name: 'MySQL', level: '85%' },
                    // Add more skills as needed here
                ]
            };
        }
    };
    </script>
    
    <style scoped>
    .skill-container {
        display: flex;
        min-height: 100vh;
        background-color: #eff3f6;
    }
    
    .left-col {
        padding: 20px;
    }
    
    .hero-image {
        width: 100%;
        max-width: 100%;
        height: auto;
        display: block;
        margin-bottom: 20px;
    }
    
    .right-col {
        background: #363636;
        color: #fff;
        padding: 40px;
    }
    
    .skills-title {
        font-size: 2rem;
        margin-bottom: 20px;
    }
    
    .skill-entry {
        margin-bottom: 20px;
    }
    
    .skill-name {
        font-size: 1.2rem;
        margin-bottom: 5px;
    }
    
    .progress {
        background: #ccc;
        border-radius: 2px;
    }
    
    .progress-bar {
        height: 10px;
        border-radius: 2px;
        background: #4caf50;
        transition: width 0.6s ease;
    }
    
    .btn.back-btn {
        margin-bottom: 30px;
        color: #fff;
        background-color: transparent;
        border: 1px solid #fff;
    }
    
    @media (max-width: 767px) {
        .skill-container {
            flex-direction: column;
        }
    
        .right-col {
            padding: 20px;
        }
    
        .skills-title {
            font-size: 1.5rem;
        }
    }
    </style>