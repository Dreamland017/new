<template>
    <div>
        <Navbar />
        <section class="home">
            <div class="image">
                <img src="images/profile.png" alt="">
            </div>
            <div class="content">
                <h3>{{name}}</h3>
                <span>{{motto}}</span>
                <p>{{content}}</p>
                <router-link to="/about" class="btn"> about me <i class="fas fa-user"></i> </router-link>
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
            name: 'Tensei Shitara Slime Datta Ken',
            motto: 'เกิดใหม่ทั้งทีก็เป็นสไลม์ไปซะแล้ว',
            content: 'ชีวิตที่น่าเบื่อของมิคามิต้องจบลงอย่างกะทันหันเมื่อจู่ๆ เขาก็กลับชาติมาเกิดเป็นสัตว์ประหลาดเหนียวหนืด หลังจากนั้นก็จัดตั้งกลุ่มสัตว์ประหลาดและเปลี่ยนแปลงทุกสิ่งทุกอย่าง',
         } 
}
}
</script>

<style>

</style>