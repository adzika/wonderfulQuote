<template>
  <div class="container">
    <div class="row">
      <div class="col-xs-12">
        <app-quote>
          <h2 slot="quoteTitle">{{ quoteTitle }}</h2>
          <p slot="content">A wonderful Quote</p>
        </app-quote>
      </div>
    </div>
  </div>
</template>

<script>
  import Quote from './components/Quote.vue';
  import Author from './components/Author';
  import New from './components/New';

  export default {
    data: function() {
      return {
        quoteTitle: "The Quote"
      }
    },
    components: {
      appQuote: Quote,
      appAuthor: Author,
      appNew
    }
  }
</script>
