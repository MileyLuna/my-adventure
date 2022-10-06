<script>
    let img; 
</script>


<div>
    <h1>Secret Stash</h1>
    <p>
    This application allows registered users to add, edit, and delete their recipes. I hope to add in functionality to search,
    add image, and favorite a recipe.
    <br/>
    Secret Stash was built on a 2-week sprint as Prime Digital Academy solo project. P.E.R.N Stack was utilized to make this application interactive. Intergrated some Material UI and Sweet Alerts.
    </p> 

    <div class="container">
        <img src={'image/home.png'} bind:this={img} width={52} height={48} alt='home'/>
        <img src={'image/add.png'} bind:this={img} width={52} height={48} alt='add'/>
        <img src={'image/edit.png'} bind:this={img} width={52} height={48} alt='edit'/>
    </div>
</div>

<style>
    img {
        width: 100px;
        height: 100px;

    }
    div {  
        margin-left: 12rem;
    }
</style>
