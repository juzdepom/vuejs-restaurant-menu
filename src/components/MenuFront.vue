<template>
    <div class="rm-cover">
        <div class="rm-front">
                <div class="rm-content">

                    <div class="rm-logo"></div>
                    <h2>Gourmet Castle</h2>
                    <h3>Fine Dining &amp; Gourmet Takeaway</h3>

                    <a href="#" class="rm-button-open" @click="openMenu">View the Menu</a>
                    <div class="rm-info">
                        <p>
                        <strong>Gourmet Castle Restaurant</strong><br>
                        246 Wonderful Paradise Ln.<br>
                        Pasadena, CA 91101<br>
                        <strong>Phone</strong> 626.511.1170<br>
                        <strong>Fax</strong> 626.992.1020</p>
                    </div>
                </div><!-- /rm-content -->
        </div><!-- /rm-front -->
    </div>
</template>

<script>
export default {
  methods: {
      openMenu(){
          var container = $( '#rm-container' )
          container.addClass( 'rm-open' )
      }
  }
}
</script>

