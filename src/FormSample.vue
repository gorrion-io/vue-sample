<template>

<section class="section">
    <div class="container">
        <h2 class="title">{{title}}</h2>
        <div class="columns">
            <div class="column">
                <div class="field">
                    <label class="label">Name</label>
                    <div class="control">
                        <input class="input" type="text" v-model="name">
                    </div>
                </div>
                <div class="field">
                    <label class="label">Employer</label>
                    <div class="control">
                        <input class="input" type="text" v-model="employer">
                    </div>
                </div>
            </div>
            <div class="column">
                <label class="label">Message</label>
                <div class="box">
                    Hello, I am <span class="has-text-primary">{{name}}</span> and I work for <span class="has-text-info">{{employer}}</span>!
                </div>
            </div>
        </div>
    </div>
</section>

</template>

<script>

export default {
    data() {
        return {
            title: "Form example",
            name: "Dominik",
            employer: "Gorrion"
        };
    }
};

</script>
