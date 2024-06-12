<template>
  <div class=" justify-content-center rounded-4" >
    <button
      class="btn sidebar-btn"
      @click="toggleSelected"
    >
      Clique em mim
    </button>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const isSelected = ref(false);

const toggleSelected = () => {
  isSelected.value = !isSelected.value;
};

defineOptions({
  name: 'EssentialLink'
});

export interface EssentialLinkProps {
  title: string;
  caption?: string;
  link?: string;
  icon?: string;
};

withDefaults(defineProps<EssentialLinkProps>(), {
  caption: '',
  link: '#',
  icon: '',
});
</script>

<style scoped>
.sidebar-btn {
  background-color: transparent;
  border: none;
  cursor: pointer;
}


.sidebar-btn:hover {
  background-color: #5d87ff;
  color: white;
}

.sidebar-btn.selected:hover {
  background-color:  #5d87ff;
  opacity: 0.75;
  color: white;
}
</style>
