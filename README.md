# Kestanepazari24
Kestanepazarı


**Test URL**

https://yeni24.kestanepazari.org.tr

**FTP & Cpanel**

FTP: 45.195.25.11

Cpanel: https://213.238.181.63:2083

kestanepazariorg

jijxuk-jacfo7-cirpIv

**MySQL**

Kullanıcı: kestanepazariorg_groiraz

Veritabanı: kestanepazariorg_groiraz

Şifre: =*x+q+3B81.$


**Zepto API Bilgileri**

https://yeni24.kestanepazari.org.tr/mail.php üzerinde denedim çalışıyor şu anda.

```
<?php

$curl = curl_init();

curl_setopt_array($curl, array(
    CURLOPT_URL => "https://api.zeptomail.com/v1.1/email",
    CURLOPT_RETURNTRANSFER => true,
    CURLOPT_ENCODING => "",
    CURLOPT_MAXREDIRS => 10,
    CURLOPT_TIMEOUT => 30,
    CURLOPT_SSLVERSION => CURL_SSLVERSION_TLSv1_2,
    CURLOPT_HTTP_VERSION => CURL_HTTP_VERSION_1_1,
    CURLOPT_CUSTOMREQUEST => "POST",
    CURLOPT_POSTFIELDS => '{
"from": { "address": "noreply@bagis.kestanepazari.org.tr"},
"to": [{"email_address": {"address": "baris@b3dp.com","name": "Barış"}}],
"subject":"Test Email",
"htmlbody":"<div><b> Test email sent successfully. </b></div>",
}',
    CURLOPT_HTTPHEADER => array(
        "accept: application/json",
        "authorization: Zoho-enczapikey wSsVR61z/hX4WKp+nTf4L+oxnAtTVQn2Rhsr3AH3uHH8SPGT9Mc5wkSbVlPzTfJMEmJrQmcXrOovnh4C0GcN3dl+yw0CDSiF9mqRe1U4J3x17qnvhDzJW29ckxqLLI4BxgxrmWRjFstu",
        "cache-control: no-cache",
        "content-type: application/json",
    ),
));

$response = curl_exec($curl);
$err = curl_error($curl);

curl_close($curl);

if ($err) {
    echo "cURL Error #:" . $err;
} else {
    echo $response;
}
?>
```
