<template>
    <div>
        <Navbar />

        <section class="about">

            <h1 class="heading"> about <span>me</span> </h1>

            <div class="row">

                <div class="info-container">

                    <h1>personal info</h1>

                    <div class="box-container">

                        <div class="box">
                            <h3> <span>name : </span> {{name}} </h3>
                            <h3> <span>age : </span> {{age}} </h3>
                            <h3> <span>status : </span> {{status}} </h3>
                        </div>

                        <div class="box">
                            <h3> <span>newname : </span> {{newname}} </h3>
                            <h3> <span>ร่างใหม่ : </span> {{ร่างใหม่}} </h3>
                        </div>

                    </div>

                </div>

                <div class="count-container">

                    <div class="box" v-for="e in Freetime" :key="e.hobby" >
                        <h3>{{e.hobby}}</h3>
                        <p>{{e.ex}}</p>
                    </div>

                    <div class="box" v-for="e in Attention" :key="e.one">
                        <h3>{{e.one}}</h3>
                        <p>{{e.two}}</p>
                    </div>
                </div>

            </div>

        </section>

        <!-- about section ends -->

        <!-- skills section starts  -->

        <section class="skills">

            <h1 class="heading"> <span>my</span> character </h1>

            <div class="box-container">
                <div class="box">
                    <img src="images/icon-5.png">
                    <h3>slime</h3>
                </div>
                <div class="box">
                    <img src="images/icon-6.png">
                    <h3>ริมุรุ</h3>
                </div>
            </div>

        </section>
    </div>
</template>

<script>
import Navbar from "../components/Navbar.vue";
export default {
    components: { Navbar },
    data() {
        return {
            name: 'มิคามิ ซาโตรุ',
            age: '37',
            status:'หนุ่มโสด ไม่เคยมีแฟน',
            newname:'ริมุรุ เทนเปสึโตะ',
            ร่างใหม่: 'slime',
        Freetime: [{
            hobby:'98%',
            ex:' Unique Skill Predator',
        },{
            hobby:'99%',
            ex:'level',
        }]
    }
}
}
</script>

<style>

</style>