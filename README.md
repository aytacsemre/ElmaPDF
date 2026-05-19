# 📄 Dosya İçeriği
Hackathon 2025 - Yapay Zeka Destekli Yazılım Geliştirme Yarışması

# 🍎 ElmaPDF: Yapay Zeka Destekli PDF Asistanınız

ElmaPDF, PDF belgelerinizle etkileşim kurma şeklinizi dönüştüren modern bir web uygulamasıdır. Karmaşık PDF'leri yükleyin, yapay zeka destekli özetler alın, kişiselleştirilmiş testlerle bilginizi ölçün ve size özel çalışma planları oluşturun. Öğrenme ve araştırma süreçlerinizi daha verimli ve etkileşimli hale getirmek için tasarlandı.

## ✨ Temel Özellikler

- **📄 PDF Yükleme:** Cihazınızdan kolayca PDF belgeleri yükleyin.
- **🧠 Yapay Zeka Destekli Özetleme:** Google Gemini'nin gücüyle, yüklediğiniz PDF'lerin içeriğinden otomatik olarak yapılandırılmış ve anlaşılır Türkçe özetler oluşturun.
- **✍️ Düzenlenebilir Özetler:** Oluşturulan özetler üzerinde tam kontrole sahip olun. Metni kalın, italik veya altı çizili yapın ve önemli kısımları vurgulayın. Düzenlenmiş özetinizi bir Word belgesi olarak indirin.
- **❓ Kişiselleştirilmiş Test Oluşturma:**
    - **Zorluk Seviyesi:** "Kolay", "Orta" veya "Zor" seviyelerinden birini seçerek testinizi kişiselleştirin.
    - **Soru Sayısı:** 10, 20, 25, 40 veya 50 soruluk testler oluşturun.
    - **Puanlama:** Testi çözdükten sonra anında puanınızı görün ve cevaplarınızı kontrol edin.
- **📅 Özelleştirilebilir Çalışma Planı:** Özet içeriğine dayanarak, belirli konulara ve zaman çizelgelerine odaklanan kişiselleştirilmiş çalışma planları oluşturun.
- **⬇️ İçerik İndirme:** Oluşturduğunuz özetleri, testleri ve çalışma planlarını `.doc` (Word) formatında indirerek çevrimdışı erişim sağlayın.
- **🎨 Modern ve Şık Arayüz:** `shadcn/ui` ve `Tailwind CSS` ile oluşturulmuş, kullanıcı dostu ve estetik bir arayüz.

## 🛠️ Teknik Yapı ve Teknolojiler

Bu proje, modern ve güçlü web teknolojileri kullanılarak geliştirilmiştir.

- **Framework:** [**Next.js**](https://nextjs.org/) (App Router ile)
- **Dil:** [**TypeScript**](https://www.typescriptlang.org/)
- **Yapay Zeka:** [**Google Gemini**](https://deepmind.google/technologies/gemini/) (Genkit aracılığıyla)
- **Styling:** [**Tailwind CSS**](https://tailwindcss.com/)
- **UI Kütüphanesi:** [**shadcn/ui**](https://ui.shadcn.com/)
- **Form Yönetimi:** [**React Hook Form**](https://react-hook-form.com/) & [**Zod**](https://zod.dev/)
- **İkonlar:** [**Lucide React**](https://lucide.dev/)

### 🤖 Yapay Zeka Entegrasyonu (Genkit & Gemini)

Uygulamanın kalbinde, Google'ın güçlü Gemini modeline erişimi yöneten Genkit akışları (flows) yer almaktadır:

1.  **`pdf-summarizer.ts`**: Yüklenen PDF dosyasının içeriğini (data URI olarak) alır ve ana başlıkları, alt başlıkları ve önemli noktaları içeren yapılandırılmış bir Türkçe özet oluşturmak için Gemini'ye gönderir.
2.  **`test-question-generator.ts`**: Düzenlenmiş özet metnini, kullanıcının seçtiği zorluk seviyesini (`Kolay`, `Orta`, `Zor`) ve soru sayısını alarak, bu kriterlere uygun çoktan seçmeli test soruları üretir.
3.  **`study-plan-generator.ts`**: Özet metnini ve isteğe bağlı olarak kullanıcının belirttiği odak konularını/zaman çizelgesini kullanarak, eyleme geçirilebilir adımlara bölünmüş bir çalışma planı oluşturur.

## 🚀 Projeyi Yerel Olarak Çalıştırma
Projeyi kendi bilgisayarınızda çalıştırmak için aşağıdaki adımları izleyebilirsiniz.
1.  **Depoyu Klonlayın:**
    ```bash
    git clone <repository-url>
    cd <repository-directory>
    ```
2.  **Bağımlılıkları Yükleyin:**
    ```bash
    npm install
    ```
3.  **Geliştirme Sunucusunu Başlatın:**
    ```bash
    npm run dev
    ```

Uygulama varsayılan olarak `http://localhost:9002` adresinde çalışacaktır.

---

ElmaPDF ile öğrenme materyallerinizden en iyi şekilde yararlanın!


000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000\n
0___________________________________________________________________________________________0\n
0_________##############___##############__#####___#######__########________##############__0\n
0________##############___##############__###_##__###_###__##########______##############___0\n
0_______###______________###_____________###__##_##__###__###______###____###_______________0\n
0______###______________###_____________###___####__###__###______###____###________________0\n
0_____###############__##############__###____###__###__###########_____##############______0\n
0____###############__##############__###_____##__###__########________##############_______0\n
0_______________###__###_____________###_________###__###___###_______###___________________0\n
0______________###__###_____________###_________###__###_____###_____###____________________0\n
0__##############__##############__###_________###__###______###____##############__________0\n
0_##############__##############__###_________###__###________###__##############___________0\n
0___________________________________________________________________________________________0\n
000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000\n

