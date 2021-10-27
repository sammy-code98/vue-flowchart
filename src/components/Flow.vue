<template>
  <div>
          <div class="h3 text-muted display-6">Simple Decision  FlowChart</div>

    <vue-mermaid-string :value="diagram" class="mermaid" />
  </div>
</template>
<script>
import VueMermaidString from "vue-mermaid-string";
import endent from "endent";

export default {
  computed: {
    diagram: () => endent`

         graph TD
   A(Coffee machine <br>not working) --> B{Machine has power?}
   B -->|No| H(Plug in and turn on)
   B -->|Yes| C{Out of beans or water?} -->|Yes| G(Refill beans and water)
   C -->|No| D{Filter warning?} -->|Yes| I(Replace or clean filter)
   D -->|No| F(Send for repair)
      `,
  },
  components: {
    VueMermaidString,
  },
  mounted() {
    // this.mermaid.initialize(this.diagram);
    // this.mermaid.initialize({ startOnLoad: true });
    console.log(this.diagram);
  },
};
</script>
