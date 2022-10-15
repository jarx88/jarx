<template>
  <div class="mb-6">
    <h2
      class="mt-6 text-4xl text-gray-700 font-bold capitalize dark:text-blue-200"
    >
      Witam🖖
    </h2>
    <p class="mt-8 mb-4 dark:bg-gray-800 dark:text-blue-200 text-justify">
    Informatyka jest moją pasją i zajmuje się nią od najmłodszych lat. Dzięki temu posiadam bogaty wachlarz doświadczeń. Chcąc poszerzyć swoje zainteresowania wybrałem kierunek studiów związany z moją pasją.
    Od 2019 jestem specjalistą od sp. Informatyki w mini korporacji. Do zakresu moich obowiązków należy administrowanie Serwerów opartych na linuxie ponad 10 maszyn. Systemy zostały własnoręcznie wdrożone od zera w serowni Oracle. Administruje bardzo dużą bazę PostgreSQL. Dodatkowo jestem administratorem Active Directory. Zajmuje się bezpieczeństwem sieci i konfiguracją sieci wraz z rozwiązaniami VPN dla pracy zdalnej. Dodatkowo jestem osobą odpowiedzialny za wsparcie zdalne ponad 500 komputerów. W celu usprawnienia pracy korporacji napisałem kilkanaście programów do wsparcia i automatyzacji działu zakupów i działu księgowego.

    Zajmuje się dodatkowo tworzeniem stron internetowych. Napisałem kilka programów w środowisku skryptowym, w tym kilka botów.

    Jestem osobą bardzo spokojną i opanowaną, dlatego wspaniale się dogaduję
    z innymi. Współpraca ze mną zawsze jest na najwyższym poziomie.
    </p>
    <p class="mt-8 mb-4 dark:bg-gray-800 dark:text-blue-200"> <vue-typed-js :strings="['programować', 'administrować'] " :loop="true" >
  <h1>Kocham <span class="typing"></span></h1>
</vue-typed-js>
</p>
  </div>
</template>
<script>
import VueTypedJs from "~/plugins/vue-typed-js";
export default {
  mounted() {
    VueTypedJs.initTypedJS();
  },  
};
</script>
<style></style>