---
category: Sensors
---

# onStartTyping

Fires when users start typing on non-editable elements.

## Usage

```html
<input ref="input" type="text" placeholder="Start typing to focus" />
```

```ts {4-7}
<script setup lang="ts">
const input = ref(null)

onStartTyping(() => {
  if (!input.value.active)
    input.value.focus()
})
</script>
```
