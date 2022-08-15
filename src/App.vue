<template>
  <div id="app">
    <router-view />
   <!--  <Pageination
      :total="299"
      :page-size="10"
      :current-page="current"
      @changePageEvent="changePageEvent"
    /> -->
  </div>
</template>

<script>
// import Pageination from "@/components/Pageination";
export default {
  name: "App",
  components: {
   // Pageination,
  },
  data() {
    return {
      current: 1,
    };
  },
  methods: {
    changePageEvent(val) {
      this.current = val;
      console.log(val);
    },
  },
};
</script>
