<template>
  <div class="container">
    <div class="row row-cols-md-4 justify-content-center mt-5">
      <InfoComponent v-for="info in infos" :title="info.title"  :number="info.num"/>
    </div>
  </div>
  <div class="container marg">
    <div class="row">
      <AboutMeComponents />
    </div>
  </div>
  <div class="container marg2">
    <div class="row">
      <VideoComponent />
    </div>
  </div>
  <div class="container marg">
    <div class="row">
      <div class="col text-center">
        <p>Being your Journey at MaxCoach</p>
        <h2 class="fs-1">Latest <span>Online Courses</span></h2>
      </div>
    </div>
    <div class="row mt-5">
      <LatestCourses v-for="course in courses" :image="course.image" :price="course.price" :name="course.name" :lessons="course.lessons" :students="course.students"/>

    </div>
    <div class="row marg2">
      <div class="col text-center">
        <button type="button" class="btn text-white">View All Courses <i class="fa-solid fa-arrow-right ps-2"></i></button>
      </div>
    </div>
  </div>
  <div class="container marg">
    <div class="row">
      <BookStoreComponent />

    </div>
  </div>
  <div class="container marg">
    <div class="row row-cols-md-6 m-0">
        <ClientLogComponent v-for="log in clientLog" :image="log.image"/>

    </div>
  </div>
  <div class="container-fluid marg back">
    <div class="row row-cols-md-2">
     <RealStoriesComponent />
    </div>
  </div>
  <div class="container marg">
    <div class="row">
      <div class="col">
        <h6>Blog Updated</h6>
        <h2>Interesting <span>articles update</span> daily</h2>
      </div>
    </div>
    <div class="row row-cols-md-4 mt-5">
      <BlogComponents v-for="choice in blog"  :image="choice.image" :data="choice.data" :text="choice.text" :name="choice.name"/>
    </div>
    <div class="row mt-4">
      <div class="col text-center">
         <a class="fw-bold" href="">View all posts</a>
      </div>
    </div>
    
  </div>
</template>

<script>
import InfoComponent from '../components/InfoComponent.vue';
import AboutMeComponents from '../components/AboutMeComponents.vue'
import VideoComponent from '../components/VideoComponent.vue'
import LatestCourses from '../components/LatestCourses.vue'
import BookStoreComponent from '../components/BookStoreComponent.vue';
import ClientLogComponent from '../components/ClientLogComponent.vue'
import RealStoriesComponent from '../components/RealStoriesComponent.vue';
import BlogComponents from '../components/BlogComponents.vue';
import { infos } from '../data/store';
import { courses } from '../data/store';
import { clientLog } from '../data/store';
import { blog } from '../data/store';

export default {
  name: 'MainComponent',
  components: {
       InfoComponent,
       AboutMeComponents,
       VideoComponent,
       LatestCourses,
       BookStoreComponent,
       ClientLogComponent,
       RealStoriesComponent,
       BlogComponents,
  },
  data () {
    

    return {
      infos,
      courses,
      clientLog,
      blog,
    }
  }
}
</script>

<style lang="scss" scoped>
 .marg {
  margin-top: 170px;
 }
 .marg2 {
  margin-top: 80px;
 }

 p {
  text-transform: uppercase;
 }

 span {
  color:  #20ad96;
 }
 button {
    background-color: #20ad96;
    padding: 13px 100px;
  }
  .back {
    background-image: url('../assets/icon/background-pattern-wavify.png');
    background-color: #f5f1ed;
  }
  h6 {
    text-transform: uppercase;
  }

  a {
    color:  #20ad96;
    text-decoration: none;
    border-bottom: 2px solid  #20ad96 ;
    text-transform: uppercase;
    font-size: 14px;
    padding-bottom: 3px;
  }
</style>