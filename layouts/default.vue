<template>
    <div>
        <nav class=" bg-grey text-black text-l flex gap-10 shadow-lg p-3 pl-6  mb-0 justify-start">
            <NuxtLink to="/">Letter</NuxtLink>
            <NuxtLink to="/form">Form</NuxtLink>
            <NuxtLink to="/testing">Testing</NuxtLink>
        </nav>
        <slot></slot>
    </div>
</template>