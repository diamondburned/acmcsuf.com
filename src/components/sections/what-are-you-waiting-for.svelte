<script lang="ts">
  import CallToAction from "../../components/ui/call-to-action.svelte";
</script>

<section class="info-screen screen-wyd">
  <div>
    <h2>so what you are waiting for?</h2>
    <p>
      We invite you to become a part of our chapter consisting of
      <b>350<span class="plus">+</span> members</b>, and rising! All of our
      coding workshops, info sessions, and community events were designed to
      start off your tech journey on the right foot.
    </p>
    <CallToAction text="join us today!" />
  </div>
</section>

<style>
  .screen-wyd {
    background: none;
    padding-bottom: 333px;

    --min-padding: 10px;
  	  --max-padding: 150px;
  }

  .screen-wyd div {
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;

    padding-top: 333px;
    padding-left: var(--min-padding);
    padding-right: var(--min-padding);
    padding-bottom: var(--min-p-font-size);
  }

  .screen-wyd h2 {
    font-weight: bold;
    font-size: var(--min-h-font-size);
  }

  .screen-wyd p {
    font-size: var(--min-p-font-size);
  }

  .screen-wyd p,
  .screen-wyd h2 {
    padding-bottom: var(--min-p-font-size);
    margin: 0;
  }

  .screen-wyd span.plus {
    color: var(--acm-blue);
  }

  @media screen and (min-width: 768px) {
    .screen-wyd div {
      padding-left: var(--max-padding);
      padding-right: var(--max-padding);
      padding-bottom: var(--max-p-font-size);
    }

    .screen-wyd p {
      font-size: var(--max-p-font-size);
      padding-bottom: var(--max-p-font-size);
    }

    .screen-wyd h2 {
      font-size: var(--max-h-font-size-med);
      padding-bottom: var(--max-p-font-size);
    }
  }
</style>
