<template>
    <div id="basicLayout">
        <a-layout style="min-height: 100vh;">
            <a-layout-header class="header">
                <GlobalHeader />
            </a-layout-header>
            <a-layout-content class="content">
                <router-view></router-view>
            </a-layout-content>
            <a-layout-footer class="footer">
                <a href="https://newerproduct.github.io/" target="_blank">小李の学习博客</a>
            </a-layout-footer>
        </a-layout>
    </div>
</template>

<script setup>
import { RouterView } from 'vue-router';
import GlobalHeader from '@/components/GlobalHeader.vue'

</script>

<style scoped>
#basicLayout {

}
#basicLayout .footer {
    background-color: #efefef;
    padding: 16px;
    position: fixed;
    bottom: 0;
    left: 0;
    right: 0;
    text-align: center;
}
#basicLayout .content {
    background: linear-gradient(to right, #fefefe,#fff);
    margin-bottom: 28px;
    padding: 20px;
}
#basicLayout .header {
    padding-inline: 20px;
    margin-bottom: 16px;
    color:unset;
    background-color: white;
}
</style>