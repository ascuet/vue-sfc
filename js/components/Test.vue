<template>
	<div >
		<table class="table">
			<thead class="thead-dark">
				<tr>
					<th scope="col">ID</th>
					<th scope="col">First Name</th>
					<th scope="col">Last Name</th>
					<th scope="col">Email</th>
				</tr>
			</thead>
			<tbody>
				<tr v-for="employee in employees">
					<th scope="row"> {{ employee.id }} </th>
					<td> {{ employee.f_name }} </td>
					<td> {{ employee.l_name }} </td>
					<td> {{ employee.email }} </td>
				</tr>
			</tbody>
		</table>
	</div>
</template>

<script>
module.exports = {

	data() {
		return {
			employees: [
				{
					id: 1,
					f_name: 'Anik',
					l_name: 'Sen',
					email: 'ascuet@gmail.com'
				},
				{
					id: 2,
					f_name: 'Minhaz',
					l_name: 'Hossain',
					email: 'minhaz@gmail.com'
				},
				{
					id: 3,
					f_name: 'Fahad',
					l_name: 'Bin Munir',
					email : 'fahadbinmnr@gmail.com'
				}
			]
		}
	},	

	mounted () {
		console.log('Hello World')
	}
};
</script>

<style scoped>
span {
	background-color: yellow;
}
</style>