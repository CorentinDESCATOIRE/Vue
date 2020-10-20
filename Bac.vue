<template>
  <div class="page-container">
    <md-app md-waterfall md-mode="flexible">
      <md-app-toolbar class="md-large md-primary">
        <div class="md-toolbar-row">
          <div class="md-toolbar-section-start">
            <md-button
              class="md-icon-button"
              @click="menuVisible = !menuVisible"
            >
              <md-icon>menu</md-icon>
            </md-button>
          </div>

          <div class="md-toolbar-section-end">
            <md-button class="md-icon-button">
              <md-icon>more_vert</md-icon>
            </md-button>
          </div>
        </div>

        <div class="md-toolbar-row md-toolbar-offset">
          <span class="md-display-1">Le Lycée de l'Europe</span>
        </div>
      </md-app-toolbar>

      <md-app-drawer :md-activevbind="menuVisible">
        <md-toolbar class="md-transparent" md-elevation="3"
          >Menu</md-toolbar>

        <md-list>
          <md-list-item>
            <md-icon>send</md-icon>
            <md-button>acceuil</md-button>
          </md-list-item>

          <md-list-item>
            <md-icon>send</md-icon>
            <md-button>Le lycée</md-button>
          </md-list-item>

          <md-list-item>
            <md-icon>send</md-icon>
            <md-button>Objectif BAC</md-button>
          </md-list-item>

          <md-list-item>
            <md-icon>send</md-icon>
            <md-button>La Seconde</md-button>
          </md-list-item>

           <md-list-item>
            <md-icon>send</md-icon>
            <md-button>Le BAC</md-button>
          </md-list-item>


 <md-list-item>
            <md-icon>send</md-icon>
            <md-button>Les BTS</md-button>
          </md-list-item>


 <md-list-item>
            <md-icon>send</md-icon>
            <md-button>La Prepa PTSI PT</md-button>
          </md-list-item>

        </md-list>
      </md-app-drawer>

      <md-app-content>
        <p>
       <h1> La reforme du Baccalauréa </h1>
      </p>
    <p>
        <iframe width="560" height="315" src="https://www.youtube.com/embed/TNzvEbJdNPY" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </p> 
     <p>
               <div class="viewport2">
      <md-toolbar :md-elevation="1">
      </md-toolbar>
               </div>
        </p>
    <p>
       <iframe width="560" height="315" src="https://www.youtube.com/embed/SaF71ZadHGg" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
      </p>
      <p>
        Diaporama et Plaquette
      </p>
     <p> 
       
      <a href="https://view.genial.ly/5c0637826f191d2ca33a5640/interactive-content-1"> <img alt="" align="center" src="https://www.lycee-europe-dunkerque.fr/userfiles/images/rentree_2019/visu_diapo_2019.jpg"  width="200" height="200" /> </a>
       
      <a href="https://drive.google.com/file/d/1MhvRlbdAM-jkkF9nGZ-R-zJLUeh7xrwZ/view"> <img alt="" align="center" src="https://www.lycee-europe-dunkerque.fr/userfiles/images/rentree_2019/visu_plaq_SG_01.png"  width="150" height="100" /> </a>
     
     </p>  
      
      </md-app-content>
    </md-app>
  </div>
  
</template>


<style lang="scss" scoped>
.md-app {
  max-height: 2800px;
  border: 1px solid rgba(#000, 0.14);
}

.viewport2 {
  width: 800px;
  height: 4px;
  max-width: 100%;
  display: inline-block;
  vertical-align: top;
  overflow: auto;
  border: 2px solid rgba(#000, 0.5);
}
</style>

<script>
export default {
  name: "Flexible",
  data: () => ({
    menuVisible: false,
  }),
};
</script>