<script>
  import bookCover from "$assets/book_cover.png";
  import phoneCover from "$assets/phone_cover.png";
  import Button from "./Button.svelte";
</script>

<section class="hero">
  <div class="hero-showcase text-center bold">
    <h1 class="purple uppercase">Move to</h1>
    <h1 class="purple mb-xs uppercase">Spain</h1>
    <h4 class="italic semi-bold">
      There is no need to make the same mistakes as I made.
    </h4>
    <img src={bookCover} class="book-cover" alt="Book cover image" />
    <img src={phoneCover} class="phone-cover" alt="Phone cover image" />
  </div>
  <div class="hero-text white text-center">
    <h1 class="uppercase">This ebook will</h1>
    <h1 class="uppercase">save your money</h1>
    <h1 class="uppercase">time and nerves</h1>
    <p class="light-grey mb-l">
      I moved to Spain seven years ago. The process was painful and difficult. I
      learned most things the hard way: finding a job, getting a visa,
      calculating my cost of living, choosing an apartment. That's why I wrote
      this e-book, to tell you how I did it. No bullshit, no stress.
    </p>
    <Button color="red" size="big" onclick={() => console.log("test")}
      >Purchase E-book for $10</Button
    >
  </div>
</section>

<style>
  .hero {
    display: flex;
    height: 100vh;
    overflow-y: hidden;
  }

  .hero-showcase {
    position: relative;
    width: 50%;
    padding: 100px 16px 0 16px;
    background: linear-gradient(
      135deg,
      #e2cbff,
      #e2cbff 25%,
      #deeaff 50%,
      #ece5ff 75%,
      #927bce
    );
  }

  .hero-text {
    padding: 100px 5%;
    width: 50%;
    background-color: black;
  }

  .book-cover {
    position: absolute;
    right: 2%;
    bottom: 0;
    width: 65%;
    transform: translateY(30%);
  }

  .phone-cover {
    position: absolute;
    width: 35%;
    bottom: 0;
    right: 52%;
    transform: translateY(30%);
  }
</style>
