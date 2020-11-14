<template>
  <section>
    <div class="container full-height-screen flex flex-column flex-v-center flex-h-center">
      <div class="card border-shadow border-round">
        <img
          src="../assets/images/kidsloop_min_logo.svg"
          alt="kidsloop"
          class="card__logo"
        />
        <h1 class="no-bold">Sign In</h1>
        <form action="" class="card__form" role="login">
          <div class="card__form-item">
            <label for="email_or_name">
              <input 
                id="email_or_name"
                name="email_or_name"
                type="text"
                placeholder="Email or Phone *"
                autocomplete="email-or-name"
                aria-required="true"
              />
            </label>
          </div>
          <div class="card__form-item">
            <label for="password">
              <input
                id="password"
                name="password"
                type="password"
                placeholder="Password *"
                aria-required="true"
              />
            </label>
          </div>
          <div class="card__form-item flex flex-v-center flex-h-bet mb-30">
            <a href="#">Forgot Password?</a>
            <button
              type="submit"
              name="submit"
              class="btn btn--blue border-round"
            >
              Sign In
            </button>
          </div>
          <a href="#">Create an account</a>
        </form>
      </div>
      <div class="flex flex-h-bet full-width mt-20">
        <details class="language">
          <summary>
            <span>
              Select Language
            </span>
            <span></span>
          </summary>
          <ul class="mt-10 border-shadow" role="dropdown">
            <li>English</li>
            <li>Korean</li>
            <li>Spanish</li>
            <li>Italian</li>
          </ul>
        </details>
        <nav class="other-services" role="navigation">
          <a href="#" class="mr-20">Help</a>
          <a href="#" class="mr-20">Privacy</a>
          <a href="#">Terms</a>
        </nav>
      </div>
    </div>
  </section>
</template>
<style scoped>
.card {
  background: var(--white-color);
  padding: 2em;
  width: 100%;
}

.card > h1 {
  font-size: 2.4em;
  margin: 1em 0;
}

.card__logo {
  max-width: 80px;
  height: 80px;
  width: 100%;
}

.card__form {
  margin: 1em 0;
}

.card__form-item {
  margin: 0 0 15px;
}

.card__form-item > label {
  display: flex;
}

.card__form-item > label > input {
  border-radius: 12px;
  font-size: 1em;
  line-height: 25px;
  border: 1px solid #cacaca;
  padding: 10px 10px 10px 15px;
  width: 100%;
}

.card__form-item a,
form a {
  color: var(--navy-blue-color);
}

::placeholder {
  color: #787878;
}

.language *,
.other-services a {
  color: var(--black-color);
}

.language {
  font-size: 1.1em;
  max-width: 150px;
  width: 100%;
}

.language summary {
  list-style-type: none;
}

.language summary > span:first-child {
  border-bottom: 1.5px solid var(--black-color);
  line-height: 21px;
  padding: 1px 0;
}

.language summary,
.language ul > li {
  cursor: pointer;
}

.language ul {
  padding: 0px 10px;
}

.language ul > li {
  padding: 10px 0;
  border-bottom: 1px solid #cacaca;
  color: #787878;
  transition: font-size ease-in .2s;
}

.language ul > li:hover {
  transition: font-size ease-out .2s;
  font-size: 1.2em;
}

.language ul > li:last-child {
  border-bottom: none;
}

</style>