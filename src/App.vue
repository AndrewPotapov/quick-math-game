<template>
  <div
    class="h-screen w-screen p-7 grid grid-cols-4 grid-rows-4 gap-4 xl:gap-7 text-on-surface-light dark:text-on-surface-dark bg-light dark:bg-dark"
  >
    <div class="flex flex-col justify-center">
      <img
        src="../img/logo-dark.svg"
        alt="logo"
        class="w-2/3 h-fit self-center rounded-lg transition-colors p-2"
      />
      <div class="flex justify-between flex-row mt-5">
        <button class="accessibility-button py-2 px-3 xl:py-4 xl:px-7">
          <span
            class="text-inhirit text-base xl:text-2xl font-semibold text-on-light dark:text-on-dark"
            >Pomoc</span
          >
        </button>
        <button class="accessibility-button p-2 xl:p-4">
          <span class="text-inhirit">
            <svg
              width="48"
              height="48"
              viewBox="0 0 48 48"
              xmlns="http://www.w3.org/2000/svg"
              class="w-6 h-6 xl:w-8 xl:h-8 fill-on-light dark:fill-on-dark"
            >
              <path
                d="M24 4C12.96 4 4 12.96 4 24C4 35.04 12.96 44 24 44C35.04 44 44 35.04 44 24C44 12.96 35.04 4 24 4ZM22 39.86C14.1 38.88 8 32.16 8 24C8 22.76 8.16 21.58 8.42 20.42L18 30V32C18 34.2 19.8 36 22 36V39.86ZM35.8 34.78C35.28 33.16 33.8 32 32 32H30V26C30 24.9 29.1 24 28 24H16V20H20C21.1 20 22 19.1 22 18V14H26C28.2 14 30 12.2 30 10V9.18C35.86 11.56 40 17.3 40 24C40 28.16 38.4 31.94 35.8 34.78Z"
              />
            </svg>
          </span>
        </button>
        <button @click="toggleTheme" class="accessibility-button p-2 xl:p-4">
          <span class="text-inhirit">
            <svg
              width="48"
              height="48"
              viewBox="0 0 48 48"
              xmlns="http://www.w3.org/2000/svg"
              class="w-6 h-6 xl:w-8 xl:h-8 fill-on-light dark:fill-on-dark"
            >
              <path
                d="M24 18C27.3 18 30 20.7 30 24C30 27.3 27.3 30 24 30C20.7 30 18 27.3 18 24C18 20.7 20.7 18 24 18ZM24 14C18.48 14 14 18.48 14 24C14 29.52 18.48 34 24 34C29.52 34 34 29.52 34 24C34 18.48 29.52 14 24 14ZM4 26H8C9.1 26 10 25.1 10 24C10 22.9 9.1 22 8 22H4C2.9 22 2 22.9 2 24C2 25.1 2.9 26 4 26ZM40 26H44C45.1 26 46 25.1 46 24C46 22.9 45.1 22 44 22H40C38.9 22 38 22.9 38 24C38 25.1 38.9 26 40 26ZM22 4V8C22 9.1 22.9 10 24 10C25.1 10 26 9.1 26 8V4C26 2.9 25.1 2 24 2C22.9 2 22 2.9 22 4ZM22 40V44C22 45.1 22.9 46 24 46C25.1 46 26 45.1 26 44V40C26 38.9 25.1 38 24 38C22.9 38 22 38.9 22 40ZM11.98 9.16C11.2 8.38 9.92 8.38 9.16 9.16C8.38 9.94 8.38 11.22 9.16 11.98L11.28 14.1C12.06 14.88 13.34 14.88 14.1 14.1C14.86 13.32 14.88 12.04 14.1 11.28L11.98 9.16ZM36.72 33.9C35.94 33.12 34.66 33.12 33.9 33.9C33.12 34.68 33.12 35.96 33.9 36.72L36.02 38.84C36.8 39.62 38.08 39.62 38.84 38.84C39.62 38.06 39.62 36.78 38.84 36.02L36.72 33.9ZM38.84 11.98C39.62 11.2 39.62 9.92 38.84 9.16C38.06 8.38 36.78 8.38 36.02 9.16L33.9 11.28C33.12 12.06 33.12 13.34 33.9 14.1C34.68 14.86 35.96 14.88 36.72 14.1L38.84 11.98ZM14.1 36.72C14.88 35.94 14.88 34.66 14.1 33.9C13.32 33.12 12.04 33.12 11.28 33.9L9.16 36.02C8.38 36.8 8.38 38.08 9.16 38.84C9.94 39.6 11.22 39.62 11.98 38.84L14.1 36.72Z"
              />
            </svg>
          </span>
        </button>
      </div>
    </div>
    <div
      class="card col-span-2 flex flex-col justify-between row-span-2 px-14 py-9"
    >
      <h1 class="xl:text-6xl font-semibold block">Strefa gry</h1>
      <div class="flex flex-row h-full justify-between">
        <div class="flex flex-col w-1/2 justify-between mt-6">
          <button class="game-mode-button">Tryb edukacyjny</button>
          <button class="game-mode-button">Wkrótce</button>
          <button class="game-mode-button">Wkrótce</button>
        </div>
        <div class="flex flex-row justify-between w-1/2">
          <div class="flex flex-col justify-between">
            <span>level 1</span>
            <span>level 2</span>
            <span>level 3</span>
          </div>
          <button class="game-mode-button pr-6">Zacznij</button>
        </div>
      </div>
    </div>
    <div class="card p-9 row-span-2">
      <h2>Porady i Wskazówki</h2>
    </div>
    <div class="card p-9 row-span-2">
      <h2>Powiadomiena</h2>
    </div>
    <div class="card card-disabled"></div>
    <div class="card card-disabled"></div>
    <div class="card p-9 row-span-2 flex flex-col justify-between">
      <h2>Przyjaciele</h2>
      <div class="flex items-center h-full w-full">
        <p class="block mx-auto">
          Po<button class="login-button">zalogowaniu / rejestracji</button>
          <br />
          tu będziesz mógł dodawać przyjaciele
        </p>
      </div>
    </div>
    <div class="card flex justify-center items-center">
      <p class="block">
        Po<button class="login-button">zalogowaniu / rejestracji</button>
        <br />
        tu będzie twój profil
      </p>
    </div>
    <div class="card card-disabled"></div>
    <div class="card card-disabled"></div>
  </div>
</template>

<script>
export default {
  name: "App",
  components: {},
  created() {
    if (localStorage.theme == undefined) {
      localStorage.setItem(
        "theme",
        window.matchMedia("(prefers-color-scheme: dark)").matches
      );
    }
    this.theme = JSON.parse(localStorage.getItem("theme"));
  },
  data() {
    return {
      theme: false,
    };
  },
  methods: {
    toggleTheme() {
      this.theme = !this.theme;
    },
  },
  watch: {
    theme(themeToSet) {
      const rootNode = document.documentElement;
      localStorage.theme = themeToSet;
      if (themeToSet) {
        rootNode.classList.add("dark");
        return;
      }
      rootNode.classList.remove("dark");
    },
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
