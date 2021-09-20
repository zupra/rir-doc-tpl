<template>
  <div class="embed-responsive aspect-9/16">
    <iframe class="embed-responsive-item" :src="`https://www.youtube.com/embed/${video}`"
            frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope;
            picture-in-picture" allowfullscreen
    >
    </iframe>
  </div>
</template>

<script>
export default {
  props: {
    video: {type: String, required:true}
  }
}
</script>
