<template onselectstart="return false">
  <div class="background" ref="vantaBg">
    <p>trevor</p>
    <p>capozza</p>
  </div>
</template>

<script>
document.oncontextmenu =new Function("return false;")

import * as THREE from 'three';
import GLOBE from 'vanta/dist/vanta.globe.min';

export default {
  mounted() {
    this.vantaEffect = GLOBE({
      el: this.$refs.vantaBg,
      THREE: THREE, // Use the imported THREE
      mouseControls: true,
      touchControls: true,
      gyroControls: false,
      minHeight: 200.00,
      minWidth: 200.00,
      scale: 1.00,
      scaleMobile: 1.00,
      color: 0x595959,
      color2: 0x7d7d7d,
      backgroundColor: 0x0
    });
  },
  beforeDestroy() {
    if (this.vantaEffect) this.vantaEffect.destroy();
  }
};

</script>



