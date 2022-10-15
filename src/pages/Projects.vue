<template>
    <div>
        <Navbar />
        <section class="projects">
            <h1 class="heading"> <span>It's</span> Anime </h1>
            <h3>{{project_name}}</h3>
            <p>{{project_detail}}</p>
            <div class="box-container">
                <iframe width="1140" height="641" src="https://www.youtube.com/embed/LvWK-3sROdM?list=PLIa05JMgYhhacplnc2ZE7eSnNcmWcCfW5" title="เกิดใหม่ทั้งทีก็เป็นสไลม์ไปซะแล้ว - ตอนที่ 01 [ซับไทย]" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
            </div>
        </section>
    </div>
</template>

<script>
import Navbar from '../components/Navbar.vue';
export default {
    components: { Navbar },
    data() {
         return {
            project_name: 'Tensei Shitara Slime Datta Ken',
            project_detail: 'เกิดใหม่ทั้งที ก็เป็นสไลม์ไปซะแล้ว',
         } 
}
}
</script>

<style>

</style>