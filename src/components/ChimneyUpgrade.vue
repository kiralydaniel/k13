<template>
  <div class="text-box">
    <h1>
      <span class="text-dark" style="margin-top: 30px;">A kéményátalakítás</span>
      <br/>
      <span class="text-light">lépésről lépésre</span>
    </h1>
    <div class="text-box-row">
      <div class="text-box-left">
        <div class="circle">1</div>
        <p>A meglévő készülékek ideiglenes lecsatlakoztatásával lehetőve tesszük a kémény pontos felmérését és előkészítjük a bekötő nyílásokat az acél béléscső fogadására.</p>
      </div>
      <div class="text-box-right">
        <div class="circle">2</div>
        <p>A felmért adatok alapján összeállítjuk teljes hosszában a bélésszerkezetet, melyet a kémény felső kitorkollásánál bevezetve nyerjük a bélelt kürőt.</p>
      </div>
    </div>
    <div class="text-box-row" ref="targetElement">
      <div class="text-box-left">
        <div class="circle">3</div>
        <p>A kazáncsatlakoztatásoknál beépítjük a speciális füstgázcsappantyúkat, valamint kialakítjuk az alsó kondenzátumelvezetési pontot is.</p>
      </div>
      <div class="text-box-right">
        <div class="circle">4</div>
        <p>Miután mérőműszerrel ellenőrizzük a megfelelő nyomásállóságot, felhelyezzük a membrános takarólemezeket, végül visszacsatlakoztatjuk a kazánokat.</p>
      </div>
    </div>
  </div>
</template>

<style src="./Style.css"></style>

<script>
export default {
  name: 'ChimneyUpgrade',
};
</script>
