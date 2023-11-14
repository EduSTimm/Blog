# Blog
 A minha ideia do projeto é um blog simples, onde eu posso além de fazer um portifólio, comentar assuntos do meu interesse.


*{
	box-sizing: border-box;
	margin: 0;
	padding: 0;
}
:root{
	--maincolor: #000a61;
}
/* --------------HEADER------------------------------------------------------------------------------------------ */
.nav_ul_li_a{
	color: #fff;
	text-decoration: none;
	padding: 2px;
}
.nav_ul_li_a:hover{
	opacity: 0.8;
}
.nav_ul li:hover{
	background: rgba(255, 255, 255, 0.2);
	border-radius: 6px;
}
.logo_nav{
	font-size: 24px;
	text-transform: uppercase;
	letter-spacing: 4px;
}
nav{
	display: flex;
	justify-content: space-around;
	align-items: center;
	font-family: system-ui, -apple-system, Helvetica, Arial, sans-serif;
	background: var(--maincolor);
	height: 9vh;
	width: 100vw;
}
.nav_ul{
	list-style: none;
	display: flex;
}
.nav_ul li{
	letter-spacing: 3px;
	margin-left: 32px;
	padding: 6px;
}
/*Criar as barras do menu para telefone*/
.nav_menu_bars div{
	width: 32px;
	height: 2px;
	background: #eee;
	margin: 8px;
	transition: 0.3s;
}
/*Para ocultar as barras do menu de telefone na 
página do site para computadores*/
.nav_menu_bars{
	display: none;
	cursor: pointer;
}

/* ------------------MAIN-------------------------------------------------------------------------------------------- */
body{
	font-family: 'Poppins', sans-serif;
	background: #ddd;
	color: #333;
	overflow-x: hidden;

}
/*Primeira página com foto e descrição.*/
.description{
	height: 91vh;
	display: flex;
	width: 75vw;
	align-items: center;
	justify-content: center;
	margin-left: 12vw;
}
.main_photo{
	display: flex;
	flex-basis: 50%;
	border-radius: 50%;
	justify-content: center;
	padding: 15px;
}
.main_photo img{
	width: 350px;
	height: 350px;
	margin: 100px 0;
	border-radius: 50%;
	object-fit: cover;
	z-index: -1;
	box-shadow: 4px 0 10px 0 #777, 8px 0 10px 0 #aaa, 12px 0 10px 0 #eee;
}
.description_text{
	flex-basis: 50%;
	padding: 15px 35px 0 20px;
	width: 100%;
}
.greeting{
	letter-spacing: 1.5px;
	font-size: 1em;
	line-height: 1.5;
}
h1{
	font-size: 2.5em;
	letter-spacing: 2.5px;
	margin: 24px 0;
}
h1 span{
	color: var(--maincolor);
}
.smalldescription{
	letter-spacing: 1px;
	color: #555551;
	font-size: 1.2rem;
	min-width: 250px;
	line-height: 1.5;
}
.smalldescription span{
	color: var(--maincolor);
	font-size: 1.2rem;
	font-weight: 550;
}
/*-----------------LINKS GITHUB/LINKEDIN---------------------------------------------------------------------------------------------*/
.socialmedia{
	display: flex;
	margin-top: 30px;
}
.resumelink{
	background: var(--maincolor);
	margin: -13px 0;
	padding: 15px 35px;
	border-radius: 40px;
	letter-spacing: 2.5px;
	font-size: 1rem;
	font-weight: 300;
	display: inline-block;
	transition: box-shadow 0.2s;
	color: #eee;
	text-decoration: none;
}
.resumelink:hover{
	box-shadow: 0 2px 15px 0 #000070;
}
.sociallist{
	margin: 40px 0;
	list-style: none;
	display: flex;
}
.sociallist li a{
	margin: 0 14px;
	padding: 9px 10px;
	background: #fff;
	border-radius: 6px;
	color: var(--maincolor);
	border: 1px solid #ccc;
	box-shadow: 0 4px 6px 0 #777;
}
.sociallist li a:hover{
	box-shadow: 0 2px 15px 0 #000070;
}
.sociallist li a i{
	color: var(--maincolor);
}
/*---------------ABOUT ME------------------------------------------------------------------------------------------------.*/
.about{
	display: flex;
	flex-direction: column;
	margin: 30px 40px;
}
.titulo-about{
	margin: 50px 20px;
	padding-top: 25px;
	font-weight: 500;
	letter-spacing: 2px;
	font-size: 1.6rem;
}
.information{
	background: #fff;
	padding: 30px 10vw;
	border-radius: 50px;
	font-size: 1.1rem;
	letter-spacing: 1px;
	width: 75vw;
	text-align: justify;
	align-self: center;
}
/*--------------SKILLS-----------------------------------------------------------------------------------------------------------------*/
.skills{
	margin: 0 40px;
	display: flex;
	flex-direction: column;
}
.titulo-skills{
	margin: 50px 20px;
	padding-top: 25px;
	font-weight: 500;
	letter-spacing: 2px;
	font-size: 1.6rem;
}
.grid_container{
	display: grid;
	grid-template-columns: repeat(auto-fill, minmax(100px, 1fr));
	justify-content: center;
	align-items: center;
	background: #fff;
	padding: 30px;
	border-radius: 50px;
	list-style: none;
	grid-column-gap: 45px;
	grid-row-gap: 50px;
	width: 75vw;
	align-self: center;
}
.grid_items{
	justify-self: center;
	padding: 10px 4px 5px 4px;
	border-radius: 20px;
	border: 0.5px solid #aaa;
	transition-duration: 0.2s;
}
.grid_items:hover{
	box-shadow: 0 2px 15px 0 #aaa;
}
.grid_items p{
	padding: 1px;
	font-size: 14px;
	text-align: center;
}
.grid_items img{
	width: 50px;
	height: 50px;
	margin: 0 20px;
}
.sketchup{
	transform: scaleY(2.5);
	margin-bottom: 10px;
}
/*---------------PROJECTS----------------------------------------------------------------------------------------------------*/
.works{
	margin: 0 40px;
	margin-bottom: 20px;
	display: flex;
	flex-direction: column;
	justify-content: center;
}
.titulo-works{
	margin: 50px 20px;
	padding-top: 25px;
	font-weight: 500;
	letter-spacing: 2px;
	font-size: 1.6rem;
	display: block;
}
.grid_container_works{
	display: grid;
	grid-template-columns: repeat(2, 30vw);
	grid-template-rows: repeat(3, 18vw);
	justify-content: center;
	align-self: center;
	background-color: #fff;
	padding: 30px;
	border-radius: 50px;
	width: 75vw;
}
.grid_items_div{
	display: flex;
	flex-direction: column;
	justify-items: center;
	align-items: center;
}
.grid_items_div h3{
	text-align: center;
}
.grid_items_works{
	width: 20vw;
	height: 12vw;
	border-radius: 20px;
}
.grid_items_works:hover{
	box-shadow: 0 3px 15px 0 #555;
}
/*-------------CONTACT--------------------------------------------------------------------------------------------------*/
.contact{
	margin: 0 40px;
	display: flex;
	flex-direction: column;
}
.titulo-contact{
	margin: 30px 20px;
	padding-top: 25px;
	font-weight: 500;
	letter-spacing: 2px;
	font-size: 1.6rem;
}
.contact-details{
	display: flex;
	flex-direction: column;
	background: #fff;
	border-radius: 20px;
	margin: 50px 35px;
	width: 75vw;
	align-items: center;
	justify-content: center;
	align-self: center;
}
.contact-details-email{
	margin: 30px;
	margin-top: 30px;
	transition-duration: 0.7s;
	border-radius: 10px;
	border: 0.5px solid #ddd;
}
.contact-details-email img{
	width: 50px;
	display: block;
	margin-left: auto;
	margin-right: auto;
	padding-top: 10px;
}
.contact-details-email a{
	display: block;
	text-align: center;
	text-decoration: none;
	padding: 10px;
	color: var(--maincolor);
	font-size: 18px;
}
.contact-details-email p{
	display: block;
	text-align: center;
	padding-bottom: 10px;
	color: #555;
	font-size: 15px;
}
.contact-details-email:hover{
	box-shadow: 0 2px 15px 0 #aaa;
}
.titulo-contact_form{
	margin: 20px 20px;
	font-weight: 500;
	letter-spacing: 2px;
	font-size: 1.2rem;
	align-self: flex-start;
}
.form_contact{
	padding: 20px;
	margin: 10px;
	height: 60vh;
}
.name{
	height: 8vh;
	width: 32.4vw;
	border-radius: 10px;
	margin-bottom: 10px;
	margin-right: 0.4vw;
	padding: 7px;
	border-color: #aaa;
	border-style: solid;
}
.email{
	display: inline;
	height: 8vh;
	width: 36.5vw;
	border-radius: 10px;
	margin-bottom: 10px;
	padding: 7px;
	border-color: #aaa;
	border-style: solid;
}
.subject{
	height: 8vh;
	width: 70vw;
	border-radius: 10px;
	margin-bottom: 10px;
	padding: 7px;
	border-color: #aaa;
	border-style: solid;
}
.form_contact textarea{
	resize: none;
	height: 25vh;
	width: 70vw;
	margin: 10px 0;
	border-radius: 15px;
	padding: 10px;
}
.submit{
	margin-top: 15px;
	font-size: 18px;
	padding: 10px 10px;
	border-radius: 15px;
	border: 1px solid #aaa;
	color: #eee;
	background: var(--maincolor);
	position: relative;
	left: 45%;
}
/* ------------------FOOTER------------------------------------------------------------------------------------------------------------------ */
footer{
	margin-top: 15px;
	width: 100vw;
	height: 8vh;
	bottom: 0;
	display: inline-block;
	background-color: var(--maincolor);
}
.copyright{
	text-align: center;
	padding: 2vh 0;
	font-weight: bold;
	color: #eee;
	font-size: 1rem;
}
/* --------------------RESPONSIVIDAD------------------------------------------------------------------------------------------------- */
@media screen and (min-width: 300px) and (max-width:  750px){
	body{
		overflow-x: hidden;
	}
	.nav_ul{
		flex-direction: column;
		position: absolute;
		top: 9vh;
		right: 0;
		width: 36vw;
		height: 91vh;
		background: #23232e;
		align-items: center;
		justify-content: space-around;
		transform: translateX(110%);
		opacity: 0.9;
		transition: transform 0.3s ease-in;
		display: none;
	}
	.nav_ul li{
		margin-left: 0;
		opacity: 1;
	}
	.nav_menu_bars{
		display: block;
	}
	/*Quando esta ativo o botão do menu a lista de links
	volta para o lugar que deve*/
	.nav_ul_active{
		transform: translateX(0);
		display: flex;
	}
	/*Quando as barras do menu estão ativas
	mudam de posição formando um x */
	.nav_menu_bars_active .line1{
		transform: rotate(-45deg) translate(-8px, 8px);
	}
	.nav_menu_bars_active .line2{
		opacity: 0;
	}
	.nav_menu_bars_active .line3{
		transform: rotate(45deg) translate(-5px, -7px);
	}
	/*Animação dos links do menu para telefones*/
	@keyframes navLinksEntrance{
		0% {
			opacity: 0;
			transform: translateX(50px);
		}100%{
			transform: translateX(0);
			opacity: 1;
		}
	}
	.description{
		display: block;
		margin-bottom: 250px;
	}
	.description_text{
		text-align: center;
	}
	.socialmedia{
		display: inline-flex;
		flex-direction: column;
	}
	.main_photo img{
		width: 250px;
		height: 250px;
	}
	.sociallist li a:hover{
		box-shadow: 0 2px 15px 0 #000070;
	}
	.sociallist li a i{
		color: var(--maincolor);
	}
	.titulo-about{
		margin-top: 10vh;
		margin-bottom: 40px;
	}
	.grid_container_works{
		grid-template-columns: repeat(2, 35vw);
		grid-template-rows: repeat(3, 27vw);
	}
	.grid_items_works{
		width: 25vw;
		height: 17vw;
	}
	.grid_items_div h3{
		text-align: center;
		font-size: 2.5vw;
	}
	.name{
		width: 32vw;
	}
}
