<script setup>
    
</script>
<template>
    <div v-if="mostrarResultado" class="contenedor-resultado">
        <h2>
          Cotizacion
        </h2>

        <div class="resultado">
          <img 
            :src="'https://cryptocompare.com/' + cotizacion.IMAGEURL" 
            alt="imagen">
          <div>
            <p>El precio es de: <span>{{ cotizacion.PRICE }}</span></p>
            <p>Precio mas alto es: <span>{{ cotizacion.HIGHDAY }}</span></p>
            <p>Precio mas bajo del dia: <span>{{ cotizacion.LOWDAY }}</span></p>
            <p>Variacion ultimas 24hr: <span>{{ cotizacion.CHANGEPCT24HOUR }}%</span></p>
            <p>Ultima actualizacion: <span>{{ cotizacion.LASTUPDATE }}</span></p>
          </div>
        </div>
      </div>
</template>