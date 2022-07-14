<template>
    <nav class="navbar-bar navbar navbar-expand navbar-light bg-light">
      <div class="container-fluid">
        <!-- Logo -->
        <a class="navbar-brand" href="#">HiCT</a>

        <div id="navbarSupportedContent" class="collapse navbar-collapse">
          <ul class="navbar-nav me-auto mb-2 mb-lg-0">
            <!-- File -->
            <li class="nav-item dropdown">
              <a class="nav-link active dropdown-toggle" data-bs-toggle="dropdown" href="#">File</a>
              <ul class="dropdown-menu">
                <li><a class="dropdown-item" href="#">Open...</a></li>
                <li><a class="dropdown-item" href="#">Save as...</a></li>
                <li><a class="dropdown-item" href="#">Close</a></li>
              </ul>
            </li>
            <!-- View -->
            <li class="nav-item dropdown">
              <a class="nav-link active dropdown-toggle" data-bs-toggle="dropdown" href="#">View</a>
              <ul class="dropdown-menu">
                <li><a class="dropdown-item" href="#">Choose color scheme</a></li>
                <li><a class="dropdown-item" href="#">Show borders</a></li>
                <li><a class="dropdown-item" href="#">Something else</a></li>
              </ul>
            </li>
            <!-- Bookmarks -->
            <li class="nav-item">
              <a aria-current="page" class="nav-link active" href="#">Bookmarks</a>
            </li>
            <!-- Assembly -->
            <li class="nav-item dropdown">
              <a class="nav-link active dropdown-toggle" data-bs-toggle="dropdown" href="#">Assembly</a>
              <ul class="dropdown-menu">
                <li><a class="dropdown-item" href="#">Link FASTA</a></li>
                <li><a class="dropdown-item" href="#">Export assembly</a></li>
                <li><a class="dropdown-item" href="#">Export FASTA for selection</a></li>
              </ul>
            </li>
            <!-- Dev -->
            <li class="nav-item">
              <a aria-current="page" class="nav-link active" href="#">Dev</a>
            </li>
            <!-- Connection settings -->
            <li class="nav-item">
              <a aria-current="page" class="nav-link active" href="#">Connection Settings</a>
            </li>
            <!-- Report a bug -->
            <li class="nav-item">
              <a aria-current="page" class="nav-link active" href="#">Report a bug</a>
            </li>
          </ul>
        </div>
      </div>
    </nav>
</template>

<script>
export default {
  name: "NavigationBar"
}
</script>

<style scoped>
.navbar-bar {
  /* Navbar */

  /* Auto layout */
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  padding: 8px 16px;

  width: 1440px;
  height: 56px;

  /* Global/07. Light */
  background: #F8F9FA;

  /* Shadows/02. Regular */
  box-shadow: 0px 8px 16px rgba(0, 0, 0, 0.15);

  /* Inside auto layout */
  flex: none;
  order: 0;
  flex-grow: 0;
}
</style>