<!DOCTYPE html>
<html lang="en" dir="ltr">
    <head>
        <title>Demo: 2 applets communicating - GeoGebra</title>        <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1, user-scalable=yes">

                <!-- Chrome, Firefox OS and Opera -->
        <meta name="theme-color" content="#6161FF">
        <!-- Windows Phone -->
        <meta name="msapplication-navbutton-color" content="#6161FF">
        <!-- iOS Safari -->
        <meta name="apple-mobile-web-app-capable" content="yes">
        <meta name="apple-mobile-web-app-status-bar-style" content="#6161FF">

        <meta property="og:title" content="Demo: 2 applets communicating" />
<meta property="og:description" content="Demo: 2 applets communicating
" />
<meta property="og:site_name" content="GeoGebra" />
<meta property="og:type" content="article" />
<meta property="og:image" content="https://cdn.geogebra.org/resource/dnsmqsty/cEVOuGNpyOfiqnfE/material-dnsmqsty-thumb.png" />
<meta property="twitter:card" content="summary" />
<meta property="twitter:site" content="@geogebra" />
<meta property="fb:app_id" content="185307058177853" />
<meta property="article:published_time" content="2022-06-29" />
<meta property="article:publisher" content="https://www.facebook.com/geogebra" />
        <link rel="stylesheet" type="text/css" href="GeoGebra/includes/css/structure.ltr.css?v=1714646928" />
        <link rel="stylesheet" type="text/css" href="GeoGebra/includes/css/screen.ltr.css?v=1714646928" media="screen and (min-width: 769px)" />
        <link rel="stylesheet" type="text/css" href="GeoGebra/includes/css/tablet.ltr.css?v=1714646928" media="screen and (min-width: 641px) and (max-width: 768px)" />
        <link rel="stylesheet" type="text/css" href="GeoGebra/includes/css/phone.ltr.css?v=1714646928" media="screen and (min-width: 0px) and (max-width: 640px)" />
        <link rel="stylesheet" type="text/css" href="GeoGebra/css/general.ltr.css?v=1714646928" />
                <link rel="stylesheet" type="text/css" href="GeoGebra/css/worksheet/ws.view.ltr.css?v=1714646928" />

        <link href="GeoGebra/css/wysibb/default/wbbtheme.css" media="screen" rel="stylesheet" type="text/css" />
<link href="GeoGebra/css/wysibb/wysibb.css" media="screen" rel="stylesheet" type="text/css" />
<link href="GeoGebra/css/group/groups.ltr.css?v=1714646928" media="screen" rel="stylesheet" type="text/css" />
<link href="GeoGebra/css/compiled.css?v=1714646928" media="screen" rel="stylesheet" type="text/css" />
                    <script type="text/javascript" src="GeoGebra/scripts/jquery.min.js?v=1714646928"></script>
        
        <script type="text/javascript" src="GeoGebra/scripts/jquery.simplemodal.js?v=1714646928"></script>
        <script type="text/javascript" src="GeoGebra/scripts/worksheet/ws-header-footer.js?v=1714646928"></script>


        <script type="text/javascript" src="GeoGebra/scripts/jlatexmath/texthandlers.js?v=1714646928"></script>
<script type="text/javascript" src="GeoGebra/scripts/jlatexmath/jlatexmath.js"></script>
<script type="text/javascript" src="GeoGebra/scripts/jlatexmath/jlatexmath-tube.js"></script>
<script type="text/javascript">
    //<![CDATA[
    window.GGBT_texthandlers.setLatexRenderer("jlatexmath");    //]]>
</script>
<script type="text/javascript">
    //<![CDATA[
    
                function escapeHtml(text) {
                  return text
                      .replace(/(&)/g, "&amp;")
                      .replace(/(<)/g, "&lt;") 
                      .replace(/(>)/g, "&gt;")
                      .replace(/(")/g, "&quot;")
                      .replace(/(')/g, "&#039;");
                }

                function GGBT_parseLatexes() {
                  if (window.GGBT_texthandlers.isLatexRenderer("mathquill")) {
                        $(".mathquill-embedded-latex").mathquill();
                    } else {
                        window.GGBT_jlatexmath.drawLatexOnjQuery($(".jlatexmath"));
                    }
                }
                jQuery(document).ready(function(e) {
                    var content = $(".bbcode-text");
                    content.each(function(index) {
                        var html = window.GGBT_texthandlers.getHTMLFromBBCode(escapeHtml($(this).text())),
                            t = $(this);
                            t.removeClass("bbcode-text");
                            t.html(html);
                    });
                    if (window.GGBT_ws_header_footer) {
                        window.GGBT_ws_header_footer.setWsScrollerHeight();
                    }
                });
                 jQuery(window).on("resize",function(e) {
                    GGBT_parseLatexes();
                });
                document.addEventListener("DOMContentLoaded", function(e) {
                    window.GGBT_parseLatexes();
                });
                //]]>
</script>
<script type="text/javascript" src="GeoGebra/scripts/general.original.js"></script>
<script type="text/javascript" src="GeoGebra/scripts/general.original.js?v=1714646928"></script>
<script type="text/javascript" src="GeoGebra/scripts/worksheet/general.js?v=1714646928"></script>
<script type="text/javascript" src="GeoGebra/scripts/worksheet/view.js?v=1714646928"></script>
<script type="text/javascript">
    //<![CDATA[
    
                    window.GGBT_wsf_view.setDefaults({
                        input: {
                            text: {
                                toolbar: {"math":{"text":"Math","title":"Insert Math"},"icons":{"text":"Icons","title":"Insert icons of GeoGebra tools"},"text":{"title":"Text tools"}},
                                dlg_math: {"title":"Edit Math","btn_basic":"Basic","btn_greek":"Greek","btn_operators":"Operators","btn_relationships":"Relationships","btn_arrows":"Arrows","btn_delimiters":"Delimiters","btn_misc":"Misc"},
                                dlg_icons: {"title":"Choose an Icon"},
                                wysibb_lang: ""
                            }
                        },
                        useplaybutton: true
                    });
    
                    //]]>
</script>
<script type="text/javascript" src="GeoGebra/scripts/spin.js?v=1714646928"></script>
<script type="text/javascript" src="GeoGebra/scripts/spinner.js?v=1714646928"></script>
<script type="text/javascript" src="GeoGebra/scripts/deployggb.js"></script>
<script type="text/javascript" src="GeoGebra/scripts/objects/timeago/jquery.timeago.js?v=1714646928"></script>
<script type="text/javascript">
    //<![CDATA[
    
            jQuery.timeago.settings.cutoff = 7*24*60*60*1000;
            jQuery.timeago.settings.allowFuture = true;
            //]]>
</script>
<script type="text/javascript" src="GeoGebra/scripts/objects/timeago/locales/jquery.timeago.en.js?v=1714646928"></script>        <script type="text/javascript">
            //<![CDATA[
            var ROOT_URL = 'https://www.geogebra.org';
            var BASE_URL = 'https://www.geogebra.org';
            var lang_confirm = "Are you sure you want to carry out this operation? It probably can not be undone!";
            var age_label = "Age:";
            //]]>
        </script>

    </head>

    <body class="ws">
    <script>
    var _paq = window._paq = window._paq || [];
    _paq.push(["setDocumentTitle", document.domain + "/" + document.title]);
    _paq.push(["setExcludedQueryParams", ["\/u\/"]]);
    _paq.push(["disableCookies"]);
    _paq.push(['trackPageView']);
    _paq.push(['enableLinkTracking']);
    (function() {
        var u="//matomo.geogebra.org/";
        _paq.push(['setTrackerUrl', u+'matomo.php']);
        _paq.push(['setSiteId', '12']);
        var d=document, g=d.createElement('script'), s=d.getElementsByTagName('script')[0];
        g.async=true; g.src=u+'matomo.js'; s.parentNode.insertBefore(g,s);
    })();
</script>
<script>
    var _mtm = window._mtm = window._mtm || [];
    _mtm.push({'mtm.startTime': (new Date().getTime()), 'event': 'mtm.Start'});
    (function() {
        var d=document, g=d.createElement('script'), s=d.getElementsByTagName('script')[0];
        g.async=true; g.src='https://matomo.geogebra.org/js/container_SH8ChHMF.js'; s.parentNode.insertBefore(g,s);
    })();
</script>
    
<div class="page" itemscope itemtype="http://schema.org/CreativeWork">
    <div style="direction: ltr">

        
            <div class="wsf-ws-scroller " data-id="42907556" data-mode="view" data-taskisro="true" data-taskissaveable="false" data-grouptype="" >
                <div class="wsf-wrapper">

                    
                    <!-- APPENDWORKSHEETSCRIPTS starts --><!-- APPENDWORKSHEETSCRIPTS ends -->
<div class="worksheet_tbl" data-appmode="">
    <script type="text/javascript">
        window.worksheet_applet_ids_42907556 = [];
    </script>
    <h1 itemprop="headline" class="wsf-worksheet-title"
        >Demo: 2 applets communicating            </h1>
    
    <div id="worksheet_element_38636598" class="worksheet_element wsf-content-added content-added-content" data-mat-id="38636598" data-type="G" >

    
<div class="ws-element-header notitle">
    <ul class="wsf-buttons wsf-element-toolbar">

    </ul>
    <div class="clear"></div>
</div>

            <div style="padding: 0" class="ws-element-applet">

                <div class="applet_container" id="applet_container_42907557">
    </div>
<script type="text/javascript">
    var parameters = {"id":"ggbApplet42907557","height":"271","width":"519","allowStyleBar":false,"allowUpscale":false,"apiUrl":"https://api.geogebra.org","appname":"classic","canary":false,"enableLabelDrags":false,"enableRightClick":false,"enableShiftDragZoom":true,"errorDialogsActive":true,"fixApplet":false,"ggbBase64":"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AgQIECBAgAABAgQaCAjYDRAtQYAAAQIECBAgQIAAAQIEBGx7gAABAgQIECBAgAABAgQINBAQsBsgWoIAAQIECBAgQIAAAQIECAjY9gABAgQIECBAgAABAgQIEGggIGA3QLQEAQIECBAgQIAAAQIECBAQsO0BAgQIECBAgAABAgQIECDQQEDAboBoCQIECBAgQIAAAQIECBAgIGDbAwQIECBAgAABAgQIECBAoIGAgN0A0RIECBAgQIAAAQIECBAgQEDAtgcIECBAgAABAgQIECBAgEADAQG7AaIlCBAgQIAAAQIECBAgQICAgG0PECBAgAABAgQIECBAgACBBgICdgNESxAgQIAAAQIECBAgQIAAAQHbHiBAgAABAgQIECBAgAABAg0EBOwGiJYgQIAAAQIECBAgQIAAAQICtj1AgAABAgQIECBAgAABAgQaCAjYDRAtQYAAAQIECBAgQIAAAQIEBGx7gAABAgQIECBAgAABAgQINBAQsBsgWoIAAQIECBAgQIAAAQIECAjY9gABAgQIECBAgAABAgQIEGggIGA3QLQEAQIECBAgQIAAAQIECBAQsO0BAgQIECBAgAABAgQIECDQQEDAboBoCQIECBAgQIAAAQIECBAgIGDbAwQIECBAgAABAgQIECBAoIGAgN0A0RIECBAgQIAAAQIECBAgQEDAtgcIECBAgAABAgQIECBAgEADAQG7AaIlCBAgQIAAAQIECBAgQICAgG0PECBAgAABAgQIECBAgACBBgICdgNESxAgQIAAAQIECBAgQIAAAQHbHiBAgAABAgQIECBAgAABAg0EBOwGiJYgQIAAAQIECBAgQIAAAQICtj1AgAABAgQIECBAgAABAgQaCAjYDRAtQYAAAQIECBAgQIAAAQIEBGx7gAABAgQIECBAgAABAgQINBAQsBsgWoIAAQIECBAgQIAAAQIECAjY9gABAgQIECBAgAABAgQIEGggIGA3QLQEAQIECBAgQIAAAQIECBAQsO0BAgQIECBAgAABAgQIECDQQEDAboBoCQIECBAgQIAAAQIECBAgIGDbAwQIECBAgAABAgQIECBAoIGAgN0A0RIECBAgQIAAAQIECBAgQEDAtgcIECBAgAABAgQIECBAgEADAQG7AaIlCBAgQIAAAQIECBAgQICAgG0PECBAgAABAgQIECBAgACBBgICdgNESxAgQIAAAQIECBAgQIAAAQHbHiBAgAABAgQIECBAgAABAg0EBOwGiJYgQIAAAQIECBAgQIAAAQICtj1AgAABAgQIECBAgAABAgQaCAjYDRAtQYAAAQIECBAgQIAAAQIEBGx7gAABAgQIECBAgAABAgQINBAQsBsgWoIAAQIECBAgQIAAAQIECAjY9gABAgQIECBAgAABAgQIEGggIGA3QLQEAQIECBAgQIAAAQIECBAQsO0BAgQIECBAgAABAgQIECDQQEDAboBoCQIECBAgQIAAAQIECBAgIGDbAwQIECBAgAABAgQIECBAoIGAgN0A0RIECBAgQIAAAQIECBAgQEDAtgcIECBAgAABAgQIECBAgEADAQG7AaIlCBAgQIAAAQIECBAgQICAgG0PECBAgAABAgQIECBAgACBBgICdgNESxAgQIAAAQIECBAgQIAAAQHbHiBAgAABAgQIECBAgAABAg0EBOwGiJYgQIAAAQIECBAgQIAAAQICtj1AgAABAgQIECBAgAABAgQaCAjYDRAtQYAAAQIECBAgQIAAAQIEBGx7gAABAgQIECBAgAABAgQINBAQsBsgWoIAAQIECBAgQIAAAQIECAjY9gABAgQIECBAgAABAgQIEGggIGA3QLQEAQIECBAgQIAAAQIECBAQsO0BAgQIECBAgAABAgQIECDQQEDAboBoCQIECBAgQIAAAQIECBAgIGDbAwQIECBAgAABAgQIECBAoIGAgN0A0RIECBAgQIAAAQIECBAgQEDAtgcIECBAgAABAgQIECBAgEADAQG7AaIlCBAgQIAAAQIECBAgQICAgG0PECBAgAABAgQIECBAgACBBgICdgNESxAgQIAAAQIECBAgQIAAAQHbHiBAgAABAgQIECBAgAABAg0EBOwGiJYgQIAAAQIECBAgQIAAAQICtj1AgAABAgQIECBAgAABAgQaCAjYDRAtQYAAAQIECBAgQIAAAQIEBGx7gAABAgQIECBAgAABAgQINBAQsBsgWoIAAQIECBAgQIAAAQIECAjY9gABAgQIECBAgAABAgQIEGggIGA3QLQEAQIECBAgQIAAAQIECBAQsO0BAgQIECBAgAABAgQIECDQQEDAboBoCQIECBAgQIAAAQIECBAgIGDbAwQIECBAgAABAgQIECBAoIGAgN0A0RIECBAgQIAAAQIECBAgQEDAtgcIECBAgAABAgQIECBAgEADAQG7AaIlCBAgQIAAAQIECBAgQICAgG0PECBAgAABAgQIECBAgACBBgICdgNESxAgQIAAAQIECBAgQIAAAQHbHiBAgAABAgQIECBAgAABAg0EBOwGiJYgQIAAAQIECBAgQIAAAQICtj1AgAABAgQIECBAgAABAgQaCAjYDRAtQYAAAQIECBAgQIAAAQIEBGx7gAABAgQIECBAgAABAgQINBAQsBsgWoIAAQIECBAgQIAAAQIECAjY9gABAgQIECBAgAABAgQIEGggIGA3QLQEAQIECBAgQIAAAQIECBAQsO0BAgQIECBAgAABAgQIECDQQEDAboBoCQIECBAgQIAAAQIECBAgIGDbAwQIECBAgAABAgQIECBAoIGAgN0A0RIECBAgQIAAAQIECBAgQEDAtgcIECBAgAABAgQIECBAgEADAQG7AaIlCBAgQIAAAQIECBAgQICAgG0PECBAgAABAgQIECBAgACBBgICdgNESxAgQIAAAQIECBAgQIAAAQHbHiBAgAABAgQIECBAgAABAg0EBOwGiJYgQIAAAQIECBAgQIAAAQICtj1AgAABAgQIECBAgAABAgQaCAjYDRAtQYAAAQIECBAgQIAAAQIEBGx7gAABAgQIECBAgAABAgQINBAQsBsgWoIAAQIECBAgQIAAAQIECAjY9gABAgQIECBAgAABAgQIEGggIGA3QLQEAQIECBAgQIAAAQIECBAQsO0BAgQIECBAgAABAgQIECDQQEDAboBoCQIECBAgQIAAAQIECBAgIGDbAwQIECBAgAABAgQIECBAoIGAgN0A0RIECBAgQIAAAQIECBAgQEDAtgcIECBAgAABAgQIECBAgEADAQG7AaIlCBAgQIAAAQIECBAgQICAgG0PECBAgAABAgQIECBAgACBBgICdgNESxAgQIAAAQIECBAgQIAAAQHbHiBAgAABAgQIECBAgAABAg0EBOwGiJYgQIAAAQIECBAgQIAAAQICtj1AgAABAgQIECBAgAABAgQaCAjYDRAtQYAAAQIECBAgQIAAAQIEBGx7gAABAgQIECBAgAABAgQINBAQsBsgWoIAAQIECBAgQIAAAQIECAjY9gABAgQIECBAgAABAgQIEGggIGA3QLQEAQIECOQReOaZZ8p5551XXnjhhTJr1qwyadKkPM3phAAB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DAICdoYp6oEAAQIECBAgQIAAAQIEei4gYPd8BE6AAAECBAgQIECAAAECBDIICNgZpqgHAgQIECBAgAABAgQIEOi5gIDd8xE4AQIECPS3wOrVq8uSJUvKiy++WF577bXy6quvlpdeeqmsXLmy7LbbbmX33XcvI0eOLLvssksZP3582Xvvvfu7YWdPgAABAgQIEHgHAQHb1iBAgACBrRKoIboG60WLFpUnn3yyLF++vLzyyivljTfeKDvssEPZfvvty+uvv17eeuutLlyPGjWqjB49uhx++OHlkEMOKQcddNBW1fUlAgQIECBAgMBQFRCwh+pknBcBAgSGsMC9995b5s2bV5566qny/PPPlz333LPsscceZcSIEd3fhsebb75ZVq1aVVasWFGWLVvW/edx48Z1Qbv+HXjggUO4U6dGgAABAgQIENh8AQF78618kgABAtu8wJo1a8rtt99easCuwbpe7r3XXnt1v1hv7lF/6a5Bu/7aPXHixHL88ceXY445ZnO/7nMECBAgQIAAgSErIGAP2dE4MQIECAwtgRqob7zxxvLoo4+W7bbbrhx66KGb/Fq9JWe8dOnS7hLzeqn4YYcdVs4666wt+brPEiBAgAABAgSGnICAPeRG4oQIECAw9ATq5d3XXHNNeeSRR8qYMWPKwQcf/K4nWcN4/c4+++xTdtppp3f8bH0o2oIFC7pfwd///veXc889d+g174wIECBAgAABApspIGBvJpSPESBAYFsVqE8Dv/baa8uDDz7Y/Wr9nve8ZxOK+kt0vWz8mWeeKU8//XT3BPF1R703+4ADDuguJ58yZUoZO3bsJt+va9d/P/XUU8uxxx67rVLrmwABAgQIEOhzAQG7zwfo9AkQIDCYAvWe6zvuuKP7q08A32+//TYp96c//anMnDlzs06jhvPPfe5zm9xzXR+Eds8995RJkyaVz3zmM2Xy5MmbtZ4PESBAgAABAgSGkoCAPZSm4VwIECAwxATmzJlT7rzzzu7d1jX8bnjUS8CvvPLK7hfrLT1OPPHEct555230tfoe7ccff7wceeSR5fTTT+9+9XYQIECAAAECBPpJQMDup2k5VwIECAQK1Puob7jhhjJ//vzyoQ99aKN7qesl4F/96lcHdDaf+MQnyrRp0zZa47///W+pv5qfdtpp5YQTThjQ+r5MgAABAgQIEIgWELCjxdUjQIBAnwj84x//KL/73e9KvXy7vk5rw+P73/9+qWF4oMeMGTPKhAkT1i9Tg/sDDzzQhetzzjnnXR+QNtDavk+AAAECBAgQaC0gYLcWtR4BAgSSCFx//fWl3l9dn+49atSo9V3dfPPNXfBucdSnjF9yySXda7/WHfUy8ZEjR5azzz57k8vSW9S0BgECBAgQIEBgsAQE7MGStW6YQP3Fa/HixaVezrp27dqwugoRyCxQ//9Uw/Vzzz1XDjzwwPWtLlu2rHugWb2Mu9XxkY98pJx00knrl3vllVdKrXP00UeXo446qlUZ6yQU2GWXXcr48ePLvvvum7A7LREgQIBAPwoI2P04Nee8XuDf//53+dvf/lZWr15NhQCBhgI14Nanetdfljd8LdfChQtLvXS85bHzzjuXL3zhCxst+cQTT3S/Xh9zzDEtS1krqcD73ve+cvzxxyftTlsECBAg0E8CAnY/Tcu5biTwwgsvlJtuuokKAQKDIPDUU091AbteGr7rrruur/D3v/+9/Otf/2pe8YwzzihjxoxZv269v3uvvfbqftnecccdm9ezYD6Bww8/vNSrIRwECBAgQKCXAgJ2L/XVHpBAfXXQokWLBrSGLxMg8PYCNUTPnTu37L333mXEiBHrP/TrX/+6e2VX66NeDr7ha8D+97//deH+2GOP3egX9NZ1rZdHoF5tMX369LL99tvnaUonBAgQINB3AgJ2343MCa8TuPHGG8tLL70EhACBQRB49NFHy7x587r7r9c9gKzeGz1YV43Up5RveInvs88+W3bYYYfundjurx2EASddcurUqfZL0tlqiwABAv0iIGD3y6Sc5yYCs2bNKitWrCBDgMAgCEQH7IMOOmij916vC9j1kt9x48YNQoeWzChw6qmnlv333z9ja3oiQIAAgT4RELD7ZFBOc1OBOXPmlPqQMwcBAu0F3ukS8XrlSH1yf+ujPi28vg5s3bF06dLu3u/jjjuu7L777q3LWS+pQH13en2yuIMAAQIECPRKQMDulby6AxZ45plnym233TbgdSxAgMCmAvUhZ3fffXfZbbfdNnrIWX1q/5NPPtmc7LTTTit77rnn+nVr/T322KNMmTLFQ86aa+dc8L3vfW858cQTczanKwIECBDoGwEBu29G5UTfTuChhx4q9913HxwCBBoL1Nd01YA9fPjwjR4y9s9//rM88MADTavVe63PPvvsMmzYsPXrek1XU+L0i9X79E855ZRuvzoIECBAgEAvBQTsXuqr3USgPm348ccfL88991xZu3ZtkzUtQmBbF3jxxRdLfVL/8uXLy3777bee4+mnny633HJLU556//WnPvWp9Wu+9tprpQb8+oCz+uolB4F3EqiXg0+YMKFMnjwZEgECBAgQGBICAvaQGIOTIECAwNATuP7668sdd9zRhdwN72u99tpry1133dXshC+99NLudWDrjnr/d33VUr2fdsP7spsVtBABAgQIECBAYJAEBOxBgrUsAQIE+l2gXgp+ww03dPdAjx8/fqN2vva1r5X6S/NAjwsuuKDUB5ytO1avXl3uv//+8uEPf7icf/75ZeTIkQMt4fsECBAgQIAAgTABATuMWiECBAj0l0B9VdbMmTPLY4891l2uveFRX+N11VVXDaihSZMmlW9+85sbrVGfHv7yyy+X+tCzk08+eUDr+zIBAgQIECBAIFpAwI4WV48AAQJ9JPDb3/623HvvvWXNmjWlPqV5w6M+BO2aa67Zqm7qE8Mvu+yyjb5b7/uuwf2II44oU6dOLYcccshWre1LBAgQIECAAIFeCQjYvZJXlwABAn0gUB8iePvtt5d58+Z176M++OCDNzrrV199tbuMvIbt+hTwzXnQ4EknnVTOPffcTbqfO3duOeCAA8oJJ5zg1+s+2BtOkQABAgQIENhUQMC2KwgQIEDgXQUWL15cZs+eXebPn18++MEPltGjR2/y+b/85S+lviO7vp/+rbfe2uR/rw9Jq69S+uQnP9ndX/3/HzXA13du10vRp02bZiIECBAgQIAAgb4UELD7cmxOmgABArEC9f3Xt956a3nkkUfKoYceWvbZZ5+3PYE33nij1F+969+KFSvK/vvvX/baa69SLwl/u6N+/uGHH+4eZlafGF7fh73rrrvGNqcaAQIECBAgQKCRgIDdCNIyBAgQyC5Q74++7bbbysKFC8vYsWO79w/X12lt7VHfXV8foDZu3Ljufuszzzyz7LHHHlu7nO8RIECAAAECBHouIGD3fAROgAABAv0jUENxffBZ/SV71apV3a/T9W+HHXbY7CaWL19eli1b1v1NnDixu9/6+OOP3+zv+yABAgQIECBAYKgKCNhDdTLOiwABAkNUoL7/+q677ureV/3000+Xepl3vQS8/vo8YsSI7m/D48033yyvv/56eeWVV7pQXQN2/dW6PtBsypQpZfLkyUO0U6dFgAABAgQIENgyAQF7y7x8mgABAgT+r8CSJUtK/VuwYEF5/vnnu+C8cuXKMnz48LLjjjt2l4/XX7lrAK//NmrUqDJmzJgyfvz4LlTXy8Lrf3cQIECAAAECBLIICNhZJqkPAgQI9EigPtCsBu16+fhLL73U/dVfresru7bbbrvuF+16z3Z9eFm9b7sG65122qlHZ6ssAQIECBAgQGDwBATswbO1MgECBLZJgfqrdb2MfPXq1aW+nqs+Iby+I9tBgAABAgQIEMguIGBnn7D+CBAgQIAAAQIECBAgQCBEQMAOYVaEAAECBAgQIECAAAECBLILCNjZJ6w/AgQIECBAgAABAgQIEAgRELBDmBUhQIAAAQIECBAgQIAAgewCAnb2CeuPAAECBAgQIECAAAECBEIEBOwQZkUIECBAgAABAgQIECBAILuAgJ19wvojQIAAAQIECBAgQIAAgRABATuEWRECBAgQIECAAAECBAgQyC4gYGefsP4IECBAgAABAgQIECBAIERAwA5hVoQAAQIECBAgQIAAAQIEsgsI2NknrD8CBAgQIECAAAECBAgQCBEQsEOYFSFAgAABAgQIECBAgACB7AICdvYJ648AAQIECBAgQIAAAQIEQgQE7BBmRQgQIECAAAECBAgQIEAgu4CAnX3C+iNAgAABAgQIECBAgACBEAEBO4RZEQIECBAgQIAAAQIECBDILiBgZ5+w/ggQIECAAAECBAgQIEAgREDADmFWhAABAgQIECBAgAABAgSyCwjY2SesPwIECBAgQIAAAQIECBAIERCwQ5gVIUCAAAECBAgQIECAAIHsAgJ29gnrjwABAgQIECBAgAABAgRCBATsEGZFCBAgQIAAAQIECBAgQCC7gICdfcL6I0CAAAECdy1zZQAAFpFJREFUBAgQIECAAIEQAQE7hFkRAgQIECBAgAABAgQIEMguIGBnn7D+CBAgQIAAAQIECBAgQCBEQMAOYVaEAAECBAgQIECAAAECBLILCNjZJ6w/AgQIECBAgAABAgQIEAgRELBDmBUhQIAAAQIECBAgQIAAgewCAnb2CeuPAAECBAgQIECAAAECBEIEBOwQZkUIECBAgAABAgQIECBAILuAgJ19wvojQIAAAQIECBAgQIAAgRABATuEWRECBAgQIECAAAECBAgQyC4gYGefsP4IECBAgAABAgQIECBAIERAwA5hVoQAAQIECBAgQIAAAQIEsgsI2NknrD8CBAgQIECAAAECBAgQCBEQsEOYFSFAgAABAgQIECBAgACB7AICdvYJ648AAQIECBAgQIAAAQIEQgQE7BBmRQgQIECAAAECBAgQIEAgu4CAnX3C+iNAgAABAgQIECBAgACBEAEBO4RZEQIECBAgQIAAAQIECBDILiBgZ5+w/ggQIECAAAECBAgQIEAgREDADmFWhAABAgQIECBAgAABAgSyCwjY2SesPwIECBAgQIAAAQIECBAIERCwQ5gVIUCAAAECBAgQIECAAIHsAgJ29gnrjwABAgQIECBAgAABAgRCBATsEGZFCBAgQIAAAQIECBAgQCC7gICdfcL6I0CAAAECBAgQIECAAIEQAQE7hFkRAgQIECBAgAABAgQIEMguIGBnn7D+CBAgQIAAAQIECBAgQCBEQMAOYVaEAAECBAgQIECAAAECBLILCNjZJ6w/AgQIECBAgAABAgQIEAgRELBDmBUhQIAAAQIECBAgQIAAgewCAnb2CeuPAAECBAgQIECAAAECBEIEBOwQZkUIECBAgAABAgQIECBAILuAgJ19wvojQIAAAQIECBAgQIAAgRABATuEWRECBAgQIECAAAECBAgQyC4gYGefsP4IECBAgAABAgQIECBAIERAwA5hVoQAAQIECBAgQIAAAQIEsgsI2NknrD8CBAgQIECAAAECBAgQCBEQsEOYFSFAgAABAgQIECBAgACB7AICdvYJ648AAQIECBAgQIAAAQIEQgQE7BBmRQgQIECAAAECBAgQIEAgu4CAnX3C+iNAgAABAgQIECBAgACBEAEBO4RZEQIECBAgQIAAAQIECBDILiBgZ5+w/ggQIECAAAECBAgQIEAgREDADmFWhAABAgQIECBAgAABAgSyCwjY2SesPwIECBAgQIAAAQIECBAIERCwQ5gVIUCAAAECBAgQIECAAIHsAgJ29gnrjwABAgQIECBAgAABAgRCBATsEGZFCBAgQIAAAQIECBAgQCC7gICdfcL6I0CAAAECBAgQIECAAIEQAQE7hFkRAgQIECBAgAABAgQIEMguIGBnn7D+CBAgQIAAAQIECBAgQCBEQMAOYVaEAAECBAgQIECAAAECBLILCNjZJ6w/AgQIECBAgAABAgQIEAgRELBDmBUhQIAAAQIECBAgQIAAgewCAnb2CeuPAAECBAgQIECAAAECBEIEBOwQZkUIECBAgAABAgQIECBAILuAgJ19wvojQIAAAQIECBAgQIAAgRABATuEWRECBAgQIECAAAECBAgQyC4gYGefsP4IECBAgAABAgQIECBAIERAwA5hVoQAAQIECBAgQIAAAQIEsgsI2NknrD8CBAgQIECAAAECBAgQCBEQsEOYFSFAgAABAgQIECBAgACB7AICdvYJ648AAQIECBAgQIAAAQIEQgQE7BBmRQgQIECAAAECBAgQIEAgu4CAnX3C+iNAgAABAgQIECBAgACBEAEBO4RZEQIECBAgQIAAAQIECBDILiBgZ5+w/ggQIECAAAECBAgQIEAgREDADmFWhAABAgQIECBAgAABAgSyCwjY2SesPwIECBAgQIAAAQIECBAIERCwQ5gVIUCAAAECBAgQIECAAIHsAgJ29gnrjwABAgQIECBAgAABAgRCBATsEGZFCBAgQIAAAQIECBAgQCC7gICdfcL6I0CAAAECBAgQIECAAIEQAQE7hFkRAgQIECBAgAABAgQIEMguIGBnn7D+CBAgQIAAAQIECBAgQCBEQMAOYVaEAAECBAgQIECAAAECBLILCNjZJ6w/AgQIECBAgAABAgQIEAgRELBDmBUhQIAAAQIECBAgQIAAgewCAnb2CeuPAAECBAgQIECAAAECBEIEBOwQZkUIECBAgAABAgQIECBAILuAgJ19wvojQIAAAQIECBAgQIAAgRABATuEWRECBAgQIECAAAECBAgQyC4gYGefsP4IECBAgAABAgQIECBAIERAwA5hVoQAAQIECBAgQIAAAQIEsgsI2NknrD8CBAgQIECAAAECBAgQCBEQsEOYFSFAgAABAgQIECBAgACB7AICdvYJ648AAQIECBAgQIAAAQIEQgQE7BBmRQgQIECAAAECBAgQIEAgu4CAnX3C+iNAgAABAgQIECBAgACBEAEBO4RZEQIECBAgQIAAAQIECBDILiBgZ5+w/ggQIECAAAECBAgQIEAgREDADmFWhAABAgQIECBAgAABAgSyCwjY2SesPwIECBAgQIAAAQIECBAIERCwQ5gVIUCAAAECBAgQIECAAIHsAgJ29gnrjwABAgQIECBAgAABAgRCBATsEGZFCBAgQIAAAQIECBAgQCC7gICdfcL6I0CAAAECBAgQIECAAIEQAQE7hFkRAgQIECBAgAABAgQIEMguIGBnn7D+CBAgQIAAAQIECBAgQCBEQMAOYVaEAAECBAgQIECAAAECBLILCNjZJ6w/AgQIECBAgAABAgQIEAgRELBDmBUhQIAAAQIECBAgQIAAgewCAnb2CeuPAAECBAgQIECAAAECBEIEBOwQZkUIECBAgAABAgQIECBAILuAgJ19wvojQIAAAQIECBAgQIAAgRABATuEWRECBAgQIECAAAECBAgQyC4gYGefsP4IECBAgAABAgQIECBAIERAwA5hVoQAAQIECBAgQIAAAQIEsgsI2NknrD8CBAgQIECAAAECBAgQCBEQsEOYFSFAgAABAgQIECBAgACB7AICdvYJ648AAQIECBAgQIAAAQIEQgQE7BBmRQgQIECAAAECBAgQIEAgu4CAnX3C+iNAgAABAgQIECBAgACBEAEBO4RZEQIECBAgQIAAAQIECBDILiBgZ5+w/ggQIECAAAECBAgQIEAgREDADmFWhAABAgQIECBAgAABAgSyCwjY2SesPwIECBAgQIAAAQIECBAIERCwQ5gVIUCAAAECBAgQIECAAIHsAgJ29gnrjwABAgQIECBAgAABAgRCBATsEGZFCBAgQIAAAQIECBAgQCC7gICdfcL6I0CAAAECBAgQIECAAIEQAQE7hFkRAgQIECBAgAABAgQIEMguIGBnn7D+CBAgQIAAAQIECBAgQCBEQMAOYVaEAAECBAgQIECAAAECBLILCNjZJ6w/AgQIECBAgAABAgQIEAgRELBDmBUhQIAAAQIECBAgQIAAgewCAnb2CeuPAAECBAgQIECAAAECBEIEBOwQZkUIECBAgAABAgQIECBAILuAgJ19wvojQIAAAQIECBAgQIAAgRABATuEWRECBAgQIECAAAECBAgQyC4gYGefsP4IECBAgAABAgQIECBAIERAwA5hVoQAAQIECBAgQIAAAQIEsgsI2NknrD8CBAgQIECAAAECBAgQCBEQsEOYFSFAgAABAgQIECBAgACB7AICdvYJ648AAQIECBAgQIAAAQIEQgQE7BBmRQgQIECAAAECBAgQIEAgu4CAnX3C+iNAgAABAgQIECBAgACBEAEBO4RZEQIECBAgQIAAAQIECBDILiBgZ5+w/ggQIECAAAECBAgQIEAgREDADmFWhAABAgQIECBAgAABAgSyCwjY2SesPwIECBAgQIAAAQIECBAIERCwQ5gVIUCAAAECBAgQIECAAIHsAgJ29gnrjwABAgQIECBAgAABAgRCBATsEGZFCBAgQIAAAQIECBAgQCC7gICdfcL6I0CAAAECBAgQIECAAIEQAQE7hFkRAgQIECBAgAABAgQIEMguIGBnn7D+CBAgQIAAAQIECBAgQCBEQMAOYVaEAAECBAgQIECAAAECBLILCNjZJ6w/AgQIECBAgAABAgQIEAgRELBDmBUhQIAAAQIECBAgQIAAgewCAnb2CeuPAAECBAgQIECAAAECBEIEBOwQZkUIECBAgAABAgQIECBAILuAgJ19wvojQIAAAQIECBAgQIAAgRABATuEWRECBAgQIECAAAECBAgQyC4gYGefsP4IECBAgAABAgQIECBAIERAwA5hVoQAAQIECBAgQIAAAQIEsgsI2NknrD8CBAgQIECAAAECBAgQCBEQsEOYFSFAgAABAgQIECBAgACB7AICdvYJ648AAQIECBAgQIAAAQIEQgQE7BBmRQgQIECAAAECBAgQIEAgu4CAnX3C+iNAgAABAgQIECBAgACBEAEBO4RZEQIECBAgQIAAAQIECBDILiBgZ5+w/ggQIECAAAECBAgQIEAgREDADmFWhAABAgQIECBAgAABAgSyCwjY2SesPwIECBAgQIAAAQIECBAIERCwQ5gVIUCAAAECBAgQIECAAIHsAgJ29gnrjwABAgQIECBAgAABAgRCBATsEGZFCBAgQIAAAQIECBAgQCC7gICdfcL6I0CAAAECBAgQIECAAIEQAQE7hFkRAgQIECBAgAABAgQIEMguIGBnn7D+CBAgQIAAAQIECBAgQCBEQMAOYVaEAAECBAgQIECAAAECBLILCNjZJ6w/AgQIECBAgAABAgQIEAgRELBDmBUhQIAAAQIECBAgQIAAgewCAnb2CeuPAAECBAgQIECAAAECBEIEBOwQZkUIECBAgAABAgQIECBAILuAgJ19wvojQIAAAQIECBAgQIAAgRABATuEWRECBAgQIECAAAECBAgQyC4gYGefsP4IECBAgAABAgQIECBAIERAwA5hVoQAAQIECBAgQIAAAQIEsgsI2NknrD8CBAgQIECAAAECBAgQCBEQsEOYFSFAgAABAgQIECBAgACB7AICdvYJ648AAQIECBAgQIAAAQIEQgQE7BBmRQgQIECAAAECBAgQIEAgu4CAnX3C+iNAgAABAgQIECBAgACBEAEBO4RZEQIECBAgQIAAAQIECBDILiBgZ5+w/ggQIECAAAECBAgQIEAgREDADmFWhAABAgQIECBAgAABAgSyCwjY2SesPwIECBAgQIAAAQIECBAIERCwQ5gVIUCAAAECBAgQIECAAIHsAgJ29gnrjwABAgQIECBAgAABAgRCBATsEGZFCBAgQIAAAQIECBAgQCC7gICdfcL6I0CAAAECBAgQIECAAIEQAQE7hFkRAgQIECBAgAABAgQIEMguIGBnn7D+CBAgQIAAAQIECBAgQCBEQMAOYVaEAAECBAgQIECAAAECBLILCNjZJ6w/AgQIECBAgAABAgQIEAgRELBDmBUhQIAAAQIECBAgQIAAgewCAnb2CeuPAAECBAgQIECAAAECBEIEBOwQZkUIECBAgAABAgQIECBAILuAgJ19wvojQIAAAQIECBAgQIAAgRABATuEWRECBAgQIECAAAECBAgQyC4gYGefsP4IECBAgAABAgQIECBAIERAwA5hVoQAAQIECBAgQIAAAQIEsgsI2NknrD8CBAgQIECAAAECBAgQCBEQsEOYFSFAgAABAgQIECBAgACB7AICdvYJ648AAQIECBAgQIAAAQIEQgQE7BBmRQgQIECAAAECBAgQIEAgu4CAnX3C+iNAgAABAgQIECBAgACBEAEBO4RZEQIECBAgQIAAAQIECBDILiBgZ5+w/ggQIECAAAECBAgQIEAgREDADmFWhAABAgQIECBAgAABAgSyCwjY2SesPwIECBAgQIAAAQIECBAIERCwQ5gVIUCAAAECBAgQIECAAIHsAgJ29gnrjwABAgQIECBAgAABAgRCBATsEGZFCBAgQIAAAQIECBAgQCC7gICdfcL6I0CAAAECBAgQIECAAIEQAQE7hFkRAgQIECBAgAABAgQIEMguIGBnn7D+CBAgQIAAAQIECBAgQCBEQMAOYVaEAAECBAgQIECAAAECBLILCNjZJ6w/AgQIECBAgAABAgQIEAgRELBDmBUhQIAAAQIECBAgQIAAgewCAnb2CeuPAAECBAgQIECAAAECBEIEBOwQZkUIECBAgAABAgQIECBAILuAgJ19wvojQIAAAQIECBAgQIAAgRABATuEWRECBAgQIECAAAECBAgQyC4gYGefsP4IECBAgAABAgQIECBAIERAwA5hVoQAAQIECBAgQIAAAQIEsgsI2NknrD8CBAgQIECAAAECBAgQCBEQsEOYFSFAgAABAgQIECBAgACB7AICdvYJ648AAQIECBAgQIAAAQIEQgQE7BBmRQgQIECAAAECBAgQIEAgu4CAnX3C+iNAgAABAgQIECBAgACBEAEBO4RZEQIECBAgQIAAAQIECBDILiBgZ5+w/ggQIECAAAECBAgQIEAgREDADmFWhAABAgQIECBAgAABAgSyCwjY2SesPwIECBAgQIAAAQIECBAIERCwQ5gVIUCAAAECBAgQIECAAIHsAgJ29gnrjwABAgQIECBAgAABAgRCBATsEGZFCBAgQIAAAQIECBAgQCC7gICdfcL6I0CAAAECBAgQIECAAIEQAQE7hFkRAgQIECBAgAABAgQIEMguIGBnn7D+CBAgQIAAAQIECBAgQCBEQMAOYVaEAAECBAgQIECAAAECBLILCNjZJ6w/AgQIECBAgAABAgQIEAgRELBDmBUhQIAAAQIECBAgQIAAgewCAnb2CeuPAAECBAgQIECAAAECBEIEBOwQZkUIECBAgAABAgQIECBAILuAgJ19wvojQIAAAQIECBAgQIAAgRABATuEWRECBAgQIECAAAECBAgQyC4gYGefsP4IECBAgAABAgQIECBAIERAwA5hVoQAAQIECBAgQIAAAQIEsgsI2NknrD8CBAgQIECAAAECBAgQCBEQsEOYFSFAgAABAgQIECBAgACB7AICdvYJ648AAQIECBAgQIAAAQIEQgQE7BBmRQgQIECAAAECBAgQIEAgu4CAnX3C+iNAgAABAgQIECBAgACBEAEBO4RZEQIECBAgQIAAAQIECBDILiBgZ5+w/ggQIECAAAECBAgQIEAgREDADmFWhAABAgQIECBAgAABAgSyCwjY2SesPwIECBAgQIAAAQIECBAIERCwQ5gVIUCAAAECBAgQIECAAIHsAgJ29gnrjwABAgQIECBAgAABAgRCBATsEGZFCBAgQIAAAQIECBAgQCC7gICdfcL6I0CAAAECBAgQIECAAIEQAQE7hFkRAgQIECBAgAABAgQIEMguIGBnn7D+CBAgQIAAAQIECBAgQCBEQMAOYVaEAAECBAgQIECAAAECBLILCNjZJ6w/AgQIECBAgAABAgQIEAgRELBDmBUhQIAAAQIECBAgQIAAgewCAnb2CeuPAAECBAgQIECAAAECBEIEBOwQZkUIECBAgAABAgQIECBAILuAgJ19wvojQIAAAQIECBAgQIAAgRABATuEWRECBAgQIECAAAECBAgQyC4gYGefsP4IECBAgAABAgQIECBAIERAwA5hVoQAAQIECBAgQIAAAQIEsgsI2NknrD8CBAgQIECAAAECBAgQCBH4P++tasT6Zs5CAAAAAElFTkSuQmCCUEsBAhQAFAAAAAgAqUHdVHNkA/0NBQAAISYAABcAAAAAAAAAAAAAAAAAAAAAAGdlb2dlYnJhX2RlZmF1bHRzMmQueG1sUEsBAhQAFAAAAAgAqUHdVOcVowd3AwAANxEAABcAAAAAAAAAAAAAAAAAQgUAAGdlb2dlYnJhX2RlZmF1bHRzM2QueG1sUEsBAhQAFAAAAAgAqUHdVEFTjB88AAAARgAAABYAAAAAAAAAAAAAAAAA7ggAAGdlb2dlYnJhX2phdmFzY3JpcHQuanNQSwECFAAUAAAACACpQd1UdHUV64MGAABFEQAADAAAAAAAAAAAAAAAAABeCQAAZ2VvZ2VicmEueG1sUEsBAhQAFAAAAAAAqUHdVA5uqM/jNgAA4zYAABYAAAAAAAAAAAAAAAAACxAAAGdlb2dlYnJhX3RodW1ibmFpbC5wbmdQSwUGAAAAAAUABQBMAQAAIkcAAAAA","isPreloader":false,"language":"en","playButton":false,"playButtonAutoDecide":true,"prerelease":false,"preventFocus":true,"scale":"1","screenshotGenerator":false,"showAlgebraInput":false,"showFullscreenButton":false,"showMenuBar":false,"showResetIcon":true,"showSplash":false,"showToolBar":false,"showToolBarHelp":false,"showZoomButtons":false,"useBrowserForJS":false};
    parameters.appletOnLoad = function() {
        if (typeof $ === "function" && window.GGBT_wsf_view !== undefined) {
            var container =  $("#applet_container_42907557");
            window.GGBT_wsf_view.postProcessApplet(container.parents('.content-added-content'));
        }
    };
    /** is3D=is 3D applet using 3D view, AV=Algebra View, SV=Spreadsheet View, CV=CAS View, EV2=Graphics View 2, CP=Construction Protocol, PC=Probability Calculator, DA=Data Analysis, FI=Function Inspector, macro=Macro View */
    var views = {"is3D":0,"AV":0,"SV":0,"CV":0,"EV2":0,"CP":0,"PC":0,"DA":0,"FI":0,"PV":0,"macro":0};
    var applet_42907557 = new GGBApplet('5.0', parameters, views, true);

    if ((navigator.appVersion.indexOf('MSIE')+1?parseFloat(navigator.appVersion.split('MSIE')[1]):999) < 11) { // WebGL is supported since IE 11
        applet_42907557.setHTML5Codebase('GeoGebra/HTML5/5.0/web/', 'true');
    } else {
        applet_42907557.setHTML5Codebase('GeoGebra/HTML5/5.0/web3d/', 'true');
    }
    applet_42907557.setPreviewImage(null, 'GeoGebra/images/GeoGebra_loading.png', null);
    var appletType_42907557 = 'auto';
    $(function($) {
        applet_42907557.inject('applet_container_42907557', 'auto');
    });
</script>
            <script type="text/javascript">
                window.worksheet_applet_ids_42907556.push(42907557);
            </script>
        </div>

            
        
    </div>

    <div id="worksheet_element_38636599" class="worksheet_element wsf-content-added content-added-content" data-mat-id="38636599" data-type="G" >

    
<div class="ws-element-header notitle">
    <ul class="wsf-buttons wsf-element-toolbar">

    </ul>
    <div class="clear"></div>
</div>

            <div style="padding: 0" class="ws-element-applet">

                <div class="applet_container" id="applet_container_42907558">
    </div>
<script type="text/javascript">
    var parameters = {"id":"ggbApplet42907558","height":"269","width":"517","allowStyleBar":false,"allowUpscale":false,"apiUrl":"https://api.geogebra.org","appname":"classic","canary":false,"enableLabelDrags":false,"enableRightClick":false,"enableShiftDragZoom":false,"errorDialogsActive":true,"fixApplet":false,"ggbBase64":"UEsDBBQAAAAIAJpB3VRzZAP9DQUAACEmAAAXAAAAZ2VvZ2VicmFfZGVmYXVsdHMyZC54bWztWl9z4jYQf+59Co2e2oeADRhIJs5N7mY6zUwud9NkOn0VRhg1QnItOfz59F1JxjYBcgl/AlwvDxErS2vt77darSRffpyMOHqiqWJShNiveRhREck+E3GIMz046+KPVx8uYypj2ksJGsh0RHSIA9Oy6AdSreN3TR1JkhBHnCjFIowSTrTpEuIxRmii2IWQd2REVUIieh8N6Yjcyohoq2WodXJRr4/H49r8fTWZxnVQqeoT1a/Hsa5BiREMWqgQ5z8uQO9C73HT9mt4nl//+8ute88ZE0oTEVGMwKA+HZCMawU/KacjKjTS04SGOJFMaIw46VEe4m9GQr8OUkp/wyjvBDh5+OrDL5dqKMdI9v6hEdTpNAPVeT8r1E0bePxZcpmiNMSdDkYAqyl6IW4EAcDFkyEJsecaczKlKXoioCGvIZmWke1vaweEq1yxfdMX2afuSStvLxjwA3AipSkw4dV8jFRCaR9GjXMb4QcQM7UcVzRa0+/ZLNcYVGv1lOfV+cAiKdO+QpMQ35E7jKZ5OXMlNLms58C+DuI+TajoQ6MFnP2NcG53Lc6mAJxNsW+YNwY513dQkNv/U5BhFu8B5a+iim1jI2z9BoQGMMmW7xUqTiJQ3Ig/aQxjrmLc/InxHj24tRG6kAmAPfD/+JC1YDkMlfkP6YocJZxO3hd4zkQJ4q0VCtAbm+UXVdBNKnaI3ALeuwp0Y62DTw9Z9CiogvwN3KLoZH78wfqwOFllEhJEpgFPv9N1Gui/YoE0BpwxaLM1EYNMRMaqAtzPWfpUZaPZ8g7BR6lz4xmwJzLWY6lobKQCl/u5XLr2ZindD+3aMtPcqL0RGnZUAAkMRC2N/JHS5AFUfRUPKRHKbKueOwpscNJqlMpRzyeQyKPe8qMtZk9Kpi+xHZwC2yfJ9Q4inngiacFElbXNMqq1a34N3ODA1L0h/FeB2D75OWX33cqJ2ptN/YbXWo1erXPETvQE5skShr9ysUwhTiKhe884uCILh7WLKkbEDvY0fBpXZvS3uVzw0XF8bG/Gm3edQdNyGoC2Z/7te+7Pb517vt+Go4OjdXcD8ML+xSDsKkqIXaL3/hAfbaq4Hs9ICnNaPt9/OKlAsvUzeLxpL0hZTIWLyBA/PKtjCgVonhnJXFNMfCtPoYCnM1NAte0OVqVsgq5dj2vX8LrhiqYrWq4IcvS+w2wCka2SJD9bG1qb7YhOKZLsn/OdpdXH5DwiG9G0Ehju5nLhO4ELDWBDtngwpTjrA9kjBnCeAc4jAgupScl7SvJMw90bXGmJ8u7NOdyY9fXQ5GAwvgGbGGIdemgoUzaTQhdgIeOv19ze0i2cVawiuvFSivmqqLXOp9d7cMVXtwvORMS8nIzXTioZcCf8ttHy+eDLxMBALC/tWqPb9LtB0+v4nfOg234lT3635Mk92I6mdfMR6FuejySNylNSyG/XMAm87ZTLfM31/E4raDbOG4F/ft6CHzD2XW8Efy8qyk3NMR4EWg9Yarq3Mz4uo0yVJ9dOKhACl/yhkhWSTRhnJJ0uv2lvCGs6KfOFBytUPj04QoDXmwKwx+XQbpxUud93xgwYoCjguxA4QbAvYeITiR7jVGYi9+zKCHZjer72HOP2qiclp7APnpv1aS5X7pWXFv51AOUL+CFnH3x/Ez325GRhrfrO5ZgqZ8CtFSr3vStmwOutXF6Qzg7uCpuczL3xpnJlglIloF75JKo+//7q6j9QSwMEFAAAAAgAmkHdVOcVowd3AwAANxEAABcAAABnZW9nZWJyYV9kZWZhdWx0czNkLnhtbO1Y3XLTOhC+PjyFRvfEVmIndacuk+FcnDMDTBluuFVtJRE4kpGUOO6r8Q48Eyut2jrQAumEMjD4wqsf76707aeV5LNnu3VDtsJYqVVJ2SilRKhK11ItS7pxi6cn9Nn5k7Ol0EtxaThZaLPmrqS5//JGD2qjGTvxbbxtS1o13FpZUdI23HmVknaUkJ2Vp0q/4mthW16JN9VKrPkLXXEXrKyca0+TpOu60bW/kTbLBEzaZGfrZLl0I5CUwKCVLWksnILdPe1uEvTGacqSty9foJ+nUlnHVSUogQnVYsE3jbNQFI1YC+WI61sBQ9dKVhPw0fBL0ZT0f+VglqLyQyTVxmxBPyqXdMLylJ4/+ees0trUluhdSQED3aO4QtEBsAAW9m2xb4t9HTZ22NiFxsQbtCvdEX35DhyX1JkNeI0DCpXwDXQ/1402xJR0DB4gYiwFeQmyGEMomnbFweKIpfiwrEgZm7Ix6je8F4ZsORiNXvnG6SqYDK0L3tjoKzh/qWuBPVn8Xklgg0fGOgFxB+e2FaIOJcQTpgUk6AOfhvakEm9c3wjiVrJ6r4SFeOYDJV/4T9a18LREHfFBoYr175K23ACVnAGiYb9cCrUFxLSxZJeGQfQgwNqVr3l67lio9yCg98oLaA7qMBMjd2SOGnP8cD5GMUGRocgjYmdJJM9XNOI7aSf/3gRtHqsD5qSTwJxDAw3uAUl4Q5T9cosx/lkRBfL8qpiSWBYw608fvw13WJgVN05YydVg+T73HV8iP/0dkP+ZuN8PJNhXYoDfRajv4Qdp9UH4FUUAcMxAAoRB3qSo/FgwLrjfu6IJIO/9CEVg7mNmTOmYoDE/x5z93cXf6qZfidpodYvjoOkWykmE8iEr51D4WT4J+Oe4QwwYPMri/pAX0zSbZkeLxUMpfRCyc1Ot5FrUgu9DC7vcY0E7Zrj7ZrMArRd/BrYXPWRgCdlgiOvjUTakCBh8gbiO/xjOXhhp1/uoskdEdYqJGFEtoPYboqqEu5nnK18eZtX8b1Y9BMsPG16HE1ec6uvr+hBTJOgxU+M0K/wzm7L8hGVwgzkSQMc4h8p128hKuh+6Wdx5r/CNeHnoUVyBiN4OvWqQ+RTFDMUJiuK7JxG7MQu4ad91Mo5d+0HOHhZk0LvzbDya/Sjrbw0/yul4qPTN03Ey+FGQXP+VOP8MUEsDBBQAAAAIAJpB3VTQGiQ9QwAAAFYAAAAWAAAAZ2VvZ2VicmFfamF2YXNjcmlwdC5qc0srzUsuyczPU0hPT/LP88zLLNHQVKjm4lIAgsw0BY3yzLyU/HKQEEgEBCAieokFBTmpJUYKtiCdjmCONVhNLRdXLQBQSwMEFAAAAAgAmkHdVLqNVjWDBgAARxEAAAwAAABnZW9nZWJyYS54bWy9WOuO00YU/g1PceRKCKTdjcf3QAJaUNVWWhBiC6r6b2JPkmEd27Unmyyl797vzNi5LFBBFwFrz3jmzLnfJpNn21VJ16rtdF1NPXHme6SqvC50tZh6azM/zbxnT+9PFqpeqFkraV63K2mmXsyQu3P4OktFxmuyaaZeXsqu07lHTSkNH5l6G490MfXSyE/HWRacxiJLTiM/mZ/KNMpO53EgZmoezxN/7BFtO/24ql/JleoamavLfKlW8qLOpbH0lsY0j0ejzWZzNnB2VreLEYh3o21XjBaL2RlGjyBe1U29fvIYeI9Ob0J7LvB9Mfrj5YWjc6qrzsgqVx6x6Gv99P69yUZXRb2hjS7MEgKL1KOl0osldBEkYHnEQA0U0qjc6GvV4ejBpxXerBrPgsmK9++5GZU7uTwq9LUuVDv1/DMxDqMgjMdpkmZjkWTCo7rVqjI9ML4t0dGAbnKt1cbh5ZklGYvAI1PX5UwyUvpIgmIfD4kxnVCSYiUgEVOElQwrKYW8FouIQmIQEVIUYYx4WSTY4W2849gnIbBDgU9BQIGgIMRnHFMMsJTPBoBNxhafj4ehwRGekNfCEI9dCyM8Ac+AKHZowEccJnYW23fGZ0AlBr2PZLewFo1BjhfiVFAITvCd+gS8QA+OrTSRT/wnKGIiQUpBRharxe9DR9e607NSTb25LDtYXlfzFu63++7MTamsEvuFvdXECf4DQn8AeOwjCJyzYMf3T/hJ8ES8wQY7sE50bBuYwodsYNCHmHZgdpPEbcFsvOazdjBYSXyfbYMhdjCQkj8hqR0cjLUfhvCuYg5Cht8iZHYgJODYfTCwZ2AIifnGBPzzEPWfEJkH63M+fMetZvyCO8GpEkrgD5jcUSbo5H/IdDeH2dGMBFRq5GzqnV/88vPzN+dfz4G4o+ADCyI+EDv2T+yffT4hGX6T1KZd35lichQgP1xgEcB3vwfNKPtqmpE/Rmn5DmoOU1SlnTdFWXYSptlJEIC2QF35hHAKXj6TjNyIoLXjD/cAnNkRdPi+nt5ALkig0f+Mq8loKJ2TXgXULRl6kNGoFboIVJUxpSElNnnZOooCigLiimkaUBpTyqlrKKkogRklPPZ1latqdlRXY666B8U14UUUME54ZOuiq7JBNBRazG2p5TJ8XGpRE6N9WQSDjEoQoZjbdDnUR3AR7CpkAPZREJFQUaIDSjhBf6FYoqGrO72z5lKVaPZ6HVk96qpZm2Pd5SvufKxpTH0LvKjzq+e3la1kh6ZqD4YGZ99HuYbnqM26NynlTJXoWC/ZFYiuZcnZwlKY15Whwe0yXpuMbEc3Ueu81IWW1TuYfuieXq1XM9XC5TCtWUaLhI/TvvWLD1u/1IHkdd0WlzcdHIW2f6oWhwOBtvjgHxR243bCWzs+FNvlkn089o93EKc3X9yylNX1pTIG0ncktwpe2mtu0XL8HHz81j2vy/1SU+vKvJCNWbe22QelloU6rxalspq0NkZHnF/N6u1lH0oO1+83DacYx8Fs8aIu65YQgkEM5QCZHVHWeLQwzNoOClEHGLwB0duJke72xRh5BhB2BAyPFgpGdqz1ooI/J2aPRW51Z9MGcB/5lPUQzgjrSpuL4cPo/GovKR9w9gdm67DHOHuQu+OcjG753uRKtZUqnR9VsOW6XnfOjR0ty8i6U6+lWZ5XxRu1QAi+lpwHDVA70D3Lhcr1Cgfdeq87yXZ9C1bdaqEWrRpELO0Vymm2jx7qmlbJolsqBT/v9eu8/BDMijOwP0ErUyqbu1caKeIU5lvJrW2XEBkIfhtQky5vdcMuSzNk6yu1d8pCd4xit8DQUEkH2RDudQX1GlYt7plrs6zhKzgjDa9wSJdqhfsRGeud1XqlWr6E9oaS9u4Fvtc990N0wxSIeccx3NZyjFHOurpcG1w+oahqf/l0uazPBui8cbecemN0KjdcXSDqXG8PRAKX+gOsujORdYpzp/JDq+2d2yzhRLjTsYdzVbbi9JNfdVEom34d88BF9ew9suGuADpx94ix/YXQI1k2SzCBy+aQpKKxL0SCW6PjSd5wOjxIqBb7y7o41qGs4HDWQEjMLDz3tQPb+BHgxqaYA2d+L6+lcwOqq7eNs6Ge08P+nv1Arpon9tVX7jPc7UtlxCP6+8FPW/nEvgj/jrfPOmXesYkfPvhrXZsn0g0nhF8Ezi0IfjH4HMSjRw7l/vVPH6vOqXh66Im2kPS/PTz9F1BLAwQUAAAAAACaQd1UEZAwZ7g2AAC4NgAAFgAAAGdlb2dlYnJhX3RodW1ibmFpbC5wbmeJUE5HDQoaCgAAAA1JSERSAAAD2wAAAgAIBgAAAJIHf4QAAAABc1JHQgCuzhzpAAAgAElEQVR4Xu3dfcyXZdkH8BMkBRHJF5SX6eN8iZASjRJDI3VObM5qk3SDVfOPlpuzLWvVaiubtTm31trU6eY/5dsKVkyk0spCRTELhVyELwi5LE1xgKiAwLPz2mDcvsQNnHL87uP+XNu9pz38fudxHZ/j9I/vrut3XUO2b9++vTgIECBAgAABAgQIECBAgACBZgJDhO1mlhYiQIAAAQIECBAgQIAAAQKdgLBtIxAgQIAAAQIECBAgQIAAgcYCwnZjUMsRIECAAAECBAgQIECAAAFh2x4gQIAAAQIECBAgQIAAAQKNBYTtxqCWI0CAAAECBAgQIECAAAECwrY9QIAAAQIECBAgQIAAAQIEGgsI241BLUeAAAECBAgQIECAAAECBIRte4AAAQIECBAgQIAAAQIECDQWELYbg1qOAAECBAgQIECAAAECBAgI2/YAAQIECBAgQIAAAQIECBBoLCBsNwa1HAECBAgQIECAAAECBAgQELbtAQIECBAgQIAAAQIECBAg0FhA2G4MajkCBAgQIECAAAECBAgQICBs2wMECBAgQIAAAQIECBAgQKCxgLDdGNRyBAgQIECAAAECBAgQIEBA2LYHCBAgQIAAAQIECBAgQIBAYwFhuzGo5QgQIECAAAECBAgQIECAgLBtDxAgQIAAAQIECBAgQIAAgcYCwnZjUMsRIECAAAECBAgQIECAAAFh2x4gQIAAAQIECBAgQIAAAQKNBYTtxqCWI0CAAAECBAgQIECAAAECwrY9QIAAAQIECBAgQIAAAQIEGgsI241BLUeAAAECBAgQIECAAAECBIRte4AAAQIECBAgQIAAAQIECDQWELYbg1qOAAECBAgQIECAAAECBAgI2/YAAQIECBAgQIAAAQIECBBoLCBsNwa1HAECBAgQIECAAAECBAgQELbtAQIECBAgQIAAAQIECBAg0FhA2G4MajkCBAgQIECAAAECBAgQICBs2wMECBAgQIAAAQIECBAgQKCxgLDdGNRyBAgQIECAAAECBAgQIEBA2LYHCBAgQIAAAQIECBAgQIBAYwFhuzGo5QgQIECAAAECBAgQIECAgLBtDxAgQIAAAQIECBAgQIAAgcYCwnZjUMsRIECAAAECBAgQIECAAAFh2x4gQIAAAQIECBAgQIAAAQKNBYTtxqCWI0CAAAECBAgQIECAAAECwrY9QIAAAQIECBAgQIAAAQIEGgsI241BLUeAAAECBAgQIECAAAECBIRte4AAAQIECBAgQIAAAQIECDQWELYbg1qOAAECBAgQIECAAAECBAgI2/YAAQIECBAgQIAAAQIECBBoLCBsNwa1HAECBAgQIECAAAECBAgQELbtAQIECBAgQIAAAQIECBAg0FhA2G4MajkCBAgQIECAAAECBAgQICBs2wMECBAgQIAAAQIECBAgQKCxgLDdGNRyBAgQIECAAAECBAgQIEBA2LYHCBAgQIAAAQIECBAgQIBAYwFhuzGo5QgQIECAAAECBAgQIECAgLBtDxAgQIAAAQIECBAgQIAAgcYCwnZjUMsRIECAAAECBAgQIECAAAFh2x4gQIAAAQIECBAgQIAAAQKNBYTtxqCWI0CAAAECBAgQIECAAAECwrY9QIAAAQIECBAgQIAAAQIEGgsI241BLUeAAAECBAgQIECAAAECBIRte4AAAQIECBAgQIAAAQIECDQWELYbg1qOAAECBAgQIECAAAECBAgI2/YAAQIECBAgQIAAAQIECBBoLCBsNwa1HAECBAgQIECAAAECBAgQELbtAQIECBAgQIAAAQIECBAg0FhA2G4MajkCBAgQIECAAAECBAgQICBs2wMECBAgQIAAAQIECBAgQKCxgLDdGNRyBAgQIECAAAECBAgQIEBA2LYHCBAgQIAAAQIECBAgQIBAYwFhuzGo5QgQIECAAAECBAgQIECAgLBtDxAgQIAAAQIECBAgQIAAgcYCwnZjUMsRIECAAAECBAgQIECAAAFh2x4gQIAAAQIECBAgQIAAAQKNBYTtxqCWI0CAAAECBAgQIECAAAECwrY9QIAAAQIECBAgQIAAAQIEGgsI241BLUeAAAECBAgQIECAAAECBIRte4AAAQIECBAgQIAAAQIECDQWELYbg1qOAAECBAgQIECAAAECBAgI2/YAAQIECBAgQIAAAQIECBBoLCBsNwa1HAECBAgQIECAAAECBAgQELbtAQIECBAgQIAAAQIECBAg0FhA2G4MajkCBAgQIECAAAECBAgQICBs2wMECBAgQIAAAQIECBAgQKCxgLDdGNRyBAgQIECAAAECBAgQIEBA2LYHCBAgQIAAAQIECBAgQIBAYwFhuzGo5QgQIECAAAECBAgQIECAgLBtDxAgQIAAAQIECBAgQIAAgcYCwnZjUMsRIECAAAECBAgQIECAAAFh2x4gQIAAAQIECBAgQIAAAQKNBYTtxqCWI0CAAAECBAgQIECAAAECwrY9QIAAAQIECBAgQIAAAQIEGgsI241BLUeAAAECBAgQIECAAAECBIRte4AAAQIECBAgQIAAAQIECDQWELYbg1qOAAECBAgQIECAAAECBAgI2/YAAQIECBAgQIAAAQIECBBoLCBsNwa1HAECBAgQIECAAAECBAgQELbtAQIECBAgQIAAAQIECBAg0FhA2G4MajkCBAgQIECAAAECBAgQICBs2wMECBAgQIAAAQIECBAgQKCxgLDdGNRyBAgQIECAAAECBAgQIEBA2LYHCBAgQIAAAQIECBAgQIBAYwFhuzGo5QgQIECAAAECBAgQIECAgLBtDxAgQIAAAQIECBAgQIAAgcYCwnZjUMsRIECAAAECBAgQIECAAAFh2x4gQIAAAQIECBAgQIAAAQKNBYTtxqCWI0CAAAECBAgQIECAAAECwrY9QIAAAQIECBAgQIAAAQIEGgsI241BLUeAAAECBAgQIECAAAECBIRte4AAAQIECBAgQIAAAQIECDQWELYbg1qOAAECBAgQIECAAAECBAgI2/YAAQIECBAgQIAAAQIECBBoLCBsNwa1HAECBAgQIECAAAECBAgQELbtAQIECBAgQIAAAQIECBAg0FhA2G4MajkCBAgQIECAAAECBAgQICBs2wMECBAgQIAAAQIECBAgQKCxgLDdGNRyBAgQIECAAAECBAgQIEBA2LYHCBAgQIAAAQIECBAgQIBAYwFhuzGo5QgQIECAAAECBAgQIECAgLBtDxAgQIAAAQIECBAgQIAAgcYCwnZjUMsRIECAAAECBAgQIECAAAFh2x4gQIAAAQIECBAgQIAAAQKNBYTtxqCWI0CAAAECBAgQIECAAAECwrY9QIAAAQIECBAgQIAAAQIEGgsI241BLUeAAAECBAgQIECAAAECBIRte4AAAQIECBAgQIAAAQIECDQWELYbg1qOAAECBAgQIECAAAECBAgI2/YAAQIECBAgQIAAAQIECBBoLCBsNwa1HAECBAgQIECAAAECBAgQELbtAQIECBAgQIAAAQIECBAg0FhA2G4MajkCBAgQIECAAAECBAgQICBs2wMECBAgQIAAAQIECBAgQKCxgLDdGNRyBAgQIECAAAECBAgQIEBA2LYHCBAgQIAAAQIECBAgQIBAYwFhuzGo5QgQIECAAAECBAgQIECAgLBtDxAgQIAAAQIECBAgQIAAgcYCwnZjUMsRIECAAAECBAgQIECAAAFh2x4gQIAAAQIECBAgQIAAAQKNBYTtxqCWI0CAAAECBAgQIECAAAECwrY9QIAAAQIECBAgQIAAAQIEGgsI241BLUeAAAECBAgQIECAAAECBIRte4AAAQIECBAgQIAAAQIECDQWELYbg1qOAAECBAgQIECAAAECBAgI2/YAAQIECBAgQIAAAQIECBBoLCBsNwa1HAECBAgQIECAAAECBAgQELbtAQIECBAgQIAAAQIECBAg0FhA2G4MajkCBAgQIECAAAECBAgQICBs2wMECBAgQOB/CNx7771l1qxZZfbs2eXHP/5xGTFiBC8CBAgQIECAwG4FhO3dEvkAAQIECAxWgRUrVpTLLrusPPLII+XLX/6ysD1YN4K+CRAgQIDAXggI23uB5isECBAgkF9gzZo15YorrigLFy7smhW2889chwQIECBAoKWAsN1S01oECBAgkEJg6dKl5Stf+UpZvHjxzn6E7RSj1QQBAgQIENhvAsL2fqNWiAABAgR6XWDTpk3llltuKd/97nfL2rVr+5yusN3r03N+BAgQIECgtwSE7d6ah7MhQIAAgQCBN998s/zxj38s11xzTXnggQd2nsH06dPLs88+W/7973+7jTxgLkoSIECAAIGBLCBsD+TpOXcCBAgQaCJQbxc/66yzdq71f//3f+UHP/hBmTJlSvn85z9fli1bJmw3kbYIAQIECBAYPALC9uCZtU4JECCwVwLr16/vrvbOmzevC52PPfZYt86oUaPKqaeeWj75yU+WSy+9tJx88sll6NChe1Xj5ZdfLnPmzCn33HPPXn2/fum2227r1tibY0fYrj3V28WvvPLKcuyxx5aVK1d2vQnbe6PqOwQIECBAYHALCNuDe/66J0CAwLsK1Fur586dW77//e93oXN3Rw2oP/zhD7sQvqdHdNhesmRJmT9/frn88stLvao9ZMiQrgVhe08n6fMECBAgQIDADgFh214gQIAAgbcJbN++vdx5551d+NywYUP376eddlo577zzyhFHHFG2bt1aHn/88fKHP/yhz4PErrvuunLVVVeVAw44YI9Uo8P2u52ssL1HY/RhAgQIECBAYBcBYdt2IECAAIG3CewaMuuV6htvvLHMnj37bbeJv/LKK6UG7GuvvbZb4+yzzy633357GT9+fApVYTvFGDVBgAABAgRCBITtEHZFCRAg0NsCN998c3dVux7f/va3u1vJhw0b9o4nXZ/U/YUvfKH8/ve/L+PGjSsLFiwoU6dO7e0G+3l2wnY/oXyMAAECBAgQeJuAsG1TECBAgEAfgc2bN5ef/exn3W+Yn3/++XLTTTeV008//V2VXn/99fLVr3611IBejwcffLCceeaZKVSF7RRj1AQBAgQIEAgRELZD2BUlQIBAHgFhO88sdUKAAAECBAi0ExC221laiQABAoNGoAbs1atXd68B++1vf1sWLly480FprmwPmm2gUQIECBAgQOB/CAjbtgcBAgQIvKvAtm3bylNPPdXdGr506dKyYsWK7p3Ta9eufdfv7E3Y9jRym5AAAQIECBDIJiBsZ5uofggQINBAoL76q161/t73vlfuvvvud12xPqm8PgytPpW8hvB6CNsNBmAJAgQIECBAYMALCNsDfoQaIECAQHuBRYsWlS9+8YtlzZo1Oxev79meMmVKmTx5cpk0aVI5/vjjy3HHHdf9+74+IM2V7fYztCIBAgQIECAQKyBsx/qrToAAgZ4T2PVVXvXkvv71r5errrqqe63XOx0ekNZzI3RCBAgQIECAQA8ICNs9MASnQIAAgV4SWLJkSTn//PPLhg0bygUXXFBuvfXWcuSRR77rKdbXg82ZM6f86U9/6j6zN7eR91L/u56LV3/16mScFwECBAgQ6H0BYbv3Z+QMCRAgsF8FFi9eXM4666yu5qxZs8ott9xSRo8e/Y7n8Oabb5Yf/ehH5Vvf+tbOfxe29+u4FCNAgAABAgR6VEDY7tHBOC0CBAhECSxfvrwL2fUp5PUBaDfeeGOZPXt2GTp0aJ9Tqreb/+QnP+n+vV4F33HU33vPmDEj6vSb1nVluymnxQgQIECAwKASELYH1bg1S4AAgd0L1N9gf+Mb3yjXX3/9zg9PmzatnHfeeV343rx5c3nooYdKvQJeQ3b9/40ZM6asWrWq+/xtt93W3Vae4RC2M0xRDwQIECBAIEZA2I5xV5UAAQI9LfDCCy+UK6+8ssydO/d/nufMmTPL1VdfXdavX1/q/67HNddcU77zne+UIUOG9HSP/Tk5Ybs/Sj5DgAABAgQIvJOAsG1fECBAgMA7CmzatKncf//95Y477igPP/xwqcGzHmeccUY555xzyoUXXljqFe9hw4Z1rwirt5rXK9713+pD1SZMmDDgZYXtAT9CDRAgQIAAgTABYTuMXmECBAgQIECAAAECBAgQyCogbGedrL4IECBAgAABAgQIECBAIExA2A6jV5gAAQIECBAgQIAAAQIEsgoI21knqy8CBAgQIECAAAECBAgQCBMQtsPoFSZAgAABAgQIECBAgACBrALCdtbJ6osAAQIECBAgQIAAAQIEwgSE7TB6hQkQIECAAAECBAgQIEAgq4CwnXWy+iJAgAABAgQIECBAgACBMAFhO4xeYQIECBAgQIAAAQIECBDIKiBsZ52svggQIECAAAECBAgQIEAgTEDYDqNXmAABAgQIECBAgAABAgSyCgjbWSerLwIECBAgQIAAAQIECBAIExC2w+gVJkCAQE6B//73v2XDhg3ltdde6/5effXVsnnz5nLIIYeUkSNHloMPPrj7GzduXBk2bFhOBF0RIECAAAECg15A2B70WwAAAQIE2gisWbOmPP300+WZZ54p69at60L266+/XrZs2VK2bdvWBesDDzywC9qjRo3qwvYJJ5xQjj/++HL44Ye3OQmrECBAgAABAgR6REDY7pFBOA0CBAgMVIEnn3yyrFy5svzjH/8oL7zwQlm7dm0ZPXp0GT58eDnooIO6vxq0N23a1P298cYbO0P4mDFjytixY8ukSZPK5MmTu//tIECAAAECBAhkEBC2M0xRDwQIEAgSWLRoUVm6dGmpV7VriD7qqKNKDdAjRozY7RnVUP7SSy91f/Uqd73Cffrpp5cPf/jDu/2uDxAgQIAAAQIEel1A2O71CTk/AgQI9KDAxo0by4IFC8qKFSvK6tWry3HHHVcmTJhQhg4dusdnW0P6P//5z7J+/fpy4okndoF7xowZe7yOLxAgQIAAAQIEeklA2O6laTgXAgQIDACBGrTvvPPO7vfZL774YjnppJO6q9n7etSr4zV0T5w4sXz0ox8t559//r4u6fsECBAgQIAAgTABYTuMXmECBAgMTIE77rijLFu2rNTQfeqpp75jE88//3xZtWpV97C0+n9feeWVLpTXB6Ide+yx5Zhjjul+1/3Wo65Zb0uvgXv27NndFXMHAQIECBAgQGAgCgjbA3FqzpkAAQJBAn/+85+728frg9Dq7d5vPerTx+fNm1fuv//+3Z7hBRdcUC6++OK3fa4+RK3WOeWUU8pll13mSeW7lfQBAgQIECBAoBcFhO1enIpzIkCAQA8K1CeO33XXXeWJJ54oU6dO7V7htetRn0Z+/fXXd08c7+9Rbz+//PLLu6vdux71Xd3PPfdcufDCC8vMmTO9j7u/oD5HgAABAgQI9IyAsN0zo3AiBAgQ6F2BrVu37rxiPX78+HL00Uf3OdkbbrihPP7443vdwEUXXVQ+/elP9/l+vQW9vjJs1qxZZcqUKXu9ti8SIECAAAECBCIEhO0IdTUJECAwwATq767rb7XrFee3vppr4cKFZf78+fvc0bXXXluOOOKInevUK+SPPfZYOe+888qll15ahgwZss81LECA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BAgQIECAwCAWELYH8fC1ToAAgRYCTz/9dHdL+fLly0u9Ql2Pww47rBx00EFl+PDh3d+wYcNK/S13/atXxest4/V29Ho1fOzYsd3vt+vfkUce2eKUrEGAAAECBAgQCBcQtsNH4AQIECCQQ6Be3d4RvNetW9c9FK2+n3vz5s1l27ZtXeCuAXzEiBHl0EMP7R6WVq9mv9N7u3OI6IIAAQIECBAYzALC9mCevt4JECDwHgjU28LXr19fNm7c2P3Vq9j1lvGDDz64u9V8x9+4ceO6AO4gQIAAAQIECGQUELYzTlVPBAgQIECAAAECBAgQIBAqIGyH8itOgAABAgQIECBAgAABAhkFhO2MU9UTAQIECBAgQIAAAQIECIQKCNuh/IoTIECAAAECBAgQIECAQEYBYTvjVPVEgAABAgQIECBAgAABAqECwnYov+IECBAgQIAAAQIECBAgkFFA2M44VT0RIECAAAECBAgQIECAQKiAsB3KrzgBAgQIECBAgAABAgQIZBQQtjNOVU8ECBAgQIAAAQIECBAgECogbIfyK06AAAECBAgQIECAAAECGQWE7YxT1RMBAgQIECBAgAABAgQIhAoI26H8ihMgQIAAAQIECBAgQIBARgFhO+NU9USAAAECBAgQIECAAAECoQLCdii/4gQIECBAgAABAgQIECCQUUDYzjhVPREgQIAAAQIECBAgQIBAqICwHcqvOAECBAgQIECAAAECBAhkFBC2M05VTwQIECBAgAABAgQIECAQKiBsh/IrToAAAQIECBAgQIAAAQIZBYTtjFPVEwECBAgQIECAAAECBAiECgjbofyKEyBAgAABAgQIECBAgEBGAWE741T1RIAAAQIECBAgQIAAAQKhAsJ2KL/iBAgQIECAAAECBAgQIJBRQNjOOFU9ESBAgAABAgQIECBAgECogLAdyq84AQIECBAgQMiDYloAABZmSURBVIAAAQIECGQUELYzTlVPBAgQIECAAAECBAgQIBAqIGyH8itOgAABAgQIECBAgAABAhkFhO2MU9UTAQIECBAgQIAAAQIECIQKCNuh/IoTIECAAAECBAgQIECAQEYBYTvjVPVEgAABAgQIECBAgAABAqECwnYov+IECBAgQIAAAQIECBAgkFFA2M44VT0RIECAAAECBAgQIECAQKiAsB3KrzgBAgQIECBAgAABAgQIZBQQtjNOVU8ECBAgQIAAAQIECBAgECogbIfyK06AAAECBAgQIECAAAECGQWE7YxT1RMBAgQIECBAgAABAgQIhAoI26H8ihMgQIAAAQIECBAgQIBARgFhO+NU9USAAAECBAgQIECAAAECoQLCdii/4gQIECBAgAABAgQIECCQUUDYzjhVPREgQIAAAQIECBAgQIBAqICwHcqvOAECBAgQIECAAAECBAhkFBC2M05VTwQIECBAgAABAgQIECAQKiBsh/IrToAAAQIECBAgQIAAAQIZBYTtjFPVEwECBAgQIECAAAECBAiECgjbofyKEyBAgAABAgQIECBAgEBGAWE741T1RIAAAQIECBAgQIAAAQKhAsJ2KL/iBAgQIECAAAECBAgQIJBRQNjOOFU9ESBAgAABAgQIECBAgECogLAdyq84AQIECBAgQIAAAQIECGQUELYzTlVPBAgQIECAAAECBAgQIBAqIGyH8itOgAABAgQIECBAgAABAhkFhO2MU9UTAQIECBAgQIAAAQIECIQKCNuh/IoTIECAAAECBAgQIECAQEYBYTvjVPVEgAABAgQIECBAgAABAqECwnYov+IECBAgQIAAAQIECBAgkFFA2M44VT0RIECAAAECBAgQIECAQKiAsB3KrzgBAgQIECBAgAABAgQIZBQQtjNOVU8ECBAgQIAAAQIECBAgECogbIfyK06AAAECBAgQIECAAAECGQWE7YxT1RMBAgQIECBAgAABAgQIhAoI26H8ihMgQIAAAQIECBAgQIBARgFhO+NU9USAAAECBAgQIECAAAECoQLCdii/4gQIECBAgAABAgQIECCQUUDYzjhVPREgQIAAAQIECBAgQIBAqICwHcqvOAECBAgQIECAAAECBAhkFBC2M05VTwQIECBAgAABAgQIECAQKiBsh/IrToAAAQIECBAgQIAAAQIZBYTtjFPVEwECBAgQIECAAAECBAiECgjbofyKEyBAgAABAgQIECBAgEBGAWE741T1RIAAAQIECBAgQIAAAQKhAsJ2KL/iBAgQIECAAAECBAgQIJBRQNjOOFU9ESBAgAABAgQIECBAgECogLAdyq84AQIECBAgQIAAAQIECGQUELYzTlVPBAgQIECAAAECBAgQIBAqIGyH8itOgAABAgQIECBAgAABAhkFhO2MU9UTAQIECBAgQIAAAQIECIQKCNuh/IoTIECAAAECBAgQIECAQEYBYTvjVPVEgAABAgQIECBAgAABAqECwnYov+IECBAgQIAAAQIECBAgkFFA2M44VT0RIECAAAECBAgQIECAQKiAsB3KrzgBAgQIECBAgAABAgQIZBQQtjNOVU8ECBAgQIAAAQIECBAgECogbIfyK06AAAECBAgQIECAAAECGQWE7YxT1RMBAgQIECBAgAABAgQIhAoI26H8ihMgQIAAAQIECBAgQIBARgFhO+NU9USAAAECBAgQIECAAAECoQLCdii/4gQIECBAgAABAgQIECCQUUDYzjhVPREgQIAAAQIECBAgQIBAqICwHcqvOAECBAgQIECAAAECBAhkFBC2M05VTwQIECBAgAABAgQIECAQKiBsh/IrToAAAQIECBAgQIAAAQIZBYTtjFPVEwECBAgQIECAAAECBAiECgjbofyKEyBAgAABAgQIECBAgEBGAWE741T1RIAAAQIECBAgQIAAAQKhAsJ2KL/iBAgQIECAAAECBAgQIJBRQNjOOFU9ESBAgAABAgQIECBAgECogLAdyq84AQIECBAgQIAAAQIECGQUELYzTlVPBAgQIECAAAECBAgQIBAqIGyH8itOgAABAgQIECBAgAABAhkFhO2MU9UTAQIECBAgQIAAAQIECIQKCNuh/IoTIECAAAECBAgQIECAQEYBYTvjVPVEgAABAgQIECBAgAABAqECwnYov+IECBAgQIAAAQIECBAgkFFA2M44VT0RIECAAAECBAgQIECAQKiAsB3KrzgBAgQIECBAgAABAgQIZBQQtjNOVU8ECBAgQIAAAQIECBAgECogbIfyK06AAAECBAgQIECAAAECGQWE7YxT1RMBAgQIECBAgAABAgQIhAoI26H8ihMgQIAAAQIECBAgQIBARgFhO+NU9USAAAECBAgQIECAAAECoQLCdii/4gQIECBAgAABAgQIECCQUUDYzjhVPREgQIAAAQIECBAgQIBAqICwHcqvOAECBAgQIECAAAECBAhkFBC2M05VTwQIECBAgAABAgQIECAQKiBsh/IrToAAAQIECBAgQIAAAQIZBYTtjFPVEwECBAgQIECAAAECBAiECgjbofyKEyBAgAABAgQIECBAgEBGAWE741T1RIAAAQIECBAgQIAAAQKhAsJ2KL/iBAgQIECAAAECBAgQIJBRQNjOOFU9ESBAgAABAgQIECBAgECogLAdyq84AQIECBAgQIAAAQIECGQUELYzTlVPBAgQIECAAAECBAgQIBAqIGyH8itOgAABAgQIECBAgAABAhkFhO2MU9UTAQIECBAgQIAAAQIECIQKCNuh/IoTIECAAAECBAgQIECAQEYBYTvjVPVEgAABAgQIECBAgAABAqECwnYov+IECBAgQIAAAQIECBAgkFFA2M44VT0RIECAAAECBAgQIECAQKiAsB3KrzgBAgQIECBAgAABAgQIZBQQtjNOVU8ECBAgQIAAAQIECBAgECogbIfyK06AAAECBAgQIECAAAECGQWE7YxT1RMBAgQIECBAgAABAgQIhAoI26H8ihMgQIAAAQIECBAgQIBARgFhO+NU9USAAAECBAgQIECAAAECoQLCdii/4gQIECBAgAABAgQIECCQUUDYzjhVPREgQIAAAQIECBAgQIBAqICwHcqvOAECBAgQIECAAAECBAhkFBC2M05VTwQIECBAgAABAgQIECAQKiBsh/IrToAAAQIECBAgQIAAAQIZBYTtjFPVEwECBAgQIECAAAECBAiECgjbofyKEyBAgAABAgQIECBAgEBGAWE741T1RIAAAQIECBAgQIAAAQKhAsJ2KL/iBAgQIECAAAECBAgQIJBRQNjOOFU9ESBAgAABAgQIECBAgECogLAdyq84AQIECBAgQIAAAQIECGQUELYzTlVPBAgQIECAAAECBAgQIBAqIGyH8itOgAABAgQIECBAgAABAhkFhO2MU9UTAQIECBAgQIAAAQIECIQKCNuh/IoTIECAAAECBAgQIECAQEYBYTvjVPVEgAABAgQIECBAgAABAqECwnYov+IECBAgQIAAAQIECBAgkFFA2M44VT0RIECAAAECBAgQIECAQKiAsB3KrzgBAgQIECBAgAABAgQIZBQQtjNOVU8ECBAgQIAAAQIECBAgECogbIfyK06AAAECBAgQIECAAAECGQWE7YxT1RMBAgQIECBAgAABAgQIhAoI26H8ihMgQIAAAQIECBAgQIBARgFhO+NU9USAAAECBAgQIECAAAECoQLCdii/4gQIECBAgAABAgQIECCQUUDYzjhVPREgQIAAAQIECBAgQIBAqICwHcqvOAECBAgQIECAAAECBAhkFBC2M05VTwQIECBAgAABAgQIECAQKiBsh/IrToAAAQIECBAgQIAAAQIZBYTtjFPVEwECBAgQIECAAAECBAiECgjbofyKEyBAgAABAgQIECBAgEBGAWE741T1RIAAAQIECBAgQIAAAQKhAsJ2KL/iBAgQIECAAAECBAgQIJBRQNjOOFU9ESBAgAABAgQIECBAgECogLAdyq84AQIECBAgQIAAAQIECGQUELYzTlVPBAgQIECAAAECBAgQIBAqIGyH8itOgAABAgQIECBAgAABAhkFhO2MU9UTAQIECBAgQIAAAQIECIQKCNuh/IoTIECAAAECBAgQIECAQEYBYTvjVPVEgAABAgQIECBAgAABAqECwnYov+IECBAgQIAAAQIECBAgkFFA2M44VT0RIECAAAECBAgQIECAQKiAsB3KrzgBAgQIECBAgAABAgQIZBQQtjNOVU8ECBAgQIAAAQIECBAgECogbIfyK06AAAECBAgQIECAAAECGQWE7YxT1RMBAgQIECBAgAABAgQIhAoI26H8ihMgQIAAAQIECBAgQIBARgFhO+NU9USAAAECBAgQIECAAAECoQLCdii/4gQIECBAgAABAgQIECCQUUDYzjhVPREgQIAAAQIECBAgQIBAqICwHcqvOAECBAgQIECAAAECBAhkFBC2M05VTwQIECBAgAABAgQIECAQKiBsh/IrToAAAQIECBAgQIAAAQIZBYTtjFPVEwECBAgQIECAAAECBAiECgjbofyKEyBAgAABAgQIECBAgEBGAWE741T1RIAAAQIECBAgQIAAAQKhAsJ2KL/iBAgQIECAAAECBAgQIJBRQNjOOFU9ESBAgAABAgQIECBAgECogLAdyq84AQIECBAgQIAAAQIECGQUELYzTlVPBAgQIECAAAECBAgQIBAqIGyH8itOgAABAgQIECBAgAABAhkFhO2MU9UTAQIECBAgQIAAAQIECIQKCNuh/IoTIECAAAECBAgQIECAQEYBYTvjVPVEgAABAgQIECBAgAABAqECwnYov+IECBAgQIAAAQIECBAgkFFA2M44VT0RIECAAAECBAgQIECAQKiAsB3KrzgBAgQIECBAgAABAgQIZBQQtjNOVU8ECBAgQIAAAQIECBAgECogbIfyK06AAAECBAgQIECAAAECGQWE7YxT1RMBAgQIECBAgAABAgQIhAoI26H8ihMgQIAAAQIECBAgQIBARgFhO+NU9USAAAECBAgQIECAAAECoQLCdii/4gQIECBAgAABAgQIECCQUUDYzjhVPREgQIAAAQIECBAgQIBAqICwHcqvOAECBAgQIECAAAECBAhkFBC2M05VTwQIECBAgAABAgQIECAQKiBsh/IrToAAAQIECBAgQIAAAQIZBYTtjFPVEwECBAgQIECAAAECBAiECgjbofyKEyBAgAABAgQIECBAgEBGAWE741T1RIAAAQIECBAgQIAAAQKhAsJ2KL/iBAgQIECAAAECBAgQIJBRQNjOOFU9ESBAgAABAgQIECBAgECogLAdyq84AQIECBAgQIAAAQIECGQUELYzTlVPBAgQIECAAAECBAgQIBAqIGyH8itOgAABAgQIECBAgAABAhkFhO2MU9UTAQIECBAgQIAAAQIECIQKCNuh/IoTIECAAAECBAgQIECAQEYBYTvjVPVEgAABAgQIECBAgAABAqECwnYov+IECBAgQIAAAQIECBAgkFFA2M44VT0RIECAAAECBAgQIECAQKiAsB3KrzgBAgQIECBAgAABAgQIZBQQtjNOVU8ECBAgQIAAAQIECBAgECogbIfyK06AAAECBAgQIECAAAECGQWE7YxT1RMBAgQIECBAgAABAgQIhAoI26H8ihMgQIAAAQIECBAgQIBARgFhO+NU9USAAAECBAgQIECAAAECoQLCdii/4gQIECBAgAABAgQIECCQUUDYzjhVPREgQIAAAQIECBAgQIBAqICwHcqvOAECBAgQIECAAAECBAhkFBC2M05VTwQIECBAgAABAgQIECAQKiBsh/IrToAAAQIECBAgQIAAAQIZBYTtjFPVEwECBAgQIECAAAECBAiECgjbofyKEyBAgAABAgQIECBAgEBGAWE741T1RIAAAQIECBAgQIAAAQKhAsJ2KL/iBAgQIECAAAECBAgQIJBRQNjOOFU9ESBAgAABAgQIECBAgECogLAdyq84AQIECBAgQIAAAQIECGQUELYzTlVPBAgQIECAAAECBAgQIBAqIGyH8itOgAABAgQIECBAgAABAhkFhO2MU9UTAQIECBAgQIAAAQIECIQKCNuh/IoTIECAAAECBAgQIECAQEYBYTvjVPVEgAABAgQIECBAgAABAqECwnYov+IECBAgQIAAAQIECBAgkFFA2M44VT0RIECAAAECBAgQIECAQKiAsB3KrzgBAgQIECBAgAABAgQIZBQQtjNOVU8ECBAgQIAAAQIECBAgECogbIfyK06AAAECBAgQIECAAAECGQWE7YxT1RMBAgQIECBAgAABAgQIhAoI26H8ihMgQIAAAQIECBAgQIBARgFhO+NU9USAAAECBAgQIECAAAECoQLCdii/4gQIECBAgAABAgQIECCQUUDYzjhVPREgQIAAAQIECBAgQIBAqICwHcqvOAECBAgQIECAAAECBAhkFBC2M05VTwQIECBAgAABAgQIECAQKiBsh/IrToAAAQIECBAgQIAAAQIZBYTtjFPVEwECBAgQIECAAAECBAiECgjbofyKEyBAgAABAgQIECBAgEBGAWE741T1RIAAAQIECBAgQIAAAQKhAsJ2KL/iBAgQIECAAAECBAgQIJBRQNjOOFU9ESBAgAABAgQIECBAgECogLAdyq84AQIECBAgQIAAAQIECGQUELYzTlVPBAgQIECAAAECBAgQIBAqIGyH8itOgAABAgQIECBAgAABAhkFhO2MU9UTAQIECBAgQIAAAQIECIQKCNuh/IoTIECAAAECBAgQIECAQEYBYTvjVPVEgAABAgQIECBAgAABAqECwnYov+IECBAgQIAAAQIECBAgkFFA2M44VT0RIECAAAECBAgQIECAQKiAsB3KrzgBAgQIECBAgAABAgQIZBQQtjNOVU8ECBAgQIAAAQIECBAgECogbIfyK06AAAECBAgQIECAAAECGQWE7YxT1RMBAgQIECBAgAABAgQIhAoI26H8ihMgQIAAAQIECBAgQIBARgFhO+NU9USAAAECBAgQIECAAAECoQLCdii/4gQIECBAgAABAgQIECCQUUDYzjhVPREgQIAAAQIECBAgQIBAqICwHcqvOAECBAgQIECAAAECBAhkFBC2M05VTwQIECBAgAABAgQIECAQKiBsh/IrToAAAQIECBAgQIAAAQIZBYTtjFPVEwECBAgQIECAAAECBAiECgjbofyKEyBAgAABAgQIECBAgEBGAWE741T1RIAAAQIECBAgQIAAAQKhAsJ2KL/iBAgQIECAAAECBAgQIJBRQNjOOFU9ESBAgAABAgQIECBAgECogLAdyq84AQIECBAgQIAAAQIECGQUELYzTlVPBAgQIECAAAECBAgQIBAqIGyH8itOgAABAgQIECBAgAABAhkFhO2MU9UTAQIECBAgQIAAAQIECIQKCNuh/IoTIECAAAECBAgQIECAQEYBYTvjVPVEgAABAgQIECBAgAABAqECwnYov+IECBAgQIAAAQIECBAgkFFA2M44VT0RIECAAAECBAgQIECAQKiAsB3KrzgBAgQIECBAgAABAgQIZBQQtjNOVU8ECBAgQIAAAQIECBAgECogbIfyK06AAAECBAgQIECAAAECGQX+H0eFdsRlYs4SAAAAAElFTkSuQmCCUEsBAhQAFAAAAAgAmkHdVHNkA/0NBQAAISYAABcAAAAAAAAAAAAAAAAAAAAAAGdlb2dlYnJhX2RlZmF1bHRzMmQueG1sUEsBAhQAFAAAAAgAmkHdVOcVowd3AwAANxEAABcAAAAAAAAAAAAAAAAAQgUAAGdlb2dlYnJhX2RlZmF1bHRzM2QueG1sUEsBAhQAFAAAAAgAmkHdVNAaJD1DAAAAVgAAABYAAAAAAAAAAAAAAAAA7ggAAGdlb2dlYnJhX2phdmFzY3JpcHQuanNQSwECFAAUAAAACACaQd1Uuo1WNYMGAABHEQAADAAAAAAAAAAAAAAAAABlCQAAZ2VvZ2VicmEueG1sUEsBAhQAFAAAAAAAmkHdVBGQMGe4NgAAuDYAABYAAAAAAAAAAAAAAAAAEhAAAGdlb2dlYnJhX3RodW1ibmFpbC5wbmdQSwUGAAAAAAUABQBMAQAA/kYAAAAA","isPreloader":false,"language":"en","playButton":false,"playButtonAutoDecide":true,"prerelease":false,"preventFocus":true,"scale":"1","screenshotGenerator":false,"showAlgebraInput":false,"showFullscreenButton":false,"showMenuBar":false,"showResetIcon":false,"showSplash":false,"showToolBar":false,"showToolBarHelp":false,"showZoomButtons":false,"useBrowserForJS":false};
    parameters.appletOnLoad = function() {
        if (typeof $ === "function" && window.GGBT_wsf_view !== undefined) {
            var container =  $("#applet_container_42907558");
            window.GGBT_wsf_view.postProcessApplet(container.parents('.content-added-content'));
        }
    };
    /** is3D=is 3D applet using 3D view, AV=Algebra View, SV=Spreadsheet View, CV=CAS View, EV2=Graphics View 2, CP=Construction Protocol, PC=Probability Calculator, DA=Data Analysis, FI=Function Inspector, macro=Macro View */
    var views = {"is3D":0,"AV":0,"SV":0,"CV":0,"EV2":0,"CP":0,"PC":0,"DA":0,"FI":0,"PV":0,"macro":0};
    var applet_42907558 = new GGBApplet('5.0', parameters, views, true);

    if ((navigator.appVersion.indexOf('MSIE')+1?parseFloat(navigator.appVersion.split('MSIE')[1]):999) < 11) { // WebGL is supported since IE 11
        applet_42907558.setHTML5Codebase('GeoGebra/HTML5/5.0/web/', 'true');
    } else {
        applet_42907558.setHTML5Codebase('GeoGebra/HTML5/5.0/web3d/', 'true');
    }
    applet_42907558.setPreviewImage(null, 'GeoGebra/images/GeoGebra_loading.png', null);
    var appletType_42907558 = 'auto';
    $(function($) {
        applet_42907558.inject('applet_container_42907558', 'auto');
    });
</script>
            <script type="text/javascript">
                window.worksheet_applet_ids_42907556.push(42907558);
            </script>
        </div>

            
        
    </div>


    <div class="save-wrapper" data-saveurl="/worksheet/saveexercise/id/kkdtnfub">
        <div class="wsf-btn-bar-left">
                    </div>
    </div>

</div>

                                            
<div id="save-info-inprogress" class="msg-box" style="display: none">
    <div class="message">Saving&hellip;</div>
</div>
<div id="save-info-successful" class="msg-box" style="display: none">
    <div class="message">All changes saved</div>
</div>
<div id="save-info-error" class="msg-box" style="display: none">
    <div class="message general">Error</div>
    <div class="message error_timeout_retry" style="display: none">A timeout occurred. Trying to re-save &hellip;</div>
    <div class="message error_timeout" style="display: none">Sorry, but the server is not responding. Please wait a few minutes and then try to save again.</div>
</div>
                                    </div>

                


<div class="jWS-footer sWs-footer">
    <div class="sWs-footer-content">
        <a class="sWs-GeoGebra" href="https://www.geogebra.org"></a>
            &#0150;
        <span itemprop="creator" class="sWs-footer-contributors" itemscope itemtype="http://schema.org/Person"> <a href="https://www.geogebra.org/u/michael+borcherds"><span class="notranslate" itemprop="name">Michael Borcherds</span></a></span>    

        </div>
</div>

            </div>

            <div class="wsf-info-wrapper">

        <div class="wsf-info-scroller">
            <div class="wsf-wrapper">
                <a class="wsf-button-information-close" title="Hide information"></a>
                <h1 id="wsf-info-title" class="wsf-title">Information: Demo: 2 applets communicating</h1>
                <ul id="wsf-content-info"></ul>
            </div>
        </div>

    </div>

    <script>
        if (window.GGBT_wsf_general) {
            window.GGBT_wsf_general.setDefaults({
                base_url: "https://www.geogebra.org",
                base_path: "GeoGebra",
                info: {
                    wsfButtonInformation : {
                        title: {
                            show: "Show information for this Activity",
                            hide: "Hide information"
                        }
                    },
                    title: {
                        text : "Information"
                    }
                },
                url: {
                    link: "Link"                }
            });
        }
    </script>

            </div>

</div>
        <div class="ajax-loading-glass"></div>
    </body>
</html>

