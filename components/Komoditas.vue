<template>
  <div>
    <div class="flex items-center px-4 mt-32 align-middle">
      <div class="relative hidden w-8/12 img-overlay lg:block md:block">
        <img :src="`${gambar1}`" alt="Gambar" />
      </div>
      <div class="relative w-full img-overlay">
        <img :src="`${gambar2}`" alt="Gambar" />
      </div>
      <div class="relative hidden w-8/12 lg:block md:block img-overlay">
        <img :src="`${gambar3}`" alt="Gambar" />
      </div>
    </div>
    <div class="flex flex-col justify-center px-4">
      <h1 class="mt-10 mb-5 font-serif text-3xl text-center lg:text-6xl">
        {{ judul }}
      </h1>
      <p class="text-xs lg:text-base">
        {{ deskripsi }}
      </p>
      <Button to="galeri" text="Galeri Poto" class="mx-auto mt-10" />
    </div>
  </div>
</template>

<script>
export default {
  props: ["deskripsi", "judul", "gambar1", "gambar2", "gambar3"],
};
</script>