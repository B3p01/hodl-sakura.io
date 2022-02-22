<template>
    <nav id="navbar" class="navbar navbar-expand-lg fixed-top navbar-dark" aria-label="Main navigation">
        <div class="container">
            <a class="navbar-brand logo-image" href="index.html"><img src="@/assets/images/HODL_Logo_White_no_Strap_70.png" /></a>
            <!-- Text Logo - Use this if you don't have a graphic logo <a class="navbar-brand logo-text" href="index.html"><span class="home_text">House of Delicate Leaves</span></a>-->
            <button class="navbar-toggler p-3 border-0" type="button" id="navbarSideCollapse" aria-label="Toggle navigation"><span class="navbar-toggler-icon"></span></button>
            <div class="navbar-collapse offcanvas-collapse" id="navbarsExampleDefault">
                <ul class="navbar-nav ms-auto navbar-nav-scroll">
                    <li class="nav-item"><a class="nav-link active" aria-current="page" href="#header">HOME</a></li>
                    <li class="nav-item"><a class="nav-link" href="#about">ABOUT</a></li>
                    <li class="nav-item"><a class="nav-link" href="#roadmap">ROADMAP</a></li>
                    <li class="nav-item"><a class="nav-link" href="#choose">CHOOSE</a></li>
                    <li class="nav-item"><a class="nav-link" href="#team">TEAM</a></li>
                    <li class="nav-item"><a class="nav-link" href="#faq">FAQ</a></li>
                    <li class="nav-item"><a class="nav-link" href="https://play.hodl-sakura.io">DEMO</a></li>
                </ul>
                <!--<span class="nav-item social-icons">
                    <span class="fa-stack">
                        <a href="https://discord.gg/uNKfc7pCyX"> <i class="fab fa-discord fa-stack-2x"></i> </a>
                    </span>
                    <span class="fa-stack">
                        <a href="https://twitter.com/Sakura_NFT_?t=poPtu1V1TANzv_5Iy-F4pA&s=09"> <i class="fab fa-twitter fa-stack-2x"></i> </a>
                    </span>
                </span>-->
            </div>
        </div>
    </nav>
</template>

<script>
export default {
  name: 'NavBar'
}
</script>

<style>
.nav-link {
	font-family: 'Open Sans';
}
.navbar-nav a:hover {
	color:#ffffff ;
}
.navbar {
	font-weight: 500;
	font-size: 0.875rem;
	line-height: 0.875rem;
	background-color: var(--secondary);
	box-shadow: 0 1px 6px 0 rgba(0, 0, 0, 0.025);
}
.navbar .navbar-brand {
	padding-top: 0.25rem;
	padding-bottom: 0.25rem;
}
.navbar .logo-image img {
	width: 70px;
	height: 70px;
	padding: 0px 0px 0px 0px;
}
.navbar .logo-text {
	color: #fff;
	font-weight: 500;
	line-height: 1rem;
	font-size: 1.575rem;
	text-decoration: none;
	font-family: serif;
}
.offcanvas-collapse {
	position: fixed;
	top: 5.75rem; 
	bottom: 0;
	left: 100%;
	width: 100%;
	overflow-y: auto;
	visibility: hidden;
	padding-right: 1rem;
	padding-left: 1rem;
	background-color: var(--primary-light);
	transition: transform 0.2s ease-in-out, visibility 0.2s ease-in-out;
}
.offcanvas-collapse.open {
	visibility: visible;
	transform: translateX(-100%);
}
.navbar .navbar-nav {
	margin-top: 0.75rem;
	margin-bottom: 0.5rem;
}
.navbar .dropdown-menu {
	border: none;
	margin-top: 0.25rem;
	margin-bottom: 0.25rem;
	background-color: var(--primary-light);
}
.navbar .dropdown-item {
	color: #eee;
	font-weight: 500;
	font-size: 0.875rem;
	line-height: 0.875rem;
	padding-top: 0.625rem;
	text-decoration: none;
	padding-bottom: 0.625rem;
}
.navbar .dropdown-item:hover {
    background-color: var(--tertiary);
}
.navbar .dropdown-divider {
	width: 100%;
	height: 1px;
	border: none;
	margin: 0.5rem auto 0.5rem auto;
	background-color: var(--primary-light);
}
.navbar .nav-item .nav-link {
	color: #eee;
	text-decoration: none;
	padding-top: 0.625rem;
	padding-bottom: 0.625rem;
	transition: all 0.2s ease;
}
.navbar .fa-stack {
	width: 2em;
	font-size: 0.75rem;
	margin-right: 0.5rem;
}
.navbar .fa-stack-2x {
	background: #ffffff;
	background-clip: text;
	-webkit-background-clip: text;
	-webkit-text-fill-color: transparent;
	transition: all 0.2s ease;
}
.navbar .fa-stack-1x {
	color: #ffffff;
	transition: all 0.2s ease;
}
.navbar .fa-stack:hover .fa-stack-2x {
    color: var(--primary);
}
.navbar .fa-stack:hover .fa-stack-1x {
    color: var(--primary);
}
.navbar .navbar-toggler {
	padding: 0;
	border: none;
	font-size: 1.25rem;
}
/* Dropdown Menu */
.navbar .dropdown .dropdown-menu {
    animation: fadeDropdown 0.2s; /* required for the fade animation */
}

@-webkit-keyframes fadeDropdown {
	0% {
		opacity: 0;
	}

	100% {
		opacity: 1;
	}
}

@keyframes fadeDropdown {
	0% {
		opacity: 0;
	}

	100% {
		opacity: 1;
	}
}

@media (min-width: 992px) {
/* Navigation */
	.navbar {
		box-shadow: none;
		transition: all 0.2s;
		padding-top: 1rem;
		background-color:  var(--secondary);
	}

	.navbar.top-nav-collapse {
		padding-top: 0.5rem;
		padding-bottom: 0.5rem;
		background-color: var(--secondary);
		box-shadow: 0 3px 6px 0 rgba(0, 0, 0, 0.025);
	}
    .navbar .navbar-nav {
		margin-top: 0;
		margin-bottom: 0;
	}

	.navbar .nav-item .nav-link {
		padding-right: 0.75rem;
		padding-left: 0.75rem;
	}

	.navbar .dropdown-menu {
		padding-top: 0.75rem;
		padding-bottom: 0.875rem;
		box-shadow: 0 3px 3px 1px rgba(0, 0, 0, 0.08);
	}

	.navbar .dropdown-divider {
		width: 90%;
	}

	.navbar .social-icons {
		margin-left: 0.5rem;
	}

	.navbar .fa-stack {
		margin-right: 0;
		margin-left: 0.25rem;
	}
}

@media only screen and (max-width: 540px) {
    .navbar .logo-image img {
		width: 50px;
		height: 50px;
		padding: 0px 0px 0px 0px;
	}
}
</style>