<script>
import CardListComponent from './components/CardList.component.vue';
import TableComponent from './components/Table.component.vue';

export default {
  components: {
    TableComponent,
    CardListComponent
  },
  data() {
    return {
      buttonText: 'Card'
    };
  },
  methods: {
    changeView() {
      this.buttonText = this.buttonText === 'Card' ? 'Table' : 'Card';
    }
  }
}

</script>

<template>
  <button class="btn btn-primary" @click="changeView">{{ buttonText }}</button>
  <TableComponent v-if="buttonText === 'Card'"></TableComponent>
  <CardListComponent v-if="buttonText === 'Table'"></CardListComponent>
</template>

<style scoped>
  
</style>
