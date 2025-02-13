<script setup lang="ts">
import FieldComponent from './FieldComponent.vue';

    function onsubmit(event: Event) {
        event.preventDefault();
        alert('Hello');
    }
</script>

<template>
    <form v-on:submit="onsubmit">
        <fieldset>
            <legend>Login</legend>

            <FieldComponent id="username" label="Username" placeholder="Username" />

            <section class="actions">
                <button id="login">Login</button>
                <button id="reset" type="reset">Reset</button>
            </section>
        </fieldset>
    </form>
</template>

<style scoped>
 section {
        display: flex;
        flex-direction: column;
        gap: 0.5rem;
    }

    form {
        font-family: monospace;
    }
    fieldset {
        width: 280px;
        padding: 30px;
        background: rgba(255, 255, 255, 0.85);
        border-radius: 10px;
        box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.2);
        position: absolute;
        top: 20%;
        left: 50%;
        transform: translate(-50%, -20%);
        text-align: center;
    }

    .actions {
        flex-direction: row;
        gap: 1rem;
    }

    #login {
        flex: 1 1 auto;
    }

    #reset {
        flex: 0 1 auto;
}
</style>