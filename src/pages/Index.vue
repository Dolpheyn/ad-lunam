<template>
  <q-page class="page">
    <h1 class="text-h2">Ad Lunam 🌑</h1>
    <span class="text-h5">
      Can the human civilization go to the moon–again, this time
      powered by low cost, reusable rockets?
    </span>
    <div class="q-mt-xl">

      <h2 class="text-h3">The Human and Space Chronicle</h2>

      <p>
        First, a recap. To answer the question "Can the human civilization go
        to the moon again?", we must first answer the question "Why did we go in the first
        place?".
      </p>

      <p>
        Our space story started in the 20th century, during the
        Cold War.  The Soviets launched the first ever man-made object into
        orbit, the Sputnik 1, after advancements in space technology made
        possible by the WWII.  This event triggered what we know today as the
        Space Race.
      </p>

      <p>
        NASA was born short after and for the next years, two giants–the US and the
        Soviets–made an international space show by dumping their money to prove
        who has the better technology to the world. The space programs were
        televised with the purpose of showing off how great they are,
        simultaneously pissing their rival off. For almost a decade later, what
        we saw was the giants furiously sending men to space, ending with the US
        sending Neil Armstrong to the moon in July of 1969. This continued to
        the year 1972, and by then we have sent a total of 12 humans to walk on
        the moon.
      </p>

      <p>
        Humans got super excited. We were expecting to push our boundaries far
        beyond what we were capable of. <span class="text-italic">A Moon base?
        We can do it. There's nothing that we can't do!</span> It was that
        same feeling of discovering again, like when we first sailed across the
        ocean.
      </p>

      <p>
        However for the next 49 years, the people-on-the-moon count is
        stil...12, and we don't have anything new planned, <span class="text-italic">
        at all</span>. The Space Race was just two giants being cocky during a
        war crisis, after all.  After it ended with one's satisfied ego, and the
        other's shame, the two nations don't find it worth to spend their fortunes
        to go beyond the orbit anymore.
      </p>

      <p>
        Fortunately, that was the case only until <span class="bank-gothic text-h6">SpaceX</span>
        showed up.
      </p>

      <h2 class="text-h3">History of <span class="bank-gothic">SpaceX</span></h2>

      <p>
        <span class="bank-gothic text-h6">SpaceX</span>
        <span class="text-strike">
          manufactures and launches the world’s most advanced
        </span> builds and launches
        <span class="text-italic"> cool and badass rockets</span>. The company
        was founded in 2002 by Elon Musk to revolutionize space transportation,

        <span class="text-bold">
          with the ultimate goal of making life multiplanetary.
        </span>
        Musk is famously known for founding Tesla Motors, X.com (later known as
        PayPal) and his first multimillionaire company, Zip2.
      </p>

      <p>
        Like any other successful businesses Musk had founded, SpaceX is no
        different.  It became the first privately funded group to put a payload
        in Earth orbit in 2008. Since then, the company has continued to
        impress, launching unmanned cargo vehicles to the International Space
        Station (ISS) and winning a contract from NASA to fly astronauts as
        early as 2017. One of SpaceX’s most notable history-making moments was
        when its first stage rocket—the Falcon 9🚀—became the first one to
        launch, <span class="text-bold">then autonomously landed upright on its
          feet.</span> Now in 2021, landing its rockets is already a
        routine for SpaceX.
      </p>

      <p class="text-center text-overline">
        Timeline of SpaceX's history and notable achievements.
      </p>

      <iframe
        src='https://cdn.knightlab.com/libs/timeline3/latest/embed/index.html?source=1wBuiAfJ11_6MMXc2kgYp-gD8JL3_CxxZz03sLfV4E8U&font=Default&lang=en&initial_zoom=2&height=650'
        width='100%'
        height='650'
        webkitallowfullscreen
        mozallowfullscreen
        allowfullscreen
        frameborder='0'
      />

      <h2 class="text-h3">Reusable Rockets 🚀</h2>

      <figure class="q-mx-none">
        <img
          src="https://upload.wikimedia.org/wikipedia/commons/0/0e/Falcon9_rocket_family.svg"
          alt="Falcon 9 rocket family"
          style="border: 1px solid #555; width: 100%;"
        >
        <em>
        <figcaption>The Falcon 9 rocket family | image: wikimedia</figcaption>
      </em>
      </figure>

      <p>
        <span class="bank-gothic text-h6">SpaceX</span> makes their rockets from
        scratch. They keep the outsourcing cost low by building roughly 80% from
        the parts of a rocket in their own factory. In one end of their factory
        comes the raw materials, in the other end,
        <span class="text-italic">rockets</span>. One study by NASA and the Air
        Force estimated that the price tag of the process, from designing to the
        launching of the Falcon 9 rocket, was about
        <span class="text-bold">a third of</span> what it would have cost NASA,
        shaving millions of dollars off of each launches.
      </p>

      <p>
        To reach Musk’s ultimate goal, he figured space travelling costs should
        be lowered, by a lot. He wanted to make his rockets reusable. After
        recovery from landing, the rockets must be able to be refurbished and
        reflown in minimal time, and with minimal cost. Only then can they be
        reflown, reducing launch costs significantly. Not surprisingly, Musk and
        SpaceX have been successfully doing this. Until May of 2021, SpaceX’s
        reused flights count is at 61, with the booster at the highest flight
        count being the B1051, sitting at <span class="text-bold">10 launches!</span>
      </p>

      <p>
        Boosters are the first stage of the two-stage rocket launch vehicle
        that SpaceX builds. Boosters burns rocket fuels at liftoff, up the rocket
        goes, it accelerates the rocket, and get detached at some point before
        continuing to orbit on its own path. Of course, for SpaceX's boosters
        they then land autonomously on a ground landing pad or a drone landing
        ship at the sea.
      </p>

      <p>
        <span class="text-bold">Block 5</span> is the name of the latest and
        greatest version of the Falcon 9 and Falcon Heavy rocket family's
        boosters. They have stronger heat shield, upgraded engines, new carbon
        composite sections, retracable landing legs, and you know, other cool
        reusable rocket stuffs. Block 5 boosters' name starts with "B1" with
        trailing numbers for identity purposes. They are the only ones that have
        ever reached more than 3 launch counts.
      </p>

      <q-card class="q-pa-md q-my-md">
        <q-btn-toggle
          v-model="byBoosters"
          class="q-my-md"
          no-caps
          rounded
          toggle-color="primary"
          color="white"
          text-color="primary"
          :options="[
            {label: 'By Boosters', value: true},
            {label: 'By Landing Status', value: false}
          ]"
        />
          <BoosterLaunchesBarChart v-if="byBoosters"/>
          <BoosterLaunchesPieChart v-else/>
        </q-card>

      <p class="q-my-xl">
        They've also been <span class="text-bold">dominating</span> the space
        launch market. Since 2017, SpaceX's rockets—Falcon 9 and Falcon Heavy—
        have delivered the highest number of launches compared to its
        competitors in the market, like Ariane 5 from European Space
        Agency(ESA), Proton-M and Soyuz-2 from the Soviet, and others.
      </p>

      <q-banner rounded class="bg-purple-4 text-white q-mb-md">
        <p class="text-bold text-h6 q-mt-sm"><q-icon name="info" class="q-mr-sm"/>Tip</p>
        <p style="font-size: 1.05rem">
        You can hover on the rocket names to make the chart highlight its line.
        </p>
      </q-banner>

      <q-card class="q-pa-md q-my-md">
        <SpaceLaunchMarketLineChart />
      </q-card>

      <p class="q-mt-xl">
        In April 2020, SpaceX made yet another first in history by flying 4
        astronauts in the Crew-2 mission with NASA with reused, or termed by
        NASA, “flight proven” rocket. SpaceX's Falcon 9 booster that launched
        the Crew-1 mission in November 2020—booster B1061—is brought to port
        after landing on an automatic drone ship at sea. This booster is reused
        for the Crew-2 mission, being the first rocket booster that has ever
        been used for multiple human launches.
      </p>

      <p>
        SpaceX's reusable rockets are already proven to be safe, flight proven
        and have been used by many customers around the world. Their customers
        includes big names like NASA, the USAF, and South Korea! These customers
        have been using SpaceX's services for launching communication,
        surveillance, and scientific satellites, <span><a
        href="https://en.wikipedia.org/wiki/Commercial_Resupply_Services">
        sending cargo and supplies to the ISS</a></span>, and more. Let's
        explore who have been trusting SpaceX, using their reusable rokets that
        are provided by their services.
      </p>

      <p class="text-center text-overline">
        SpaceX launches, grouped by their customers and mission categories.
      </p>

      <q-banner rounded class="bg-purple-4 text-white q-mb-md">
        <p class="text-bold text-h6 q-mt-sm"><q-icon name="info" class="q-mr-sm"/>Tip</p>
        <p style="font-size: 1.05rem">
        You can hover on the mission names to get more information.
        </p>
      </q-banner>

      <iframe
        width="100%"
        height="1060"
        frameborder="0"
        src="https://observablehq.com/embed/d65ba7542711e4bf?cells=chart"
      />

      <h2 class="text-h3">The Starship</h2>

      <figure class="q-mx-none">
        <img
          src="https://imgix.bustle.com/uploads/image/2021/4/19/1b2d4014-5a46-403f-a494-b18759fd8a29-for_press_release.jpg"
          alt="Illustration of SpaceX's lunar lander on the moon."
          style="width: 100%;"
        >
        <em>
          <figcaption>
            Illustration of Spacex's Spaceship lunar lander on the moon, as per
            proposal to NASA for its Artemis program. | image: SpaceX
          </figcaption>
      </em>
      </figure>

      <p>
        As of 2021, <span class="bank-gothic text-h6">SpaceX</span> is actively
        developing the Starship system, which is planned to be a fully-reusable
        two-stage launch vehicle, intended to replace all of its existing launch
        vehicles and spacecraft used for satellite delivery and human
        transport—Falcon 9, Falcon Heavy and Dragon. It is designed to carry
        cargo and pasengers for long durations, to eventually support flights to
        the Moon and Mars. In addition, it could be used commercially for
        point-to-point transportation on Earth.
      </p>

      <p>
        They have been iteratively designing, prototyping and testing Starship
        since 2018. Since then, there have been 22 prototypes in existence.
        However, only 12 have been on the launch site, and 8 from the 12 have
        flown. This is in fact because SpaceX likes to prototype <span
        class="text-italic">at speed</span>. Sometimes they scrap prototypes
        early, repurposing them to do other tests, or to build the next
        innovative iteration. They are also not afraid to make failures in the
        process.
      </p>

      <p>
        Notably, Starship, SpaceX’s fully reusable rocket system under development to eventually
        ferry humans and cargo to the Moon and Mars, won NASA’s award mainly for its massive cargo
        capability and its proposed bid of $2.9 billion — far cheaper than their compatitors,
        according to a NASA source selection document.
      </p>

      <p>
        So, yes! We <i>are</i> going to the moon again with reusable rockets. Right now, it's only the
        question of <b>when</b>. In the near future, space travel will be very much closer to all of
        us, and we should be <i>very</i> excited for that.
      </p>

      <!-- quote -->

      <p>
      </p>
    </div>
  </q-page>
</template>

<script>
import BoosterLaunchesBarChart from '../components/Charts/BoosterLaunchesBarChart'
import BoosterLaunchesPieChart from '../components/Charts/BoosterLaunchesPieChart'
import SpaceLaunchMarketLineChart from '../components/Charts/SpaceLaunchMarketLineChart.vue'

export default {
  name: 'PageIndex',

  components: {
    BoosterLaunchesBarChart,
    BoosterLaunchesPieChart,
    SpaceLaunchMarketLineChart,
  },

  data() {
    return {
      byBoosters: true,
    }
  }
}
</script>

<style>
p {
  font-size: 1.2rem;
}

figcaption {
  color: #626262;
}

.page {
  margin: 50px auto;
  padding: 0 40px;
  word-wrap: break-word;
  font-family: Helvetica, sans-serif;
}

@media (min-width: 786px) {
  .page {
      max-width: 720px;
  }
}

@media (min-width: 1280px) {
  .page {
      max-width: 1000px;
  }
}
</style>
