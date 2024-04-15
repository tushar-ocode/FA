<!-- DefaultLayout.svelte -->
<script>
  /**
	 * @type {any}
	 */
   export let title; // Prop to set the page title
   /**
	 * @type {any}
	 */
    export let buttonTitle;
</script>

<div class="wrapper">
  <div class="container">
      <div class="sidebar">
          <!-- Sidebar content goes here -->
          <slot name="sidebar">
          </slot>
      </div>
      <div class="main-wrapper">
        <div class="header">
          <!-- Header content goes here -->
          <div class="header--title">
            {title}
            <div class="ring-action">
              <button class="action_btn">
                <i class="material-symbols-outlined">add</i>
                {buttonTitle}</button>
            </div>

          </div>
        </div>  
        <div class="main-content">
            <!-- Main content goes here -->
            <slot></slot>
        </div>
    </div>
  </div>
</div>

<style>
  .body {
      margin: 0;
      padding: 0;
  }

  .wrapper {
      display: flex;
      flex-direction: column;
      height: 100vh;
  }

  .header {
      background-color: #333;
      color: #fff;
      padding: 10px;
      text-align: center;
      height: 43px;
      border-bottom: 1px solid #e0e5da;
      background-color: #f9faf8;
  }

  .header--title {
      margin: 0;
      padding: 10px 0px;
      font-size: 24px;
      color: #900820;
      font-weight: 300;
      font-family: sans-serif;
      display: flex;
      justify-content: space-between;

  }

  .action_btn{
    border-radius: 2px;
    background-color: #a80925;
    color: #FFFFFF;
    height: 30px;
    line-height: 9px;
    padding: 10px 20px;
    font-size: 14px;
    font-weight: 300;
    display: inline-block;
    text-decoration: none;
    margin: 0px 5px 0px 0px;
    display: flex;
    gap: 5px;
    align-items: center;
  }


  .container {
      display: flex;
  }

  .sidebar {
      background-color: #a80925;
      padding: 20px;
      width: 250px;
      height: 100vh;
  }

  .main-content {
      padding: 20px;
  }

  .main-wrapper{
    width: 100%;
  }

  .ring-action{

    display: flex;
    gap: 5px;
    align-items: center;
  }
</style>
