<template>
  <ul>
    <knowledge-element
      v-for="topic in topics"
      :key="topic.id"
      :id="topic.id"
      :topic-name="topic.title"
      :description="topic.description"
    ></knowledge-element>
  </ul>
</template>
<!--@select-topic="$emit('select-topic', $event)"-->
<script>
export default {
  inject: ['topics'],
};
</script>
//emits: ['select-topic']