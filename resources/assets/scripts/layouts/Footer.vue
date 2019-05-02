<template>
  <footer>
  	<dl>
  		<dt>Email</dt>
  		<dd><a :href="mailto">{{email}}</a></dd>
  	</dl>
  	<dl>
  		<dt>Phone</dt>
  		<dd><a :href="tel">{{phone}}</a></dd>
  	</dl>
  	<dl class="mb-0">
  		<dt>Find me on</dt>
  		<dd class="mb-0">
  			<ul class="nav nav-social">
  				<li class="nav-item">
  					<a class="nav-link" href="https://www.facebook.com/" target="_blank">
  						<i class="fa fa-facebook"></i>
  					</a>
  				</li>
  				<li class="nav-item">
  					<a class="nav-link" href="https://www.linkedin.com/in/ntsika-mark-mngoma/" target="_blank">
  						<i class="fa fa-linkedin"></i>
  					</a>
  				</li>
  				<li class="nav-item">
  					<a class="nav-link" href="https://twitter.com/" target="_blank">
  						<i class="fa fa-twitter"></i>
  					</a>
  				</li>
  				<li class="nav-item">
  					<a class="nav-link" href="https://github.com/NtsikaMngoma" target="_blank">
  						<i class="fa fa-github"></i>
  					</a>
  				</li>
  			</ul>
  		</dd>
  	</dl>
  </footer>
</template>

<script>
export default {
	data(){
		return {
			email: 'mark@mergemedia.co.za',
			phone: '082 283 2834',
			social : {
				facebook : '',
				twitter: '',
				github: ''
			}
		}
	},
	computed: {
		mailto(){
			return 'mailto:' + this.email;
		},
		tel(){
			return 'tel:' + this.phone.replace(/ /g, '')
		}
	}
}
</script>
