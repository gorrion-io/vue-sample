<template>
  <section class="section">
    <div class="container">
      <div class="columns">
        <div class="column">
          <div class="field">
            <label class="label">Name</label>
            <div class="control">
              <input class="input" type="text" v-model="name">
            </div>
          </div>
          <div class="field">
            <label class="label">Emplotyer</label>
            <div class="control">
              <input class="input" type="text" v-model="employer">
            </div>
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
          name: "Dominik",
          employer: "Gorrion"
        };
    }
};
</script>
