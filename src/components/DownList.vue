<script>
export default {
  name: 'DownList',
  data() {
    return {
      // Oggetto per la sezione DC Comics
      listcontent: [
        {
          nome: 'Characters',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Comics',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Movies',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Tv',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Games',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Videos',
          link: '#',
          target: '_self',
        },
        {
          nome: 'News',
          link: '#',
          target: '_self',
        },
      ],

      // Oggetto per la sezione Shop
      listshop: [
        {
          nome: 'Shop DC',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Shop DC Collectibles',
          link: '#',
          target: '_self',
        },
      ],
      // Oggetto per la sezione DC
      listinfo: [
        {
          nome: 'Terms Of Use',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Privacy policy (New)',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Ad Choices',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Advertising',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Jobs',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Subscriptions',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Talent Workshops',
          link: '#',
          target: '_self',
        },
        {
          nome: 'CPSC Certificates',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Ratings',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Shop Help',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Contact Us',
          link: '#',
          target: '_self',
        },
      ],
      // Oggetto per la sezione Sites
      listsites: [
        {
          nome: 'DC',
          link: '#',
          target: '_self',
        },
        {
          nome: 'MAD Magazine',
          link: '#',
          target: '_self',
        },
        {
          nome: 'DC Kids',
          link: '#',
          target: '_self',
        },
        {
          nome: 'DC Universe',
          link: '#',
          target: '_self',
        },
        {
          nome: 'DC Power Visa',
          link: '#',
          target: '_self',
        },
      ],
    };
  },
};
</script>

<template>
  <div class="list-container">
    <div class="list-col">
      <!-- Sezione Comics -->
      <h3>Dc Comics</h3>
      <ul class="list-link">
        <li v-for="li in listcontent" class="down-link">{{ li.nome }}</li>
      </ul>

      <!-- Sezione Shop -->
      <h3>Shop</h3>
      <ul class="list-link">
        <li v-for="li in listshop" class="down-link">{{ li.nome }}</li>
      </ul>
    </div>
    <div class="list-col">
      <!-- Sezione Dc -->
      <h3>Dc</h3>
      <ul class="list-link">
        <li v-for="li in listinfo" class="down-link">{{ li.nome }}</li>
      </ul>
    </div>
    <div class="list-col">
      <!-- Sezione Sites -->
      <h3>Sites</h3>
      <ul class="list-link">
        <li v-for="li in listsites" class="down-link">{{ li.nome }}</li>
      </ul>
    </div>
  </div>
</template>

<style scoped lang="scss">
.list-container {
  display: flex;

  .list-col {
    margin: 20px;
    text-align: start;

    h3 {
      text-transform: uppercase;
      font-weight: 600;
      color: white;
      margin: 5px 0;
    }

    ul {
      padding: 0px;
      line-height: 1.5;
      margin: 12px 0;

      li {
        color: gray;
        font-weight: 300;
      }
    }
  }
}
</style>
