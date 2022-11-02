<template>
   <div class="container">
      <div class="row">
         <div class="col-md-12">
            <div class="table-responsive">
 
               <table class="table">
                  <thead class="thead-dark">
                     <tr>
                        <th scope="col">name</th>
                        <th scope="col">name</th>
                        <th scope="col">name</th>
                        <th scope="col">location</th>
                        <th scope="col">gender</th>
                        <th scope="col">imagen</th>
                     </tr>
                  </thead>
                  <tbody>
                     <tr v-for="item in items" v-bind:key="item.id">
                         <td>{{ item.name.tittle }}</td>
                        <td>{{ item.name.first }}</td>
                         <td>{{ item.name.last }}</td>
                        <td>{{ item.location.country }}</td>
                        <td>{{ item.gender }}</td>
                        <td><img v-bind:src="'img/' + item.img" class="img-fluid" width="30px" v-bind:alt="item.nombre"></td>
                     </tr>
                  </tbody>
               </table>
 
            </div>
         </div>
      </div>
   </div>
</template>