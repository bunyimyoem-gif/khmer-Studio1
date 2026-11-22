KHMER STUDIO — កម្មវិធីលើទូរស័ព្ទ (PWA)
=========================================
ក្នុង folder នេះ៖ index.html, manifest.webmanifest, sw.js, folder icons/  (ត្រូវ upload ទាំងអស់ជាមួយគ្នា)

១) ដាក់លើអ៊ីនធឺណិត (ត្រូវការ HTTPS ទើបដំឡើងជាកម្មវិធីបាន)
   GitHub Pages (ឥតគិតថ្លៃ អចិន្ត្រៃយ៍)
   - បង្កើត repository Public នៅ github.com → Add file → Upload files → អូស file ទាំងអស់ (រួមទាំង folder icons) → Commit
   - Settings → Pages → Branch: main / (root) → Save → រង់ចាំ 1-2 នាទី ទទួល link https://ឈ្មោះ.github.io/ឈ្មោះ-repo/
   Netlify: app.netlify.com/drop អូស folder នេះចូល (ត្រូវចុះឈ្មោះដើម្បីកុំឲ្យ link ផុតកំណត់)

២) ដំឡើងលើទូរស័ព្ទ
   Android (Chrome): បើក link → ចុចប៊ូតុង «📲 ដំឡើងជាកម្មវិធី» ក្នុងទំព័រ (ឬ ⋮ → Install app / Add to Home screen)
   iPhone (Safari): ចុច Share → Add to Home Screen
   លទ្ធផល: icon លើ Home screen បើកពេញអេក្រង់ដូចកម្មវិធីធម្មតា ហើយបើកលឿន/បើកបានទោះគ្មានអ៊ីនធឺណិត (តែបកប្រែ/ស្តាប់ត្រូវការអ៊ីនធឺណិត)

៣) ធ្វើជា file APK (Android) — ស្រេចចិត្ត
   - ចូល pwabuilder.com → ដាក់ link របស់អ្នក → Start → Package for stores → Android → Generate
   - ទាញយក zip: មាន .apk (ដំឡើងផ្ទាល់) និង .aab (សម្រាប់ Google Play) ព្រមទាំង signing key — រក្សាទុក key ឲ្យល្អ
   - ដើម្បីឲ្យ APK បើកពេញអេក្រង់ គ្មានរបារ URL ត្រូវដាក់ file assetlinks.json (PWABuilder ផ្តល់ឲ្យ) ក្នុង folder .well-known/ នៅលើ site

៤) កែ ហើយ update
   - កែ index.html រួច upload ជំនួស ហើយប្ដូរ VERSION ក្នុង sw.js (ឧ. 'ks-v2') ទើបទូរស័ព្ទទាញកំណែថ្មី

សុវត្ថិភាព: API key របស់អ្នកប្រើនីមួយៗរក្សាក្នុងទូរស័ព្ទគេ មិនមែនក្នុង file ឬ site ទេ។ កុំដាក់ key របស់អ្នកក្នុង index.html។
