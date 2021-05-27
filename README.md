
Skip to content
Pull requests
Issues
Marketplace
Explore
@timlinux
qgis /
QGIS-Website

36
73

    220

Code
Issues 19
Pull requests 2
Actions
Projects
Wiki
Security
Insights

    Settings

QGIS-Website/themes/qgis-theme/getinvolved_donations.html
@andreasneumann
andreasneumann Some additional information about Stripe fees are lower than Paypal f…
Latest commit b1a6f2f on 21 Jun 2018
History
5 contributors
@andreasneumann
@rduivenvoorde
@pcav
@jef-n
@anitagraser
122 lines (117 sloc) 5.79 KB

<div class="getinvolved" id="color-identifier"></div>

<section class="sub-landing-page" id="top">
    <div class="container-fluid banner">
        <div class="row-fluid">
            <div class="span12">
                <h2>{{ _('QGIS Donations') }}</h2>
                <p>{{ _('QGIS is developed by a team of dedicated volunteers, companies and organisations.') }}</p>
                <p>{{ ('We rely on sponsorships and donations for much of our funding. If you would like to support us, donations are very welcome.
                        Donations can be made by electronic funds transfer, by credit card, or by PayPal.') }}
                </p>
                <p>{{ _('Donations to QGIS are tax-deductible in several countries. Please refer to your local tax office for details.
                    If you want to tax-deduct as a german company or organization, please donate through the ') }}<a href="http://www.qgis.de/">{{ _('German QGIS user group') }}</a>{{ _('. They can issue a payment confirmation as a tax-exempt german association.') }}
                </p>
                <p><strong>{{ _('You can get involved!') }}</strong></p>

            </div>
        </div>
    </div>
</section>
<section class="sub-landing-page menu">
    <div class="container-fluid">
        <div class="row-fluid">
            <div class="span12">
                <nav class="subnav">
                    <header>
                        <h3>{{ _('DONATE TO THE PROJECT') }}</h3>
                    </header>

                    <!--<ul id="subnav">
                        <li>
                            <a href="#bank">{{ _('Bank Transfer') }}</a>
                        </li>
                        <li>
                            <a href="#paypal">{{ _('Credit card and Paypal') }}</a>
                        </li>
                    </ul>-->
                </nav>
            </div>
        </div>
    </div>
</section>

<section class="sub-landing-page main" id="bank">
    <div class="container-fluid">
        <div class="row-fluid">
            <div class="span3">
                <img src='../../_static/images/get-involved-translate.png' class="text-center background-mask non-mobile-image wd" alt="translate bubbles icon" />
            </div>
            <div class="span1"></div>
            <div class="span8">
                <h3>{{ _('Bank Transfer') }}</h3>
                <p>{{ _('Use the details below to make a donation via international money transfer:') }}</p>
                <p>
                <pre>
Account name: QGIS.ORG
Address:      Boeschacherstrasse 10a
              CH-8624 Gruet
BIC/SWIFT:    POFICHBEXXX 
IBAN:         CH09 0900 0000 9146 3839 8
Reference:    Donation QGIS
Currency:     EUR
Bank name:    PostFinance AG 
Bank address: Mingerstrasse 20 
              3030 Berne 
              Switzerland
VAT-number:   CHE-489.853.176
                </pre>
                </p>
            </div>
        </div>
        <hr>
        <div class="row-fluid">
                <h3>{{ _('Stripe') }}</h3>
                <p>{{ _("We use the stripe.com service to receive credit card donations. Note that the payment fees at Stripe are substantially lower than at Paypal - so we would appreciate it, if you could use Stripe instead of PayPal. No signup needed.") }}</p>
                <div id="stripe">{{_("If you do not see a Payment Form here please let us know via finance@qgis.org.") }}<!-- content gets injected here via js in themes/qgis-theme/languageswitch.html --></div>
        </div>
        <hr>
        <div class="row-fluid" id="paypal">
            <div class="span8">
                <h3>{{ _('Paypal') }}</h3>
                <p>{{ _("You can use Paypal to donate using your own credit card (but we prefer to use Stripe for that). 
                    The payment is processed by PayPal but you don't need to have a PayPal account 
                    or sign-up for one if you are paying by credit card.") }}</p>
                <p>{{ _('You can also use your own Paypal account to donate.') }}</p>
                <!--<h4 class="subsection-link"><a href="{{ pathto('site/forusers/support') }}">{{ _('List of QGIS Support Channels') }}</a></h4>-->
                <div>
                    <form action="https://www.paypal.com/cgi-bin/webscr" method="post">
                    <input type="hidden" name="cmd" value="_s-xclick">
                    <input type="hidden" name="hosted_button_id" value="GTYJSTG8LXKW6">
                    <input type="hidden" name="image_url" value="https://qgis.org/en/_static/images/logo_for_paypal_checkout.png">
                    <input type="image" src="https://www.paypalobjects.com/en_US/i/btn/btn_donate_LG.gif"
                        border="0" name="submit" alt="{{ _('Donate via PayPal.com') }}">
                    <input type="hidden" name="lc" value="us">
                    <img alt="" border="0" align="center" src="https://www.paypal.com/en_US/i/scr/pixel.gif" width="1" height="1">
                    <!--<a href="http://www.qgis.org/en/sponsorship.html"><div style="margin-left:7px">more information</div></a>-->
                    </form>
                </div>
            </div>
            <div class="span1"></div>
            <div class="span3">
                <img src="../../_static/images/paypal-logo.jpg" class="text-center background-mask non-mobile-image wd" alt="participate icon" />
            </div>
        </div>
        <hr>
    </div>
</section>
<section class="sub-landing-page">
    <div class="container-fluid banner">
        <div class="row-fluid">
            <div class="offset5 span2">
                <h5 class="text-center">
                    <a href="#top"> <i class="icon-arrow-up"></i>
                        {{ _('Back to Top') }}
                    </a>
                </h5>
            </div>
            <div class="span5"></div>
        </div>
    </div>
</section>

    © 2021 GitHub, Inc.
    Terms
    Privacy
    Security
    Status
    Docs

    Contact GitHub
    Pricing
    API
    Training
    Blog
    About

Loading complete
