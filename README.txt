آپلود صفحهٔ دعوت روی گیت‌هاب (فقط یک‌بار)

۱) در گیت‌هاب یک مخزن (repository) تازه بساز با نام دقیقاً:  ahmadqrs.github.io
   (حتماً Public باشد.)
۲) همهٔ محتوای همین پوشه را داخلش آپلود کن، با همین ساختار:
     .nojekyll
     index.html
     khatm/index.html
     .well-known/assetlinks.json
   توجه: پوشهٔ .well-known و فایل .nojekyll با نقطه شروع می‌شوند؛ حتماً آپلود شوند.
۳) در فایل assetlinks.json، عبارت REPLACE_WITH_SHA256_FROM_PLAY_CONSOLE را با
   اثر انگشت SHA-256 کلید امضا از Play Console عوض کن
   (App integrity ← App signing key certificate)، با همان قالب دونقطه‌ای مثل  AA:BB:CC:...
۴) در Settings ← Pages همان مخزن، Branch را main و پوشه را / (root) انتخاب کن.
۵) بعد از چند دقیقه این دو نشانی باید باز شوند:
     https://ahmadqrs.github.io/khatm/?c=123456789
     https://ahmadqrs.github.io/.well-known/assetlinks.json
