<template>
	<div id="search-section-main">
		<div class="filter-location__container">
            <div class="filter-location__typeahead">
                <md-field>
                    <div class="image-a md-button md-icon-button md-theme-dark">
						<i aria-hidden="true" class="md-icon md-theme-dark material-icons">pageview</i>
						<div class="md-ink-ripple">
							<div class="md-ripple" style="width: 40px; height: 40px;"></div>
						</div>
					</div>
                    <label>Buscar trabajos</label>
                    <md-input v-model="type"></md-input>
                </md-field>
            </div>
        </div>
	</div>
</template>

<script>

    import axios from 'axios'
	export default {
		name: 'SearchSectionMain',
		data() {
			return {
				subtitulo: "Subtítulo del componente"
			}
		}, mounted (){
            this.getUser();
        }, 
        methods: {
            getUser(){
                console.log('Pureba');
                axios.get('https://torre.bio/api/bios/stevenandresgutierrezpadilla')
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

</style>