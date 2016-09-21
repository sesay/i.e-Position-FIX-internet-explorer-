# i.e-Position-FIX-internet-explorer-

// Fix Internet Explorer "Position Fixed issue"

<!-- fix header i.e -->
    <style type="text/css">
    .global-header-bg {
        /* Netscape 4, IE 4.x-5.0/Win and other lesser browsers will use this */
        position: absolute;
        left:0;
        top:0;
    }
    body .global-header-bg {
        /* used by Opera 5+, Netscape6+/Mozilla, Konqueror, Safari, OmniWeb 4.5+, iCab, ICEbrowser */
        position: fixed;
    }
    </style>
    <!--[if gte IE 5.5]>
<![if lt IE 7]>
<style type="text/css">
.global-header-bg {
  /* IE5.5+/Win - this is more specific than the IE 5.0 version */
  left: expression( ( 20 + ( ignoreMe2 = document.documentElement.scrollLeft ? document.documentElement.scrollLeft : document.body.scrollLeft ) ) + 'px' );
  top: expression( ( 10 + ( ignoreMe = document.documentElement.scrollTop ? document.documentElement.scrollTop : document.body.scrollTop ) ) + 'px' );
}
</style>
<![endif]>
<![endif]-->
<!-- /fix -->
