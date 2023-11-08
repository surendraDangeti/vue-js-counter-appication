<template>
    <li>
        <div>
            <heading>
                <h3>{{ title }}</h3>
                <button>Delete</button>
             </heading>   
         </div>
         <p>{{ description }}</p>
         <nav> <a :href="link">view Resources</a></nav>   
     </li>   
</template>

<script>
 export default{
    props:{title:String, description:String, link:String}
    

 }
</script>

<style scoped>
li{
    margin: auto;
    max-width: 40rem;
}
header{
    display: flex;
    justify-content: space-between;
    align-items: center;
}
h3{
    font-size: 1.25rem;
    margin: 0.5rem 0;
}

p{
    margin: 0.5rem 0;
}

a{
    text-decoration: none;
    color: red;
}
a:hover a:active {
    color:#965725;
}

</style>