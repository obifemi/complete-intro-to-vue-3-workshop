<script>
export default {
  name: 'artists',
 data(){
    return{
      artists: [
        {name: 'Adele'},
        {name: 'Beyonce'},
        {name: 'Coldplay'},
        {name: 'David Bowie'},
        {name: 'Ed Sheeran'},
        {name: 'Foo Fighters'},
        {name: 'Guns N Roses'},
        {name: 'Hozier'},
        {name: 'Imagine Dragons'},
        {name: 'Justin Bieber'},
        {name: 'Katy Perry'},
        {name: 'Lady Gaga'},
        {name: 'Muse'},
        {name: 'Nirvana'},
        {name: 'One Direction'},
        {name: 'Prince'},
        {name: 'Queen'},
        {name: 'Rihanna'},
        {name: 'Sia'},
        {name: 'Taylor Swift'},
        {name: 'U2'},
        {name: 'Van Halen'},
        {name: 'Whitney Houston'},
        {name: 'X Ambassadors'},
        {name: 'Zayn Malik'}
      ]
    }
  }
}

</script>

<template>
  <div v-if="artists.length>0">
    <h1>Artists</h1>
    <ul>
      <li v-for="(artist,index) in artists" :key="artist">{{ index }}:{{artist.name}}</li>
     
    </ul>
  </div>
</template>
