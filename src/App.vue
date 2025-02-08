<script setup></script>

<template>
  <div>
    <!-- NAVBAR -->
    <nav class="navbar navbar-expand-lg border-bottom">
      <div class="container-fluid">
        <!-- avatar -->
        <div class="container avatar rounded w-auto">
          <div class="row d-flex align-items-center justify-content-center">
            <div class="image col-6">
              <img
                id="userAvatar"
                src="./assets/navbar/ImagemPerfilFoto.svg"
                alt=""
              />
            </div>

            <!-- avatar-dropdown -->
            <div class="info dropdown text-nowrap col-6">
              <p class="name fw-bold">Administrador</p>
              <button
                class="btn dropdown-toggle"
                type="button"
                data-bs-toggle="dropdown"
                aria-expanded="false"
              >
                professor, dape
              </button>
              <ul class="dropdown-menu">
                <li>
                  <a class="dropdown-item" href="#">
                    <!-- modal professor -->
                  </a>
                </li>
                <li>
                  <a class="dropdown-item" href="#">
                    <!-- modal dape -->
                  </a>
                </li>
              </ul>
            </div>
          </div>
        </div>

        <!-- menu -->
        <div class="collapse navbar-collapse" id="navbarNavDropdown">
          <ul class="navbar-nav ms-auto">
            <li class="nav-item">
              <a class="nav-link" href="#">
                <img src="./assets/navbar/Property 1=Sun.svg" alt="" />
              </a>
            </li>

            <li class="nav-item dropdown">
              <a
                class="nav-link"
                href="#"
                role="button"
                data-bs-toggle="dropdown"
                aria-expanded="false"
              >
                <img src="./assets/navbar/Notificacao-Off.svg" alt="" />
              </a>
              <ul class="dropdown-menu">
                <li>
                  <a class="dropdown-item border-bottom" href="#"
                    >Novo evento gerado.</a
                  >
                </li>
                <li>
                  <a class="dropdown-item border-bottom" href="#"
                    >O evento IFRO Party foi agendado.</a
                  >
                </li>
                <li>
                  <a class="dropdown-item" href="#"
                    >Novo calendário cadastrado.</a
                  >
                </li>
              </ul>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">
                <img src="./assets/navbar/sisgha-logo.svg" alt="" />
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
              <img class="icone" src="./assets/sidebar/Home.svg" alt="Inicio" />
              <span class="item-description">Início</span>
            </a>
          </li>
          <li class="side-item">
            <a href="#">
              <img
                class="icone"
                src="./assets/sidebar/Usuarios.svg"
                alt="usuario"
              />
              <span class="item-description">Turmas</span>
            </a>
          </li>
          <li class="side-item">
            <a href="#">
              <img
                class="icone"
                src="./assets/sidebar/Disciplina.svg"
                alt="discplinas"
              />
              <span class="item-description">Disciplinas</span>
            </a>
          </li>
          <li class="side-item">
            <a href="#">
              <img
                class="icone"
                src="./assets/sidebar/Diario.svg"
                alt="calendario"
              />
              <span class="item-description">Diário</span>
            </a>
          </li>
          <li class="side-item">
            <a href="#">
              <img
                class="icone"
                src="./assets/sidebar/Calendario.svg"
                alt="calendario"
              />
              <span class="item-description">Calendário</span>
            </a>
          </li>
          <li class="side-item">
            <a href="#">
              <img
                class="icone"
                src="./assets/sidebar/Outros-Itens.svg"
                alt="calendario"
              />
              <span class="item-description">Outros</span>
            </a>
          </li>
        </ul>
      </div>
      <div class="sidebar-content__bottom">
        <div id="configuracoes" class="side-item">
          <a href="#">
            <img
              class="icone"
              src="./assets/sidebar/Configuracoes.svg"
              alt="configuracoes"
            />
            <span class="item-description">Configurações</span>
          </a>
        </div>
        <div id="logout">
          <button id="logout-btn">
            <img class="icone" src="./assets/sidebar/Sair.svg" alt="sair" />
            <span class="item-description">Sair</span>
          </button>
        </div>
      </div>
    </nav>

    <!-- CONTENT -->
    <main>
      <div class="container">
        <div class="main-top">
          <!--Caixa de pesquisa começo-->
          <div class="form">
            <input
              type="text"
              placeholder="Digite aqui"
              id="input-id"
              required
            />
            <label for="input-id" class="label">Pesquisar</label>
            <button class="pesquisar">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                width="14"
                height="14"
                fill="currentColor"
                class="bi bi-search"
                viewBox="0 0 16 16"
              >
                <path
                  d="M11.742 10.344a6.5 6.5 0 1 0-1.397 1.398h-.001q.044.06.098.115l3.85 3.85a1 1 0 0 0 1.415-1.414l-3.85-3.85a1 1 0 0 0-.115-.1zM12 6.5a5.5 5.5 0 1 1-11 0 5.5 5.5 0 0 1 11 0"
                />
              </svg>
            </button>
          </div>
          <!--Caixa de pesquisa final-->

          <!-- botão de adicionar -->
          <button type="button" class="btn add-button">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              width="28"
              height="28"
              fill="currentColor"
              class="bi bi-plus-lg"
              viewBox="0 0 16 16"
            >
              <path
                fill-rule="evenodd"
                d="M8 2a.5.5 0 0 1 .5.5v5h5a.5.5 0 0 1 0 1h-5v5a.5.5 0 0 1-1 0v-5h-5a.5.5 0 0 1 0-1h5v-5A.5.5 0 0 1 8 2"
              />
            </svg>
          </button>

          <!-- modal de cadastrar usuario -->

          <!-- final do modal -->
          <!-- final do botao de adicionar -->
        </div>
        <!-- cards de usuarios inicio -->
        <div class="usuarios-card">
          <div class="card" style="width: 12rem; height: 15rem">
            <div
              class="user-image d-flex align-items-center justify-content-center"
            >
              <img
                src="./assets/main/Imagem.svg"
                class="d-block mx-auto img-fluid"
                alt="..."
              />
            </div>
            <div class="card-body">
              <h5 class="card-title">Nome do usuario</h5>
              <div class="group d-flex justify-content-between">
                <p class="card-text">funções</p>
                <a href="#" class="btn">
                  <img src="./assets/main/Editar.svg" alt="" />
                </a>
              </div>
            </div>
          </div>

          <div class="card" style="width: 12rem; height: 15rem">
            <div
              class="user-image d-flex align-items-center justify-content-center"
            >
              <img
                src="./assets/main/Imagem.svg"
                class="d-block mx-auto img-fluid"
                alt="..."
              />
            </div>
            <div class="card-body">
              <h5 class="card-title">Nome do usuario</h5>
              <div class="group d-flex justify-content-between">
                <p class="card-text">funções</p>
                <a href="#" class="btn">
                  <img src="./assets/main/Editar.svg" alt="" />
                </a>
              </div>
            </div>
          </div>

          <div class="card" style="width: 12rem; height: 15rem">
            <div
              class="user-image d-flex align-items-center justify-content-center"
            >
              <img
                src="./assets/main/Imagem.svg"
                class="d-block mx-auto img-fluid"
                alt="..."
              />
            </div>
            <div class="card-body">
              <h5 class="card-title">Nome do usuario</h5>
              <div class="group d-flex justify-content-between">
                <p class="card-text">funções</p>
                <a href="#" class="btn">
                  <img src="./assets/main/Editar.svg" alt="" />
                </a>
              </div>
            </div>
          </div>

          <div class="card" style="width: 12rem; height: 15rem">
            <div
              class="user-image d-flex align-items-center justify-content-center"
            >
              <img
                src="./assets/main/Imagem.svg"
                class="d-block mx-auto img-fluid"
                alt="..."
              />
            </div>
            <div class="card-body">
              <h5 class="card-title">Nome do usuario</h5>
              <div class="group d-flex justify-content-between">
                <p class="card-text">funções</p>
                <a href="#" class="btn">
                  <img src="./assets/main/Editar.svg" alt="" />
                </a>
              </div>
            </div>
          </div>

          <div class="card" style="width: 12rem; height: 15rem">
            <div
              class="user-image d-flex align-items-center justify-content-center"
            >
              <img
                src="./assets/main/Imagem.svg"
                class="d-block mx-auto img-fluid"
                alt="..."
              />
            </div>
            <div class="card-body">
              <h5 class="card-title">Nome do usuario</h5>
              <div class="group d-flex justify-content-between">
                <p class="card-text">funções</p>
                <a href="#" class="btn">
                  <img src="./assets/main/Editar.svg" alt="" />
                </a>
              </div>
            </div>
          </div>

          <div class="card" style="width: 12rem; height: 15rem">
            <div
              class="user-image d-flex align-items-center justify-content-center"
            >
              <img
                src="./assets/main/Imagem.svg"
                class="d-block mx-auto img-fluid"
                alt="..."
              />
            </div>
            <div class="card-body">
              <h5 class="card-title">Nome do usuario</h5>
              <div class="group d-flex justify-content-between">
                <p class="card-text">funções</p>
                <a href="#" class="btn">
                  <img src="./assets/main/Editar.svg" alt="" />
                </a>
              </div>
            </div>
          </div>

          <div class="card" style="width: 12rem; height: 15rem">
            <div
              class="user-image d-flex align-items-center justify-content-center"
            >
              <img
                src="./assets/main/Imagem.svg"
                class="d-block mx-auto img-fluid"
                alt="..."
              />
            </div>
            <div class="card-body">
              <h5 class="card-title">Nome do usuario</h5>
              <div class="group d-flex justify-content-between">
                <p class="card-text">funções</p>
                <a href="#" class="btn">
                  <img src="./assets/main/Editar.svg" alt="" />
                </a>
              </div>
            </div>
          </div>

          <div class="card" style="width: 12rem; height: 15rem">
            <div
              class="user-image d-flex align-items-center justify-content-center"
            >
              <img
                src="./assets/main/Imagem.svg"
                class="d-block mx-auto img-fluid"
                alt="..."
              />
            </div>
            <div class="card-body">
              <h5 class="card-title">Nome do usuario</h5>
              <div class="group d-flex justify-content-between">
                <p class="card-text">funções</p>
                <a href="#" class="btn">
                  <img src="./assets/main/Editar.svg" alt="" />
                </a>
              </div>
            </div>
          </div>
        </div>
        <!-- cards de usuarios final -->
      </div>
    </main>

    <!-- FOOTER -->
  </div>
</template>

<style scoped>
* {
  font-family: "Poppins", sans-serif;
}
/* NAVBAR */
.navbar {
  background-color: #fff;
  z-index: 100;
}

.container-fluid {
  display: flex;
}

.avatar {
  background-color: #2f9e411a;
  padding-left: 0;
}

.row {
  padding: 0.2rem 1rem 0.2rem 0;
}

.image {
  align-items: center;
  background-color: #9f9f9f33;
  border-radius: 50%;
  display: flex;
  justify-content: center;
  height: 3rem;
  width: 3rem;
}

.image img {
  height: 1rem;
}

.info {
  align-items: center;
  display: flex;
  flex-direction: column;
  justify-content: center;
  margin: 0 0 0 0.5rem;
}

.name {
  font-size: 14px;
  margin-bottom: 0;
}

.dropdown-toggle {
  font-size: 12px;
  margin-top: 0;
}

/* SIDEBAR */
#sidebar {
  background-color: #39a048;
  display: flex;
  flex-direction: column;
  font-size: 1rem;
  font-weight: 400;
  height: 100vh;
  justify-content: space-between;
  left: 0;
  min-width: 4rem;
  overflow: hidden;
  position: fixed;
  top: 0rem;
  transition: width 0.5s;
  width: 2rem;
}

#sidebar:hover {
  width: 12rem;
}

#sidebar-content {
  padding-top: 5rem;
}

#side_items {
  display: flex;
  flex-direction: column;
  flex-grow: 1;
  list-style: none;
  margin: 0.3rem;
  padding: 0;
}

.side-item {
  align-items: center;
  border-radius: 1rem;
  cursor: pointer;
  display: flex;
  height: 3rem;
  justify-content: center;
  margin-bottom: 0.5rem;
  padding: 0;
  transition: background-color 0.3s, transform 0.3s;
  width: auto;
}

.side-item:hover {
  background-color: #1bba47;
}

.side-item a {
  align-items: center;
  border-radius: 2rem;
  color: #fff;
  display: flex;
  height: 100%;
  padding: 1rem;
  text-decoration: none;
  width: 100%;
}

.side-item .icone {
  margin-right: 1rem;
}

.item-description {
  opacity: 0;
  transition: opacity 0.3s, visibility 0.3s, color 0.3s;
  visibility: hidden;
}

#sidebar:hover .item-description {
  opacity: 1;
  visibility: visible;
}
.sidebar:hover ~ .background .informacoes,
.sidebar.open ~ .background .informacoes {
  transform: translateX(20rem);
}

.sidebar-content__bottom {
  margin: 0.3rem;
}

#logout {
  border-top: 0.1rem solid #39a048;
}

#logout-btn {
  align-items: center;
  background-color: transparent;
  border: none;
  border-radius: 1rem;
  color: #fff;
  display: flex;
  font-size: 1rem;
  font-weight: 400;
  gap: 1rem;
  height: 100%;
  line-height: 1.5rem;
  padding: 0.5rem 1rem 0.5rem 0;
  text-align: start;
  transition: background-color 0.3s, transform 0.3s;
  width: 100%;
}

#logout-btn img {
  margin-left: 0.5rem;
}

#logout-btn:hover {
  background-color: #e9001c;
}
#sidebar:hover + main {
  padding-left: 15rem;
}

/* CONTENT */
main {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  margin-top: 2rem;
  transition: padding-left 0.5s;
}

.container {
  width: 62.3rem;
}

/* MAIN TOP */

.main-top {
  display: flex;
  justify-content: space-between;
}

.form {
  height: 3rem;
  width: 31rem;
  position: relative;
}

.form input {
  width: 100%;
  height: 100%;
  background: transparent;
  border-radius: 0.5rem;
  border: 1.5px solid #9f9f9f;
  outline: none;
  padding: 0 0.6rem;
  font-size: 0.75rem;
  padding-left: 1rem;
}

.form input:active,
.form input:focus {
  border-color: #1bba47;
}

.form label {
  position: absolute;
  left: 1rem;
  text-transform: capitalize;
  font-size: 0.75rem;
  background-color: #fff;
  color: #9f9f9f;
  padding: 0 0.6rem;
  font-weight: 600;
}

.form input {
  width: 100%;
  height: 100%;
  background: transparent;
  border-radius: 0.5rem;
  border: 1.5px solid #9f9f9f;
  outline: none;
  padding: 0 0.6rem;
  font-size: 0.75rem;
  padding-left: 1rem;
}

.form input:active,
.form input:focus {
  border-color: #1bba47;
}

.form label {
  position: absolute;
  top: -0.5rem;
  left: 1rem;
  text-transform: capitalize;
  font-size: 0.75rem;
  background-color: #fff;
  color: #9f9f9f;
  padding: 0 0.3rem;
  font-weight: 600;
}

.form input:focus + .label,
.form input:active + .label {
  color: #1bba47;
}

.pesquisar {
  position: absolute;
  top: 0;
  right: 0;
  height: 100%;
  width: 3.1rem;
  cursor: pointer;
  border: none;
  background-color: transparent;
}

.add-button {
  background-color: #39a048;
  color: #fff;
  padding: 0.3rem 0.5rem;
}

/* CARDS */

.usuarios-card {
  display: grid;
  gap: 1rem;
  grid-template-columns: repeat(4, 1fr);
  margin-top: 2rem;
}

.card {
  border: 1.5px solid #9f9f9f;
  border-radius: 0.5rem;
}

.user-image {
  background-color: #9f9f9f20;
  height: 40vh;
}

.card-img-top img {
  height: 1rem;
}

.card-body {
  margin-top: 0.5rem;
  padding: 0.5rem;
}
</style>
