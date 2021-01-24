<template>
	<div id="search-section-main">
        <div class="data-c" v-for="(item) in data" :key="item.id">
            <h2>{{ item.name }}</h2>
            <span class="inten">{{ item.inten }}</span>
            <br>
            <span class="comp">{{ item.comp }}</span>
            <br>
            <span class="place">{{ item.place }}</span>
        </div>
	</div>
</template>

<script>

    import axios from 'axios'
	export default {
		name: 'SearchSectionMain',
		data() {
			return {
                subtitulo: "Subtítulo del componente",
                latitude: 0,
                longitude: 0,
                data: [
                    {
                        name: 'name1',
                        inten: 'inten1',
                        comp: 'comp1',
                        place: 'place1'
                    },
                    {
                        name: 'name2',
                        inten: 'inten2',
                        comp: 'comp2',
                        place: 'place2'
                    },
                    {
                        name: 'name2',
                        inten: 'inten2',
                        comp: 'comp2',
                        place: 'place2'
                    },
                    {
                        name: 'name2',
                        inten: 'inten2',
                        comp: 'comp2',
                        place: 'place2'
                    }
                ]
			}
		}, mounted (){
            this.getUser();
        }, 
        methods: {
            getUser(){
                axios.get('/api/auth-fetch/auth-fetch?search=stevenandresgutierrezpadilla')
                .then(Response => {
                    console.log(Response)
                    this.latitude = Response.data.msg.person.location.latitude;
                    this.longitude = Response.data.msg.person.location.longitude;
                    console.log(this.latitude);
                    console.log(this.longitude);
                    this.getJobs();
                })
                .catch( e => console.log(e))
            },
            getJobs(){
                axios.get('/api/auth-fetch2/auth-fetch2?search=stevenandresgutierrezpadilla')
                .then(Response => {
                    console.log(Response)
                    var id;
                    var results = Response.data.msg.results;
                    results.forEach(element => {
                        id = element.id
                        this.getJob(id);
                    });
                })
                .catch( e => console.log(e))
            },
            getJob(id){
                axios.get('/api/auth-fetch2/auth-fetch3?search='+id)
                .then(Response => {
                    console.log(Response)
                })
                .catch( e => console.log(e))
            }
        }
	}
</script>

<style scoped>

.md-field label{
    color: rgb(172, 177, 181);
    background-color: black;
    padding: 0 2px;
    top: 29px;
    left: 60px;
}

.md-field .md-input{
    color: white;
    border: 1px solid rgb(143, 143, 146) !important;
    max-width: 510px;
    border-radius: 30px;
    height: 45px;
}

.md-field.md-focused label{
    color: rgb(178, 191, 55);
    top: 5px;
    left: 23px;
}

.md-field.md-focused .md-input{
    border: 2px solid rgb(178, 191, 55) !important;
}

.md-field.md-focused .image-a i{
    color: rgb(178, 191, 55) !important;
    transition: none;
}

.filter-location__container {
    margin-left: auto;
}

.image-a {
    position: absolute;
    top: 20px;
    left: 6px;
}

.image-a i{
    color:rgb(143, 143, 146);
    font-size: 31px;
}

.data-c {
    width: 300px;
    height: 150px;
    background-color: #27292d;
    text-align: justify;
    padding: 10px;
    margin: 50px;
    float: left;
    padding-left: 40px;
}

.data-c h2{
    color: #b2bf37;
}

.data-c span {
    color: rgba(255, 255, 255, 0.65);
}


</style>