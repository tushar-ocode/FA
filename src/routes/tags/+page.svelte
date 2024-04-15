<script>
    import DefaultLayout from '../../layouts/Layout_fa.svelte';
	import Sidebar from '$lib/sidebar.svelte'
</script>


<DefaultLayout title="Tags" buttonTitle="Add Tag">
    <!-- Slot for sidebar content -->
	<div slot="sidebar">
		<Sidebar />
	</div>
</DefaultLayout>