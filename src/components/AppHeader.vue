<script>
export default {
data () {
    return {
        name: 'AppHeader',
        linkList:[
            {name: 'Characters', active: false},
            {name: 'Comics', active: false},
            {name: 'Movies', active: true},
            {name: 'Tv', active: false},
            {name: 'Games', active: false},
            {name: 'Collectibles', active: false},
            {name: 'Videos', active: false},
            {name: 'Fans', active: false},
            {name: 'News', active: false},
            {name: 'Shop', active: false}
        ]
    }
   },
   methods: {
    addActiveIndex(index) {
        this.linkList.forEach((item, i) => {
            item.active = i === index;
        })
    }
   }
 }
</script>

<template>
<header>
    <div class="nav-container container d-flex justify-content-between align-items-center">
        <div>
            <img id="dc-logo" src="../assets/img/dc-logo.png" alt="dc logo">
        </div>
        
        <nav>
            <ul class="list-unstyled d-flex gap-3">
                <li v-for="(item, index) in linkList" :key="index" :class="{active: item.active}" @click="addActiveIndex(index)" >{{ item.name }}</li>
            </ul>
        </nav>
    </div>
</header>
</template>

<style lang="scss" scoped>
.nav-container {
    height: 100px;

    #dc-logo {
        height: 80px;
    }
}
</style>
