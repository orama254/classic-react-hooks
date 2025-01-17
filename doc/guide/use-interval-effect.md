---
outline: deep
---
# useIntervalEffect

- A hooks that runs the provided callback only once after the timer is completed.


## Example


<div ref="el" />

<script setup>
import { createElement } from 'react'
import { createRoot } from 'react-dom/client'
import { ref, onMounted } from 'vue'
import Example from '../../src/hooks/use-interval-effect/example'
import useIntervalEffect from '../../src/hooks/use-interval-effect/use-interval-effect'

const el = ref()
onMounted(() => {
   const root = createRoot(el.value)
   root.render(createElement(Example, {}, null))
})
</script>

## Code Snippets

::: details Example.tsx
<<< @/../src/hooks/use-interval-effect/example.tsx{2,6,17,18,13}
:::

::: details useIntervalEffect.tsx
<<< @/../src/hooks/use-interval-effect/use-interval-effect.tsx
:::
