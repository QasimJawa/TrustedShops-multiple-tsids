# TrustedShops-multiple-tsids
The eTrusted Reviews Plugin for WooCommerce enables you to automatically collect seller reviews and product reviews from your happy customers while using its plugin you have to give trustedshop id which you will find in trustshop details so this package is all about how to use multiple trustedshops id for different version of website

With your WooCommerce store you can start in less than 66 seconds

Sign up for a free Trustbadge Reviews account.
Install the Trustbadge Reviews Toolkit in your WooCommerce store
Customize your Trustbadge in the backend of WooCommerce
As promised, it´s easy like that. Welcome on board!

Now begings the fun part

there are two way to do this task 

1) Open plugin settings 
2) Select Expert Mode
3) put below js code in Trustbadge code

`(function () {
   var _tsid = '{id}';
   var lang = document.getElementsByTagName('html')[0].lang; 

   if ( lang === 'de-DE' ) {
      _tsid = 'X*************************';
   }

   _tsConfig = {
       'yOffset': '{offset}', //offset from page bottom
       'variant': 'reviews' //text, default, small, reviews
   };
   var _ts = document.createElement('script');
   _ts.type = 'text/javascript';
   _ts.charset = 'utf-8';
   _ts.src = '//widgets.trustedshops.com/js/' + _tsid + '.js';
   var __ts = document.getElementsByTagName('script')[0];
   __ts.parentNode.insertBefore(_ts, __ts);
})();`

let's say you have  https://wpml.org on your site then you can easily get your language of website and if it's matched the required lanague or what ever the condition you set you can replace the _tsid 
we shows that version of trusted shop
