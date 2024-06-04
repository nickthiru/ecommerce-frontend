<script>
  import {Route, Router, Link} from "svelte-routing";
  import "@picocss/pico";

  import NavBar from "./lib/common/NavBar.svelte";
  import HomePage from "./lib/page/HomePage.svelte";
  import SignUpPage from "./lib/page/SignUpPage.svelte";
  import SignInPage from "./lib/page/SignInPage.svelte";
  import VerifyOtpPage from "./lib/page/VerifyOtpPage.svelte";
</script>

<Router>
  <NavBar />

  <main class="container">
    <Route path={"/"} component={HomePage} />
    <Route path={"/sign-up"} component={SignUpPage} />  
    <Route path={"/verify-otp"} component={VerifyOtpPage} />
    <Route path={"/sign-in"} component={SignInPage} />
  </main>

</Router>

