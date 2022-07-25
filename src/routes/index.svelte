<script>
  import { url } from '@roxi/routify'
</script>

<h1>Outer Page</h1>

<a href={$url('../[fooId]', { fooId: 'foobar' })}>Goto Inner Page</a>