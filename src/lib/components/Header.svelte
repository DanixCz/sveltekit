<script>

</script>

<header>
    <nav>
        <a href="/">Home page</a>
        <a href="/">About</a>
        <a href="/">Svelte</a>
    </nav>

</header>

<style>


nav{
    display: flex;
    margin-right: 28px;
    gap: 20px;
    padding: 30px;
}

header{
    display: flex;
    position: sticky;
    background-color: rgb(0, 0, 0, 0.61);
    color: white;
    justify-content: right;
    width: 100%;
    height: 100px;
    backdrop-filter: blur(10px);
    align-items: center;
    position: sticky;
    margin: 0;
    top: 0;
}

a{
    box-shadow: 0px 0px 1px black;
    text-shadow: 0px 0px 1px black;
    color: white;
    text-decoration: none;  
    font-weight: 400;
    font-size: 20px;
    border-radius: 5px;
    border: 4px solid rgb(221, 37, 37);
    background-color: rgb(221, 37, 37);
    padding-left: 5px;
    padding-right: 5px;
}

a:hover{
    border: 4px solid rgb(69, 165, 243);
    background-color: rgb(69, 165, 243);
    color: white;
    transition: 0.1s;
}
</style>