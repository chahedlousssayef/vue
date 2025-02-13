<template>
    <header>
        <h1>
            Shadow's Beauty
        </h1>
        <ul>
            <li>
                <router-link to="/">Home</router-link>
            </li>
            <li>
                <router-link to="/login">Login</router-link>
            </li>
        </ul>
    </header>
    <router-view></router-view>
</template>

<script setup lang="ts"></script>

<style>
    header {
        background-color: pink;
        color: white;
        width: 100%;
        display: flex;
        padding: 0,65rem;
        justify-content:space-evenly;
        align-items: center;
    }
    ul {
        display: flex;
        gap: 1rem;
    }
    li {
        list-style: none;
    }
    a {
        text-decoration: none;
        color: white;
    }
    a:hover {
        text-decoration: underline;
    }
</style>