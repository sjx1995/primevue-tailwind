<template>
    <DocComponent title="Vue Menu Component" header="Menu" description="Menu displays a list of items in vertical orientation." :componentDocs="docs" :presetDoc="presetDoc" apiLink="/menu/#api" ptLink="/menu/#pt" />
</template>

<script>
import AccessibilityDoc from '@/doc/menu/AccessibilityDoc.vue';
import BasicDoc from '@/doc/menu/BasicDoc.vue';
import CommandDoc from '@/doc/menu/CommandDoc.vue';
import GroupDoc from '@/doc/menu/GroupDoc.vue';
import ImportDoc from '@/doc/menu/ImportDoc.vue';
import PopupDoc from '@/doc/menu/PopupDoc.vue';
import RouterDoc from '@/doc/menu/RouterDoc.vue';
import TemplateDoc from '@/doc/menu/TemplateDoc.vue';
import PresetDoc from '@/doc/menu/preset/index.vue';

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
                    id: 'popup',
                    label: 'Popup',
                    component: PopupDoc
                },
                {
                    id: 'template',
                    label: 'Template',
                    component: TemplateDoc
                },
                {
                    id: 'command',
                    label: 'Command',
                    component: CommandDoc
                },
                {
                    id: 'router',
                    label: 'Router',
                    component: RouterDoc
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
