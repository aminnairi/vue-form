<template>
    <div class="flex flex-col items-center">
        <app-logo width="48" height="48" />
        <h1 class="text-center"><span class="uppercase font-thin">job</span><span class="uppercase font-bold">finder</span></h1>

        <app-form :values="values" class="flex flex-col items-center mt-3">
            <app-form-field name="email">
                <app-form-label>Email ({{ values.email }})</app-form-label>
                <app-form-input />
            </app-form-field>

            <app-form-field name="password">
                <app-form-label>Password ({{ values.password }})</app-form-label>
                <app-form-input type="password" />
            </app-form-field>

            <app-form-button>Login</app-form-button>
        </app-form>
    </div>
</template>

<script>
import AppLogo from "./components/AppLogo.vue";
import AppForm from "./components/AppForm.vue";
import AppFormInput from "./components/AppFormInput.vue";
import AppFormLabel from "./components/AppFormLabel.vue";
import AppFormField from "./components/AppFormField.vue";
import AppFormButton from "./components/AppFormButton.vue";

export default {
    components: {
        AppLogo,
        AppForm,
        AppFormInput,
        AppFormLabel,
        AppFormField,
        AppFormButton
    },

    data() {
        return {
            values: {
                email: "nairi.amin@gmail.com",
                password: "abcABC123!@#"
            }
        };
    }
}
</script>
