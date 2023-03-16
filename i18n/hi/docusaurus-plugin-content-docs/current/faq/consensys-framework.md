---
id: consensys-framework
title: फ्रेमवर्क FAQ स्केलिंग
sidebar_label: Scaling Framework FAQ
description: पॉलीगॉन पर अपनी अगली ब्लॉकचेन ऐप बनाएँ.
keywords:
  - docs
  - matic
  - wiki
  - polygon
image: https://wiki.polygon.technology/img/polygon-wiki.png
---
import useBaseUrl from '@docusaurus/useBaseUrl';

यह फ्रेमवर्क Consensys's के चार सवालों से लिया गया है [जिससे किसी भी स्केलिंग समाधान को जज किया](https://consensys.net/?p=19015&preview=true&_thumbnail_id=19017) जा सके.

## इसका संचालन कौन करता है? {#who-operates-it}
मेंनेट एथेरेयम पर माइनर नोड्स काम के सबूत को हल कर और नए ब्लॉक का निर्माण कर नेटवर्क को चलाते या उसका "संचालन" कर उसे आगे बढ़ाते हैं. L2 सोल्यूशन को अपने नेटवर्क पर इसी तरह के "ऑपरेटर" की भूमिका की आवश्यकता होती है, जो एथेरेयम मेंनेट का माइनर समकक्ष है जो L2 नेटवर्क को आगे बढ़ा सकता है. लेकिन, कुछ फ़र्क हैं. उदाहरण के लिए, माइनर के रूप में ट्रांज़ैक्शन को प्रोसेस और अधिकृत करने के साथ, एक L2 ऑपरेटर यूज़र्स को खुद L2 लेयर में प्रवेश करने और बाहर करने की सुविधा भी प्रदान कर सकता है.

### - पॉलीगॉन भागीदारी के सबूत नेटवर्क का संचालन करने के लिए कौन या क्या चाहिए होता है? {#who-or-what-is-required-to-operate-the-polygon-proof-of-stake-network}

पॉलीगॉन पॉस कमिट चेन नेटवर्क को सुरक्षित करने के लिए वैलीडेटर के एक वर्ग पर निर्भर करता है. वैलीडेटर की भूमिका नोड को रन करना है; ब्लॉक बनाना, एथेरेयम मेन-चेन पर वैलीडेट करना और सहमति में और चेक पॉइंट लगाने में हिस्सा लेना शामिल है. वैलिडेटर बनने के लिए, एथेरेयम चेन पर रहने वाले मैनेजमेंट कॉन्ट्रैक्ट स्टेकिंग के साथ उन्हें अपने मैटिक टोकन स्टेक करने की आवश्यकता होती है.

अधिक विवरण के लिए, कृपया [वैलिडेटर सेक्शन](/maintain/validate/getting-started.md) को देखें.

### - पॉलीगॉन पॉस नेटवर्क में वे ऑपरेटर कैसे बनते हैं? वे किन नियमों का पालन करते हैं? {#how-do-they-become-operators-in-the-polygon-pos-network-what-rules-do-they-abide-by}

वैलिडेटर बनने के लिए, स्टेकिंग के साथ उन्हें अपने मैटिक टोकन स्टेक करने की आवश्यकता होती है एथेरेयम मेनचेन पर रहने वाले मैनेजमेंट कॉन्ट्रैक्ट.

चेकपॉइंट पर उनके स्टेक के अनुपात में सभी स्टेकर्स को रिवॉर्ड वितरित किए जाते हैं, इसमें एक अपवाद है कि प्रपोज़र को अतिरिक्त बोनस मिलता है. अनुबंध में यूज़़र रिवॉर्ड बैलेंस अपडेट होता है जिसे तब संदर्भित किया जाता है
जब रिवॉर्ड का क्लेम किया जाता है.

स्टेक के घटने का खतरा रहता है अगर वैलिडेटर नोड कुछ
दुर्भावनापूर्ण कृत्य जैसे डबल साइनिंग, वैलिडेटर डाउनटाइम जो लिंक किए गए डेलिगेटर को चेकपॉइंट पर
भी प्रभावित करता है.

अधिक विवरण के लिए कृपया refer र करें [एक पॉलीगॉन वैलिडेटर में End-to-end का बहाव](/maintain/polygon-basics/who-is-validator.md#end-to-end-flow-for-a-polygon-validator) और [वैलिडेटर की जिम्मेदारी](/maintain/validate/validator-responsibilities.md)


### - पॉलीगॉन पॉस यूज़र्स को ऑपरेटर के बारे में किन-किन बातों पर भरोसा करने के बारे में सोचना चाहिए? {#what-trust-assumptions-must-the-polygon-pos-users-make-about-the-operator}

पॉलीगॉन पॉस कमिट चेन नेटवर्क को सुरक्षित करने के लिए वैलीडेटर के एक वर्ग पर निर्भर करता है. वैलीडेटर की भूमिका में एक पूरी नोड को रन करना; ब्लॉक बनाना, मेन-चेन पर वैलीडेट करना और सहमति में और चेक पॉइंट लगाने में हिस्सा लेना शामिल है. वैलिडेटर बनने के लिए, उन्हें मेन-चेन. पर रहने वाले मैनेजमेंट कॉन्ट्रैक्ट स्टेकिंग के साथ अपने मैटिक टोकन स्टेक करने की आवश्यकता होती है.
वैलिडेटर का कोई लगाए स्टेक का ⅔ हिस्सा जब तक ईमानदारी का है, चेन सही तरीके से आगे बढ़ेगी.

### - ऑपरेटर किस चीज़ के लिए ज़िम्मेदार होते हैं? उनके पास कौन-कौन से अधिकार हैं? {#what-are-the-operators-responsible-for-what-power-do-they-have}

वैलीडेटर की भूमिका में पूरी नोड को रन करना; ब्लॉक बनाना, मेन-चेन पर वैलीडेट करना और सहमति में और चेक पॉइंट लगाने में हिस्सा लेना शामिल है.

वैलिडेटर के पास चेन के बढ़ने को रोकने, ब्लॉक रीऑर्डर करने आदि का अधिकार है अगर यह मान लिया जाए कि वैलीडेटर के लगाए हिस्से का ⅔ हिस्सा ईमानदारी का नहीं है. उनके पास स्टेट, यूज़़र असेट बैलेंस आदि बदलने का अधिकार नहीं है.

### - पॉलीगॉन पॉस का ऑपरेटर बनने के लिए क्या प्रेरित करता है? {#what-are-the-motivations-to-become-an-operator-of-the-polygon-pos}

नेटवर्क की सुरक्षा के लिए काम करने के लिए और सेवा के बदले रिवॉर्ड कमाने के लिए वैलिडेटर अपने मैटिक टोकन स्टेक गिरवी रखते हैं.

कृपया ध्यान दें कि अधिक विवरण के लिए [प्रोत्साहन क्या](/maintain/validator/rewards.md#what-is-the-incentive) है.

## डेटा कैसा है? {#how-s-the-data}
परिभाषा के अनुसार, लेयर 2 तकनीक को एक लेयर 1 (एथेरेयम मेंनेट) पर डेटा चेकपॉइंट बनाना चाहिए. तब हमारी चिंता बार-बार होने वाले उन लेयर 1 चेक-इन के बीच के समय को लेकर है. विशेष रूप से, लेयर 2 का डेटा तब कैसे पैदा, स्टोर और प्रबंधित होता है जब वह लेयर 1 की सुरक्षित देखरेख से दूर होता है? हम इसे लेकर सबसे अधिक चिंतित होते हैं क्योंकि यह तब होता है जब यूज़़र सार्वजनिक मेंनेट की विश्वास न करने योग्य सुरक्षा से दूर होता है.

### - पॉलीगॉन पॉस के लिए लॉक-अप शर्तें क्या हैं? {#what-are-the-lock-up-conditions-for-polygon-pos}

टोकन डिजाइन के अधिकांश पैटर्न में, टोकन को एथेरेयम पर मिंट किया जाता है और पॉलीगॉन पॉस पर भेजा जा सकता है. एथेरेयम से पॉलीगॉन पॉस पर इस तरह के टोकन को भेजने के लिए, यूज़़र को एथेरेयम पर अनुबंध में फ़ंड को लॉक करने की ज़रूरत होती है और इसके बाद संबंधित टोकन पॉलीगॉन पॉस पर मिंट किए जाते हैं.

ब्रिज रिले मैकेनिज्म पॉलीगॉन पॉस वैलिडेटर द्वारा रन किया जाता है जिन्हें एथेरेयम पर संबंधित टोकन को मिंट करने के लिए ⅔ लॉक्ड टोकन इवेंट पर सहमत होना पड़ता है.

एथेरेयम पर ऐसेट की वापस निकासी की प्रक्रिया दो स्टेप की है जिसमें असेट टोकन को पहले पॉलीगॉन पॉस कमिट चेन पर बर्न किया जाना होता है और फिर इस बर्न ट्रांज़ैक्शन का सबूत एथेरेयम चेन पर पेश करना होता है.


अधिक विवरण के लिए, [PoS ब्रिज का इस्तेमाल करने के लिए स्टेप्स](/develop/ethereum-polygon/pos/getting-started.md#steps-to-use-the-pos-bridge) का उल्लेख करें.

### - पॉलीगॉन पॉस पर यह फ़ंड कितने जल्द उपलब्ध हो जाते हैं? {#how-soon-are-those-funds-available-on-the-polygon-pos}

करीब ~22-30 मिनट. यह एक मैसेज पास करने वाली मैकेनिज्म के माध्यम से किया जाता है जिसे नाम दिया जाता `state sync`है. अधिक विवरण [यहाँ](/pos/state-sync/state-sync-mechamism.md) मिल सकते हैं.

क्या पॉलीगॉन पॉस L1 लॉक-अप के बिना प्रवेश करने वाले यूज़़र के लिए सहायता देता है (यानी, पॉलीगॉन पर यूज़़र को सीधे ऑनबोर्ड करने के मामले में, फिर यूज़़र एथेरेयम मेंनेट से बाहर निकलना चाहता है)?

हाँ इसे पूरा करने के लिए एक खास ब्रिज मैकेनिज्म का इस्तेमाल किया जाता है. जब यूज़़र एथेरेयम से बाहर निकलना चाहता है लेकिन बिना किसी खास अनुबंध में टोकेन को अनलॉक करने के आम तरीके से, जहाँ वह मिंट किया जाता है.

आप उनके बारे में [यहाँ](/develop/ethereum-polygon/mintable-assets.md) पढ़ सकते हैं.

### - यूज़़र किसी अवैध पॉलीगॉन पॉस ट्रांज़ैक्शन को कैसे चुनौती देगा? पॉलीगॉन पॉस के वैध ट्रांज़ैक्शन को साबित करें? {#how-would-a-user-dispute-an-invalid-polygon-pos-transaction-prove-a-valid-polygon-pos-transaction}

वर्तमान में पॉलीगॉन पॉस पर किसी अवैध ट्रांज़ैक्शन को चुनौती देने का ऑन-चेन कोई रास्ता नहीं है. हालांकि, पॉलीगॉन PoS चेन के वैलिडेटर Ethereum को आवधिक चेकपॉइंट सौंपते हैं - आप [यहां](/pos/heimdall/modules/checkpoint.md) और विवरण देख सकते हैं. पॉलीगॉन PoS चेन पर एक transaction the को मर्कल ट्री प्रूफ का निर्माण करके और पॉलीगॉन PoS transaction the के Ethereum पर होने वाले आवधिक चेकपॉइंट के खिलाफ सत्यापित करना संभव है और मर्कल ट्री की जड़ों को प्राप्त करना भी संभव है.

### - एक बार पॉलीगॉन का यूज़र बाहर निकलना चाहता है, तो कितने जल्द ही L1 फंड (प्लस या मिनस किसी भी L2 गेन या losses) L1 पर वापस उपलब्ध हैं) {#once-a-polygon-user-wishes-to-exit-how-soon-are-the-locked-up-layer-1-fund-plus-or-minus-any-l2-gains-or-losses-available-back-on-l1}

लगभग 1-3 घंटे चेकपॉइंट की आवृत्ति पर निर्भर [करते हैं](/pos/heimdall/modules/checkpoint.md). चेकपॉइंट कितनी बार सबमिट किए जाते हैं उसका संबंध इससे है कि वैलिडेटर एथ गैस के लिए फ़ीस पर कितना खर्च करने के लिए तैयार हैं.

### - क्या आप अनुमान लगाते हैं कि लेयर 1 पर कोई ऐसे लिक्विडिटी प्रोवाइडर हैं जो पहले से मौजूद पॉलीगॉन पॉस यूज़र्स को एकदम से रिडीम होने वाले L1 funds फ़ंड देने के लिए तैयार हैं? {#do-you-anticipate-there-being-liquidity-providers-on-layer-1-willing-to-provide-immediately-redeemable-l1-funds-to-existing-polygon-pos-users}

[Connext](https://connext.network/) और [Biconomy](https://biconomy.io/) जैसे कुछ खिलाड़ी पहले से ही हैं जो इस सर्विस को प्रदान कर रहे हैं या नहीं होंगे. कई अन्य लोग भी हैं जो बहुत जल्द ही शुरू जा रहे हैं.

## स्टैक कैसा है? {#how-s-the-stack}
स्टेक की तुलना यह उजागर करने के लिए ज़रूरी है कि लेयर 2 से एथेरेयम मेंनेट में क्या बदला है या नहीं.

### - पॉलीगॉन पॉस स्टैक एथेरेयम मेंनेट स्टैक के साथ कितना सांझा करता है? {#how-much-does-the-polygon-pos-stack-share-with-the-ethereum-mainnet-stack}

यदि आप एथेरेयम डेवलपर हैं, तो आप पहले से ही पॉलीगॉन पॉस डेवलपर हैं. आप जिन सभी टूल से परिचित हैं वे पॉलीगॉन पॉस में पहले से ही चलते हैं: Truffle, Remix, Web3js और कई अन्य.

एथेरेयम को लेकर पॉलीगॉन पॉस के लिए ईवीएम इंटरफ़ेस में कोई बड़े बदलाव नहीं हैं.

### - पॉलीगॉन पॉस एथेरेयम मेंनेट स्टैक से कहाँ अलग है और इससे कौन से जोखिम / रिवॉर्ड जुड़ते हैं? {#where-does-the-polygon-pos-differ-from-ethereum-mainnet-stack-and-what-risks-rewards-does-that-introduce}

कोई बड़े बदलाव नहीं हैं.

## सबसे बुरा होने के लिए तैयारी {#preparing-for-the-worst}
पॉलीगॉन पॉस सिस्टम इनके लिए कैसे तैयार होते हैं:

### - यूज़़र्स का बड़ी संख्या में बाहर निकलना? {#a-mass-exit-of-users}

जब तक ⅔ वैलिडेटर ईमानदार हैं, चेन पर फ़ंड सुरक्षित हैं. अगर यह धारणा मान्य नहीं है, तो इस तरह के परिदृश्य में चेन रुक सकती है या फिर से रिऑर्डरिंग हो सकती हैं. चेन को फिर से किसी पुरानी स्तिथि से शुरू करने के लिए सामाजिक सहमति की ज़रूरत होगी - इसमें पॉलीगॉन पॉस स्टेट के स्नैपशॉट भी शामिल हैं जिन्हें चेकपॉइंट के ज़रिए सबमिट किया जाता है जो इसके लिए इस्तेमाल किए जा सकते हैं.

### - पॉलीगॉन के साझीदार पॉलीगॉन सहमति बनाने की कोशिश करते हैं. उदाहरण के लिए, एक गुट बनाकर? {#polygon-participants-attempting-to-game-the-polygon-consensus-for-example-by-forming-a-cartel}

चेन को फिर से किसी पुरानी स्तिथि से शुरू करने के लिए उन वैलीडेटर को हटाकर और नए वैलीडेटर के साथ दुबारा शुरू करने के लिए फिर सामाजिक सहमति की ज़रूरत होगी - इसमें पॉलीगॉन पॉस स्टेट के स्नैपशॉट भी शामिल हैं जिन्हें चेकपॉइंट के ज़रिए सबमिट किया जाता है जो इसके लिए इस्तेमाल किए जा सकते हैं.


### - सिस्टम के महत्वपूर्ण हिस्से में बग या कोई सेंधबाजी मिली? {#a-bug-or-exploit-discovered-in-a-critical-part-of-its-system}

सिस्टम को बनाने वाले सिस्टम में इस बात का ध्यान रखा जाता है कि उन घटकों को फिर से इस्तेमाल किया जाए जिनका पहले से ही पूरी तरह परीक्षण किया गया है. हालाँकि, अगर सिस्टम के महत्वपूर्ण हिस्से में बग या कोई सेंधमारी है तो चेन को किसी पुरानी स्तिथि में बहाल करने के लिए सामाजिक सहमति ही हल का मुख्य रास्ता है.