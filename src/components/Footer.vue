<template>
   <footer>
			<div class="container">
				<div class="footer-box">
					<router-link to="/" class="footer-logo logo">
						<img src="../assets/img/icon/logo.svg" alt="Logo" />
					</router-link>
					<div class="footer-nav">
						<ul>
							<li><router-link class="products-card" to="/rest"> Ресторанам</router-link></li>
							<li><router-link class="products-card" to="/rest">Курьерам</router-link></li>
							<li><router-link class="products-card" to="/rest">Пресс-центр</router-link></li>
							<li><router-link class="products-card" to="/rest">Контакты</router-link></li>
						</ul>
					</div>
					<div class="footer-social">
						<router-link to="/" class="social-link"><img src="../assets/img/social/instagram.svg" alt="instagram" /></router-link>
						<router-link to="/" class="social-link"><img src="../assets/img/social/fb.svg" alt="facebook" /></router-link>
						<router-link to="/" class="social-link"><img src="../assets/img/social/vk.svg" alt="vk" /></router-link>
					</div>
				</div>
			</div>
			<!-- /.container  -->
		</footer>
    </template>
    <script>
    export default{
    
    }
    </script>
   <style scoped>
   footer {
    min-height: 156px;
    padding: 60px 0;

}

.footer-box {
    height: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 36px;
    flex-wrap: wrap;

}

.footer-nav {
    flex-grow: 1;
}

.footer-nav ul {
    display: flex;
    align-items: center;
    list-style: none;
    padding: 0;
    gap: 15px;
    flex-wrap: wrap;
}

.footer-nav__link {
    color: #595959;
    font-weight: 400;
    font-size: 18px;
    text-decoration: none;

}

.footer-social {
    display: flex;
    align-items: center;
    justify-content: flex-end;
    gap: 20px;
}

</style>