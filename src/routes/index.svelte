<script lang="ts">
  import { url } from '@roxi/routify'
  
</script>

<ul>
  <li><a href={$url('/search-params-only', {foo: 'bar'})}>Search Params Only</a></li>
  <li><a href={$url('/fruits/[fruitId]', {fruitId: '123', foo: 'bar'})}>Normal Params</a></li>

</ul>