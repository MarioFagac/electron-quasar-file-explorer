<template>
  <q-list
    no-border
    link
    inset-delimiter
  >
    <q-item-label header>Shortcuts</q-item-label>
    <q-item @click.native="onHome" clickable>
      <q-item-section side>
        <q-icon name="home" />
      </q-item-section>
      <q-item-section>Home</q-item-section>
    </q-item>
    <q-item @click.native="onDesktop" clickable>
      <q-item-section side>
         <q-icon name="desktop_windows" />
         </q-item-section>
      <q-item-section>Desktop</q-item-section>
    </q-item>
    <q-item @click.native="onDocuments" clickable>
         <q-item-section side>
         <q-icon name="folder" />
         </q-item-section>
      <q-item-section>Documents</q-item-section>
    </q-item>
    <q-item @click.native="onDownloads" clickable>
      <q-item-section side>
         <q-icon name="vertical_align_bottom" />
         </q-item-section>
      <q-item-section>Downloads</q-item-section>
    </q-item>
    <q-item @click.native="onPictures" clickable>
      <q-item-section side>
         <q-icon name="image" />
         </q-item-section>
      <q-item-section>Pictures</q-item-section>
    </q-item>
    <q-item @click.native="onMusic" clickable>
      <q-item-section side>
        <q-icon name="music_note" />
        </q-item-section>
      <q-item-section>Music</q-item-section>
    </q-item>
    <q-item @click.native="onMovies" clickable>
      <q-item-section side>
        <q-icon name="local_movies" />
        </q-item-section>
      <q-item-section>Movies</q-item-section>
    </q-item>
  </q-list>
</template>

<script>
export default {
  name: 'Shortcuts',

  data () {
    return {}
  },

  methods: {
    onHome: function () {
      this.$emit('selected', 'home')
    },
    onDesktop: function () {
      this.$emit('selected', 'desktop')
    },
    onDocuments: function () {
      this.$emit('selected', 'documents')
    },
    onDownloads: function () {
      this.$emit('selected', 'downloads')
    },
    onPictures: function () {
      this.$emit('selected', 'pictures')
    },
    onMusic: function () {
      this.$emit('selected', 'music')
    },
    onMovies: function () {
      this.$emit('selected', 'videos')
    }
  }
}
</script>

<style>
</style>
