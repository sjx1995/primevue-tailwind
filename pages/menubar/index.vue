<template>
    <DocComponent title="Vue Navbar Component" header="Menubar" description="Menubar also known as Navbar, is a horizontal menu component." :componentDocs="docs" :presetDoc="presetDoc" apiLink="/menubar/#api" ptLink="/menubar/#pt" />
</template>

<script>
import AccessibilityDoc from '@/doc/menubar/AccessibilityDoc.vue';
import BasicDoc from '@/doc/menubar/BasicDoc.vue';
import CommandDoc from '@/doc/menubar/CommandDoc.vue';
import ImportDoc from '@/doc/menubar/ImportDoc.vue';
import RouterDoc from '@/doc/menubar/RouterDoc.vue';
import TemplateDoc from '@/doc/menubar/TemplateDoc.vue';
import PresetDoc from '@/doc/menubar/preset/index.vue';
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
