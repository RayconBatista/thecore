<template>
  <section class="bg-gray-100"><!-- Start Features -->
    <div class="container mx-auto px-4 py-12 sm:py-16 md:py-20 xl:py-28">
      <div class="space-y-4 text-center mb-10 lg:mb-16">
        <h2 class="text-4xl md:text-5xl font-semibold">Nossos Produtos</h2>
        <!--        <p class="text-lg md:max-w-md mx-auto">Aliquid officiis cumque sunt sint. Et quo culpa. Enim sed natus molestiae fugiat cum consequatur quia sunt.</p>-->
      </div>
      <div class="grid sm:grid-cols-2 xl:grid-cols-4 gap-6 lg:gap-10">
        <div class="bg-white transition-shadow duration-200 shadow hover:shadow-xl p-6 rounded-lg space-y-6" v-for="(product, index) in getProducts" :key="index">
          <!--          <div class="bg-blue-800 flex items-center justify-center w-12 h-12 rounded-full text-white">-->
          <!--            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor">-->
          <!--              <path fill-rule="evenodd" d="M12.395 2.553a1 1 0 00-1.45-.385c-.345.23-.614.558-.822.88-.214.33-.403.713-.57 1.116-.334.804-.614 1.768-.84 2.734a31.365 31.365 0 00-.613 3.58 2.64 2.64 0 01-.945-1.067c-.328-.68-.398-1.534-.398-2.654A1 1 0 005.05 6.05 6.981 6.981 0 003 11a7 7 0 1011.95-4.95c-.592-.591-.98-.985-1.348-1.467-.363-.476-.724-1.063-1.207-2.03zM12.12 15.12A3 3 0 017 13s.879.5 2.5.5c0-1 .5-4 1.25-4.5.5 1 .786 1.293 1.371 1.879A2.99 2.99 0 0113 13a2.99 2.99 0 01-.879 2.121z" clip-rule="evenodd" />-->
          <!--            </svg>-->
          <!--          </div>-->
          <div class="space-y-4">
            <h4 class="text-2xl md:text-3xl font-semibold">{{ product.title }}</h4>
            <img :src="product.urlImage" alt="">
            <p>Adipisci tempora pariatur modi recusandae. Omnis neque dolorum. Natus facere voluptatem.</p>
          </div>
        </div>
        <!--        <div class="bg-white transition-shadow duration-200 shadow hover:shadow-xl p-6 rounded-lg space-y-6">-->
        <!--          <div class="bg-blue-800 flex items-center justify-center w-12 h-12 rounded-full text-white">-->
        <!--            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor">-->
        <!--              <path fill-rule="evenodd" d="M6.672 1.911a1 1 0 10-1.932.518l.259.966a1 1 0 001.932-.518l-.26-.966zM2.429 4.74a1 1 0 10-.517 1.932l.966.259a1 1 0 00.517-1.932l-.966-.26zm8.814-.569a1 1 0 00-1.415-1.414l-.707.707a1 1 0 101.415 1.415l.707-.708zm-7.071 7.072l.707-.707A1 1 0 003.465 9.12l-.708.707a1 1 0 001.415 1.415zm3.2-5.171a1 1 0 00-1.3 1.3l4 10a1 1 0 001.823.075l1.38-2.759 3.018 3.02a1 1 0 001.414-1.415l-3.019-3.02 2.76-1.379a1 1 0 00-.076-1.822l-10-4z" clip-rule="evenodd" />-->
        <!--            </svg>-->
        <!--          </div>-->
        <!--          <div class="space-y-4">-->
        <!--            <h4 class="text-2xl md:text-3xl font-semibold">Confecção</h4>-->
        <!--            <p>Adipisci tempora pariatur modi recusandae. Omnis neque dolorum. Natus facere voluptatem.</p>-->
        <!--          </div>-->
        <!--        </div>-->
        <!--        <div class="bg-white transition-shadow duration-200 shadow hover:shadow-xl p-6 rounded-lg space-y-6">-->
        <!--          <div class="bg-blue-800 flex items-center justify-center w-12 h-12 rounded-full text-white">-->
        <!--            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor">-->
        <!--              <path fill-rule="evenodd" d="M3.172 5.172a4 4 0 015.656 0L10 6.343l1.172-1.171a4 4 0 115.656 5.656L10 17.657l-6.828-6.829a4 4 0 010-5.656z" clip-rule="evenodd" />-->
        <!--            </svg>-->
        <!--          </div>-->
        <!--          <div class="space-y-4">-->
        <!--            <h4 class="text-2xl md:text-3xl font-semibold">Brindes Personalizados</h4>-->
        <!--            <p>Adipisci tempora pariatur modi recusandae. Omnis neque dolorum. Natus facere voluptatem.</p>-->
        <!--          </div>-->
        <!--        </div>-->
        <!--        <div class="bg-white transition-shadow duration-200 shadow hover:shadow-xl p-6 rounded-lg space-y-6">-->
        <!--          <div class="bg-blue-800 flex items-center justify-center w-12 h-12 rounded-full text-white">-->
        <!--            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor">-->
        <!--              <path fill-rule="evenodd" d="M11.3 1.046A1 1 0 0112 2v5h4a1 1 0 01.82 1.573l-7 10A1 1 0 018 18v-5H4a1 1 0 01-.82-1.573l7-10a1 1 0 011.12-.38z" clip-rule="evenodd" />-->
        <!--            </svg>-->
        <!--          </div>-->
        <!--          <div class="space-y-4">-->
        <!--            <h4 class="text-2xl md:text-3xl font-semibold">Decoração de Eventos</h4>-->
        <!--            <p>Adipisci tempora pariatur modi recusandae. Omnis neque dolorum. Natus facere voluptatem.</p>-->
        <!--          </div>-->
        <!--        </div>-->
      </div>
    </div>
  </section><!-- End Features -->
</template>

<script>
export default {
  name: "produtos",
  data() {
    return {
      getProducts: [
        {
          id: 1,
          title: 'Banners',
          urlImage: 'https://graficaproarte.com/862-large_default/banners-impressao-digital-express.jpg',
        },
        {
          id: 2,
          title: 'Cartão de Visita',
          urlImage: 'https://http2.mlstatic.com/D_NQ_NP_711634-MLB44545678392_012021-O.jpg',
        },
        {
          id: 3,
          title: 'Cardápios',
          urlImage: 'https://www.diferenterj.com.br/uploads/produtos/cardapio-pvc-1-mm-laminacao-corte-reto-4-4-frente-e-verso-16090830986982264895fe8a8daca5fe.png',
        },
        {
          id: 4,
          title: 'Panfletos',
          urlImage: 'https://http2.mlstatic.com/D_NQ_NP_674260-MLB40724961091_022020-O.jpg',
        },
        {
          id: 5,
          title: 'Quadros em MDF',
          urlImage: 'https://cdn.iset.io/assets/55268/produtos/23149/kit-5-placa-decorativa-paisagens-13-fases-eclipse-luar-1.jpg',
        },
        {
          id: 6,
          title: 'Camisas Personalizadas',
          urlImage: 'https://a-static.mlcdn.com.br/618x463/kit-camisetas-personalizadas-coffee-print-personalizados/coffeeprintpersonalizados/79045c88c24d11eba6714201ac18500e/1dec440ef644b01fbed0619ec5f9c00e.jpg',
        },

        {
          id: 7,
          title: 'Fachadas',
          urlImage: 'https://www.acassius.com.br/wp-content/uploads/Fachada1.jpg',
        },
        {
          id: 8,
          title: 'Cavaletes',
          urlImage: 'https://manausimpressos.com/wp-content/uploads/2019/07/cavalete.jpg',
        },
      ]
    }
  }
}
</script>

<style scoped>

</style>
