<template>
  <div>

  	{{sublingChild}}
  </div>
</template>

<script>
export default {
  name: 'sublingChild',
  data () {
    return {
      sublingChild: 'sublingChild1'
    }
  },
  created () {
    this.$emit('sublingParent', this.sublingChild)
  }
}
</script>