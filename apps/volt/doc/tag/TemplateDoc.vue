<template>
    <DocSectionText v-bind="$attrs">
        <p>Children of the component are passed as the content for templating.</p>
    </DocSectionText>
    <div class="card flex justify-center">
        <Tag style="border: 2px solid var(--border-color); background: transparent; color: var(--text-color)">
            <div class="flex items-center gap-2 px-1">
                <img alt="Country" src="https://primefaces.org/cdn/primevue/images/flag/flag_placeholder.png" class="flag flag-it" style="width: 18px" />
                <span class="text-base">Italy</span>
            </div>
        </Tag>
    </div>
    <DocSectionCode :code="code" />
</template>

<script setup lang="ts">
import Tag from '@/volt/Tag.vue';
import { ref } from 'vue';

const code = ref(`
<template>
    <div class="card flex justify-center">
        <Tag style="border: 2px solid var(--border-color); background: transparent; color: var(--text-color)">
            <div class="flex items-center gap-2 px-1">
                <img alt="Country" src="https://primefaces.org/cdn/primevue/images/flag/flag_placeholder.png" class="flag flag-it" style="width: 18px" />
                <span class="text-base">Italy</span>
            </div>
        </Tag>
    </div>
</template>

<script setup lang="ts">
import Tag from '@/volt/Tag.vue';
<\/script>
`);
</script>
