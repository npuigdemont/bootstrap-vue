<template>
    <div>
    <h1>Jobs</h1>
        <div v-if="jobs.length">
            <div v-for="job in jobs" :key="job.id" class="job">
                <h3>{{job.title}}</h3>
                <h5>{{job.details}}</h5>
        
            </div>
        </div>
        <div v-else>
            <p>Loading...</p>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            jobs: []
        }
    },
    mounted(){
        fetch('http://localhost:3000/jobs')
        .then((res)=> res.json())
        .then(data => this.jobs = data)
        .catch(err => console.log(err.message))
    },
    name: 'Jobs'
}
</script>