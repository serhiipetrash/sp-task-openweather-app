<template>
  <div>
    <header>
      <nav>
        <NuxtLink to="/">Main</NuxtLink>
        <NuxtLink to="/favorites">Favorites</NuxtLink>

      </nav>
    </header>

    <slot />

  </div>
</template>

<style>
*,
*::before,
*::after{box-sizing:border-box;}
a{text-decoration:none; color:inherit; cursor:pointer;}
button{background-color:transparent; color:inherit; border-width:0; padding:0; cursor:pointer;}
figure{margin:0;}
input::-moz-focus-inner {border:0; padding:0; margin:0;}
ul, ol, dd{margin:0; padding:0; list-style:none;}
/* h1, h2, h3, h4, h5, h6{margin:0; font-size:inherit; font-weight:inherit;} */
/* p{margin:0;} */
cite {font-style:normal;}
fieldset{border-width:0; padding:0; margin:0;}

body {
  font-family: Arial, Helvetica, sans-serif;
  margin: 0;
}
header {
  background-color: #6b5b95;
}
nav {
  max-width: 1200px;
  margin: 0 auto;
  display: flex;
  gap: 1rem;
  padding: 1rem;
  font-size: 1.2rem;
  font-weight: bold;
  color: white;
  text-transform: uppercase;
}
.router-link-active {
  color:tomato
}
</style>