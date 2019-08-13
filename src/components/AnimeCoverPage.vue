<template>
  <div class="uk-section anime-cover-section">
    <!-- <div class="uk-container"> -->
    <div class="anime-cover">
      <div
        id="test-target"
        class="uk-height-large uk-background-cover uk-light uk-flex uk-flex-top anime-cover-image uk-background-fixed"
        uk-parallax="bgy: -200"
      >
        <!-- <h1 class="uk-width-1-2@m uk-text-left uk-margin-small uk-margin-auto-vertical" uk-parallax="y: 100,0"></h1> -->
      </div>
    </div>
    <!-- <div class="uk-card uk-card-default uk-card-hover uk-card-body uk-width-1-2@m anime-profile-card"> -->
    <!-- <h3 class="uk-card-title">Default</h3>
                <p>Lorem ipsum <a href="#">dolor</a> sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p> -->
    <span class="ab">
      <img
        src="https://media.kitsu.io/anime/poster_images/1/small.jpg?1431697256"
        alt=""
        class="card-poster uk-card uk-card-default uk-card-hover uk-card-body uk-width-1-2@m"
      />

      <div
        class="uk-card uk-card-secondary uk-card-body uk-width-1-3@m anime-side-info-quick-nav"
      >
        <div
          class="uk-grid-collapse uk-child-width-1-3@m uk-grid-small uk-grid-match"
          uk-grid
        >
          <div>
            <div
              class="uk-card uk-card-primary uk-card-body uk-card-hover anime-side-info-quick-nav-icon"
              uk-tooltip="title: Favorites Count; pos: bottom-right"
            >
              <span class="" uk-icon="icon: heart;"></span>
              <span class="uk-text-meta">2348</span>
            </div>
          </div>
          <div>
            <div
              class="uk-card uk-card-primary uk-card-body uk-card-hover anime-side-info-quick-nav-icon"
              uk-tooltip="title: Users Count; pos: bottom-right"
            >
              <span class="" uk-icon="icon: users;"></span>
              <span class="uk-text-meta">6565</span>
            </div>
          </div>
          <div>
            <div
              class="uk-card uk-card-primary uk-card-body uk-card-hover anime-side-info-quick-nav-icon"
              uk-tooltip="title: Length of episodes; pos: bottom-right"
            >
              <span class="" uk-icon="icon: video-camera;"></span>
              <div class="uk-text-meta">25[min]</div>
            </div>
          </div>
        </div>
      </div>

      <div
        class="uk-card uk-card-secondary uk-card-body uk-width-1-3@m anime-side-info"
      >
        <table class="uk-table uk-text-small">
          <tbody>
            <tr>
              <td class="uk-text-left">avg.score</td>
              <td class="uk-text-right">3.5/5</td>
            </tr>
            <tr>
              <td class="uk-text-left">avg.score</td>
              <td class="uk-text-right">3.5/5</td>
            </tr>
            <tr>
              <td class="uk-text-left">avg.score</td>
              <td class="uk-text-right">3.5/5</td>
            </tr>
            <tr>
              <td class="uk-text-left">avg.score</td>
              <td class="uk-text-right">3.5/5</td>
            </tr>
            <tr>
              <td class="uk-text-left">avg.score</td>
              <td class="uk-text-right">3.5/5</td>
            </tr>
          </tbody>
        </table>
      </div>
    </span>
    <!-- </div>               -->
    <div class="uk-section anime-cover-info uk-align-right">
      <div class="uk-card uk-card-secondary uk-card-body">
        <h1 class="uk-text-left uk-heading-hero uk-heading-bullet">Toradora</h1>
        <div class="uk-clearfix">
          <span class="uk-label uk-align-left uk-text-bold">Adventure</span>
          <span class="uk-label uk-align-left uk-text-bold">Fantasy</span>
          <span class="uk-label uk-align-left uk-text-bold">Historical</span>
          <span class="uk-label uk-align-left uk-text-bold">Mystery</span>
        </div>
        <div>
          <p class="uk-text-left">
            "Mushi": the most basic forms of life in the world. They exist
            without any goals or purposes aside from simply "being." They are
            beyond the shackles of the words "good" and "evil." Mushi can exist
            in countless forms and are capable of mimicking things from the
            natural world such as plants, diseases, and even phenomena like
            rainbows. This is, however, just a vague definition of these
            entities that inhabit the vibrant world of Mushishi, as to even call
            them a form of life would be an oversimplification. Detailed
            information on Mushi is scarce because the majority of humans are
            unaware of their existence. So what are Mushi and why do they exist?
            This is the question that a "Mushi-shi," Ginko, ponders constantly.
            Mushi-shi are those who research Mushi in hopes of understanding
            their place in the world's hierarchy of life. Ginko chases rumors of
            occurrences that could be tied to Mushi, all for the sake of finding
            an answer. It could, after all, lead to the meaning of life itself.
            [Written by MAL Rewrite]
          </p>
        </div>
      </div>
      <div class="uk-container"></div>
    </div>

    <!-- </div> -->
  </div>
</template>

<script>
import UIkit from "uikit";
import Icons from "uikit/dist/js/uikit-icons";
UIkit.use(Icons);
UIkit.parallax(document.getElementsByClassName("anime-cover"));
UIkit.grid(document.getElementsByClassName("anime-cover-card-grid"));
UIkit.img(document.getElementsByClassName("element"));
UIkit.icon(document.getElementsByClassName("anime-side-info-quick-nav-icon"));

export default {
  name: "AnimeCoverPage"
};
</script>

<style lang="scss" scoped>
.anime-cover {
  height: 10%;
}

.anime-cover-image {
  background-image: url("https://media.kitsu.io/anime/cover_images/2/original.png");
}

.anime-cover-section {
  padding-top: 0px;
  padding-bottom: 0px;
  transform: translateY(0%);
  background: #282828;
}
.anime-cover-info {
  background: #424242;
  margin: 0%;
  margin-right: 5%;
  width: 63.5%;
  padding: 0%;
}

.card-poster {
  padding: 0%;
  // height: 100%;
  object-fit: contain;
  // width: 100%;
  width: 100%;
  // float: left;
  // transform: translateY(-50%);
  //margin-left: 5%;
}

.anime-side-info {
  // float: left;
  width: 100%;
  margin-top: 2%;
  padding: 2%;
  //margin-left: 5%;
  //position: absolute;
}

.anime-side-info-quick-nav {
  // float: left;
  width: 100%;
  margin-top: 2%;
  padding: 0%;
  //margin-left: 5%;
  //position: absolute;
}

.ab {
  float: left;
  display: flex;
  flex-direction: column;
  transform: translateY(-35%);
  width: 25%;
  margin-left: 5%;
  margin-right: 0%;
}

.each-side-info {
  display: inline;
}

td {
  padding-top: 0%;
  padding-bottom: 0%;
  text-transform: uppercase;
}

.anime-side-info-quick-nav-icon {
  padding-top: 5%;
  padding-bottom: 5%;
}
</style>
