<template>
	<div id="app-bar-wrapper">
		<div class="wrap">
			<button type="button" class="menu md-button md-icon-button md-theme-dark">
				<i aria-hidden="true" class="md-icon md-theme-dark material-icons">menu</i>
				<div class="md-ink-ripple">
					<div class="md-ripple" style="width: 40px; height: 40px;"></div>
				</div>
			</button>
			<div class="tdl-brand-logo md-theme-dark svg-container">
				<svg viewBox="0 0 113 33" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" class="logo-svg">
					<g id="Page-1" stroke="none" stroke-width="1">
						<path d="M10.9635,32.423 C13.1255,32.423 14.6765,31.953 16.0865,31.154 L16.0865,26.501 C14.9585,27.065 13.8305,27.347 12.5615,27.347 C10.6345,27.347 9.5065,26.454 9.5065,24.245 L9.5065,12.072 L16.1805,12.072 L16.1805,7.184 L9.5065,7.184 L9.5065,0.369 L3.8195,0.369 L3.8195,7.184 L0.6705,7.184 L0.6705,12.072 L3.8195,12.072 L3.8195,25.138 C3.8195,30.59 6.7805,32.423 10.9635,32.423 Z M33.0535,32.564 C40.6050571,32.564 46.1929447,26.8556582 46.3510575,19.9404098 L46.3545,19.545 C46.3545,12.448 40.7615,6.667 33.1475,6.667 C25.6422714,6.667 20.0550457,12.3753418 19.8969424,19.3356046 L19.8935,19.733 C19.8935,26.783 25.4865,32.564 33.0535,32.564 Z M33.1475,27.582 C28.8144615,27.582 25.7020847,24.1008539 25.5839803,19.8876586 L25.5805,19.545 C25.5805,15.221 28.4945,11.649 33.0535,11.649 C37.4326346,11.649 40.5458979,15.1301461 40.6640193,19.3876816 L40.6675,19.733 C40.6675,24.01 37.7535,27.582 33.1475,27.582 Z M52.0885,32 L57.8225,32 L57.8225,22.553 C57.8225,15.973 61.3005,12.73 66.2825,12.73 L66.6115,12.73 L66.6115,6.714 C62.2405,6.526 59.3735,9.064 57.8225,12.777 L57.8225,7.184 L52.0885,7.184 L52.0885,32 Z M71.4995,32 L77.2335,32 L77.2335,22.553 C77.2335,15.973 80.7115,12.73 85.6935,12.73 L86.0225,12.73 L86.0225,6.714 C81.6515,6.526 78.7845,9.064 77.2335,12.777 L77.2335,7.184 L71.4995,7.184 L71.4995,32 Z M101.4855,32.564 C106.0445,32.564 109.2875,30.731 111.6375,27.911 L108.3005,24.95 C106.3265,26.877 104.3525,27.911 101.5795,27.911 C97.9135,27.911 95.0465,25.655 94.4355,21.613 L112.6715,21.613 C112.7185,21.049 112.7655,20.532 112.7655,20.015 C112.7655,12.871 108.7705,6.667 100.8745,6.667 C93.8818676,6.667 88.896859,12.3248486 88.7517533,19.2797349 L88.7485,19.686 C88.7485,27.347 94.2945,32.564 101.4855,32.564 Z M94.3885,17.853 C94.9055,13.999 97.3495,11.32 100.8275,11.32 C104.5875,11.32 106.7495,14.187 107.1255,17.853 L94.3885,17.853 Z"></path>
					</g>
				</svg>
			</div>
			<div class="md-menu tdl-app-bar__user-menu user-menu">
				<div class="user-menu__picture entity-picture entity-picture--is-hexagon entity-picture--has-shadow" md-menu-trigger="" style="--size:38px; --font-size:16.625px; --border-width:2px; --box-shadow:0px 2px 4px rgba(0,0,0,0.5);"><div class="hexagon-border hexagon-border--no-margins"></div> <img data-url="https://starrgate.s3.amazonaws.com:443/CACHE/images/users/0559cbb5a64e672cca9c0a2783472a796bfa948e/profile_rScvYr7/6f7a35588c06b9a1bfbae963f39a643b.jpg" alt="Steven Andres Gutierrez Padilla" class="entity-picture__thumbnail entity-picture__thumbnail--image entity-picture__thumbnail--no-margins" src="https://starrgate.s3.amazonaws.com:443/CACHE/images/users/0559cbb5a64e672cca9c0a2783472a796bfa948e/profile_rScvYr7/6f7a35588c06b9a1bfbae963f39a643b.jpg"></div>  
			</div>
			<div class="topnav">
				<a href="#mensajes" class="image-text-a">
					<div class="image-a md-button md-icon-button md-theme-dark">
						<i aria-hidden="true" class="md-icon md-theme-dark material-icons">question_answer</i>
						<div class="md-ink-ripple">
							<div class="md-ripple" style="width: 40px; height: 40px;"></div>
						</div>
					</div>
					<div class="text-a">Mensajes</div>
				</a>
				<a href="#signals" class="image-text-a">
					<div class="image-a md-button md-icon-button md-theme-dark">
						<i aria-hidden="true" class="md-icon md-theme-dark material-icons">emoji_people</i>
						<div class="md-ink-ripple">
							<div class="md-ripple" style="width: 40px; height: 40px;"></div>
						</div>
					</div>
					<div class="text-a">Signals</div>
				</a>
				<a href="#genoma" class="image-text-a">
					<div class="image-a md-button md-icon-button md-theme-dark">
						<i aria-hidden="true" class="md-icon md-theme-dark material-icons">person</i>
						<div class="md-ink-ripple">
							<div class="md-ripple" style="width: 40px; height: 40px;"></div>
						</div>
					</div>
					<div class="text-a">Tu genoma</div>
				</a>
				<a href="#alertas" class="image-text-a">
					<div class="image-a md-button md-icon-button md-theme-dark">
						<i aria-hidden="true" class="md-icon md-theme-dark material-icons">notifications</i>
						<div class="md-ink-ripple">
							<div class="md-ripple" style="width: 40px; height: 40px;"></div>
						</div>
					</div>
					<div class="text-a">Alertas</div>
				</a>
				<a href="#publicaciones" class="image-text-a">
					<div class="image-a md-button md-icon-button md-theme-dark">
						<i aria-hidden="true" class="md-icon md-theme-dark material-icons">work</i>
						<div class="md-ink-ripple">
							<div class="md-ripple" style="width: 40px; height: 40px;"></div>
						</div>
					</div>
					<div class="text-a">Publicaciones</div>
				</a>
				<a href="#publicarTrabajo" class="image-text-a">
					<div class="image-a md-button md-icon-button md-theme-dark">
						<i aria-hidden="true" class="md-icon md-theme-dark material-icons">campaign</i>
						<div class="md-ink-ripple">
							<div class="md-ripple" style="width: 40px; height: 40px;"></div>
						</div>
					</div>
					<div class="text-a">Publicar trabajo</div>
				</a>
				<a href="#trabajos" class="image-text-a">
					<div class="image-a md-button md-icon-button md-theme-dark">
						<i aria-hidden="true" class="md-icon md-theme-dark material-icons">pageview</i>
						<div class="md-ink-ripple">
							<div class="md-ripple" style="width: 40px; height: 40px;"></div>
						</div>
					</div>
					<div class="text-a">Trabajos</div>
				</a>
				<a href="#buscar" class="image-text-a">
					<div class="image-a md-button md-icon-button md-theme-dark">
						<i aria-hidden="true" class="md-icon md-theme-dark material-icons">search</i>
						<div class="md-ink-ripple">
							<div class="md-ripple" style="width: 40px; height: 40px;"></div>
						</div>
					</div>
					<div class="text-a">Buscar</div>
				</a>
			</div>
		</div>
		<div class="md-toolbar-container md-toolbar-container--title-bar"><h2 class="md-title">Buscar</h2></div>
		<div class="wrap mid">
			<div class="midnav">
				<a href="#mensajes" class="active">
					<div class="nav-text-a">EMPLEOS</div>
				</a>
				<a href="#signals">
					<div class="nav-text-a">PERSONAS</div>
				</a>
			</div>
		</div>
	</div>
</template>

<script>
	export default {
		name: 'AppBarWrapper',
		data() {
			return {
				subtitulo: "Subtítulo del componente"
			}
		}
	}
</script>

<style scoped>

#app-bar-wrapper {
	height: 100%;
	width: 100%;
	position: absolute;
}

#app-bar-wrapper .wrap.mid{
	background-color: #27292d;
	height: 35%;
	padding-left: 29%;
	box-shadow: 0px 1px 1px rgba(0, 0, 0, 0.678);
	position: absolute;
	top: 65%;
	width: 100%;
	z-index: 1;
}

#app-bar-wrapper .wrap{
	background-color: #27292d;
	height: 35%;
	width: 100%;
}

#app-bar-wrapper .md-toolbar-container--title-bar{
	background-color: #27292d;
	height: 30%;
	border-width: 1px;
	border-bottom: 0;
	border-left: 0;
	border-right: 0;
	border-style: groove;
	border-top: 1px solid rgba(255, 255, 255, 0.12);
	width: 100%;
	padding: 12px 15px;
	top: 35%;
	position: absolute;
}

#app-bar-wrapper .md-toolbar-container--title-bar .md-title{
	margin: 0;
	width: fit-content;
	color: rgba(255, 255, 255, 0.90);
}

.menu {
	float: left;
	top: 8px;
}

.menu i{
	color: #a0a0a3;
	position: absolute;
	top: 50%;
	left: 50%;
	transform: translate(-50%,-50%);
}

.svg-container {
	width: fit-content;
	float: left;
	position: relative;
	top: 14px;
	left: 23px;
}

.svg-container svg {
	width: 63px;
	height: 27px;
	fill: #F3F3F3;
}

.image-a {
	position: relative;
	top: 0px;
}

.image-a i{
	color: #a0a0a3;
	position: absolute;
	top: 50%;
	left: 50%;
	transform: translate(-50%,-50%);
}

.text-a {
	position: relative;
	top: -8px;
	font-weight: 550;
	font-size: 10px;
	color: #a0a0a3;
}

.nav-text-a {
	position: relative;
	top: 18px;
	font-weight: 600;
	font-size: 13px;
	color: #a0a0a3;
}

.topnav {
  overflow: hidden;
  background-color: #27292d;
  float: right;
  height: 100%;
}

.topnav a {
  float: left;
  color: #f2f2f2;
  text-align: center;
  padding: 2px 10px;
  text-decoration: none;
  font-size: 17px;
  float: right;
}

.topnav a:hover {
  background-color: rgb(25, 37, 40);
  color: black;
}

.topnav a.active {
  background-color: #4CAF50;
  color: white;
}

.entity-picture--is-hexagon .entity-picture__thumbnail {
    -webkit-clip-path: polygon(45% 1.33975%,46.5798% .60307%,48.26352% .15192%,50% 0,51.73648% .15192%,53.4202% .60307%,55% 1.33975%,89.64102% 21.33975%,91.06889% 22.33956%,92.30146% 23.57212%,93.30127% 25%,94.03794% 26.5798%,94.48909% 28.26352%,94.64102% 30%,94.64102% 70%,94.48909% 71.73648%,94.03794% 73.4202%,93.30127% 75%,92.30146% 76.42788%,91.06889% 77.66044%,89.64102% 78.66025%,55% 98.66025%,53.4202% 99.39693%,51.73648% 99.84808%,50% 100%,48.26352% 99.84808%,46.5798% 99.39693%,45% 98.66025%,10.35898% 78.66025%,8.93111% 77.66044%,7.69854% 76.42788%,6.69873% 75%,5.96206% 73.4202%,5.51091% 71.73648%,5.35898% 70%,5.35898% 30%,5.51091% 28.26352%,5.96206% 26.5798%,6.69873% 25%,7.69854% 23.57212%,8.93111% 22.33956%,10.35898% 21.33975%);
    -webkit-transform: translateY(var(--border-width));
    border: unset;
    border-radius: 0;
    clip-path: polygon(45% 1.33975%,46.5798% .60307%,48.26352% .15192%,50% 0,51.73648% .15192%,53.4202% .60307%,55% 1.33975%,89.64102% 21.33975%,91.06889% 22.33956%,92.30146% 23.57212%,93.30127% 25%,94.03794% 26.5798%,94.48909% 28.26352%,94.64102% 30%,94.64102% 70%,94.48909% 71.73648%,94.03794% 73.4202%,93.30127% 75%,92.30146% 76.42788%,91.06889% 77.66044%,89.64102% 78.66025%,55% 98.66025%,53.4202% 99.39693%,51.73648% 99.84808%,50% 100%,48.26352% 99.84808%,46.5798% 99.39693%,45% 98.66025%,10.35898% 78.66025%,8.93111% 77.66044%,7.69854% 76.42788%,6.69873% 75%,5.96206% 73.4202%,5.51091% 71.73648%,5.35898% 70%,5.35898% 30%,5.51091% 28.26352%,5.96206% 26.5798%,6.69873% 25%,7.69854% 23.57212%,8.93111% 22.33956%,10.35898% 21.33975%);
    height: calc(var(--size) - var(--border-width) * 2)!important;
    transform: translateY(var(--border-width));
    width: calc(var(--size) - var(--border-width) * 2);
}

.user-menu {
	float: right;
	padding: 8px 12px;
	margin-right: 10px;
}

.tdl-divider {
	margin: 0;
	clear: both;
}

.midnav {
  overflow: hidden;
  background-color: #27292d;
  height: 100%;
  margin: auto;
  width: fit-content;
}

.midnav a {
  float: left;
  color: #f2f2f2;
  text-align: center;
  padding: 2px 10px;
  text-decoration: none;
  font-size: 18px;
  float: right;
  height: 100%;
  min-width: 324px;
}

.midnav a:hover {
  background-color: rgb(25, 37, 40) !important;
  color: black !important;
}

.midnav a.active:hover {
  background-color: rgb(25, 37, 40) !important;
  color: black !important;
}

.midnav a.active .nav-text-a {
  background-color: #27292d !important;
  color: rgb(178, 191, 55) !important;
  width: fit-content;
  margin: auto;
}

.midnav a.active {
  color: white;
  border-color: rgb(178, 191, 55) !important;
  border-style: solid;
  border-top: 0;
  border-left: 0;
  border-right: 0;
}

</style>