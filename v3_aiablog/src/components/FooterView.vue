<template>
  <v-footer>
      <v-card
        elevation="0"
        rounded="0"
        width="100%"
        class="bg-grey text-center"
      >
        <v-card-text>
          <v-btn
            class="mx-4"
            icon="fa-brands fa-facebook"
            variant="plain"
            color="white"
            href="https://www.facebook.com/a11anigue/"
            target="_blank"
          ></v-btn>
          <v-btn
            class="mx-4"
            icon="fa-brands fa-instagram"
            variant="plain"
            color="white"
            href="https://www.instagram.com/aia11anigue/"
            target="_blank"
          ></v-btn>
        </v-card-text>

        <v-card-text class="text-white">
          @ {{ new Date().getFullYear() }} —
          <strong>AIAllanigue Blog</strong>
        </v-card-text>
      </v-card>
    </v-footer>
</template>

<script>
export default {

}
</script>

<style>
.v-footer {
  padding: 8px 0 !important;
}
</style>