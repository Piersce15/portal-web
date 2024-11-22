<script setup>
import AuthenticatedLayout from '@/Layouts/Authenticated.vue'
import Button from '@/Components/Button.vue'
import { PlusIcon } from '@/Components/Icons/outline'
</script>
<template>
    <Head title="Usuarios" />
    <AuthenticatedLayout title="Usuarios">
        <template #header>
            <div class="flex flex-col gap-4 md:flex-row md:items-center md:justify-between">
                <h2 class="text-xl font-semibold leading-tight">
                    Usuarios
                </h2>
                <Button
                    external
                    variant="new"
                    target="_blank"
                    class="items-center gap-2 max-w-xs"
                    v-slot="{ iconSizeClasses }"
                    href=""
                >
                    <PlusIcon aria-hidden="true" :class="iconSizeClasses" />

                    <span>Agregar nuevo</span>
                </Button>
            </div>
            
        </template>
        
        <div class="p-6 overflow-hidden bg-white rounded-md shadow-md dark:bg-dark-eval-1">
            Listado
        </div>
    </AuthenticatedLayout>
</template>