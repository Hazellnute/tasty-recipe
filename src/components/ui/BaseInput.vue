<template>
    <div>
        <label :for="identity" class="fw-semibold">
            {{label}} <span style="color: #cb3a31">*</span>
            <slot></slot>
        </label>
        <input :class="[{ 'd-none': isImage}, 'form-control' ]" 
        :type="type" :id="identity" :placeholder="placeholder" :value="modelValue"
            :readonly="readonly === '1'" />
    </div>
</template>

<script setup>
defineProps({
    type: { type: String, require: true },
    label: { type: String, require: true },
        identiy: { type: String, require: true },
    placeholder: { type: String, require: false },
    readonly: { type: String, require: true, default: "0" },
    isImage: { type: Boolean, require: true, default: false },
})
</script>