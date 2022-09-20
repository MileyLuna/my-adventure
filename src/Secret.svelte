<script>
    let src = 'image/home.png';
    let src1 = 'image/add.png';
    let src2 = 'image/edit.png';
    let img; 
</script>


<div>

    <h1>Secret Stash</h1>
    <p>This application is one of Prime Digital Academy capstone. This was a solo project built on 
        a 2-week sprint.
    </p>
    <p>Secret Stash is recipe vault for registered users to contribute and 
        share their recipe with other users. Users have access to make changes 
        and delete their contributions.
    </p>
    <p>
    Technology used: HTML, JavaScript, Node.js, React, Redux, Saga, Material UI, CSS, PostgreSQL
    </p> 

    <p> Home Page:</p>
    <img {src} bind:this={img} width={46} height={46} alt='home'/>
    <img {src1} alt='add'/>
    <img {src2} alt='edit'/>
</div>

<style>
    img {
        width: 100%;
        height:100%;
    }
</style>
