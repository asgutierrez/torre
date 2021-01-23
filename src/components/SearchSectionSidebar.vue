<template>
	<div id="search-section-sidebar">
		<h2 class="md-title">Filtrar trabajos por</h2>
        <div class="search-filters__section">
            <div class="collapsible-filter-list">
                <h3 class="search-filters__title md-subheading-1">Para ti</h3>
                <div class="md-subheading-1 collapsible-filter-list__item">
                <a href="/es/search/jobs?q=dreamjobs%3Astevenandresgutierrezpadilla" class="router-link-active">Tus trabajos soñados (4k+)</a>
                </div>
                <div class="collapsible-filter-list__expand"></div>
            </div>
            <div class="collapsible-filter-list">
                <h3 class="search-filters__title md-subheading-1">Estado</h3>
                <div class="md-subheading-1 collapsible-filter-list__item">
                <a href="/es/search/jobs?q=status%3Aclosed" class="router-link-active">Cerrado (56k+)</a>
                </div>
                <div class="md-subheading-1 collapsible-filter-list__item">
                <a href="/es/search/jobs?q=status%3Aopen" class="router-link-active">Abierto (742+)</a>
                </div>
                <div class="collapsible-filter-list__expand"></div>
            </div>
            <div class="filter-opportunity-type">
                <h3 class="search-filters__title md-subheading-1">Tipo de trabajo</h3>
                <div class="md-subheading-1 filter-opportunity-type__option">
                <a href="/es/search/jobs?q=type%3Afull-time-employment" class="md-primary router-link-active">Empleo a tiempo completo (48k+)</a>
                </div>
                <div class="md-subheading-1 filter-opportunity-type__option">
                <a href="/es/search/jobs?q=type%3Apart-time-employment" class="md-primary router-link-active">Empleo a medio tiempo (3k+)</a>
                </div>
                <div class="md-subheading-1 filter-opportunity-type__option">
                <a href="/es/search/jobs?q=type%3Afreelance-gigs" class="md-primary router-link-active">Trabajos temporales/freelance (4k+)</a>
                </div>
                <div class="md-subheading-1 filter-opportunity-type__option">
                <a href="/es/search/jobs?q=type%3Ainternships" class="md-primary router-link-active">Pasantías (1k+)</a>
                </div>
            </div>
            <div class="filter-location">
                <h3 class="search-filters__title md-subheading-1">Ubicación(es)</h3>
                <div >
                    <a href="/es/search/jobs?q=remote%3Ayes" class="md-subheading-1 router-link-active">Remoto (38k+)</a>
                </div>
                <div class="filter-location__container">
                    <div class="filter-location__typeahead">
                        <md-field>
                            <label>Ubicación(es) específica(s)</label>
                            <md-input v-model="type"></md-input>
                        </md-field>
                    </div>
                </div>
            </div>
            <div class="collapsible-filter-list">
                <h3 class="search-filters__title md-subheading-1">Habilidades destacadas</h3>
                <div class="md-subheading-1 collapsible-filter-list__item">
                <a href="/es/search/jobs?q=skill%3ASoftware%20Development" class="router-link-active">Software Development (5k+)</a>
                </div>
                <div class="md-subheading-1 collapsible-filter-list__item">
                <a href="/es/search/jobs?q=skill%3ACommunication" class="router-link-active">Communication (3k+)</a>
                </div>
                <div class="md-subheading-1 collapsible-filter-list__item">
                <a href="/es/search/jobs?q=skill%3ASales" class="router-link-active">Sales (3k+)</a>
                </div>
                <div class="md-subheading-1 collapsible-filter-list__item">
                <a href="/es/search/jobs?q=skill%3AMarketing" class="router-link-active">Marketing (3k+)</a>
                </div>
                <div class="md-subheading-1 collapsible-filter-list__item">
                <a href="/es/search/jobs?q=skill%3AManagement" class="router-link-active">Management (2k+)</a>
                </div>
                <div class="collapsible-filter-list__expand">
                <button type="button" class="md-button md-primary md-theme-dark">Ver más
                    <div class="md-ink-ripple">
                    <div class="md-ripple" style="width: 94px; height: 94px;"></div>
                    </div>
                </button>
                </div>
            </div>
            <div class="collapsible-filter-list">
                <h3 class="search-filters__title md-subheading-1">Organización(es)</h3>
                <div class="md-subheading-1 collapsible-filter-list__item">
                <a href="/es/search/jobs?q=organization%3ACollage.com" class="router-link-active">Collage.com (354+)</a>
                </div>
                <div class="md-subheading-1 collapsible-filter-list__item">
                <a href="/es/search/jobs?q=organization%3AStripe" class="router-link-active">Stripe (314+)</a>
                </div>
                <div class="md-subheading-1 collapsible-filter-list__item">
                <a href="/es/search/jobs?q=organization%3ARobert%20Half" class="router-link-active">Robert Half (282+)</a>
                </div>
                <div class="md-subheading-1 collapsible-filter-list__item">
                <a href="/es/search/jobs?q=organization%3ABairesDev" class="router-link-active">BairesDev (255+)</a>
                </div>
                <div class="md-subheading-1 collapsible-filter-list__item">
                <a href="/es/search/jobs?q=organization%3AInVisionApp" class="router-link-active">InVisionApp (254+)</a>
                </div>
                <div class="md-subheading-1 collapsible-filter-list__item">
                <a href="/es/search/jobs?q=organization%3ABlizzard%20Entertainment" class="router-link-active">Blizzard Entertainment (201+)</a>
                </div>
                <div class="collapsible-filter-list__expand">
                <button type="button" class="md-button md-primary md-theme-dark">Ver más
                    <div class="md-ink-ripple">
                    <div class="md-ripple" style="width: 94px; height: 94px;"></div>
                    </div>
                </button>
                </div>
            </div>
            </div>
	</div>
</template>

<script>
	export default {
		name: 'SearchSectionSidebar',
		data() {
			return {
				subtitulo: "Subtítulo del componente"
			}
		}
	}
</script>

<style scoped>

.md-title {
    background: rgba(255, 255, 255, 0.06);
    margin: 0px;
    padding: 12px 16px;
    color: rgba(255, 255, 255, 0.90);
    text-align: left;
}

.search-filters__title.md-subheading-1 {
    color: white;
}

.search-filters__section {
    text-align: left;
}

.search-filters__section .md-subheading-1{
    margin-left: 16px;
}

.router-link-active {
    color: rgb(178, 191, 55);
}

.md-subheading-1 {
    font-size: 16px;
    font-weight: 400;
}

.collapsible-filter-list__item:not(:last-child), .filter-opportunity-type__option:not(:last-child) {
    padding-bottom: 8px;
}

.search-filters__section > .collapsible-filter-list, .search-filters__section > .filter-opportunity-type {
    margin-bottom: 36px;
}

.collapsible-filter-list__expand button {
    color: rgb(178, 191, 55);
    margin-left: 0;
}

.md-field label{
    color: rgb(172, 177, 181);
    background-color: #27292d;
    padding: 0 2px;
    top: 29px;
    left: 13px;
}

.md-field .md-input{
    color: white;
    border: 1px solid rgb(143, 143, 146) !important;
    max-width: 300px;
    border-radius: 3px;
    height: 45px;
}

.md-field.md-focused label{
    color: rgb(178, 191, 55);
    top: 5px;
}

.md-field.md-focused .md-input{
    border: 2px solid rgb(178, 191, 55) !important;
}

.filter-location__container {
    margin-left: 16px;
}

</style>