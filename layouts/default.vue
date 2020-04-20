<template>
 	<div id="wrapper">
			<div id="header">
				<div id="logo">
				</div>
				<div id="orglogo">
				</div>
			</div>
			<div id="bar">
				<div id="menu">
          <div v-for="(item, key) in menu" :key="key">
            <nuxt-link :to="item">{{item}}</nuxt-link>
          </div>
				</div>
				<div id="blog">
					<!-- <?php
						foreach ($blog as $key => $value) 
						{
					?>
						<div><a href="<?php echo $value; ?>.php"><?php echo $value; ?></a></div>
					<?php
						}
					?>
				</div> -->
				<div id="profile">
					<img src="images/avatar.png" />
					<table>
						<tr>
							<td>Monique Schuurman Hess</td>
						</tr>
						<tr>
                <td><a href="mailto:m.g.schuurmanhess@gmail.com">m.g.schuurmanhess@gmail.com</a></td>
						</tr>
						<tr>
							<td>+316 488 26537</td>
						</tr>
					</table>
				</div>
			</div>
			<nuxt/>

		</div>
    </div>
</template>

<style>

</style>
<script>
export default {
  data(){
    return{
      menu: ['index', 'identiteit', 'werkwijze', 'kosten', 'relatietherapie', 'contact']
    }
  }
}
</script>