<template>
  <div>
  	{{parentChild}}{{child}}{{sublingChild}}
  </div>
</template>

<script>
export default {
  name: 'child',
  data () {
    return {
      child: 'child1'
    }
  },
  props: [ 'parentChild', 'sublingChild' ]
}
</script>