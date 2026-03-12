<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>تجربة الصلاح الديني</title>
    <style>
        body { font-family: sans-serif; background: #f4f7f6; text-align: center; padding: 20px; }
        .sura-card { background: white; padding: 15px; margin: 10px; border-radius: 12px; border-right: 5px solid #0a3622; cursor: pointer; box-shadow: 0 2px 5px rgba(0,0,0,0.1); }
        #player-area { background: #0a3622; color: white; padding: 20px; border-radius: 15px; margin-top: 20px; display: none; }
        audio { width: 100%; margin-top: 10px; }
        #tafsir-text { background: white; padding: 15px; margin-top: 10px; border-radius: 10px; text-align: justify; line-height: 1.6; }
    </style>
</head>
<body>

    <h2>🕋 تجربة "قصة التفسير" (الخيار الأول)</h2>
    <p style="color: #666;">اختر سورة للتجربة الحية:</p>

    <div class="sura-card" onclick="startTafsir(1, 'الفاتحة')">1. سورة الفاتحة (نموذج قصير)</div>
    <div class="sura-card" onclick="startTafsir(2, 'البقرة')">2. سورة البقرة (نموذج طويل)</div>
    <div class="sura-card" onclick="startTafsir(112, 'الإخلاص')">112. سورة الإخلاص (نموذج من الأواخر)</div>

    <div id="player-area">
        <h3 id="playing-title"></h3>
        <audio id="tafsir-audio" controls></audio>
        <div id="tafsir-text">جاري تحميل قصة التفسير المكتوبة...</div>
    </div>

    <script>
        async function startTafsir(id, name) {
            const playerArea = document.getElementById('player-area');
            const audio = document.getElementById('tafsir-audio');
            const title = document.getElementById('playing-title');
            const textDiv = document.getElementById('tafsir-text');

            // 1. إظهار منطقة المشغل
            playerArea.style.display = 'block';
            title.innerText = "🎙️ قصة تفسير سورة " + name;
            textDiv.innerHTML = "جاري جلب نص التفسير...";

            // 2. تشغيل الصوت من السيرفر المضمون (الخيار الأول)
            const audioId = String(id).padStart(3, '0');
            audio.src = `https://archive.org/download/Tafsir_Moyassar_Audio/${audioId}.mp3`;
            audio.play().catch(() => console.log("في انتظار ضغطة المستخدم لتشغيل الصوت"));

            // 3. جلب التفسير المكتوب (API)
            try {
                const res = await fetch(`https://api.alquran.cloud/v1/surah/${id}/ar.jalalayn`);
                const data = await res.json();
                let html = "";
                data.data.ayahs.forEach(a => {
                    html += `<p><b>(${a.numberInSurah})</b> ${a.text}</p>`;
                });
                textDiv.innerHTML = html;
            } catch (e) {
                textDiv.innerHTML = "تعذر تحميل النص، تأكد من اتصال الإنترنت.";
            }
        }
    </script>
</body>
</html>
