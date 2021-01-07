<template>
    <div>
        <b-col>
          <b-card :title="name"
          :img-src="img"
          img-alt="Job-info"
          img-top
          tag="article"
          style="max-width:20rem"
          class="mb-2"
          :b-card="text"
          :sub-title="text"
          >
            <b-card-text :text="text">
            </b-card-text>
            <b-button :href="link" variant="primary" >Visit</b-button>
          </b-card>
        </b-col>
    </div>
</template>

<script>
    export default {
        props: ["name", "text", "img", "link"],
    }
</script>

<style lang="scss" scoped>

</style>