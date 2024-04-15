<script>
    import DefaultLayout from '../../layouts/Layout_fa.svelte';
	import Sidebar from '$lib/sidebar.svelte'
</script>


<DefaultLayout title="Users" buttonTitle="Add User">
    <!-- Slot for sidebar content -->
	<div slot="sidebar">
		<Sidebar />
	</div>
</DefaultLayout>