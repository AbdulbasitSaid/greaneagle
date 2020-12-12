<template>
  <div>
    <div class="flex flex-col h-screen justify-between">
      <Header />
      <div>
        <div class="flex font-sans leading-normal">
          <aside class="w-3/12">
            <side-nav> </side-nav>
          </aside>
          <main class="w-9/12">
            <nuxt />
          </main>
        </div>
      </div>
      <Footer />
    </div>
  </div>
</template>
<style>
</style>