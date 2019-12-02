<script>
  import {send, receive} from './crossfade.js';
</script>


<style>
img{
  display: block;

}
</style>

<main>
  <h1 out:send="{{key: 'h1'}}" in:receive="{{key: 'h1'}}">Look, I'm above the image</h1>
  <img out:send="{{key: 'borat'}}" in:receive="{{key: 'borat'}}" alt='Borat' src='favicon.png'>
</main>
