<template>
	<div id="search-section-content">
		<div class="SearchSectionSidebar">
			<SearchSectionSidebar></SearchSectionSidebar>
		</div>
		<div class="SearchSectionMain">
			<SearchSectionMain></SearchSectionMain>
		</div>
	</div>
</template>

<script>
	import SearchSectionSidebar from './SearchSectionSidebar.vue'
	import SearchSectionMain from './SearchSectionMain.vue'
    
	export default {
		name: 'SearchSectionContent',
		components: {
			SearchSectionSidebar,
			SearchSectionMain
		},
		data() {
			return {
				subtitulo: "Subtítulo del componente"
			}
		}
	}
</script>

<style scoped>

#search-section-content {
	height: 100%;
}

.SearchSectionSidebar {
	float: left;
	width: 29%;
	background-color: #27292d;
	padding: 25px 0px;
	height: 100%;
	overflow-y: scroll;
}

.SearchSectionMain {
	float: left;
	width: 71%;
	background-color: #000;
	height: 100%;
}

</style>