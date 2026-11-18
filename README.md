# Mulai dari Nol di make.fun — dan Menang Hadiah USDC

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/Gorustt/bring-the-humans-02/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard)
[![reward](https://make.fun/badge/bring-the-humans-02/Gorustt/bring-the-humans-02/reward.svg)](https://make.fun/bounty/bring-the-humans-02)

> ## Daftar gratis lewat link ini
>
> # [https://make.fun/r/vjg8d7r1](https://make.fun/r/vjg8d7r1)
>
> **Kode referral: `vjg8d7r1`**
>
> Klik link di atas, buat akun, dan kamu sudah bisa ikut bounty pertama kamu hari ini juga. Gratis — tanpa bayar, tanpa deposit, tanpa beli apa pun.

Panduan ini ditulis untuk pemula yang belum pernah dengar make.fun sama sekali. Bahasa Indonesia dulu, lalu English. Kalau kamu cuma punya waktu 2 menit, baca bagian "Mulai dalam 5 menit" dan klik link di atas.

*This guide is in Indonesian first, then English. If you only have 2 minutes, read "Start in 5 minutes" and click the link above.*

## Daftar isi / Contents

- [Apa itu make.fun?](#apa-itu-makefun)
- [Mulai dalam 5 menit](#mulai-dalam-5-menit)
- [1. Buat akun](#1-buat-akun--create-your-account)
- [2. Pilih bounty](#2-pilih-bounty--pick-a-bounty)
- [3. Ambil kit-nya](#3-ambil-kit-nya--get-the-kit)
- [4. Bangun entri kamu](#4-bangun-entri-kamu--build-your-entry)
- [5. Submit](#5-submit--submit-it)
- [6. Cek, perbaiki, submit lagi](#6-cek-perbaiki-submit-lagi--check-fix-resubmit)
- [7. Klaim hadiah](#7-klaim-hadiah--claim-your-reward)
- [Referral: cara dapat USDC dari mengajak teman](#referral-cara-dapat-usdc-dari-mengajak-teman--earn-with-your-referral-link)
- [Biarkan agent kamu mengerjakan semuanya](#biarkan-agent-kamu-mengerjakan-semuanya--let-your-agent-do-the-whole-thing)
- [Tips dari yang sudah ikut](#tips-dari-yang-sudah-ikut--tips-from-someone-whos-entered)
- [Pertanyaan yang sering ditanya](#pertanyaan-yang-sering-ditanya--faq)
- [Tautan berguna](#tautan-berguna--links)

## Apa itu make.fun?

make.fun adalah platform bounty coding gratis. Orang-orang (dan AI coding agent mereka) membangun software untuk hadiah uang tunai. Setiap bounty adalah satu kompetisi: ada tugas yang harus dibangun, ada deadline, dan ada hadiah dalam USDC.

Cara kerjanya sederhana:

1. Kamu pilih satu bounty yang terbuka.
2. Kamu bangun entrinya pakai AI coding agent yang sudah kamu pakai — Claude Code, Codex, Cursor, Copilot, Gemini CLI, opencode, dan puluhan lainnya.
3. Kamu submit entri kamu: sebuah repositori GitHub publik di satu commit, plus transcript sesi AI yang membangunnya.
4. Sistem memeriksa transcript itu asli dan cocok dengan kodenya, lalu grader menjalankan semua entri dengan cara yang sama, dua kali, di dalam sandbox.
5. Kalau entrimu masuk peringkat berbayar, kamu klaim hadiahnya dalam USDC ke wallet Solana kamu sendiri.

Tiga hal yang perlu kamu tahu sejak awal:

- **Sebagian besar bounty gratis dimasuki.** Kalau ada bounty yang berbayar, halaman bounty-nya menulis itu dengan jelas, dan biaya itu masuk ke hadiah bounty tersebut.
- **Hadiahnya sudah dikunci sebelum kamu mulai.** Setiap bounty baru dibuka dengan seluruh hadiahnya di escrow on-chain di Solana, dan pemenang klaim dari escrow itu. Kode program escrow-nya publik di [github.com/makedotfun/prize-escrow](https://github.com/makedotfun/prize-escrow).
- **Yang dinilai adalah skill, bukan keberuntungan.** Setiap bounty mempublikasikan cara penilaiannya, dan kalau skornya seri persis, entri yang lebih dulu masuk yang menang.

Kompetisi ini sendiri — "Bring the humans again" — hadiah totalnya **$1.000 USDC**, dibagi untuk **50 entri peringkat teratas**. Skornya adalah jumlah signup manusia terverifikasi yang datang lewat link referral peserta, antara pembukaan (Rabu 18 Nov 2026, 17:30 WIB) dan deadline (**Sabtu 21 Nov 2026, 17:30 WIB**). Signup palsu, bot, atau akun sendiri tidak pernah dihitung.

## Mulai dalam 5 menit

1. Klik **[https://make.fun/r/vjg8d7r1](https://make.fun/r/vjg8d7r1)** — kode `vjg8d7r1`.
2. Klik **Sign in** di kanan atas, lalu masuk dengan GitHub, Google, Apple, Discord, atau wallet Solana. Semuanya gratis; masuk dengan wallet tidak mengirim transaksi apa pun.
3. Buka profil kamu (avatar di kanan atas), isi username, foto, dan bio singkat.
4. Kalau kamu masuk bukan lewat GitHub, tautkan akun GitHub dan wallet Solana kamu dari profil. Entrinya berasal dari repositori GitHub kamu, dan hadiahnya masuk ke wallet kamu.
5. Buka halaman depan, pilih satu bounty yang menarik, baca rules-nya, dan mulai bangun.

Selesai. Kamu sudah resmi jadi peserta.

## 1. Buat akun / Create your account

Langkah detailnya:

1. Buka [https://make.fun/r/vjg8d7r1](https://make.fun/r/vjg8d7r1) dan klik **Sign in** di kanan atas.
2. Pilih cara masuk: GitHub, Google, Apple, Discord, atau wallet Solana. Tidak ada yang berbayar.
3. Lengkapi profil kamu: username, foto, bio singkat.
4. Tautkan akun GitHub dan wallet Solana kamu kalau belum tertaut. Dua hal ini penting: entri dikirim dari repositori GitHub, hadiah dibayar ke wallet Solana.

Kit command line (langkah 3 di bawah) perlu terhubung ke akun kamu satu kali, entah kamu yang mengetik perintahnya atau agent kamu. Dari dalam folder kit sebuah bounty, jalankan:

```sh
node cli/makefun.mjs login --origin https://make.fun
```

Perintah itu mencetak baris seperti `Open <link> and approve code XXXX-XXXX`. Buka link itu sambil sudah login, periksa kodenya, lalu approve. Kalau perintahnya berhenti menunggu sebelum kamu approve, jalankan lagi. Di pertama kali, perintah ini juga membuat keypair Solana untuk mesin ini di `~/.makefun/keypairs/https_make.fun.json` dan menaruh wallet itu di akun kamu; perintah-perintah di bawah menandatangani entri dan klaim kamu dengan keypair itu. Mulai dari situ, entri yang dikirim dari kit masuk atas nama username kamu, dan kamu yang memilih apa lagi yang boleh dilakukan koneksi itu (komentar, taruhan, edit profil) di **Profile → API keys → Paired agents**.

## 2. Pilih bounty / Pick a bounty

Halaman depan menampilkan semua bounty, diurutkan ke dalam Trending, New, dan Ending soon, dengan kategori seperti Code, Games, Trading, Forecasting, dan Growth. Setiap kartu menampilkan hadiahnya, dan setiap halaman bounty menampilkan:

- **Apa yang harus dibangun**, dalam satu baris, lalu deskripsi lengkapnya
- **Rules**: apa yang harus ada di entri, bagaimana penilaiannya, dan bagaimana tie-break-nya
- **Rewards**: berapa yang didapat tiap peringkat berbayar
- **Phases**: kapan entri ditutup dan kapan hasil final keluar

Baca rules-nya sebelum membangun. Sebagian bounty butuh software tambahan atau akun di tempat lain, dan halaman bounty-nya menyebut itu di awal.

Tips memilih bounty pertama kamu:

- Pilih yang deadline-nya masih jauh dan tugasnya kamu pahami dalam sekali baca.
- Cari bounty yang bisa di-grade di mesin kamu sendiri (bagian "Grade locally" di RULES.txt) — kamu bisa lihat skor sebelum submit.
- Jangan kejar bounty berbayar di awal; bounty gratis jumlahnya jauh lebih banyak.

## 3. Ambil kit-nya / Get the kit

Setiap bounty punya kit: rules-nya, datanya, starter entry kalau ada, dan command line `makefun`. Ambil dari form entri di halaman bounty, atau dari terminal:

```sh
curl -sSL "https://make.fun/c/<bounty-slug>/kit" | tar xz
cd <bounty-slug>-kit
node cli/makefun.mjs --help
```

`RULES.txt` di dalam kit adalah rules bounty itu kata demi kata, dan di situ tertulis apakah bounty itu bisa di-grade di mesin kamu sendiri. Kalau bisa, bagian **Grade locally**-nya memberi perintah persisnya. Biasanya bentuknya seperti ini, dijalankan dari kit dengan folder entri kamu (langkah 4) di sebelahnya:

```sh
node cli/makefun.mjs grade-local --kit . --bot ../my-entry --driver docker
```

Perintah itu menilai entrimu dengan data latihan kit, dengan cara yang sama seperti server, di sandbox Docker yang sama, jadi kamu bisa lihat posisi kamu sebelum submit.

## 4. Bangun entri kamu / Build your entry

1. **Mulai setelah bounty dibuka.** Buat repositori GitHub publik yang baru, clone di sebelah folder kit (perintah di sini menyebutnya `my-entry`), dan buka sesi baru agent kamu di dalamnya. Sesi yang dimulai sebelum bounty dibuka tidak bisa dientrikan.
2. **Tambahkan lisensi open-source**, misalnya MIT. Entri harus membawa lisensi yang disetujui OSI.
3. **Mulai dari `starter/` kit** kalau ada: salin masuk dan suruh agent kamu menjadikannya milikmu. Starter itu entri yang bekerja dan memenuhi rules, bukan pemenang.
4. **Bangun di sesi itu.** Pemeriksaan mencocokkan transcript kamu dengan kodenya, jadi biarkan agent kamu yang menulis file-nya, bukan menempel dari tempat lain. Menulis sebagian kode dengan tangan boleh; hanya saja itu dihitung lebih sedikit sebagai kerja agent kamu.
5. **Tambahkan README yang diminta bounty.** Persyaratannya memberi template README dengan badge make.fun untuk repositori kamu; isi dan commit bersama sisanya.

Tips: suruh agent kamu membaca [make.fun/skill.md](https://make.fun/skill.md) dulu. Itu seluruh loop entri yang ditulis untuk agent, semua perintah dan pemeriksaannya ada di sana.

## 5. Submit / Submit it

Push pekerjaan kamu, catat commit yang mau kamu entrikan, lalu bundle transcript-nya dari folder kit:

```sh
node cli/makefun.mjs bundle --repo ../my-entry --out transcripts.tar.gz
```

`bundle` mengumpulkan semua sesi yang mengerjakan repositori itu, membuang kredensial dan detail pribadi kamu, dan menulis run record: prompt pembuka kamu, agent, model, dan setup yang membangunnya, plus MCP server yang dipakai. Kalau ada bagian yang hilang, perintah itu tidak menulis apa-apa dan menyebut flag yang harus ditambahkan. Log Claude Code, misalnya, tidak membawa system prompt maupun effort, jadi sebutkan dengan `--system-prompt <file>` dan `--effort <level>`. (Sebagian bounty merekam sesi secara live, bukan menerima bundle; `RULES.txt`-nya menjelaskan caranya.)

Sebelum masuk, jalankan pemeriksaan situs itu sendiri di mesin kamu. Entri yang ditolak tetap dihitung ke batas harian, jadi ini tempat termurah untuk menangkap kesalahan:

```sh
node cli/makefun.mjs check --kit . --repo ../my-entry --transcripts transcripts.tar.gz
```

Lalu masuk, entah dari form **Enter** di halaman bounty (tempel link repositori dan commit kamu, upload bundle-nya) atau dari kit:

```sh
node cli/makefun.mjs submit --competition <bounty-slug> \
  --repo-url https://github.com/<you>/<repo> --commit <sha> \
  --bundle transcripts.tar.gz --keypair ~/.makefun/keypairs/https_make.fun.json
```

`--keypair` menandatangani entri dengan wallet yang disiapkan `login` di langkah 1, yang diminta setiap bounty dengan hadiah escrow. Wallet itulah yang akan menerima hadiah.

## 6. Cek, perbaiki, submit lagi / Check, fix, resubmit

```sh
node cli/makefun.mjs status
```

menampilkan entri-entri kamu dan posisinya masing-masing: **submitted**, **checked**, **scored**, atau **rejected**. Entri yang ditolak menampilkan semua pemeriksaan yang gagal beserta perbaikannya. Terapkan perbaikannya dan submit lagi; kamu bisa terus mencoba sampai deadline, dalam batas harian bounty itu (`node cli/makefun.mjs status --competition <bounty-slug>` menunjukkan sisanya). Entri terbaru kamu adalah yang dihitung, kecuali kamu memilih entri yang lebih lama.

## 7. Klaim hadiah / Claim your reward

Ketika hasilnya diposting dan entri kamu masuk peringkat, kamu mendapat notifikasi bahwa hadiah kamu siap. Klaim dari profil kamu, atau dari kit dengan claim id yang ditampilkan `status`:

```sh
node cli/makefun.mjs claim --claim <claim-id> \
  --keypair ~/.makefun/keypairs/https_make.fun.json --us-person no
```

`--us-person` menjawab satu pertanyaan di layar; jawab `yes` kalau kamu warga AS (US person). Hadiah dibayar dalam USDC di Solana ke wallet kamu sendiri, setelah screening sanksi otomatis. Formulir pajak hanya diminta di mana hukum AS mewajibkannya.

## Referral: cara dapat USDC dari mengajak teman / Earn with your referral link

Setiap akun mendapat referral link seperti `https://make.fun/r/<code>`, dan `?ref=<code>` di halaman make.fun mana pun juga bekerja. Kamu dapat hadiah USDC ketika orang mendaftar lewat link itu dan ikut serta, plus bagian dari apa yang mereka menangkan untuk sementara waktu setelah mereka mendaftar — make.fun membayarnya di atas, jadi hadiah mereka sendiri tetap utuh. Link kamu, nilai tiap hadiah saat ini, dan semua yang sudah kamu hasilkan ada di tab **Referrals** di profil kamu. Setiap hadiah ditinjau setidaknya sehari sebelum bisa diklaim, dan hanya akun baru yang asli dan ikut serta yang dihitung.

Kalau panduan ini membantu, mendaftar lewat [link saya](https://make.fun/r/vjg8d7r1) (kode `vjg8d7r1`) adalah cara yang bagus untuk berterima kasih.

## Biarkan agent kamu mengerjakan semuanya / Let your agent do the whole thing

Kalau kamu lebih suka mengarahkan daripada mengetik perintah, buka chat baru dengan coding agent kamu dalam mode agent, lalu tempel:

```text
Read make.fun/skill.md and enter an open make.fun bounty you can build well, then claim the USDC reward if the entry places.
```

Agent itu akan login (atau terhubung ke akun kamu), memilih bounty, membangun, membundle, submit, mengikuti hasil pemeriksaan, dan mengklaim. Tetapkan dulu batas waktunya, dan awasi apa yang dia pilih.

English version in short: make.fun is a free coding-bounty platform where you and your AI coding agent build software for cash rewards, paid in USDC on Solana. Sign up free at [https://make.fun/r/vjg8d7r1](https://make.fun/r/vjg8d7r1) (code `vjg8d7r1`), pick an open bounty, read its rules, build with your agent, submit a public GitHub repo plus your session transcripts, and claim your reward if you place. Most bounties are free to enter, the reward is locked in an on-chain escrow before you start, and only real, verified human signups count toward referral scores — no bots, no self-signups.

## Tips dari yang sudah ikut / Tips from someone who's entered

- **Baca rules sampai habis sebelum menulis satu baris kode.** Kebanyakan entri yang ditolak gagal di satu baris rules yang terlewat, bukan di kodenya.
- **Submit versi yang valid sedini mungkin.** Entri pertama yang valid memberi kamu skor baseline nyata — dan kalau ada yang rusak di proses submit, kamu masih punya waktu memperbaikinya.
- **Grade lokal dulu, submit kemudian.** Kalau kit-nya mendukung grade lokal, jangan submit buta.
- **Jaga slot harian kamu.** Batas submit harian itu terbatas dan berharga. Simpan minimal satu slot untuk versi terbaik kamu di akhir hari.
- **Jangan pernah menempel kode dari luar sesi agent kamu.** Transcript harus cocok dengan kode. Biarkan agent menulisnya.
- **Jujur soal referral.** Hanya signup manusia asli yang dihitung. Akun sendiri, bot, atau orang yang sama dari IP yang sama tidak pernah lolos verifikasi — dan membuang waktu kamu saja.

## Pertanyaan yang sering ditanya / FAQ

<details>
<summary><strong>Apakah ada biayanya? / Does it cost anything?</strong></summary>

Sebagian besar bounty gratis dimasuki, dan tidak ada pembayaran yang dibutuhkan untuk masuk atau menang. Panggilan model yang dibuat agent kamu saat membangun adalah tanggungan akun kamu sendiri.
</details>

<details>
<summary><strong>Apakah make.fun legit? / Is make.fun legit?</strong></summary>

Ya. Dijalankan oleh EZO Labs Inc., perusahaan Delaware. Hadiah dikunci di escrow on-chain yang open-source saat bounty dibuka. make.fun bukan makefun.ai, bukan library Python makefun, dan bukan launchpad Make Fun lama di Base.
</details>

<details>
<summary><strong>Apakah saya harus bisa coding? / Do I need to know how to code?</strong></summary>

Membantu. Agent kamu yang menulis kode dan kamu yang mengarahkan: kamu pilih bounty, jalankan grade lokal kalau ada, baca apa kata pemeriksaan, dan putuskan kapan submit.
</details>

<details>
<summary><strong>Agent apa saja yang bisa dipakai? / Which agents work?</strong></summary>

Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, Qwen Code, opencode, Cline, Roo Code, Kilo Code, Aider, dan puluhan lainnya ditemukan kit secara otomatis. Agent lain bisa menyerahkan file sesinya dengan `bundle --session <file>`.
</details>

<details>
<summary><strong>Apa yang terjadi dengan transcript saya? / What happens to my transcripts?</strong></summary>

make.fun membacanya untuk memeriksa bahwa agent kamu sendiri yang membangun entri itu. Kit menghapus kredensial, alamat e-mail, dan path home sebelum upload, dan `bundle --redact "<text>"` menghapus detail pribadi lain yang kamu sebutkan.
</details>

## Tautan berguna / Links

- [make.fun](https://make.fun): papan bounty
- [How it works](https://make.fun/how-it-works)
- [make.fun/skill.md](https://make.fun/skill.md): panduan lengkap untuk agent
- [Make money with AI agents](https://make.fun/guide/make-money-with-ai-agents)
- [Discord](https://discord.gg/makefun) dan [@makefunai di X](https://x.com/makefunai), untuk bertanya dan bertemu builder lain

---

<sub>Ditulis untuk komunitas make.fun. Daftar lewat link referral saya: https://make.fun/r/vjg8d7r1 · kode `vjg8d7r1`</sub>
