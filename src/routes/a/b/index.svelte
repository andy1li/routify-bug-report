<script >
  import { url, isActive } from '@roxi/routify'
</script>

<ol>
  <li>
    <a href={$url('/')}>
      / is active (non-recursive): {$isActive('/', {}, {recursive: false})}
    </a>
  </li>
  <li>
    <a href={$url('/a')}>
      /a is active (non-recursive): {$isActive('/a', {}, {recursive: false})}
    </a>
  </li>
  <li>
    <a href={$url('/a')}>
      /a is active: {$isActive('/a')}
    </a>
  </li>
  <li>
    <a href={$url('/a/b')}>
      /a/b is active (non-recursive): {$isActive('/a/b', {}, {recursive: false})}
    </a>
  </li>
  <li>
    <a href={$url('/a/b')}>
      /a/b is active: {$isActive('/a/b')}
    </a>
  </li>
</ol>