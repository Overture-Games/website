<script lang="ts">
  import Anchor from './components/Anchor.svelte';
  import LargeLink from './components/LargeLink.svelte';
  import Paragraph from './components/Paragraph.svelte';
  import Section from './components/Section.svelte';
  import TagLine from './components/TagLine.svelte';
  import Title from './components/Title.svelte';
  import YouTube from 'svelte-youtube-embed';
</script>

<Anchor name="intervallic" />
<Section>
  <TagLine>Intervallic</TagLine>
  <Title>
    Get motivated and pick up that dusty instrument!
  </Title>
  <Paragraph>
    Intervallic is an audio-responsive video game that gives real-time feedback 
    and makes even the most boring music practice fun! Use a microphone, MIDI instrument, 
    or computer keyboard to control a flying robot space cat around the planet of 
    Audius!
  </Paragraph>
  <Section>
    <YouTube 
      id="npvPh99QvkY"
      --title-color="white" 
      --title-shadow-color="black" 
      --title-font-family="Alegreya"
      --overlay-bg-color="hsla(0, 0%, 0%, 0.4)"
    >
      <i class="fas fa-play"></i>
    </YouTube>
  </Section>
  <Paragraph>
    In this single-player 2D side scroller, each note that you play moves the 
    cat up and down on the screen based on the musical intervals that you play. 
    Objects are arranged so that by the end of each level as you collect notes 
    and dodge obstacles you have played a full song. Collect notes in each 
    phrase to unlock each sample and collect all of the samples to beat the 
    level.
  </Paragraph>
  <Title>
    Support our mission by downloading Intervallic below!
  </Title>
  <div class="outer">
    <LargeLink to="https://store.steampowered.com/app/2270460" faIcon="fab fa-steam" newTab className="">
      Intervallic on Steam
    </LargeLink>
  </div>
</Section>

<style lang="scss">
  .outer {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    padding-top: 20px;

    @media (max-width: $desktop) {
      flex-direction: column;
    }
  }

  .inner {
    width: 50%;
    height: 100%;

    @media (max-width: $desktop) {
      width: 100%;
      padding: 15px 0 15px 0;
    }
  }

  i {
    font-size: 80px;
    color: white;
    filter: drop-shadow(5px 5px 5px black);
  }
</style>