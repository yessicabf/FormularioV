<template>
    <h3>Total proyectos: {{ numeroProyectos }}</h3>

   <div class="table-responsive">
           <table class="table table-dark">
               <thead>
                   <tr>
                       <th>#</th>
                       <th>proyecto</th>
                       <th>Tipo</th>
                       <th>Urgente</th>
                       <th>Completado</th>
                   </tr>
               </thead>

               <tbody>
                   <tr v-for="(proyecto,index) in proyectos" :key="index">
                       <td>{{ index+1 }}</td>
                       <td>{{ proyecto.proyecto }}</td>
                       <td>{{proyecto.tipo }}</td>
                       <td @click="CambiarEstado(proyecto, 'urgente')" :class="proyecto.urgente ? 'bg-success' : 'bg-danger'">{{ proyecto.urgente ? "Si" : "No"}}</td>
                       <td @click="CambiarEstado(proyecto, 'completado')" :class="proyecto.completado ? 'bg-success' : 'bg-danger'">{{ proyecto.completado ? "Completo" : "Incompleto"}}</td>
                   </tr>
               </tbody>
           </table>
       </div>
       <hr>
</template>

<script>
   export default{
       props:['numeroProyectos', 'proyectos', 'CambiarEstado'],
   }
</script>