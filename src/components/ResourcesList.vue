<template>
    <ul>
        <ResourceItem v-for="res in resources"
        :key="res.id"
        :title="res.title"
        :description="res.description"
        :link="res.link"
        >
        </ResourceItem >
    </ul>
       
 </template>    
 
 
 
 <script>
    import ResourceItem from './ResourceItem.vue';
import ResourceItem from './ResourceItem.vue';
    
    export default{
    props: { title: String, description: String, link: String },
    comments: {
        ResourceItem
    },
}

 </script>
 




