<template>

<section class="section">
    <div class="container">
        <h2 class="title">{{title}}</h2>
        <div class="columns">
            <div class="column">
                <div class="field">
                    <label class="label">Markdown input</label>
                    <div class="control">
                        <textarea class="textarea" v-model="inputMarkdown"></textarea>
                    </div>
                </div>
            </div>
            <div class="column">
                <label class="label">Markdown output</label>
                <div class="box" v-html="compiledMarkdown"></div>
            </div>
        </div>
    </div>
</section>

</template>

<script>

import * as marked from "marked";
export default {
    data() {
            return {
                title: "Markdown Editor",
                inputMarkdown: `I'm __using__ *markdown*`
            };
        },
        computed: {
            compiledMarkdown: function() {
                return marked(this.inputMarkdown, {
                    sanitize: true
                });
            }
        }
};

</script>
