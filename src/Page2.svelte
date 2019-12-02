<script>
  import {send, receive} from './crossfade.js';
</script>
<style>
img{
  display: block;

}

</style>
<main>
  <img out:send="{{key: 'borat'}}" in:receive="{{key: 'borat'}}" alt='Borat' src='favicon.png'>
  <h1 out:send="{{key: 'h1'}}" in:receive="{{key: 'h1'}}">Now I am below the image</h1>
</main>