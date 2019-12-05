<template>
  <div>
    <Carousel />
    <v-row id="about" justify="center" align="center">
      <v-col class="d-flex justify-center">
        <v-avatar size="230">
          <img src="~static/img/Titouan.jpg" alt="Titouan">
        </v-avatar>
      </v-col>
      <v-col cols="8">
        <v-card class="mt-5">
          <v-card-title class="red lighten-1">
            A propos de moi
          </v-card-title>
          <v-card-text class="body-1 pt-3">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Perferendis, at aliquid odio nam aspernatur reiciendis minus culpa, dolore hic, ratione dolorum facilis rem explicabo earum iure voluptates! Ducimus magni sint repellat itaque iure earum molestias hic tempore illo pariatur architecto fuga ad, mollitia, quidem aperiam culpa alias, labore necessitatibus autem. Pariatur, labore magni! Fuga, consequuntur. Inventore fugiat voluptatem perspiciatis dicta amet odit officiis, quidem maxime repellendus mollitia est aliquam eaque voluptatum officia praesentium explicabo totam, adipisci optio autem a animi alias? Minus illum error veritatis repudiandae laudantium enim doloremque quas? Aspernatur ipsa quia voluptas autem omnis quo nobis nostrum laboriosam nisi deleniti. Ipsam odit beatae enim sequi commodi est placeat, eveniet, aut possimus mollitia porro, optio harum! Eaque, ea? Quam beatae aut porro inventore architecto ex consequuntur laboriosam. Autem, recusandae animi magnam ab, molestias quia dignissimos veniam, tempore non commodi similique accusantium inventore impedit culpa aut consectetur quaerat obcaecati maxime.
          </v-card-text>
        </v-card>
      </v-col>
    </v-row>
    <v-row id="projects" justify="center" align="start">
      <v-col v-for="project in projects" :key="project.name">
        <v-card min-height="320">
          <v-card-title class="red lighten-1">
            {{ project.name }}
          </v-card-title>
          <v-card-text class="pt-3">
            {{ project.description }}
          </v-card-text>
        </v-card>
      </v-col>
    </v-row>
    <v-row id="skills">
      <Chart />
    </v-row>
  </div>
</template>

<script>
import Carousel from '~/components/Carousel'
import Chart from '~/components/Chart'
export default {
  components: {
    Carousel,
    Chart
  },
  data () {
    return {
      projects: [
        {
          name: 'lorem lorem lorem',
          image: 'static/img/logo.png',
          description: 'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Illo aliquid obcaecati quibusdam dicta neque ut eligendi fugit fuga velit error cum nostrum distinctio tempora iusto odit culpa exercitationem, consequatur voluptatem, vel laborum amet porro sed autem. Esse quae voluptatum sint quas facilis, impedit tempora velit culpa iste! Corrupti ullam culpa quasi eveniet officiis nisi obcaecati facilis delectus nostrum. Vero, sunt!'
        },
        {
          name: 'lorem yes lorem',
          image: 'static/img/logo.png',
          description: 'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Illo aliquid obcaecati quibusdam dicta nint qs nisi obcaecati facilis delectus nostrum. Vero, sunt!'
        },
        {
          name: 'lorem lorem yes yes',
          image: 'static/img/logo.png',
          description: 'Lorem ipsum, dolor sit amet consectetur adipisicing elit. Illo aliquid obcaecati quibusdam dicta neque ut eligendi fugit fuga velit error cum nostrum distinctio tempora iusto odit culpa exercitationem, consequatur voluptatem, vel laborum amet porro sed autem. Esse quae voluptatum sint quas facilis, impedit tempora velit culpa iste! Corrupti ullam culpa quasi eveniet officiis nisi obcaecati facilis delectus nostrum. Vero, sunt! velit error cum nostrum distinctio tempora iusto odit culpa exercitationem, consequatur voluptatem, vel laborum amet porro sed autem. Esse quae voluptatum sint quas facilis, impedit tempora velit culpa iste! Corrupti ullam culpa quasi eveniet officiis nisi obcaecati facilis delectus nostrum. Vero, sunt!'
        },
      ]
    }
  }
}
</script>

<style scoped lang="sass">
#about
  margin-bottom: 100px
</style>
