<template>
  <section>
    <b-container class="bv-example-row">
      <b-row>
        <b-col class="text-white">
          <h2>
            Lorem ipsum
            <span
              ><script src="https://cdn.lordicon.com/libs/mssddfmo/lord-icon-2.1.0.js"></script>
              <lord-icon
                src="https://cdn.lordicon.com/zzcjjxew.json"
                trigger="hover"
                colors="primary:#eee966,secondary:#eee966"
                style="width: 45px; height: 45px"
              >
              </lord-icon
            ></span>
          </h2>
          <p>
            spanLorem ipsum dolor sit amet consectetur adipisicing elit. Maxime
            unde quidem neque magni distinctio veniam ab, perferendis quasi
            harum quisquam aperiam itaque commodi sunt qui non modi repellendus.
            Recusandae, odio.nihil magni voluptatem totam nihil magni voluptatem
            totam
          </p>
        </b-col>
        <b-col class="text-white text-center mobile">
          <iframe id="map"
            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d15447.102861560237!2d4.483204015207343!3d52.16057733997295!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x47c642489521527b%3A0x9f4852fc4854709!2sBurcht%20van%20Leiden!5e0!3m2!1snl!2snl!4v1631516351306!5m2!1snl!2snl"
            width="600"
            height="450"
            style="border: 0"
            allowfullscreen=""
            loading="lazy"
            alt="google maps"  
          ></iframe>
        </b-col>
      </b-row>
    </b-container>
  </section>
</template>

<style lang="css" scoped>
section {
  margin-bottom: 5rem;
  margin-top: 5rem;
}
@media only screen and (max-width: 767px) and (min-width: 300px)  {
    .mobile{
        display: none;
    }
}

iframe{
  border-radius: 5px;
}
</style>

<script>

function initMap() {
  // Styles a map in night mode.
  const map = new google.maps.Map(document.getElementById("map"), {
    center: { lat: 40.674, lng: -73.945 },
    zoom: 12,
    styles: [
      { elementType: "geometry", stylers: [{ color: "#242f3e" }] },
      { elementType: "labels.text.stroke", stylers: [{ color: "#242f3e" }] },
      { elementType: "labels.text.fill", stylers: [{ color: "#746855" }] },
      {
        featureType: "administrative.locality",
        elementType: "labels.text.fill",
        stylers: [{ color: "#d59563" }],
      },
      {
        featureType: "poi",
        elementType: "labels.text.fill",
        stylers: [{ color: "#d59563" }],
      },
      {
        featureType: "poi.park",
        elementType: "geometry",
        stylers: [{ color: "#263c3f" }],
      },
      {
        featureType: "poi.park",
        elementType: "labels.text.fill",
        stylers: [{ color: "#6b9a76" }],
      },
      {
        featureType: "road",
        elementType: "geometry",
        stylers: [{ color: "#38414e" }],
      },
      {
        featureType: "road",
        elementType: "geometry.stroke",
        stylers: [{ color: "#212a37" }],
      },
      {
        featureType: "road",
        elementType: "labels.text.fill",
        stylers: [{ color: "#9ca5b3" }],
      },
      {
        featureType: "road.highway",
        elementType: "geometry",
        stylers: [{ color: "#746855" }],
      },
      {
        featureType: "road.highway",
        elementType: "geometry.stroke",
        stylers: [{ color: "#1f2835" }],
      },
      {
        featureType: "road.highway",
        elementType: "labels.text.fill",
        stylers: [{ color: "#f3d19c" }],
      },
      {
        featureType: "transit",
        elementType: "geometry",
        stylers: [{ color: "#2f3948" }],
      },
      {
        featureType: "transit.station",
        elementType: "labels.text.fill",
        stylers: [{ color: "#d59563" }],
      },
      {
        featureType: "water",
        elementType: "geometry",
        stylers: [{ color: "#17263c" }],
      },
      {
        featureType: "water",
        elementType: "labels.text.fill",
        stylers: [{ color: "#515c6d" }],
      },
      {
        featureType: "water",
        elementType: "labels.text.stroke",
        stylers: [{ color: "#17263c" }],
      },
    ],
  });
}
</script>
