<template>
    <DocSectionText v-bind="$attrs">
        <p>When <i>editable</i> is present, the input can also be entered with typing.</p>
    </DocSectionText>
    <div class="card flex justify-center">
        <Dropdown v-model="selectedCity" editable :options="cities" optionLabel="name" placeholder="Select a City" class="w-full md:w-14rem" />
    </div>
    <DocSectionCode :code="code" />
</template>

<script>
export default {
    data() {
        return {
            selectedCity: null,
            cities: [
                { name: 'New York', code: 'NY' },
                { name: 'Rome', code: 'RM' },
                { name: 'London', code: 'LDN' },
                { name: 'Istanbul', code: 'IST' },
                { name: 'Paris', code: 'PRS' }
            ],
            code: {
                basic: `
<Dropdown v-model="selectedCity" editable :options="cities" optionLabel="name" placeholder="Select a City" class="w-full md:w-14rem" />
`,
                options: `
<template>
    <div class="card flex justify-center">
        <Dropdown v-model="selectedCity" editable :options="cities" optionLabel="name" placeholder="Select a City" class="w-full md:w-14rem" />
    </div>
</template>

<script>
export default {
    data() {
        return {
            selectedCity: null,
            cities: [
                { name: 'New York', code: 'NY' },
                { name: 'Rome', code: 'RM' },
                { name: 'London', code: 'LDN' },
                { name: 'Istanbul', code: 'IST' },
                { name: 'Paris', code: 'PRS' }
            ]
        };
    }
};
<\/script>
`,
                composition: `
<template>
    <div class="card flex justify-center">
        <Dropdown v-model="selectedCity" editable :options="cities" optionLabel="name" placeholder="Select a City" class="w-full md:w-14rem" />
    </div>
</template>

<script setup>
import { ref } from "vue";

const selectedCity = ref();
const cities = ref([
    { name: 'New York', code: 'NY' },
    { name: 'Rome', code: 'RM' },
    { name: 'London', code: 'LDN' },
    { name: 'Istanbul', code: 'IST' },
    { name: 'Paris', code: 'PRS' }
]);
<\/script>
`
            }
        };
    }
};
</script>
