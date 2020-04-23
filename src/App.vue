<template>
<div>
  <div class="etabs-tabgroup">
    <div class="etabs-tabs"></div>
    <div class="etabs-buttons"></div>
  </div>
  <div class="etabs-views">
  </div>
</div>
</template>

<script>
//const TabGroup = require("electron-tabs");
import TabGroup from 'electron-tabs'
export default {
  name: 'App'
};
setTimeout(function(){
  let tabGroup = new TabGroup();
  tabGroup.addTab({
    title: "Portal",
    src: "https://portal.daou.co.kr",
    visible: true
  });
  tabGroup.addTab({
    title: "Jira",
    src: "https://issue.daou.co.kr",
    visible: true
  });
  tabGroup.addTab({
    title: "Stash",
    src: "https://stash.daou.co.kr",
    visible: true
  });
},1000);

</script>
