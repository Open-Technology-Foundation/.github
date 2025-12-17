# <img src="https://yatti.id/images/logo.svg" alt="YaTTI Logo" height="32" style="vertical-align: middle"> YaTTI - Indonesian Open Technology Foundation

[![English](https://img.shields.io/badge/lang-English-blue)](#english) | [![Bahasa Indonesia](https://img.shields.io/badge/lang-Bahasa_Indonesia-red)](#bahasa-indonesia)

---

## English

**Building Indonesia's digital future through open technology, one project at a time.**

YaTTI (Yayasan Teknologi Terbuka Indonesia) has been democratizing technology access across Indonesia since 2014. We build practical open source tools that solve real problems—from AI-powered legal search to cultural knowledge preservation—while advocating for transparency and collaboration. With 72 repositories and 13 specialized knowledgebases, we're making technology work for everyone.

### Featured Projects

#### API & CLI Tools
- **[yatti-api](https://github.com/Open-Technology-Foundation/yatti-api)** - Command-line interface for querying YaTTI knowledgebases with LLM-powered responses. Features multi-model support (GPT, Claude, Gemini), retry logic, GPG-verified updates, and 240+ tests.
- **[dejavu2-cli](https://github.com/Open-Technology-Foundation/dejavu2-cli)** - Elegant terminal interface for querying knowledge bases and interacting with LLMs. Your command-line gateway to AI.

#### AI & Knowledge Infrastructure
- **[customkb](https://github.com/Open-Technology-Foundation/customkb)** - Build your own AI knowledge bases with vector search, semantic queries, and LLM integration. Powers all YaTTI knowledge systems.
- **[peraturan.go.id](https://github.com/Open-Technology-Foundation/peraturan.go.id)** - AI-powered search for 5,800+ Indonesian regulations. Transforms impenetrable legal PDFs into actionable insights for 66 million SMEs, law firms, and citizens.

#### Knowledge Preservation
- **[appliedanthropology](https://github.com/Open-Technology-Foundation/appliedanthropology)** - 777,000+ documents bridging anthropology, evolution, and cultural studies. Making academic knowledge accessible.
- **[seculardharma](https://github.com/Open-Technology-Foundation/seculardharma)** - Ancient wisdom meets modern science. Ethical living resources for the "spiritual but not religious" demographic.

#### Developer Tools
- **[en_ID](https://github.com/Open-Technology-Foundation/en_ID)** - The missing English (Indonesia) locale. Proper date, time, and currency formatting for software used in Indonesia.
- **[md2ansi](https://github.com/Open-Technology-Foundation/md2ansi)** - Beautiful markdown rendering in your terminal. Tables, syntax highlighting, custom themes—because terminals deserve good typography.
- **[rtfm](https://github.com/Open-Technology-Foundation/rtfm)** - Smart documentation search that actually finds what you're looking for. "Read The Fine Manual" made easy.
- **[checkpoint](https://github.com/Open-Technology-Foundation/checkpoint)** - Intelligent backup system for developers. Never lose work again.

#### System Utilities
Browse our [full repository list](https://github.com/Open-Technology-Foundation) for specialized tools including process monitors, time utilities, and shell enhancements.

### Knowledgebases

YaTTI maintains 13 specialized knowledgebases covering Indonesian law, anthropology, philosophy, and culture:

| Knowledgebase | Description |
|---------------|-------------|
| **[peraturan.go.id](https://yatti.id)** | Indonesian laws and regulations (5,800+ documents) |
| **[appliedanthropology](https://yatti.id)** | 777,000+ scholarly documents on evolution, culture, and dharma |
| **[seculardharma](https://yatti.id)** | Secular dharma philosophy and ethical living |
| **[wayang.net](https://yatti.id)** | Indonesian wayang culture and traditional performing arts |

Query any knowledgebase via the [yatti-api CLI](#api-access) or [REST API](https://yatti.id/v1/help).

### API Access

#### Using yatti-api CLI (Recommended)

The easiest way to query YaTTI knowledgebases:

```bash
# Install yatti-api
curl -fsSL https://yatti.id/v1/client/download -o yatti-api && chmod +x yatti-api
sudo mv yatti-api /usr/local/bin/

# Configure your API key
yatti-api configure

# Query Indonesian regulations
yatti-api query -K peraturan.go.id -q "pajak UMKM"

# Get anthropology insights
yatti-api query -K appliedanthropology -q "cultural evolution"

# List available knowledgebases
yatti-api kb list
```

#### Using REST API

For programmatic access, use the REST API with authentication:

```bash
# Set your API key
export YATTI_API_KEY="your-api-key"

# Search Indonesian regulations
curl -s -H "Authorization: Bearer $YATTI_API_KEY" \
  "https://yatti.id/v1/peraturan.go.id?q=pajak%20umkm" | jq

# List all available knowledge bases
curl -s -H "Authorization: Bearer $YATTI_API_KEY" \
  "https://yatti.id/v1/list" | jq
```

Full API documentation: [https://yatti.id/v1/help](https://yatti.id/v1/help)

### Get Involved

#### For Developers
- **Contribute**: Pick any repository and dive in. We welcome PRs that align with our open technology mission.
- **Build**: Use our tools as foundations for your own projects. Everything is MIT/GPL licensed.
- **Learn**: Our codebases demonstrate practical AI implementation, vector search, and clean architecture.

#### For Organizations
- **Adopt**: Our tools are production-ready and serving millions. Free to use, modify, and deploy.
- **Partner**: Collaborate on open technology initiatives that benefit Indonesian communities.
- **Support**: Help sustain our infrastructure and development efforts.

#### For Citizens
- **Use**: Access legal information, cultural knowledge, and powerful tools—all free.
- **Share**: Spread awareness about open technology alternatives.
- **Advocate**: Push for transparency and openness in your communities.

### Our Approach

We believe sustainable progress comes from:
- **Open Source** - Every line of code freely available
- **Open Data** - Public information as public resource
- **Open Standards** - Interoperability over vendor lock-in
- **Open Science** - Knowledge sharing for collective advancement
- **Open Governance** - Transparent decision-making
- **Open Commons** - Shared resources for collective benefit

Read our detailed [position papers](https://yatti.id/statements/) on each principle.

### Connect

- **Website**: [https://yatti.id](https://yatti.id)
- **Email**: admin@yatti.id
- **Location**: Jakarta, Indonesia
- **Established**: April 28, 2014

---

## Bahasa Indonesia

**Membangun masa depan digital Indonesia melalui teknologi terbuka, satu proyek pada satu waktu.**

YaTTI (Yayasan Teknologi Terbuka Indonesia) telah mendemokratisasi akses teknologi di seluruh Indonesia sejak 2014. Kami membangun alat open source praktis yang memecahkan masalah nyata—dari pencarian hukum bertenaga AI hingga pelestarian pengetahuan budaya—sambil mengadvokasi transparansi dan kolaborasi. Dengan 72 repositori dan 13 basis pengetahuan khusus, kami membuat teknologi bekerja untuk semua orang.

### Proyek Unggulan

#### Alat API & CLI
- **[yatti-api](https://github.com/Open-Technology-Foundation/yatti-api)** - Antarmuka baris perintah untuk mengkueri basis pengetahuan YaTTI dengan respons bertenaga LLM. Fitur dukungan multi-model (GPT, Claude, Gemini), logika retry, pembaruan terverifikasi GPG, dan 240+ tes.
- **[dejavu2-cli](https://github.com/Open-Technology-Foundation/dejavu2-cli)** - Antarmuka terminal yang elegan untuk mengkueri basis pengetahuan dan berinteraksi dengan LLM. Gerbang baris perintah Anda ke AI.

#### Infrastruktur AI & Pengetahuan
- **[customkb](https://github.com/Open-Technology-Foundation/customkb)** - Bangun basis pengetahuan AI Anda sendiri dengan pencarian vektor, kueri semantik, dan integrasi LLM. Menggerakkan semua sistem pengetahuan YaTTI.
- **[peraturan.go.id](https://github.com/Open-Technology-Foundation/peraturan.go.id)** - Pencarian bertenaga AI untuk 5.800+ peraturan Indonesia. Mengubah PDF hukum yang sulit dipahami menjadi wawasan yang dapat ditindaklanjuti untuk 66 juta UMKM, firma hukum, dan warga negara.

#### Pelestarian Pengetahuan
- **[appliedanthropology](https://github.com/Open-Technology-Foundation/appliedanthropology)** - 777.000+ dokumen yang menjembatani antropologi, evolusi, dan studi budaya. Membuat pengetahuan akademis dapat diakses.
- **[seculardharma](https://github.com/Open-Technology-Foundation/seculardharma)** - Kebijaksanaan kuno bertemu sains modern. Sumber daya hidup etis untuk demografi "spiritual tapi tidak religius".

#### Alat Pengembang
- **[en_ID](https://github.com/Open-Technology-Foundation/en_ID)** - Locale English (Indonesia) yang hilang. Format tanggal, waktu, dan mata uang yang tepat untuk perangkat lunak yang digunakan di Indonesia.
- **[md2ansi](https://github.com/Open-Technology-Foundation/md2ansi)** - Rendering markdown yang indah di terminal Anda. Tabel, syntax highlighting, tema kustom—karena terminal layak mendapat tipografi yang baik.
- **[rtfm](https://github.com/Open-Technology-Foundation/rtfm)** - Pencarian dokumentasi cerdas yang benar-benar menemukan apa yang Anda cari. "Read The Fine Manual" dipermudah.
- **[checkpoint](https://github.com/Open-Technology-Foundation/checkpoint)** - Sistem backup cerdas untuk pengembang. Tidak akan kehilangan pekerjaan lagi.

#### Utilitas Sistem
Jelajahi [daftar repositori lengkap](https://github.com/Open-Technology-Foundation) kami untuk alat khusus termasuk pemantau proses, utilitas waktu, dan peningkatan shell.

### Basis Pengetahuan

YaTTI mengelola 13 basis pengetahuan khusus yang mencakup hukum Indonesia, antropologi, filsafat, dan budaya:

| Basis Pengetahuan | Deskripsi |
|-------------------|-----------|
| **[peraturan.go.id](https://yatti.id)** | Hukum dan peraturan Indonesia (5.800+ dokumen) |
| **[appliedanthropology](https://yatti.id)** | 777.000+ dokumen ilmiah tentang evolusi, budaya, dan dharma |
| **[seculardharma](https://yatti.id)** | Filsafat dharma sekuler dan kehidupan etis |
| **[wayang.net](https://yatti.id)** | Budaya wayang Indonesia dan seni pertunjukan tradisional |

Kueri basis pengetahuan mana pun melalui [yatti-api CLI](#akses-api) atau [REST API](https://yatti.id/v1/help).

### Akses API

#### Menggunakan yatti-api CLI (Direkomendasikan)

Cara termudah untuk mengkueri basis pengetahuan YaTTI:

```bash
# Instal yatti-api
curl -fsSL https://yatti.id/v1/client/download -o yatti-api && chmod +x yatti-api
sudo mv yatti-api /usr/local/bin/

# Konfigurasi API key Anda
yatti-api configure

# Kueri peraturan Indonesia
yatti-api query -K peraturan.go.id -q "pajak UMKM"

# Dapatkan wawasan antropologi
yatti-api query -K appliedanthropology -q "evolusi budaya"

# Daftar basis pengetahuan yang tersedia
yatti-api kb list
```

#### Menggunakan REST API

Untuk akses programatik, gunakan REST API dengan autentikasi:

```bash
# Set API key Anda
export YATTI_API_KEY="your-api-key"

# Cari peraturan Indonesia
curl -s -H "Authorization: Bearer $YATTI_API_KEY" \
  "https://yatti.id/v1/peraturan.go.id?q=pajak%20umkm" | jq

# Daftar semua basis pengetahuan yang tersedia
curl -s -H "Authorization: Bearer $YATTI_API_KEY" \
  "https://yatti.id/v1/list" | jq
```

Dokumentasi API lengkap: [https://yatti.id/v1/help](https://yatti.id/v1/help)

### Bergabunglah

#### Untuk Pengembang
- **Kontribusi**: Pilih repositori mana saja dan mulai. Kami menyambut PR yang selaras dengan misi teknologi terbuka kami.
- **Bangun**: Gunakan alat kami sebagai fondasi untuk proyek Anda sendiri. Semuanya berlisensi MIT/GPL.
- **Belajar**: Codebase kami mendemonstrasikan implementasi AI praktis, pencarian vektor, dan arsitektur bersih.

#### Untuk Organisasi
- **Adopsi**: Alat kami siap produksi dan melayani jutaan pengguna. Gratis untuk digunakan, dimodifikasi, dan dideploy.
- **Bermitra**: Berkolaborasi dalam inisiatif teknologi terbuka yang menguntungkan komunitas Indonesia.
- **Dukung**: Bantu mempertahankan infrastruktur dan upaya pengembangan kami.

#### Untuk Warga Negara
- **Gunakan**: Akses informasi hukum, pengetahuan budaya, dan alat yang powerful—semuanya gratis.
- **Bagikan**: Sebarkan kesadaran tentang alternatif teknologi terbuka.
- **Advokasi**: Dorong transparansi dan keterbukaan di komunitas Anda.

### Pendekatan Kami

Kami percaya kemajuan berkelanjutan berasal dari:
- **Open Source** - Setiap baris kode tersedia secara bebas
- **Open Data** - Informasi publik sebagai sumber daya publik
- **Open Standards** - Interoperabilitas di atas vendor lock-in
- **Open Science** - Berbagi pengetahuan untuk kemajuan kolektif
- **Open Governance** - Pengambilan keputusan yang transparan
- **Open Commons** - Sumber daya bersama untuk manfaat kolektif

Baca [makalah posisi](https://yatti.id/statements/) kami yang terperinci tentang setiap prinsip.

### Hubungi Kami

- **Website**: [https://yatti.id](https://yatti.id)
- **Email**: admin@yatti.id
- **Lokasi**: Jakarta, Indonesia
- **Didirikan**: 28 April 2014

---

*YaTTI - Membuka Teknologi, Membuka Kesempatan*
*Opening Technology, Opening Opportunities*
