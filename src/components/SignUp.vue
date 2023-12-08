<script>
export default {
  name: 'SignUp',
  data() {
    return {
      socialIcons: [
        {
          img: '../../public/img/footer-facebook.png',
          link: '#',
        },
        {
          img: '../../public/img/footer-twitter.png',
          link: '#',
        },
        {
          img: '../../public/img/footer-youtube.png',
          link: '#',
        },
        {
          img: '../../public/img/footer-pinterest.png',
          link: '#',
        },
        {
          img: '../../public/img/footer-periscope.png',
          link: '#',
        },
      ],
    };
  },
};
</script>

<template>
  <div class="social-sign-container">
    <button class="sign-btn">Sign-Up Now!</button>
    <div class="social">
      <h3>Follow Us</h3>
      <a v-for="icon in socialIcons" :key="icon.img" :href="icon.link">
        <img :src="icon.img" alt="Social Icon" />
      </a>
    </div>
  </div>
</template>

<style scoped lang="scss">
@use '../styles/partials/variables.scss' as *;

// Main container

.social-sign-container {
  display: flex;
  justify-content: space-between;
  padding: 20px 300px;
  background-color: $tertiary;
}

// Button
.sign-btn {
  color: white;
  font-size: 12px;
  background: $tertiary;
  padding: 10px 10px;
  border: solid $primary 3px;
  text-transform: uppercase;
  font-weight: 500;
  transition: all 0.2s;
}

.sign-btn:hover {
  background: $primary;
  text-decoration: none;
  color: $tertiary;
  font-weight: 600;
}

// Sezione Follow

.social {
  display: flex;
  margin: 0 10px;
  align-items: center;

  h3 {
    text-transform: uppercase;
    font-weight: 600;
    color: $primary;
    margin: 0 10px;
    font-size: 15px;
    transition: all 0.2s;

    &:hover {
      color: white;
      cursor: pointer;
    }
  }
  a {
    margin: 0 7px;
    img {
      width: 30px;
      transition: all 0.2s;

      &:hover {
        filter: brightness(1.8);
      }
    }
  }
}
</style>
