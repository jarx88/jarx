<template>
  <div class="mb-6">
    <h2
      class="mt-6 text-4xl text-gray-700 font-bold capitalize dark:text-blue-200"
    >
      Witam🖖
    </h2>
    <p class="mt-8 mb-4 dark:bg-gray-800 dark:text-blue-200 text-justify">
		Informatyka jest moją pasją i zajmuję się nią od najmłodszych lat. Dzięki temu posiadam bogaty wachlarz doświadczeń. Chcąc poszerzyć swoje zainteresowania, wybrałem kierunek studiów związany z moją pasją. Od 2019 roku jestem specjalistą ds. informatyki w mini korporacji. Do zakresu moich obowiązków należy administrowanie serwerów opartych na Linuksie, na ponad 10 maszynach. Systemy zostały własnoręcznie wdrożone od zera w serowni Oracle. Administruję bardzo dużą bazą PostgreSQL. Dodatkowo jestem administratorem Active Directory. Zajmuję się bezpieczeństwem sieci i konfiguracją sieci wraz z rozwiązaniami VPN dla pracy zdalnej. Dodatkowo jestem osobą odpowiedzialną za wsparcie zdalne ponad 500 komputerów. W celu usprawnienia pracy korporacji napisałem kilkanaście programów do wsparcia i automatyzacji działu zakupów i działu księgowego.</p>
<p>
Zajmuję się dodatkowo tworzeniem stron internetowych. Napisałem kilka programów w środowisku skryptowym, w tym kilka botów.
</p>
<p>
Jestem osobą bardzo spokojną i opanowaną, dlatego wspaniale się dogaduję z innymi. Współpraca ze mną zawsze jest na najwyższym poziomie.
     <vue-typed-js :strings="['programować⌨️', 'komputery💻','Windows🪟','Linux🐧','Ai🧠'] " :loop="true" :fadeOutDelay="1000" :typeSpeed="100">
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