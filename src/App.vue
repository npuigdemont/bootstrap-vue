<template>
  <div id="app">
    <b-navbar toggleable="md" type="dark" variant="info">

     <b-container>
       <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
       <b-navbar-brand href="#">BootstrapVue</b-navbar-brand>

        <b-collapse id="nav-collapse" is-nav>
           <b-navbar-nav>
              <b-nav-item :to="{name: 'home'}" exact>Home</b-nav-item>
                <b-nav-item :to="{name: 'about'}">About</b-nav-item>
                <b-nav-item :to="{name: 'Grid'}">Grid</b-nav-item>
                <b-nav-item :to="{name: 'Cards'}">Cards</b-nav-item>
                <b-nav-item :to="{name: 'Form'}">Form</b-nav-item>
                <b-nav-item :to="{name: 'Axios'}">Axios</b-nav-item>
                <b-nav-item :to="{name: 'Jobs'}">JsonServer</b-nav-item>
          </b-navbar-nav>
        </b-collapse>


    <b-nav-form>
      <b-form-input class="mr-sm-2" placeholder="Put your Search"></b-form-input>
      <b-button variant="outline-success" class="my-2 my-sm-0" type="submit">Search</b-button>
    </b-nav-form>
  

         <b-nav-item-dropdown text="Lang" right>
          <b-dropdown-item href="#">EN</b-dropdown-item>
          <b-dropdown-item href="#">ES</b-dropdown-item>
          <b-dropdown-item href="#">CAT</b-dropdown-item>
          <b-dropdown-item href="#">FR</b-dropdown-item>
        </b-nav-item-dropdown>

     </b-container>
     </b-navbar>


     <b-container>
        <router-view/>
     </b-container>
    
  </div>
</template>



