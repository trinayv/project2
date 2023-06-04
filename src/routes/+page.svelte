<script lang="ts">
  import Section from '$components/Section.svelte';
  import mapPin from 'svelte-awesome/icons/mapPin';
  import envelope from 'svelte-awesome/icons/envelope';
  import desktop from 'svelte-awesome/icons/desktop';
  import search from 'svelte-awesome/icons/search';
</script>

<div class="readable-area">
  <div class="header">
    <div style="background-color:#f4f4f4;padding:16px;margin:32px; width: 257px;height:746px;float: left;">
      <a href="https://i.pinimg.com/564x/08/a0/52/08a052d80710e6bea5f44cbc00088b99.jpg">
        <img
        alt="nemo avatar"
        class="center"
        src="https://i.pinimg.com/564x/08/a0/52/08a052d80710e6bea5f44cbc00088b99.jpg" title="Profile Picture" />
      </a>
      <div class="header-text">
        <h1> Nemo </h1>
        <p class="job-title"> CLOWNFISH </p>
      </div>
      <div class="content">
        <div class="content-column">
          <div class="section-title">
            <Section iconData={mapPin} title="The Great Barrier Reef" />
          </div>
        </div>
        <div class="content-column">
          <div class="section-title">
            <Section iconData={envelope} title="findingnemo@gmail.com" />
          </div>
        </div>
        <div class="content-column">
          <div class="section-title">
            <Section iconData={desktop} title="www.findingnemo.com" />
          </div>
        </div>
      </div>

      <h2 class="profile"> profile </h2>
      <hr style="height:1.5px;border-width:0;color:black;background-color:gray">
      <p class="profile-text"> Hi! I'm Nemo, born with one small fin. I'm a curious and impressionable six-year-old, only child who lives with my overprotective and single-parent father. Despite being born with a withered fin, I yearns for adventure, and as fate takes me far from home, I learns that I am capable of doing great things. </p>
    </div>
    <h2 class="profile"> skills </h2>
    <hr class="hr2">
    <li class="skill">
        <span class="skill-title">Swimming Speed</span>
        <div class="gauge">
          <div class="bullet filled-bullet"></div>
          <div class="bullet filled-bullet"></div>
          <div class="bullet filled-bullet"></div>
          <div class="bullet"></div>
          <div class="bullet"></div>
        </div>
    </li>
    <li class="skill">
      <span class="skill-title">Physical Strength</span>
      <div class="gauge">
        <div class="bullet filled-bullet"></div>
        <div class="bullet filled-bullet"></div>
        <div class="bullet filled-bullet"></div>
        <div class="bullet filled-bullet"></div>
        <div class="bullet"></div>
      </div>
    </li>
    <h2 class="profile"> education </h2>
    <hr class="hr2">
    <p class="profile-text">
    <ul>
      <li>
        <span class="profile-text2">2003</span>
        <span class="time">The School Fish</span>
    </ul>
    <h2 class="profile"> interest </h2>
    <hr class="hr2">
    <div class="section-title">
      <Section iconData={search} title="Adventure and Exploring" />
    </div>
  </div>
</div>

 
  <style>


ul {
  list-style-type: none;
}

li {
  display: flex;
  flex-direction: column;
}

.time {
  margin-left: 16px;
  text-align: justify;
  margin-right: 18px;
  font-family: "Nunito Sans", sans-serif;
}

.profile-text2 {
  text-align: justify;
  font-family: "Nunito Sans", sans-serif;
  margin-right: 40px;
  margin-left: 10px;
}

.readable-area {
  display: flex;
  flex-direction: column;
  background-color: white;
  margin: 0 5%;
}

img {
  width: 128px;
  height: 128px;
  border: 14px solid white;
  border-radius: 100%;
}

.center {
  display: block;
  margin-left: auto;
  margin-right: auto;
  width: 50%;
}

.header {
		padding: 16px;
		flex-direction: column-reverse;
		align-items: center;
		border-bottom: 2px solid black;
		text-decoration: none;
}

.header-text {
  display: flex;
  flex-direction: column;
  padding: 16px;
  justify-content: end;
  align-items: left;
  text-align: center;
}

h1 {
  font-family: "Public Sans", sans-serif;
  padding-top: 10px;
}

p {
  font-family: "Raleway", sans-serif;
  padding-top: 6px;
}

.content-column {
  text-align-last: justify;
}

.section-title {
  padding: 4px 16px;
  margin: 16px 0;
  font-family: "Nunito Sans", sans-serif;
}


.profile {
  padding: 4px 18px;
  padding-top: 32px;
  font-weight: 500;
  margin: 16px 0;
  font-family: "Source Sans Pro", sans-serif;
  font-size: 22px;
  text-transform: UPPERCASE;
  letter-spacing: 8px;
}

hr {
  display: block;
  margin-top: 0.5em;
  margin-bottom: 0.5em;
  margin-left: 16px;
  margin-right: 16px;
  border-style: inset;
  border-width: 1px;
}

.hr2{
  display: block;
  margin-top: 0.5em;
  margin-bottom: 0.5em;
  margin-left: 16px;
  margin-right: 80px;
  border-style: inset;
  border-width: 1px;
  height:1.5px;
  border-width:0;
  color: black;
  background-color:gray;
}

.profile-text {
  text-align: justify;
  margin-right: 18px;
  margin-left: 18px;
  font-family: "Nunito Sans", sans-serif;
}

.gauge {
  display: flex;
  flex-direction: row;
  margin-left: 8px;
  margin-right: 70px;
}

.bullet {
  border-radius: 100%;
  width: 16px;
  height: 16px;
  margin: 1px;
  margin-right: 10px;
  background-color: #cfcfcf;
}

.filled-bullet {
  background-color: #737373;
}

li {
  display: flex;
  flex-direction: column;
}

.skill {
  display: flex;
  flex-direction: row;
  align-items: center;
  margin-bottom: 2px;
}

.skill-title {
  flex: 1;
  margin-left: 10px;
  font-family: "Nunito Sans", sans-serif;
}



@media (min-width: 750px) {
		.header {
			flex-direction: row;
		}

		.header-text {
			text-align: justify;
		}

		.content {
			grid-template-columns: repeat(2, minmax(0, 1fr));
		}

		.readable-area {
			margin: 0 10%;
		}
	}

	@media (min-width: 500px) {
		.readable-area {
			margin: 0 20%;
		}
	}
</style>