<template>
  <div class="container">
    <div class="row">
      <div class="col-xs-12 col-sm-8 col-sm-offset-2 col-md-6 col-md-offset-3">
        <h1 class="text-center">Super Quiz</h1>
      </div>
    </div>
    <hr />
    <div class="row">
      <div class="col-xs-12 col-sm-8 col-sm-offset-2 col-md-6 col-md-offset-3">
        <component :is="mode"></component>
      </div>
    </div>
  </div>
</template>

<script>
import Answer from "./components/Answer.vue";
import Question from "./components/Question.vue";

export default {
  data() {
    return {
      mode: "Question"
    };
  },
  methods: {},
  components: {
    Answer,
    Question
  }
};
</script>

