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

      <md-app-drawer :md-active.sync="menuVisible">
        <md-toolbar class="md-transparent" md-elevation="3"
          >Menu</md-toolbar
        >

        <md-list>
          <md-list-item>
            <md-icon>send</md-icon>
            <span class="md-list-item-text">Acceuil</span>
          </md-list-item>

          <md-list-item>
            <md-icon>send</md-icon>
            <span class="md-list-item-text">Lycée</span>
          </md-list-item>

          <md-list-item>
            <md-icon>send</md-icon>
            <span class="md-list-item-text">Objectif BAC</span>
          </md-list-item>

          <md-list-item>
            <md-icon>send</md-icon>
            <span class="md-list-item-text">La Seconde</span>
          </md-list-item>

           <md-list-item>
            <md-icon>send</md-icon>
            <span class="md-list-item-text">Le BAC</span>
          </md-list-item>


 <md-list-item>
            <md-icon>send</md-icon>
            <span class="md-list-item-text">Les BTS</span>
          </md-list-item>


 <md-list-item>
            <md-icon>send</md-icon>
            <span class="md-list-item-text">La prepa PTSI PT</span>
          </md-list-item>

        </md-list>
      </md-app-drawer>

      <md-app-content>
        <p>
          En raison des mesures sanitaire due au COVID 19 le port du masque est obligatoire 
          dans l'enceinte de l'etablidement et ces abords
        </p>
        <p>
          Nous vous prions également de respecter au maximum la distanciation social ( 1m50 d'écart ) dans les salles de classes , couloir , et au refectoir
        </p>
        <p>
           <div>
    <div class="viewport">
      
      <md-toolbar :md-elevation="3">
        <span class="md-title">Contact</span>
      </md-toolbar>

      <md-list class="md-double-line">
        <span>Numéro de téléphone </span>

        <md-list-item>
          <md-icon class="md-primary">phone</md-icon>

          <div class="md-list-item-text">
            <span> 03 28 58 72 10</span>
            <span>Fixe</span>
          </div>

          <md-button class="md-icon-button md-list-action">
            <md-icon>sms</md-icon>
          </md-button>
        </md-list-item>
        

        <md-list-item >
         
          <md-icon class="md-primary">phone</md-icon>
          <div class="md-list-item-text">
            <span> 03 28 58 72 49</span>
            <span>Fax</span>
          </div>

           <md-button class="md-icon-button md-list-action">
            <md-icon>sms</md-icon>
          </md-button>
        </md-list-item>

        <md-list-item >
         
          <md-icon class="md-primary">phone</md-icon>
          <div class="md-list-item-text">
            <span> 03 28 58 72 41</span>
            <span>Intendance</span>
          </div>

          <md-button class="md-icon-button md-list-action">
            <md-icon>sms</md-icon>
          </md-button>
        </md-list-item>

        <md-divider></md-divider>
        <md-subheader>Email</md-subheader>

        <md-list-item>
          <md-icon class="md-primary">email</md-icon>

          <div class="md-list-item-text">
            <span>vie-scolaire1.0590072h@ac-lille.fr</span>
            <span>Intendance</span>
          </div>
        </md-list-item>
      </md-list>

       <md-divider></md-divider>
        <md-subheader>Adresse</md-subheader>

        <md-list-item>
          <md-icon class="md-primary">room</md-icon>

          <div class="md-list-item-text">
            <span><p>809 rue du Banc Vert</p>
                  <p>BP 58<p/>
                  <p> 59944 Dunkerque Cedex 2</p></span>
          </div>
        </md-list-item>
      </md-list>

      
    </div>
    </span>
    </div>


          </p>


        
      <p>
        <img src="https://www.justacote.com/photos_entreprises/lycee-de-l-europe-dunkerque-1321748968.jpg" alt="Avatar">
      </p>
      </md-app-content>
    </md-app>
  </div>
  
</template>


<style lang="scss" scoped>
.md-app {
  max-height: 800px;
  border: 1px solid rgba(#000, 0.14);
}

.md-app-toolbar {
  height: 196px;
}

// Demo purposes only
.md-drawer {
  width: 230px;
  max-width: calc(100vw - 125px);
}
.viewport {
  width: 420px;
  max-width: 100%;
  display: inline-block;
  vertical-align: top;
  overflow: auto;
  border: 1px solid rgba(#000, 0.12);
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
