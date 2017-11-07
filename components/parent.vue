<template>
  <div>
  	{{parent}}{{sublingEmit}}
  	<child :parentChild="parent"
  		   :sublingChild="sublingEmit"
  		   />
  	<subling-child @sublingParent="sublingEmit = arguments[0]"/>
  </div>
</template>

<script>
import child from '@/components/child'
import sublingChild from '@/components/sublingChild'

export default {
  name: 'parent',
  data () {
    return {
      parent: 'parent1',
      sublingEmit: ''
    }
  },
  components: {
    child,
    sublingChild
  }
}
</script>