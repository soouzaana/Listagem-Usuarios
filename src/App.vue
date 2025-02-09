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
                data-bs-placement="left"
                aria-expanded="false"
              >
                <img src="./assets/navbar/Notificacao-Off.svg" alt="" />
              </a>
              <ul class="dropdown-menu notify">
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
          <button
            type="button"
            class="btn add-button"
            data-bs-toggle="modal"
            data-bs-target="#cadastrar-usuario"
          >
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
          <div class="user-modal">
            <div
              class="modal fade"
              id="cadastrar-usuario"
              tabindex="-1"
              aria-labelledby="cadastrar-usuario__label"
              aria-hidden="true"
            >
              <div
                class="modal-dialog modal-dialog-centered modal-dialog-scrollable"
              >
                <div class="modal-content">
                  <div class="modal-header">
                    <h1 class="modal-title" id="cadastrar-usuario__label">
                      Cadastrar Usuarios
                    </h1>
                    <button
                      type="button"
                      class="btn-close"
                      data-bs-dismiss="modal"
                      aria-label="Close"
                    ></button>
                  </div>
                  <div class="modal-body">
                    <!-- CORPO DO MODAL -->
                    <div class="inputs">
                      <!--input de imagem início-->
                      <label
                        class="picture d-flex align-items-center justify-content-center"
                        for="picture_input"
                        tabindex="0"
                      >
                        <input
                          type="file"
                          accept="image/*"
                          id="picture_input"
                          class="d-none"
                        />
                        <img
                          src="./assets/main/Imagem-Nova.svg"
                          alt="imagemNova"
                        />
                        <span class="picure_image"
                          >Arraste e solte uma imagem ou escolha uma de até 500
                          KB .jpeg ou .png.</span
                        >
                      </label>
                      <!--input de imagem final-->

                      <!-- inputs de form inicio -->
                      <div class="inserir">
                        <input
                          type="text"
                          id="input-name"
                          placeholder="Digite aqui"
                          required
                        />
                        <label for="input-name" class="label">Nome</label>
                      </div>

                      <div class="inserir">
                        <input
                          type="email"
                          id="input-email"
                          placeholder="Digite aqui"
                          required
                        />
                        <label for="input-name" class="label">Email</label>
                      </div>

                      <div class="inserir">
                        <input
                          type="number"
                          id="input-matricula"
                          placeholder="Digite aqui"
                          required
                        />
                        <label for="input-name" class="label">Matricula</label>
                      </div>
                    </div>

                    <div class="novoVinculo-add" onclick="addVinculo()">
                      <span>Novo Vínculo</span>
                    </div>

                    <!-- 
                    <div class="form-floating">
                      <select
                        class="form-select"
                        id="floatingSelect"
                        aria-label="Floating label select example"
                      >
                        <option selected>Open this select menu</option>
                        <option value="1">One</option>
                        <option value="2">Two</option>
                        <option value="3">Three</option>
                      </select>
                      <label for="floatingSelect">Works with selects</label>
                    </div> -->

                    <!-- inputs de form final -->
                  </div>
                  <div class="modal-footer">
                    <button type="button" class="btn" data-bs-dismiss="modal">
                      Cancelar
                    </button>
                    <button type="button" class="btn">Cadastrar</button>
                  </div>
                </div>
              </div>
            </div>
          </div>
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
              <div class="group d-flex justify-content-between">
                <h5 class="card-title">Nome</h5>
                <a href="#">
                  <img src="./assets/main/Editar.svg" alt="" />
                </a>
              </div>
              <p class="card-text">funções</p>
            </div>
          </div>
        </div>
        <!-- cards de usuarios final -->
      </div>
    </main>

    <!-- FOOTER -->
    <footer
      class="theme-grey text-dark d-flex align-items-center justify-content-center"
    >
      <div class="d-flex justify-content-between">
        <div class="date">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            width="10"
            height="10"
            fill="currentColor"
            class="bi bi-c-circle"
            viewBox="0 0 16 16"
          >
            <path
              d="M1 8a7 7 0 1 0 14 0A7 7 0 0 0 1 8m15 0A8 8 0 1 1 0 8a8 8 0 0 1 16 0M8.146 4.992c-1.212 0-1.927.92-1.927 2.502v1.06c0 1.571.703 2.462 1.927 2.462.979 0 1.641-.586 1.729-1.418h1.295v.093c-.1 1.448-1.354 2.467-3.03 2.467-2.091 0-3.269-1.336-3.269-3.603V7.482c0-2.261 1.201-3.638 3.27-3.638 1.681 0 2.935 1.054 3.029 2.572v.088H9.875c-.088-.879-.768-1.512-1.729-1.512"
            />
          </svg>
          2022 - {{ new Date().getFullYear() }} <b>Ladesa</b>
        </div>
      </div>
    </footer>
  </div>
</template>

<style scoped>
* {
  font-family: "Poppins", sans-serif;
}
/* NAVBAR */
.navbar {
  background-color: #fff;
  z-index: 4;
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

.notify {
  border: 1.5px solid #1bba47;
  font-size: 14px;
  padding: 0.1rem;
  transform: translateX(-10rem);
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
  z-index: 3;
}

#sidebar:hover {
  width: 12rem;
}

#sidebar-content {
  margin-top: 5rem;
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

.card-title {
  font-size: 14px;
  font-weight: 600;
}

.card-img-top img {
  height: 1rem;
}

.card-body {
  margin-top: 0.5rem;
  padding: 0.5rem;
}

.group img {
  width: 0.8rem;
}

.card-text {
  color: #9f9f9f;
  font-size: 11px;
  font-weight: 500;
}

/* MODAL */
.modal-content {
  border: 1.5px solid #9f9f9f;
  padding: 0.8rem;
}

.modal-title {
  font-size: 1.4rem;
  font-weight: 600;
}

.modal-content {
  margin: 0.5rem;
  gap: 1.5rem;
}

.picture {
  aspect-ratio: 16/9;
  border: 1.7px solid #9f9f9f;
  border-radius: 0.5rem;
  color: #9f9f9f;
  cursor: pointer;
  flex-direction: column;
  font-size: 1rem;
  font-weight: 500;
  max-height: 25vh;
  min-width: 67vh;
  line-height: 1.2rem;
  margin-bottom: 1rem;
  padding: 2rem;
  text-align: center;
}

.picture img {
  margin-bottom: 1.5rem;
}

.picture:hover {
  background-color: #eaeaea;
  color: black;
}

.picture:hover img {
  filter: brightness(0) saturate(100%) invert(0%) sepia(100%) saturate(2000%)
    hue-rotate(90deg) brightness(90%);
}
.inputs {
  flex-wrap: wrap;
}

.inputs input {
  width: 100%;
}

.inserir {
  height: 10%;
  position: relative;
  border-radius: 8px;
  margin-bottom: 20px;
  cursor: pointer;
}

.inserir input {
  height: 100%;
  background: transparent;
  border-radius: 8px;
  border: 1.7px solid #9f9f9f;
  outline: none;
  padding: 12px;
  font-size: 12px;
  font-weight: 600;
  color: #afafaf;
  padding-left: 15px;
}

.inserir input:active,
.inserir input:focus {
  border-color: #1bba47;
}

.inserir label {
  position: absolute;
  top: -8px;
  left: 15px;
  text-transform: capitalize;
  font-size: 12px;
  background-color: #fff;
  color: #9f9f9f;
  padding: 0 5px;
  font-weight: 600;
}

.inserir input:focus + .label,
.inserir input:active + .label {
  color: #1bba47;
}

.novoVinculo-add {
  border: 3px dotted #9f9f9f;
  border-radius: 0.5rem;
  cursor: pointer;
  padding: 1rem;
  text-align: center;
  font-size: 14px;
}

.novoVinculo-add:hover {
  background-color: #39a04820;
}

/* FOOTER */
footer {
  border-top: #9f9f9f50 solid 1px;
  bottom: 0;
  font-size: 14px;
  height: 3rem;
  padding: 1rem 5rem;
  position: fixed;
  width: 100%;
  z-index: 1;
}

.theme-grey {
  background-color: #9f9f9f20;
}

.links {
  margin-left: 2rem;
  text-decoration: none;
}
</style>

<!-- .inputs {
  flex-wrap: wrap;
}

.inputs input {
  width: 100%;
}

.inserir {
  height: 10%;
  position: relative;
  border-radius: 8px;
  margin-bottom: 20px;
  cursor: pointer;
}

.inserir input {
  height: 100%;
  background: transparent;
  border-radius: 8px;
  border: 1.7px solid #9f9f9f;
  outline: none;
  padding: 12px;
  font-size: 12px;
  font-weight: 600;
  color: #afafaf;
  padding-left: 15px;
}

.inserir input:active,
.inserir input:focus {
  border-color: #1bba47;
}

.inserir label {
  position: absolute;
  top: -8px;
  left: 15px;
  text-transform: capitalize;
  font-size: 12px;
  background-color: #fff;
  color: #9f9f9f;
  padding: 0 5px;
  font-weight: 600;
}

.inserir input:focus + .label,
.inserir input:active + .label {
  color: #1bba47;
}

.botoes {
  display: flex;
  justify-content: space-between;
  text-align: center;
  width: 100%;
}

.botoes button {
  background-color: transparent;
  font-size: 14px;
  border-radius: 8px;
  padding: 5px 20px;
  cursor: pointer;
  display: flex;
  align-items: center;
  justify-content: center;
}

.botoes img {
  margin-left: 5px;
  height: 18px;
  width: 18px;
  vertical-align: middle;
}

.icones img {
  position: absolute;
  right: 0;
  width: 15px;
  cursor: pointer;
  border: none;
  background-color: transparent;
}

.close {
  border: 1.7px solid black;
}

.concluir {
  border: 1.7px solid #1bba47;
  color: #1bba47;
  font-weight: 600;
}

.concluir img {
  filter: brightness(0) saturate(100%) invert(40%) sepia(100%) saturate(2000%) hue-rotate(90deg) brightness(90%);
} -->
