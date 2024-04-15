<!-- index.svelte -->
<script>
	// You can import necessary components or define logic here
	import DefaultLayout from '../../layouts/Layout_fa.svelte';
	import Sidebar from '$lib/sidebar.svelte'

</script>

<DefaultLayout title="Rings" buttonTitle="Create Ring">
	<!-- Slot for sidebar content -->
	<div slot="sidebar">
		<Sidebar />
	</div>
	<!-- Main content -->
	<div class="main-conatiner ">
		<!-- Action content -->
		<div class="form">
			<div class="row"> 
				<div class="column">
					<label class="input-label" for="input-search">Search query</label>
					<div class="form-input">
						<input class="input-cont" type="text" placeholder="Search query">
					</div>  
				</div>
				<div class="column">
					<label class="input-label" for="input-cat">Category</label>
					<div class="form-input">
						<select class="input-cont" name="cat-sel"></select>
					</div>
				</div>
				<div class="column">
					<label class="input-label" for="form-label">Tags</label>
					<div class="form-input">
						<input class="input-cont" type="text" placeholder="Tags">
					</div>
				</div>
			</div>
    	</div>
		<!-- end   -->
	</div>
	<div class="gallery-cont">
		<div class="gallery-items">
			<div class="gallery-actions">
			</div>
			<div class="gallery-images">
				<!-- svelte-ignore a11y-img-redundant-alt -->
				<img class="ring-picture" src= {'/sabrianna-Y_bxfTa_iUA-unsplash-removebg.png'} alt="image">
			</div>
			<div class="gallery-info">
			</div>
		</div>
		<div class="gallery-items">
			<div class="gallery-actions">
			</div>
			<div class="gallery-images">
				<!-- svelte-ignore a11y-img-redundant-alt -->
				<img class="ring-picture" src= {'/sabrianna-Y_bxfTa_iUA-unsplash-removebg.png'} alt="image">
			</div>
			<div class="gallery-info">
			</div>
		</div>
		<div class="gallery-items">
			<div class="gallery-actions">
			</div>
			<div class="gallery-images">
				<!-- svelte-ignore a11y-img-redundant-alt   -->
				<img class="ring-picture" src= {'/sabrianna-kuko1hX_kXw-unsplash-removebg-preview.png'} alt="image">
			</div>
			<div class="gallery-info">
			</div>
		</div>
		<div class="gallery-items">
			<div class="gallery-actions">
			</div>
			<div class="gallery-images-fa">
				<!-- svelte-ignore a11y-img-redundant-alt   -->
				<img class="ring-picture" src= {'/sabrianna-NhrcL_C0sFA-unsplash-removebg-preview.png'} alt="image">
			</div>
			<div class="gallery-info">
			</div>
		</div>
	</div>
</DefaultLayout>

<style>

  .main-conatiner{
    align-items: flex-start;
    border-radius: 4px;
    position: relative;
    z-index: 100;
    background-color: #FFFFFF;
    border: 1px solid #d9ddd7;
    border-width: 1px 1px 2px 1px;
    padding: 10px;
    margin-bottom: 10px;
  }


  .row{
    display: flex;
    gap: 31px;
    flex-direction: row;
  }

  .column{
    width: 32%;
  }

  .input-cont{

    width:  99.99%;
    height: 30px;
    line-height: 30px;
    padding: 0px 2px;
    font-size: 14px;
    letter-spacing: 0.5px;
    font-weight: 300;
	border: 1px solid #e2e5df;
    background-color: #FFFFFF;
	font-family: sans-serif;
  }

  .input-label{

    height: 20px;
    line-height: 20px;
    font-size: 10px;
    font-weight: 500;
    text-transform: uppercase;
    color: #900820;
    letter-spacing: 0.5px;
    font-family: sans-serif;

  }

  .form-input{

	border: 1px solid #e2e5df;
    background-color: #FFFFFF;
  }



  /* main content */

  .gallery-cont{

	display: flex;
    gap: 1%;
    flex-direction: row;
    justify-content: space-around;
	padding-top: 10px;
  }

  .gallery-items{

	width: 24%;
	border: 1px solid #e2e5df;
	height: 100%;
	border-radius: 4px;

  }

  .ring-picture{

	width: 100%;
  }

  .gallery-images-fa{

	width: 66%;
    padding: 0px 53px;
	background-color: #FFFFFF;
  }

  .gallery-images{

	background-color: #FFFFFF;
  }

</style>
