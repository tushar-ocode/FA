<script>
    import DefaultLayout from '../../layouts/Layout_fa.svelte';
	import Sidebar from '$lib/sidebar.svelte'
</script>


<DefaultLayout title="Categories" buttonTitle="Add Category">
    <!-- Slot for sidebar content -->
	<div slot="sidebar">
		<Sidebar />
	</div>
</DefaultLayout>