<template>
    <DocComponent title="Vue IconFiled" header="IconFiled" description="IconField wraps an input and an icon." :componentDocs="docs" :apiDocs="['IconField', 'InputIcon']" :themingDocs="themingDoc" />
</template>

<script>
import AccessibilityDoc from '@/doc/iconfield/AccessibilityDoc.vue';
import BasicDoc from '@/doc/iconfield/BasicDoc.vue';
import ImportDoc from '@/doc/iconfield/ImportDoc.vue';
import ThemingDoc from '@/doc/iconfield/theming/index.vue';

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
                    id: 'accessibility',
                    label: 'Accessibility',
                    component: AccessibilityDoc
                }
            ],
            themingDoc: ThemingDoc
        };
    }
};
</script>
