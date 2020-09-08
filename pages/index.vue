<template>
    <div class="container">
        <div>
            <h1 class="title">nuxt-typeform</h1>
            <Typeform class="typeform" url="https://gilber963646.typeform.com/to/ebAUrvb5" :hide-headers="true" :hide-footer="true" :opacity="0" :on-submit="onSubmit" />
            <p class="who">Example using the <a href="https://www.npmjs.com/package/nuxt-typeform" target="_blank">nuxt-typeform</a> package from <a href="https://www.github.com/jgmullor" target="_blank">@jgmullor</a></p>
        </div>
    </div>
</template>

<style>
.container {
    margin: 0 auto;
    min-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
}

.title {
  font-family:
    'Quicksand',
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
  padding-bottom: 0.2em;
}
.typeform {
    height: 400px;
    border: 1px solid #666666;
}
.who {
    margin-top: 0.5em;
}
</style>

<script>
    import Typeform from 'nuxt-typeform';
    export default {
        methods: {
            onSubmit () {
                alert("Nice job! =)");
            }
        }
    };
</script>
