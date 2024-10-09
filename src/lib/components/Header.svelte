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
    background-color: black;
    color: white;
    justify-content: right;
    width: 100%;
    height: 60px;
    align-items: center;

}
a{
    color: rgb(0, 0, 0);
    text-decoration: none;  
    font-weight: 600;
    font-size: 20px;
    border-radius: 5px;
    border: 2px solid rgb(255, 255, 255);
    background-color: rgb(255, 255, 255);
    box-shadow: 0px 0px 4px white;
    padding-left: 5px;
    padding-right: 5px;
}
a:hover{
    box-shadow: 0px 0px 4px black;
    border: 2px solid rgb(0, 0, 0);
    text-shadow: 0px 0px 2px white;
    background-color: black;
    color: white;
    transition: 0.1s;
}
</style>