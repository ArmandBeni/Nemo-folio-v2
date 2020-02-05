<template>
  <div class="container">
    <div class="bg-white">
      <Card :is-featured="true" :title="projectFeatured.title" :subtitle="projectFeatured.subtitle" :excerpt="projectFeatured.excerpt" :link="projectFeatured.link" :thumbnail="projectFeatured.thumbnail"/>
    </div>

    <div class="all-cards">
      <Card v-for="post in otherProjects" :key="post.id" :title="post.title" :subtitle="post.subtitle" :excerpt="post.excerpt" :link="post.link" :thumbnail="post.thumbnail" />
    </div>

    <div class="other">
      <Other :otherWorks="otherWorks"/>
    </div>

  </div>
</template>

<script>
import Card from '../components/Card.vue'
import Other from '../components/Other.vue'

export default {
  components: {
    Card,
    Other
  },
  data () {
    return {
      projectFeatured:
        {
          title: 'Côté Nature - POS tool',
          subtitle: 'UX/UI Design - 2019',
          excerpt: "Internal POS tool which aims to allow Côté Nature's employees to create in store displays of various formats with the new graphical identity, by themselves.",
          link: 'See more',
          thumbnail: '/images/coteNature.png'
        },
      otherProjects: [
        {
          title: 'Wastic - datajournalism',
          subtitle: 'UX/UI Design - 2019',
          excerpt: "Internal POS tool which aims to allows Côté Nature’s employees to create in store displays of various formats with the new graphical identity, by themselves.",
          link: 'See more',
          thumbnail: '/images/wastic.png'
        },
        {
          title: 'Wastic - datajournalism',
          subtitle: 'UX/UI Design - 2019',
          excerpt: "Internal POS tool which aims to allows Côté Nature’s employees to create in store displays of various formats with the new graphical identity, by themselves.",
          link: 'See more',
          thumbnail: '/images/wastic.png'
        },
        {
          title: 'Wastic - datajournalism',
          subtitle: 'UX/UI Design - 2019',
          excerpt: "Internal POS tool which aims to allows Côté Nature’s employees to create in store displays of various formats with the new graphical identity, by themselves.",
          link: 'See more',
          thumbnail: '/images/wastic.png'
        },
        {
          title: 'Wastic - datajournalism',
          subtitle: 'UX/UI Design - 2019',
          excerpt: "Internal POS tool which aims to allows Côté Nature’s employees to create in store displays of various formats with the new graphical identity, by themselves.",
          link: 'See more',
          thumbnail: '/images/wastic.png'
        },
        {
          title: 'Wastic - datajournalism',
          subtitle: 'UX/UI Design - 2019',
          excerpt: "Internal POS tool which aims to allows Côté Nature’s employees to create in store displays of various formats with the new graphical identity, by themselves.",
          link: 'See more',
          thumbnail: '/images/wastic.png'
        },
        {
          title: 'Wastic - datajournalism',
          subtitle: 'UX/UI Design - 2019',
          excerpt: "Internal POS tool which aims to allows Côté Nature’s employees to create in store displays of various formats with the new graphical identity, by themselves.",
          link: 'See more',
          thumbnail: '/images/wastic.png'
        },
        {
          title: 'Wastic - datajournalism',
          subtitle: 'UX/UI Design - 2019',
          excerpt: "Internal POS tool which aims to allows Côté Nature’s employees to create in store displays of various formats with the new graphical identity, by themselves.",
          link: 'See more',
          thumbnail: '/images/wastic.png'
        },
      ],
      otherWorks:[
        {
          img: '/images/thumbnail1.png',
          alt: ''
        },
        {
          img: '/images/thumbnail2.png',
          alt: ''
        },
        {
          img: '/images/thumbnail3.png',
          alt: ''
        },
        {
          img: '/images/thumbnail4.png',
          alt: ''
        },
        {
          img: '/images/thumbnail5.png',
          alt: ''
        },
        {
          img: '/images/thumbnail6.png',
          alt: ''
        },
      ]
    }
  }
}
</script>

<style lang="scss" scoped>

.container{
  background-color: white;
  color: black;
  margin: 0 auto;
  display: flex;
  flex-direction: column;

  .bg-white{
    background-color: #f6f6f6;
  }
}


</style>