<style>
    h1 {
  color: #404040;
  font-size: 50px;
}
h4{
    color:#071d1d;
}
</style>
<template>
  <div>
  <v-container>
      <v-row>
          
         <v-col cols="6" class="pr-0">
            <v-img width="100%"
            src="@/assets/one.jpg"
        ></v-img>
         </v-col>
        
        
        <v-col class="text-left align-self-center" style=" text-align:left;" center cols="6">
            <div>
            <h1>Lorem Ipsum</h1>
            <h1>dolor sir amet</h1>
            <h4>Lorem ipsum dolor sit amet, consectetur adipiscing elit,</h4>
            <h4>eiusmod tempor incididunt ut labore et dolore magna.</h4>
            <h4>Ut enim ad minim veniam,</h4>
        </div>
        </v-col>
    </v-row>
    <v-row>
        <v-col class="my-auto" style="text-align:left;" cols="6">
            <h1>Lorem Ipsum</h1>
            <h1>dolor sir amet</h1>
            <h4>Lorem ipsum dolor sit amet, consectetur adipiscing elit,</h4>
            <h4>eiusmod tempor incididunt ut labore et dolore magna.</h4>
            <h4>Ut enim ad minim veniam,</h4>
        </v-col>
        
        <v-col cols="6" class="pl-0">
            <v-img width="100%"
            src="@/assets/two.jpg"
        ></v-img>
        </v-col>
      
  </v-row>
    </v-container>
</div>
</template>
<script>
export default{
 name: 'App',
    data: function(){
    return {
    tes: 'aha'
    }
    }
}
    
</script>
