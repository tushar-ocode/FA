<script>


</script>

<div class="dahsboard-title">Forver Artisians</div>
<div class="dashboard-menu">
    <ul>
        <div class="items-wrapper">
            <i class="material-symbols-outlined">home</i>
            <a href="/dashboard"><li>Rings</li></a>
        </div>  

        <div class="items-wrapper">
            <i class="material-symbols-outlined">group</i>
            <a href="/users"><li>Users</li></a>
        </div>
        <div class="items-wrapper">
            <i class="material-symbols-outlined">category</i>
            <a href="/categories"><li>Categories</li></a>
        </div>
        <div class="items-wrapper">
            <i class="material-symbols-outlined">sell</i>
            <a href="/tags"><li>Tags</li></a>
        </div>
        <div class="items-wrapper">
            <i class="material-symbols-outlined">account_circle</i>
            <a href="/accounts"><li>Manage Account</li></a>
        </div>
        <div class="items-wrapper">
            <i class="material-symbols-outlined">logout</i>
            <a href="/login"><li>Logout</li></a>
        </div>
    </ul>
</div>


<style>

    /* Side bar css */
	.dahsboard-title {
		border-bottom: 1px solid #9c0822;
		height: 36px;
		line-height: 23px;
		width: 100%;
		padding: 5px;
		color: #ffffff;
		text-align: center;
		font-weight: 300;
		font-family: sans-serif;
	}

	.dashboard-menu ul {
		position: relative;
		z-index: 1;
		color: #ffffff;
		padding: 0px;
		font-weight: 300;
		font-size: 14px;
		line-height: 46px;
		cursor: pointer;
	}

	.items-wrapper:hover{

		background-color:#9c0822;
	}

	.dashboard-menu li {	
		list-style-type: none;
		font-family: sans-serif;
	}

	.items-wrapper {
		display: flex;
		flex-direction: row;
		align-items: center;
		gap: 10px;

	}

	a {
    color: inherit; /* Use the color inherited from the parent element */
    text-decoration: none; /* Remove underlines */
	}	

</style>