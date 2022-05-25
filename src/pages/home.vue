<template>
  <div class="md-body">
    <div class="card__wrapper" v-for="item in items" :key="item.id">
      <Card :name="`${item.lvl} level`" :title="item.title">
       template
        {{ item.descr }}
      </Card>
    </div>
  </div>
</template>

<script>
import Card from '../components/UI/Card'
export default {
  components: { Card },
  data() {
    return {
      items: [
        {
          id: 1,
          title: 'Archer',
          descr: 'archer archer archer archer archer archer archer',
          lvl: 4
        },
        {
          id: 1,
          title: 'Wizard',
          descr: ' Wizard Wizard Wizard Wizard Wizard Wizard',
          lvl: 5
        }
      ]
    }
  }
}
</script>
