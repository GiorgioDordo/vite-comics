<script>
export default {
    name: 'AppInfo',
    data () {
        return {
            titleList: [
                {name: 'DC COMICS',
                 list: ["info", "info"],   
                },
                {name: 'SHOP',
                list: ["info", "info"],  
                },
                {name: 'DC',
                list: ["info", "info"],  
                },
                {name: 'SITES',
                list: ["info", "info"],
                },
            ],

        }
    }
}
</script>

<template>
    <section id="info"> 
        <div class="container">
            <div class="column flex-wrap">
                <div v-for="(item, index) in titleList" :key="index" class="col">
                    <h5>{{ item.name }}</h5>
                    <ul class="list-unstyled">
                        <li v-for="(listItem, index) in item.list" :key="index">
                            <a href="">{{ listItem }}</a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
#info {
    color: white;
    background-image: url(../assets/img/footer-bg.jpg);
    height: 500px;
}

</style>
