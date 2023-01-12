---
layout: two-cols-header
clicks: 10
---

# Teamfunktionen

::left::

<ul>
    <li v-if="$slidev.nav.clicks === 1"><strong>Participants</strong></li><li v-else>Participants</li>
    <li v-if="$slidev.nav.clicks === 2"><strong>Participants Pointers</strong></li><li v-else>Participants Pointers</li>
    <li v-if="$slidev.nav.clicks === 3"><strong>Dicsussion</strong></li><li v-else>Dicsussion</li>
    <li v-if="$slidev.nav.clicks === 4"><strong>Discussion: Nachrichten in Abwesenheit</strong></li><li v-else>Discussion: Nachrichten in Abwesenheit</li>
    <li v-if="$slidev.nav.clicks === 5"><strong>FollowMe Modus</strong></li><li v-else>FollowMe Modus</li>
    <li v-if="$slidev.nav.clicks === 6"><strong>Discussion: Reaktionen</strong></li><li v-else>Discussion: Reaktionen</li>
    <li v-if="$slidev.nav.clicks === 7"><strong>Discussion: Antworten</strong></li><li v-else>Discussion: Antworten</li>
    <li v-if="$slidev.nav.clicks === 8"><strong>Editoren</strong></li><li v-else>Editoren</li>
    <li v-if="$slidev.nav.clicks === 9"><strong>Laserpointer</strong></li><li v-else>Laserpointer</li>
    <li v-if="$slidev.nav.clicks === 10"><strong>Push Notifications</strong></li><li v-else>Push Notifications</li>
    
</ul>

<style>
    strong {
        color: lightgreen !important;
    }
</style>

::right::

<div class="imgContainer" v-if="$slidev.nav.clicks === 1">
  <img src="/img/teamfunktionen/participants.png" width="100">
</div>
<div class="imgContainer" v-if="$slidev.nav.clicks === 2">
  <img src="/img/teamfunktionen/ParticipantPointers.png" >
</div>
<div class="imgContainer" v-if="$slidev.nav.clicks === 3">
  <img src="/img/teamfunktionen/Discussion_expanded_small.png" >
</div>
<div class="imgContainer" v-if="$slidev.nav.clicks === 4">
  <img class="twoImg" src="/img/teamfunktionen/NewMessage_Chat.png" >
  <img class="twoImg" src="/img/teamfunktionen/NewMessage_Template.png" >
</div>
<div class="d-flex align-center flex-column" v-if="$slidev.nav.clicks === 5">
  <img src="/img/teamfunktionen/followMe.png" class="mb-3">
  <img src="/img/teamfunktionen/FollowMeGefolgt.png" >
</div>
<div class="imgContainer" v-if="$slidev.nav.clicks === 6">
  <img class="twoImg" src="/img/teamfunktionen/Discussion_Reaktionen.png" >
  <img class="twoImg" src="/img/teamfunktionen/EmojiPicker.png" >
</div>
<div class="imgContainer" v-if="$slidev.nav.clicks === 7">
  <img class="twoImg" src="/img/teamfunktionen/Answering_Indicator.png" >
  <img class="twoImg" src="/img/teamfunktionen/BeispielnachrichtAntwort.png" >
</div>
<div class="d-flex align-center flex-column" v-if="$slidev.nav.clicks === 8">
  <img src="/img/teamfunktionen/EditorsInModal.png" class="mb-3" width="240">
  <img src="/img/teamfunktionen/EditorInTemplate.png" width="240">
</div>
<div class="imgContainer" v-if="$slidev.nav.clicks === 9">
  <img src="/img/teamfunktionen/Laserpointer.png" >
</div>
<div class="imgContainer" v-if="$slidev.nav.clicks === 10">
</div>

<style>
    .imgContainer {
        display: flex;
        justify-content: center;
        align-items: center;
        height: 100%;
    }
    .twoImg {
        width: 45% !important;
        max-width: 45% !important;
        margin: 0 2.5%;
    }
</style>
