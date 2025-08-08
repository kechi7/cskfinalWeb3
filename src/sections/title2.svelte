<!-- <script>
  let { title, subtitle } = $props();
</script> -->

<!-- <div class="title-card">
  <div class="content">
    <h1>{title}</h1>
    <p>{subtitle}</p>
  </div>
</div> -->
<!-- //////////////////////////PARALLAX SCROLLING///////////////////////-->

<div class="parallax">
  <div class="parallax-text">
    <h1 class="parallax-title">Hello! I'm Nkechi:)</h1>
    <p class="parallax-subtitle">/een-kay-chee/</p>
    <div class="typewriter">
      <h1 class="welcome">Welcome to my tech corner</h1>
    </div>
    <!-- ENTER SITE BUTTON -->
    <button id="enterBtn" class="enter-btn">Enter Site</button>
  </div>
</div>

<style>
  /* /////////////////////////////PARALAX///////////////////////////////////////////// */
  .parallax {
    background-image: url("/Users/nkechi7/Documents/GitHub/cskfinalWeb3/src/images/titleGif.gif");
    min-height: 800px;
    background-attachment: fixed;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    background-color: black;
    position: relative;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  /* Overlay for better text readability */
  .parallax::before {
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: rgba(0, 0, 0, 0.4);
    z-index: 1;
  }

  /* Text overlay container */
  .parallax-text {
    position: relative;
    z-index: 2;
    text-align: center;
    color: white;
    padding: 40px;
    max-width: 800px;
  }

  /* Main title */
  .parallax-title {
    font-size: 5rem;
    font-weight: 650;
    margin-bottom: 20px;
    text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.8);
    animation: fadeInDown 1s ease-out;
  }

  .parallax-subtitle {
    font-size: 2rem;
  }

  /* TYPWRITER */
  .typewriter h1 {
    overflow: hidden; /* Ensures the content is not revealed until the animation */
    border-right: 0.15em solid indigo; /* The typewriter cursor */
    white-space: nowrap; /* Keeps the content on a single line */
    margin: 0 auto; /* Gives that scrolling effect as the typing happens */
    letter-spacing: 0.15em; /* Adjust as needed */
    animation:
      typing 3.5s steps(40, end),
      blink-caret 0.75s step-end infinite 3.5s,
      /* Start blinking after typing */ stop-caret 0s 7s forwards; /* Stop blinking after total time */
  }

  /* The typing effect */
  @keyframes typing {
    from {
      width: 0;
    }
    to {
      width: 100%;
    }
  }

  /* The typewriter cursor effect */
  @keyframes blink-caret {
    from,
    to {
      border-color: transparent;
    }
    50% {
      border-color: indigo;
    }
  }

  /* Stop the cursor blinking */
  @keyframes stop-caret {
    to {
      border-color: transparent;
    }
  }

  /* .type1 {
display:flex;
justify-content: center;
background-color: transparent;
} */

  .welcome {
    font-size: 38px;
  }

  /* .name1{
display:flex;
justify-content: center;
background-color: transparent;
} */


 .enter-btn {
  margin-top: 30px;
  padding: 12px 28px;
  font-size: 1.2rem;
  color: white;
  background-color: rgba(75, 0, 130, 0.8); /* indigo with transparency */
  border: none;
  border-radius: 8px;
  cursor: pointer;
  transition: background-color 0.3s ease, transform 0.2s ease;
}

.enter-btn:hover {
  background-color: rgba(138, 43, 226, 0.9);
  transform: scale(1.05);
}

</style>
