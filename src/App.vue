<script setup>

</script>

<template>
  <div>
    <!-- NAVBAR --> 
    <nav class="navbar navbar-expand-lg border-bottom">
      <div class="container-fluid">

        <!-- avatar -->
        <div class="container avatar rounded w-auto ">
          <div class="row d-flex align-items-center justify-content-center">
            <div class="image col-6">
              <img id="userAvatar" src="./assets/navbar/ImagemPerfilFoto.svg" alt="">
            </div>            

            <!-- avatar-dropdown -->
            <div class="info dropdown text-nowrap col-6">                            
              <p class="name fw-bold">Administrador</p>
              <button class="btn dropdown-toggle" type="button" data-bs-toggle="dropdown" aria-expanded="false">
                professor, dape
              </button>
              <ul class="dropdown-menu">
                <li><a class="dropdown-item" href="#">
                  <!-- modal professor -->
                </a></li>
                <li><a class="dropdown-item" href="#">
                  <!-- modal dape -->
                </a></li>
              </ul>
            </div>
          </div>
        </div>   
        
        <!-- menu -->
        <div class="collapse navbar-collapse" id="navbarNavDropdown">
          <ul class="navbar-nav ms-auto">
            <li class="nav-item">
              <a class="nav-link" href="#">
                <img src="./assets/navbar/Property 1=Sun.svg" alt="">
              </a>
            </li>

            <li class="nav-item dropdown">
              <a class="nav-link" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                <img src="./assets/navbar/Notificacao-Off.svg" alt="">
              </a>
              <ul class="dropdown-menu">
                <li><a class="dropdown-item border-bottom" href="#">Novo evento gerado.</a></li>
                <li><a class="dropdown-item border-bottom" href="#">O evento IFRO Party foi agendado.</a></li>
                <li><a class="dropdown-item" href="#">Novo calendário cadastrado.</a></li>
              </ul>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">
                <img src="./assets/navbar/sisgha-logo.svg" alt="">
              </a>
            </li>        
          </ul>
        </div>
      </div>
    </nav>

    <!-- SIDEBAR -->
    <nav id="sidebar">
    <div id="sidebar-content">
      <ul id="side_items">
        <li class="side-item">
          <a href="#">
            <!-- <img class="icone" src="/assets/sidebar/Home.svg" alt="Inicio"> -->
            <span class="item-description">Início</span>
          </a>
        </li>
        <li class="side-item">
          <a href="#">
            <!-- <img class="icone" src="/assets/sidebar/Usuario.svg" alt="usuario"> -->
            <span class="item-description">Perfil</span>
          </a>
        </li>
        <li class="side-item">
          <a href="#">
            <!-- <img class="icone" src="/assets/sidebar/Calendario.svg" alt="calendario"> -->
            <span class="item-description">Calendário</span>
          </a>
        </li>
      </ul>
    </div>
    <div class="bottom">
      <div id="configuracoes" class="side-item">
        <a href="#">
          <!-- <img class="icone" src="/assets/sidebar/Configurações.svg" alt="configuracoes"> -->
          <span class="item-description">Configurações</span>
        </a>
      </div>
      <div id="logout">
        <button id="logout-btn">
          <!-- <img class="icone" src="/assets/sidebar/Sair.svg" alt="sair"> -->
          <span class="item-description">Sair</span>
        </button>
      </div>
    </div>
  </nav>  

    <!-- CONTENT -->

    <!-- FOOTER -->
  </div>
</template>

<style scoped>
*{
  font-family: 'Poppins', sans-serif;
}
/* NAVBAR */
.navbar{
  background-color: transparent;
}

.container-fluid{
  display: flex;
}

.avatar{
  background-color: #2F9E411A;
  padding-left: 0;
}

.row{
  padding: .2rem 1rem .2rem 0;
}

.image{
  align-items: center;
  background-color: #9F9F9F33; 
  border-radius: 50%;  
  display: flex ;
  justify-content: center;
  height: 3rem;
  width: 3rem;
}

.image img{
  height: 1rem;
}

.info{
  align-items: center;
  display: flex;
  flex-direction: column;
  justify-content: center;
  margin: 0 0 0 .5rem;
}

.name{
  font-size: 14px;
  margin-bottom: 0;
}

.dropdown-toggle{
  font-size: 12px;
  margin-top: 0;
}

/* SIDEBAR */
#sidebar {
  position: fixed;
  top: 0;
  left: 0;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  width: 5.7rem;
  height: 100vh;
  background-color: #39a048;
  padding: 1.5rem;
  font-size: 1.3rem;
  font-weight: 600;
  line-height: 1.95rem;
  transition: width 0.5s;
  min-width: 8.2rem;
  overflow: hidden;
  z-index: 1;
}

#sidebar:hover {
  width: 25.7rem;
}

#sidebar-content {
  padding-top: 7rem;
}

#side_items {
  display: flex;
  flex-direction: column;
  flex-grow: 1;
  list-style: none;
}

.side-item {
  padding: 0;
  cursor: pointer;
  border-radius: 1rem;
  transition: background-color 0.3s, transform 0.3s;
  display: flex;
  align-items: center;
  justify-content: center;
  width: 23.7rem;
  height: 4rem;
  margin-bottom: 1rem;
}

.side-item:hover {
  background-color: #1bba47;
}

.side-item a {
  text-decoration: none;
  display: flex;
  align-items: center;
  color: #fff;
  height: 100%;
  padding: 0 1rem;
  border-radius: 2rem;
  width: 100%;
}

.side-item img {
  margin-right: 1rem;
}

.item-description {
  opacity: 0;
  visibility: hidden;
  transition: opacity 0.3s, visibility 0.3s, color 0.3s;
}

#sidebar:hover .item-description {
  opacity: 1;
  visibility: visible;
}
.sidebar:hover ~ .background .informacoes,
.sidebar.open ~ .background .informacoes {
  transform: translateX(20rem);
}

#logout {
  border-top: .1rem solid #39a048;
}

#logout-btn {
  font-size: 1.3rem;
  font-weight: 600;
  line-height: 1.95rem;
  border: none;
  display: flex;
  gap: 1rem;
  align-items: center;
  border-radius: 1rem;
  text-align: start;
  cursor: pointer;
  background-color: transparent;
  color: #fff;
  padding: 0;
  transition: background-color 0.3s, transform 0.3s;
  width: 23.7rem;
  height: 4rem;
}

#logout-btn img {
  margin-left: .5rem;
}

#logout-btn:hover {
  background-color: #e9001c;
}
#sidebar:hover + main {
  padding-left: 25.7rem;
}
</style>