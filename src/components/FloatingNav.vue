<template>
  <div id="nav">
    <router-link class="link" :to="{ name: 'Home' }"
      ><svg
        xmlns="http://www.w3.org/2000/svg"
        class="w-6 h-6"
        fill="none"
        viewBox="0 0 24 24"
        stroke="currentColor"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="1.5"
          d="M3 12l2-2m0 0l7-7 7 7M5 10v10a1 1 0 001 1h3m10-11l2 2m-2-2v10a1 1 0 01-1 1h-3m-6 0a1 1 0 001-1v-4a1 1 0 011-1h2a1 1 0 011 1v4a1 1 0 001 1m-6 0h6"
        /></svg
    ></router-link>

    <router-link class="link" :to="{ name: 'About' }"
      ><svg
        xmlns="http://www.w3.org/2000/svg"
        class="w-6 h-6"
        fill="none"
        viewBox="0 0 24 24"
        stroke="currentColor"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="1.5"
          d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z"
        />
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="1.5"
          d="M15 11a3 3 0 11-6 0 3 3 0 016 0z"
        /></svg
    ></router-link>

    <router-link class="link" to="{name: 'Account'}"
      ><svg
        xmlns="http://www.w3.org/2000/svg"
        class="w-6 h-6"
        fill="none"
        viewBox="0 0 24 24"
        stroke="currentColor"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          stroke-width="1.5"
          d="M16 7a4 4 0 11-8 0 4 4 0 018 0zM12 14a7 7 0 00-7 7h14a7 7 0 00-7-7z"
        /></svg
    ></router-link>
  </div>
</template>

<style scoped>
#nav {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 203px;
  height: 59px;
  position: fixed;
  bottom: 20px;
  left: 0;
  right: 0;
  margin: 5% auto;
  text-align: center;
  background: #1c8af0;
  box-shadow: 0px 10px 9px -2px rgba(38, 37, 37, 0.29);
  border-radius: 20px;
  z-index: 9999;
}

#nav svg {
  width: 32px;
  height: 32px;
  margin: 0 15px;
  padding-bottom: 2px;
  color: #fff;
  transition: all 0.2s ease-in-out;
}

#nav a.router-link-exact-active svg {
  border-bottom: 3px solid #fff;
  color: #fff;
}
</style>
