<template>
    <DocComponent title="Vue Checkbox Component" header="Checkbox" description="Checkbox is an extension to standard checkbox element with theming." :componentDocs="docs" :presetDoc="presetDoc" apiLink="/checkbox/#api" ptLink="/checkbox/#pt" />
</template>

<script>
import AccessibilityDoc from '@/doc/checkbox/AccessibilityDoc.vue';
import BasicDoc from '@/doc/checkbox/BasicDoc.vue';
import DisabledDoc from '@/doc/checkbox/DisabledDoc.vue';
import DynamicDoc from '@/doc/checkbox/DynamicDoc.vue';
import GroupDoc from '@/doc/checkbox/GroupDoc.vue';
import ImportDoc from '@/doc/checkbox/ImportDoc.vue';
import InvalidDoc from '@/doc/checkbox/InvalidDoc.vue';
import PresetDoc from '@/doc/checkbox/preset/index.vue';

export default {
    data() {
        return {
            docs: [
                {
                    id: 'import',
                    label: 'Import',
                    component: ImportDoc
                },
                {
                    id: 'basic',
                    label: 'Basic',
                    component: BasicDoc
                },
                {
                    id: 'group',
                    label: 'Group',
                    component: GroupDoc
                },
                {
                    id: 'dynamic',
                    label: 'Dynamic',
                    component: DynamicDoc
                },
                {
                    id: 'invalid',
                    label: 'Invalid',
                    component: InvalidDoc
                },
                {
                    id: 'disabled',
                    label: 'Disabled',
                    component: DisabledDoc
                },
                {
                    id: 'accessibility',
                    label: 'Accessibility',
                    component: AccessibilityDoc
                }
            ],
            presetDoc: PresetDoc
        };
    }
};
</script>
