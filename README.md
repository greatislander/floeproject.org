What is the Floe Project?
=========================

Floe is creating tools that help transform, augment, and personalize the learning experience.

Floe provides the resources needed to enable inclusive access to personally relevant, engaging learning opportunities 
for the full diversity of learners and content producers. 


This Repository
===============

This repository contains the markup needed to deploy the floeproject.org website.


News Item Template
==================

News item file naming convention: "YYYY-MM-DD name-name-name.html". Add this file to the news folder.

Note: you will also need to add your news item to the top of the news archive (in news/index.html).

Note: remember to update the floeproject.org page with a short summary of your news item.

The following provides a template for creating a news item html file:

<!DOCTYPE html>
<html lang="en" dir="ltr">
    <head>
        <meta content="text/html; charset=utf-8" http-equiv="Content-Type"/>
        <meta content="width=device-width, initial-scale=1.0" name="viewport">
        <title>News: Inclusive Science Lab | floe</title>
        <link type="image/x-icon" href="../images/favicon.ico" rel="shortcut icon"/>

        <!-- Foundation flex grid -->
        <link href="../lib/foundation/foundation.css" rel="stylesheet" type="text/css" />

        <link href="../css/fss/fss-reset.css" rel="stylesheet" type="text/css"/>
        <link href="../css/fss/fss-layout.css" rel="stylesheet" type="text/css"/>
        <link href="../css/fss/fss-text.css" rel="stylesheet" type="text/css"/>
        <link href="../css/style.css" media="all" rel="stylesheet" type="text/css"/>
        <link href="../css/print.css" media="print" rel="stylesheet" type="text/css"/>

        <link rel="stylesheet" type="text/css" href="../lib/infusion/src/lib/normalize/css/normalize.css" />
        <link rel="stylesheet" type="text/css" href="../lib/infusion/src/framework/core/css/fluid.css" />

        <link rel="stylesheet" type="text/css" href="../lib/infusion/src/framework/preferences/css/Enactors.css" />
        <link rel="stylesheet" type="text/css" href="../lib/infusion/src/framework/preferences/css/PrefsEditor.css" />
        <link rel="stylesheet" type="text/css" href="../lib/infusion/src/framework/preferences/css/SeparatedPanelPrefsEditor.css" />

        <!--[if lte IE 8]>
        <script type="text/javascript">document.createElement("header")</script>
        <script type="text/javascript">document.createElement("nav")</script>
        <script type="text/javascript">document.createElement("footer")</script>
        <script type="text/javascript">document.createElement("section")</script>
        <script type="text/javascript">document.createElement("aside")</script>
        <![endif]-->

        <script type="text/javascript" src="../lib/infusion/infusion-custom.js"></script>
        <script type="text/javascript" src="../js/floe.js"></script>
    </head>
    <body>
        <script type="text/javascript">
            $(document).ready(function () {
                floe.setupUIO("../");
            });
        </script>

        <!-- BEGIN markup for Preference Editor -->
        <div class="flc-prefsEditor-separatedPanel fl-prefsEditor-separatedPanel">
            <!--
                This div is for the sliding panel bar that shows and hides the Preference Editor controls in the mobile view.
                A separate panel bar for mobile displays is needed to preserve the correct tab order.
            -->
            <div class="fl-panelBar fl-panelBar-smallScreen">
                <span class="fl-prefsEditor-buttons">
                    <button id="show-hide" class="flc-slidingPanel-toggleButton fl-prefsEditor-showHide"> Show/Hide</button>
                    <button id="reset" class="flc-prefsEditor-reset fl-prefsEditor-reset"><span class="fl-icon-undo"></span> Reset</button>
                </span>
            </div>

            <!-- This is the div that will contain the Preference Editor component -->
            <div class="flc-slidingPanel-panel flc-prefsEditor-iframe"></div>

            <!--
                This div is for the sliding panel bar that shows and hides the Preference Editor controls in the desktop view.
                A separate panel bar for desktop displays is needed to preserve the correct tab order.
            -->
            <div class="fl-panelBar fl-panelBar-wideScreen">
                <span class="fl-prefsEditor-buttons">
                    <button id="show-hide" class="flc-slidingPanel-toggleButton fl-prefsEditor-showHide"> Show/Hide</button>
                    <button id="reset" class="flc-prefsEditor-reset fl-prefsEditor-reset"><span class="fl-icon-undo"></span> Reset</button>
                </span>
            </div>
        </div>
        <!-- END markup for Preference Editor -->

        <div id="skip">
            <a href="#content">Skip to Content</a>
        </div>

        <div class="floe">
            <header class="floe-header">
                <h1><a rel="home" title="Home" href="../index.html" class="floe-header-logo">floe
                    <span class="floe-header-tagline">
                        flexible learning for open education
                    </span></a>
                </h1>
            </header>

            <div class="flc-toc-tocContainer toc"> </div>
            <div class="floe-content floe-news-item">
                <h2> News </h2>

         <!-- BEGIN markup for news item -->
                <h3>News Item Title</h3>
                <p class="floe-date">Date (Month Day, Year)</p>
                <p>
                    Paragraph 1. 
                </p>
                <p>
                    Paragraph 2.
                </p>
                <p>
                    etc.
                </p>

            </div>
         <!-- END markup for news item -->
 
            <div class="floe-footer">
                <div class="floe-content row">
                    <div class="columns large-6 small-12">
                        <div>
                            <p>
                                Floe is a project of the
                                <a href="http://idrc.ocadu.ca">Inclusive Design Research Centre</a>, <a href="http://ocadu.ca">OCAD University</a>.<br/>
                            </p>
                            <p>
                                <span class="floe-hewlett-logo">Funded by a grant from <a href="http://www.hewlett.org">The William and Flora Hewlett Foundation</a>.</span>
                            </p>
                        </div>
                    </div>

                    <div class="columns large-6 small-12">
                        <address>
                            205 Richmond St. W., Second Floor<br/>
                            Toronto, Ontario, Canada<br/>
                            M5V 1V3<br/>
                            Telephone: (416) 977-6000 #3968<br/>
                            Fax: (416) 977-9844
                        </address>
                        <p>
                            <a href="mailto:jtreviranus@faculty.ocadu.ca">Jutta Treviranus</a> Principal Investigator, Director and Professor<br/>
                            <a href="mailto:jmitchell@ocadu.ca">Jess Mitchell</a> Senior Manager, Research and Development<br/>
                            <a href="mailto:cclark@ocadu.ca">Colin Clark</a> Lead Software Architect
                        </p>
                    </div>
                </div>
            </div>
        </div>

    </body>
</html>
