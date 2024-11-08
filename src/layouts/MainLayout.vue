<template>
  <q-scroll-area style="height: 100%">
    <div class="q-pt-md"></div>
    <q-btn flat align="left" class="full-width" no-caps>
      <q-avatar size="md" class="q-ma-xs">
        <img src="icons/rui.jpg" />
      </q-avatar>
      <div class="q-pa-xs">
        <span style="margin: 0 0 0 0">Rui Kamishiro</span>
      </div>
    </q-btn>
    <q-btn flat align="left" class="full-width" no-caps>
      <q-avatar size="md" class="q-ma-xs">
        <q-icon color="primary" name="people"></q-icon>
      </q-avatar>
      <div class="q-pa-xs">
        <span style="margin: 0 0 0 0">Friends (32 online)</span>
      </div>
    </q-btn>
    <q-btn flat align="left" class="full-width" no-caps>
      <q-avatar size="md" class="q-ma-xs">
        <q-icon color="primary" name="history"></q-icon>
      </q-avatar>
      <div class="q-pa-xs">
        <span style="margin: 0 0 0 0">Memories</span>
      </div>
    </q-btn>
    <q-btn flat align="left" class="full-width" no-caps>
      <q-avatar size="md" class="q-ma-xs">
        <q-icon color="pink-14" name="bookmark"></q-icon>
      </q-avatar>
      <div class="q-pa-xs">
        <span style="margin: 0 0 0 0">Saved</span>
      </div>
    </q-btn>
    <q-btn flat align="left" class="full-width" no-caps>
      <q-avatar size="md" class="q-ma-xs">
        <q-icon color="primary" name="group"></q-icon>
      </q-avatar>
      <div class="q-pa-xs">
        <span style="margin: 0 0 0 0">Groups</span>
      </div>
    </q-btn>
    <q-btn flat align="left" class="full-width" no-caps>
      <q-avatar size="md" class="q-ma-xs">
        <q-icon color="primary" name="videocam"></q-icon>
      </q-avatar>
      <div class="q-pa-xs">
        <span style="margin: 0 0 0 0">Videos</span>
      </div>
    </q-btn>
    <q-btn flat align="left" class="full-width" no-caps>
      <q-avatar size="md" class="q-ma-xs">
        <q-icon color="primary" name="storefront"></q-icon>
      </q-avatar>
      <div class="q-pa-xs">
        <span style="margin: 0 0 0 0">Marketplace</span>
      </div>
    </q-btn>
    <q-btn flat align="left" class="full-width" no-caps>
      <q-avatar size="md" class="q-ma-xs">
        <q-icon color="primary" name="feed"></q-icon>
      </q-avatar>
      <div class="q-pa-xs">
        <span style="margin: 0 0 0 0">Feeds</span>
      </div>
    </q-btn>

    <!-- HIDDEN ONES -->
    <q-btn v-show="showMore" flat align="left" class="full-width" no-caps>
      <q-avatar size="md" class="q-ma-xs">
        <q-icon color="primary" name="bar_chart"></q-icon>
      </q-avatar>
      <div class="q-pa-xs">
        <span style="margin: 0 0 0 0">Ads Manager</span>
      </div>
    </q-btn>

    <q-btn v-show="showMore" flat align="left" class="full-width" no-caps>
      <q-avatar size="md" class="q-ma-xs">
        <q-icon color="primary" name="cake"></q-icon>
      </q-avatar>
      <div class="q-pa-xs">
        <span style="margin: 0 0 0 0">Birthday</span>
      </div>
    </q-btn>

    <q-btn v-show="showMore" flat align="left" class="full-width" no-caps>
      <q-avatar size="md" class="q-ma-xs">
        <q-icon color="light-green-8" name="compost"></q-icon>
      </q-avatar>
      <div class="q-pa-xs">
        <span style="margin: 0 0 0 0">Climate Science Center</span>
      </div>
    </q-btn>

    <q-btn v-show="showMore" flat align="left" class="full-width" no-caps>
      <q-avatar size="md" class="q-ma-xs">
        <q-icon color="pink-8" name="favorite"></q-icon>
      </q-avatar>
      <div class="q-pa-xs">
        <span style="margin: 0 0 0 0">Dating</span>
      </div>
    </q-btn>

    <q-btn v-show="showMore" flat align="left" class="full-width" no-caps>
      <q-avatar size="md" class="q-ma-xs">
        <q-icon color="red-7" name="event"></q-icon>
      </q-avatar>
      <div class="q-pa-xs">
        <span style="margin: 0 0 0 0">Events</span>
      </div>
    </q-btn>

    <q-btn v-show="showMore" flat align="left" class="full-width" no-caps>
      <q-avatar size="md" class="q-ma-xs">
        <q-icon color="orange-4" name="monetization_on"></q-icon>
      </q-avatar>
      <div class="q-pa-xs">
        <span style="margin: 0 0 0 0">Fundraisers</span>
      </div>
    </q-btn>

    <q-btn v-show="showMore" flat align="left" class="full-width" no-caps>
      <q-avatar size="md" class="q-ma-xs">
        <q-icon color="primary" name="dashboard"></q-icon>
      </q-avatar>
      <div class="q-pa-xs">
        <span style="margin: 0 0 0 0">Gaming Video</span>
      </div>
    </q-btn>

    <q-btn v-show="showMore" flat align="left" class="full-width" no-caps>
      <q-avatar size="md" class="q-ma-xs">
        <q-icon color="pink-8" name="chat_bubble"></q-icon>
      </q-avatar>
      <div class="q-pa-xs">
        <span style="margin: 0 0 0 0">Messenger</span>
      </div>
    </q-btn>

    <q-btn v-show="showMore" flat align="left" class="full-width" no-caps>
      <q-avatar size="md" class="q-ma-xs">
        <q-icon color="light-green-8" name="chat_bubble"></q-icon>
      </q-avatar>
      <div class="q-pa-xs">
        <span style="margin: 0 0 0 0">Messenger Kids</span>
      </div>
    </q-btn>

    <q-btn v-show="showMore" flat align="left" class="full-width" no-caps>
      <q-avatar size="md" class="q-ma-xs">
        <q-icon color="black" name="credit_card"></q-icon>
      </q-avatar>
      <div class="q-pa-xs">
        <span style="margin: 0 0 0 0">Orders and Payments</span>
      </div>
    </q-btn>

    <q-btn v-show="showMore" flat align="left" class="full-width" no-caps>
      <q-avatar size="md" class="q-ma-xs">
        <q-icon color="orange-4" name="flag"></q-icon>
      </q-avatar>
      <div class="q-pa-xs">
        <span style="margin: 0 0 0 0">Pages</span>
      </div>
    </q-btn>

    <q-btn v-show="showMore" flat align="left" class="full-width" no-caps>
      <q-avatar size="md" class="q-ma-xs">
        <q-icon color="primary" name="sports_esports"></q-icon>
      </q-avatar>
      <div class="q-pa-xs">
        <span style="margin: 0 0 0 0">Pay Games</span>
      </div>
    </q-btn>

    <q-btn v-show="showMore" flat align="left" class="full-width" no-caps>
      <q-avatar size="md" class="q-ma-xs">
        <q-icon color="primary" name="assignment_returned"></q-icon>
      </q-avatar>
      <div class="q-pa-xs">
        <span style="margin: 0 0 0 0">Recent Ad Activities</span>
      </div>
    </q-btn>

    <q-btn v-show="showMore" flat align="left" class="full-width" no-caps>
      <q-avatar size="md" class="q-ma-xs">
        <q-icon color="pink-4" name="movie_filter"></q-icon>
      </q-avatar>
      <div class="q-pa-xs">
        <span style="margin: 0 0 0 0">Reels</span>
      </div>
    </q-btn>

    <!-- SHOW MORE -->
    <q-btn
      @click="toggleMore"
      v-show="!showMore"
      flat
      align="left"
      class="full-width"
      no-caps
    >
      <q-avatar size="md" class="q-ma-xs" color="blue-grey-11">
        <q-icon color="black" name="expand_more"></q-icon>
      </q-avatar>
      <div class="q-pa-xs">
        <span style="margin: 0 0 0 0">See More</span>
      </div>
    </q-btn>

    <!-- SHOW LESS -->
    <q-btn
      @click="toggleMore"
      v-show="showMore"
      flat
      align="left"
      class="full-width"
      no-caps
    >
      <q-avatar size="md" class="q-ma-xs" color="blue-grey-11">
        <q-icon color="black" name="expand_less"></q-icon>
      </q-avatar>
      <div class="q-pa-xs">
        <span style="margin: 0 0 0 0">See Less</span>
      </div>
    </q-btn>

    <q-separator class="q-ma-md"></q-separator>

    <div class="row q-ma-xs" style="width: 100%">
      <div class="col-6">
        <div class="flex justify-start">
          <strong style="color: gray; margin: 0 0 0 25px"
            >Your Shortcuts</strong
          >
        </div>
      </div>
      <div class="col-6">
        <div class="flex justify-end">
          <div style="color: black" class="q-mr-sm">
            <a href="#/fb" style="text-decoration: none; margin: 0 25px"
              >edit</a
            >
          </div>
        </div>
      </div>
    </div>

    <q-btn flat align="left" class="full-width" no-caps>
      <q-avatar rounded size="md" class="q-ma-xs">
        <img src="icons/wxs.jpg" />
      </q-avatar>
      <div class="q-pa-xs">
        <span style="margin: 0 0 0 0">Wonderland X Showtime</span>
      </div>
    </q-btn>

    <q-btn flat align="left" class="full-width" no-caps>
      <q-avatar rounded size="md" class="q-ma-xs">
        <img src="icons/vbs.png" />
      </q-avatar>
      <div class="q-pa-xs">
        <span style="margin: 0 0 0 0">VIVID Bad Squad</span>
      </div>
    </q-btn>

    <q-btn flat align="left" class="full-width" no-caps>
      <q-avatar rounded size="md" class="q-ma-xs">
        <img src="icons/n25.jpg" />
      </q-avatar>
      <div class="q-pa-xs">
        <span style="margin: 0 0 0 0">Nightcord at 25:00</span>
      </div>
    </q-btn>

    <q-btn flat align="left" class="full-width" no-caps>
      <q-avatar rounded size="md" class="q-ma-xs">
        <img src="icons/khs.png" />
      </q-avatar>
      <div class="q-pa-xs">
        <span style="margin: 0 0 0 0">Kamiyama High School</span>
      </div>
    </q-btn>

    <div class="q-pa-sm">
      <a class="small-lct" href="#/fb" style="font-weight: bold">Privacy</a>
      <span style="color: gray"> &#183; </span>
      <a class="small-lct" href="#/fb" style="font-weight: bold">Terms</a>
      <span style="color: gray"> &#183; </span>
      <a class="small-lct" href="#/fb" style="font-weight: bold">Advertising</a>
      <span style="color: gray"> &#183; </span>
      <a class="small-lct" href="#/fb" style="font-weight: bold"
        >Ad Choices
        <q-icon name="warning_amber"></q-icon>
      </a>
      <span style="color: gray"> &#183; </span>
      <a class="small-lct" href="#/fb" style="font-weight: bold">Cookies</a>
      <span style="color: gray"> &#183; </span>

      <a
        class="small-lct"
        href="#/fb"
        style="color: gray; text-decoration: none"
        >More</a
      >
      <span style="color: gray"> &#183; </span>

      <a
        class="small-lct"
        href="#/fb"
        style="color: gray; text-decoration: none"
        >Meta <q-icon name="copyright" /> 2024</a
      >
    </div>
  </q-scroll-area>
</template>

<script>
export default {
  name: 'FessbookLeftPanel',
  data() {
    return {
      showMore: false,
    };
  },
  methods: {
    toggleMore() {
      this.showMore = !this.showMore;
    },
  },
};
</script>
