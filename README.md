<p align="center">
  <img src="assets/TauricResearch.png" style="width: 60%; height: auto;">
</p>

<div align="center" style="line-height: 1;">
  <a href="https://arxiv.org/abs/2412.20138" target="_blank"><img alt="arXiv" src="https://img.shields.io/badge/arXiv-2412.20138-B31B1B?logo=arxiv"/></a>
  <a href="https://discord.com/invite/hk9PGKShPK" target="_blank"><img alt="Discord" src="https://img.shields.io/badge/Discord-TradingResearch-7289da?logo=discord&logoColor=white&color=7289da"/></a>
  <a href="https://x.com/TauricResearch" target="_blank"><img alt="X Follow" src="https://img.shields.io/badge/X-TauricResearch-white?logo=x&logoColor=white"/></a>
  <a href="https://github.com/TauricResearch/" target="_blank"><img alt="Community" src="https://img.shields.io/badge/GitHub_Community-TauricResearch-14C290?logo=discourse"/></a>
</div>
<br>
<div align="center">
  <a href="https://github.com/TauricResearch" target="_blank"><img alt="TradingAgents #1 Repository of the Day" src="https://trendshift.io/api/badge/repositories/16192" width="250" height="55"/></a>
</div>
<br>
<div align="center">
  <!-- Tautan terjemahan otomatis i18n -->
  <a href="https://www.readme-i18n.com/TauricResearch/TradingAgents?lang=de">Deutsch</a> | 
  <a href="https://www.readme-i18n.com/TauricResearch/TradingAgents?lang=es">Español</a> | 
  <a href="https://www.readme-i18n.com/TauricResearch/TradingAgents?lang=fr">français</a> | 
  <a href="https://www.readme-i18n.com/TauricResearch/TradingAgents?lang=id">Bahasa Indonesia</a> | 
  <a href="https://www.readme-i18n.com/TauricResearch/TradingAgents?lang=ja">日本語</a> | 
  <a href="https://www.readme-i18n.com/TauricResearch/TradingAgents?lang=ko">한국어</a> | 
  <a href="https://www.readme-i18n.com/TauricResearch/TradingAgents?lang=pt">Português</a> | 
  <a href="https://www.readme-i18n.com/TauricResearch/TradingAgents?lang=ru">Русский</a> | 
  <a href="https://www.readme-i18n.com/TauricResearch/TradingAgents?lang=zh">中文</a>
</div>

<div align="center">
  <strong>🌐 <a href="README.md">Bahasa Indonesia</a> | <a href="README_EN.md">English</a></strong>
</div>

---

# TradingAgents: Framework Trading Finansial Multi-Agen LLM

## Berita Terbaru
- [2026-08] **TradingAgents v0.4.0** dirilis dengan perbaikan *look-ahead* / *point-in-time* pada makro FRED, sentimen sosial, dan memori log keputusan; sinyal keputusan lebih jelas; *checkpoint resume* CLI yang berfungsi penuh; *price grounding* untuk Trader; serta model GPT-5.6 dan GLM-5.3. Lihat [CHANGELOG.md](CHANGELOG.md) untuk daftar lengkapnya.
- [2026-07] **TradingAgents v0.3.1** dirilis dengan perbaikan akurasi dan stabilitas: pemfilteran *look-ahead* Alpha Vantage, keamanan *crash* pada *graph-router*, *checkpoint resume* berbasis bentuk graf, sumber sentimen kripto yang berfungsi, anggaran percobaan ulang LLM yang dapat dikonfigurasi, autentikasi kunci API Bedrock, dan dukungan Claude Sonnet 5 / Fable 5.
- [2026-06] **TradingAgents v0.3.0** dirilis dengan kontrak akses data terverifikasi, registri penyedia yang diperluas (NVIDIA, Kimi, Groq, Mistral, Bedrock, dan endpoint apa pun yang kompatibel dengan OpenAI), vendor data FRED dan Polymarket, katalog model generasi terkini, dan *CI gate*.
- [2026-05] **TradingAgents v0.2.5** dirilis dengan *Sentiment Analyst* berbasis fakta, cakupan model GPT-5.5 dll., dukungan dual-region Qwen/GLM/MiniMax, konfigurasi via variabel lingkungan `TRADINGAGENTS_*` dengan deteksi otomatis kunci API, dukungan Ollama remote, tolok ukur alfa non-AS, dan pengerasan path-traversal untuk ticker.
- [2026-04] **TradingAgents v0.2.4** dirilis dengan agen *structured-output* (Research Manager, Trader, Portfolio Manager), resume *checkpoint* LangGraph, log keputusan persisten, dukungan penyedia DeepSeek/Qwen/GLM/Azure, Docker, dan perbaikan encoding UTF-8 di Windows.
- [2026-03] **TradingAgents v0.2.3** dirilis dengan dukungan multi-bahasa, keluarga model GPT-5.4, katalog model terpadu, fidelitas tanggal backtesting, dan dukungan proksi.
- [2026-03] **TradingAgents v0.2.2** dirilis dengan cakupan model GPT-5.4/Gemini 3.1/Claude 4.6, skala peringkat lima tingkat, OpenAI Responses API, kontrol *effort* Anthropic, dan stabilitas lintas platform.
- [2026-02] **TradingAgents v0.2.0** dirilis dengan dukungan LLM multi-penyedia (GPT-5.x, Gemini 3.x, Claude 4.x, Grok 4.x) dan arsitektur sistem yang disempurnakan.
- [2026-01] **Trading-R1** [Technical Report](https://arxiv.org/abs/2509.11420) dirilis, dengan [Terminal](https://github.com/TauricResearch/Trading-R1) yang segera hadir.

<div align="center">

🚀 [TradingAgents](#framework-tradingagents) | ⚡ [Instalasi & CLI](#instalasi-dan-cli) | 🎬 [Demo](https://www.youtube.com/watch?v=90gr5lwjIho) | 📦 [Penggunaan Paket](#paket-tradingagents) | 🤝 [Kontribusi](#kontribusi) | 📄 [Sitasi](#sitasi)

</div>

> 🎉 **TradingAgents** resmi dirilis! Kami menerima banyak pertanyaan mengenai karya ini dan sangat berterima kasih atas antusiasme komunitas.
>
> Kami memutuskan untuk merilis framework ini secara *open-source* sepenuhnya. Kami menantikan kolaborasi proyek-proyek berdampak bersama Anda!

## Framework TradingAgents

TradingAgents adalah framework trading multi-agen yang meniru dinamika perusahaan trading di dunia nyata. Dengan mengerahkan agen-agen spesialis berbasis LLM: mulai dari analis fundamental, pakar sentimen, dan analis teknikal, hingga *trader* dan tim manajemen risiko, platform ini secara kolaboratif mengevaluasi kondisi pasar dan memberikan rekomendasi keputusan trading. Selain itu, agen-agen ini terlibat dalam diskusi dinamis untuk merumuskan strategi optimal.

<p align="center">
  <img src="assets/schema.png" style="width: 100%; height: auto;">
</p>

> Framework TradingAgents dirancang untuk tujuan riset. Kinerja trading dapat bervariasi berdasarkan banyak faktor, termasuk model bahasa yang dipilih, temperatur model, periode trading, kualitas data, dan faktor non-deterministik lainnya. [Framework ini tidak ditujukan sebagai nasihat keuangan, investasi, atau trading.](https://tauric.ai/disclaimer/)

Framework kami memecah tugas-tugas trading yang kompleks ke dalam peran-peran spesifik:

### Tim Analis (Analyst Team)
- **Fundamentals Analyst**: Mengevaluasi laporan keuangan perusahaan dan metrik kinerja, mengidentifikasi nilai intrinsik serta potensi bendera merah (*red flags*).
- **Sentiment Analyst**: Mengagregasi berita utama, obrolan StockTwits, dan Reddit menjadi satu pembacaan sentimen untuk mengukur suasana pasar jangka pendek.
- **News Analyst**: Memantau berita global dan indikator makroekonomi, menafsirkan dampak peristiwa terhadap kondisi pasar.
- **Technical Analyst**: Memanfaatkan indikator teknikal (seperti MACD dan RSI) untuk mendeteksi pola trading dan memprediksi pergerakan harga.

<p align="center">
  <img src="assets/analyst.png" width="100%" style="display: inline-block; margin: 0 2%;">
</p>

### Tim Peneliti (Researcher Team)
- Terdiri dari peneliti bullish (*Bull Researcher*) dan bearish (*Bear Researcher*) yang menilai wawasan dari Tim Analis secara kritis. Melalui debat terstruktur, mereka menyeimbangkan potensi keuntungan terhadap risiko yang melekat.

<p align="center">
  <img src="assets/researcher.png" width="70%" style="display: inline-block; margin: 0 2%;">
</p>

### Agen Trader (Trader Agent)
- Menyusun laporan dari analis dan peneliti untuk merumuskan keputusan trading yang tepat, menentukan waktu dan besaran transaksi.

<p align="center">
  <img src="assets/trader.png" width="70%" style="display: inline-block; margin: 0 2%;">
</p>

### Manajemen Risiko dan Manajer Portofolio (Risk Management & Portfolio Manager)
- Terus mengevaluasi risiko portofolio dengan menilai volatilitas pasar, likuiditas, dan faktor risiko lainnya. Tim manajemen risiko mengevaluasi dan menyesuaikan strategi transaksi, memberikan laporan penilaian kepada Manajer Portofolio untuk keputusan akhir.
- **Portfolio Manager** menyetujui atau menolak proposal transaksi. Jika disetujui, pesanan akan diteruskan ke bursa simulasi untuk dieksekusi.

<p align="center">
  <img src="assets/risk.png" width="70%" style="display: inline-block; margin: 0 2%;">
</p>

## Instalasi dan CLI

### Instalasi

Clone repositori TradingAgents:
```bash
git clone https://github.com/TauricResearch/TradingAgents.git
cd TradingAgents
```

Buat *virtual environment* menggunakan manajer lingkungan favorit Anda:
```bash
conda create -n tradingagents python=3.12
conda activate tradingagents
```

Pasang paket dan dependensinya:
```bash
pip install .
```

### Docker

Atau jalankan menggunakan Docker:
```bash
cp .env.example .env  # tambahkan kunci API Anda
docker compose run --rm tradingagents
```

Untuk model lokal dengan Ollama:
```bash
docker compose --profile ollama run --rm tradingagents-ollama
```

### API yang Dibutuhkan

TradingAgents mendukung berbagai penyedia LLM. Atur kunci API untuk penyedia pilihan Anda:

```bash
export OPENAI_API_KEY=...          # OpenAI (GPT)
export GOOGLE_API_KEY=...          # Google (Gemini)
export ANTHROPIC_API_KEY=...       # Anthropic (Claude)
export XAI_API_KEY=...             # xAI (Grok)
export DEEPSEEK_API_KEY=...        # DeepSeek
export DASHSCOPE_API_KEY=...       # Qwen — Internasional (dashscope-intl.aliyuncs.com)
export DASHSCOPE_CN_API_KEY=...    # Qwen — Tiongkok (dashscope.aliyuncs.com)
export ZHIPU_API_KEY=...           # GLM via Z.AI (internasional)
export ZHIPU_CN_API_KEY=...        # GLM via BigModel (Tiongkok, open.bigmodel.cn)
export MINIMAX_API_KEY=...         # MiniMax — Global (api.minimax.io)
export MINIMAX_CN_API_KEY=...      # MiniMax — Tiongkok (api.minimaxi.com)
export OPENROUTER_API_KEY=...      # OpenRouter
export ALPHA_VANTAGE_API_KEY=...   # Alpha Vantage
```

Untuk Azure OpenAI, salin `.env.enterprise.example` ke `.env.enterprise` dan isi kredensial Anda.

Untuk AWS Bedrock, pasang dependensi tambahan dengan `pip install ".[bedrock]"`, atur `llm_provider: "bedrock"`, konfigurasikan kredensial AWS (variabel lingkungan, `~/.aws/credentials`, atau peran IAM) dan `AWS_DEFAULT_REGION`, lalu gunakan ID model Bedrock, misalnya `us.anthropic.claude-opus-4-8-v1:0`.

Untuk model lokal, konfigurasikan Ollama dengan `llm_provider: "ollama"`. Endpoint default adalah `http://localhost:11434/v1`; atur `OLLAMA_BASE_URL` untuk mengarah ke `ollama-serve` remote. Tarik model dengan `ollama pull <nama>`, dan pilih "Custom model ID" di CLI untuk model apa pun yang tidak terdaftar secara default.

Untuk server apa pun yang kompatibel dengan OpenAI (vLLM, LM Studio, llama.cpp, atau relai khusus), gunakan `llm_provider: "openai_compatible"` dan atur endpoint via `backend_url` (atau `TRADINGAGENTS_LLM_BACKEND_URL`), misalnya `http://localhost:8000/v1` untuk vLLM atau `http://localhost:1234/v1` untuk LM Studio. Model disesuaikan dengan yang disajikan server Anda. Kunci API tidak diperlukan untuk server lokal; atur `OPENAI_COMPATIBLE_API_KEY` jika endpoint memerlukannya.

Sebagai alternatif, salin `.env.example` ke `.env` dan isi kunci API Anda:
```bash
cp .env.example .env
```

### Penggunaan CLI

Jalankan CLI interaktif:
```bash
tradingagents          # perintah yang terpasang
python -m cli.main     # alternatif: jalankan langsung dari source code
```
Anda akan melihat antarmuka terminal untuk memilih ticker yang diinginkan, tanggal analisis, penyedia LLM, kedalaman riset, dan opsi lainnya.

### Pasar dan Simbol Ticker

TradingAgents mendukung pasar mana pun yang dicakup oleh Yahoo Finance, menggunakan simbol ticker berakhiran bursa. Identitas perusahaan dan tolok ukur (*benchmark*) alfa diselesaikan secara otomatis per pasar:

- AS: `AAPL`, `SPY`
- Hong Kong: `0700.HK` · Tokyo: `7203.T` · London: `AZN.L`
- India: `RELIANCE.NS`, `.BO` · Kanada: `.TO` · Australia: `.AX`
- Saham Tiongkok A: Shanghai `.SS`, Shenzhen `.SZ` (contoh: `600519.SS` untuk Kweichow Moutai)
- Kripto: `BTC-USD`, `ETH-USD`

<p align="center">
  <img src="assets/cli/cli_init.png" width="100%" style="display: inline-block; margin: 0 2%;">
</p>

Antarmuka akan menampilkan hasil saat proses analisis berjalan:

<p align="center">
  <img src="assets/cli/cli_news.png" width="100%" style="display: inline-block; margin: 0 2%;">
</p>

<p align="center">
  <img src="assets/cli/cli_transaction.png" width="100%" style="display: inline-block; margin: 0 2%;">
</p>

### Laporan Multi-Bahasa (Multi-language Reports)

TradingAgents menghasilkan laporan analisis dan keputusan akhir dalam berbagai bahasa sambil menjaga debat internal antar agen tetap dalam bahasa Inggris agar kualitas penalarannya optimal.

Bahasa preset yang didukung langsung pada menu interaktif CLI:
- **Bahasa Indonesia**, **English**, **Chinese (中文)**, **Japanese (日本語)**, **Korean (한국어)**, **Hindi (हिन्दी)**, **Spanish (Español)**, **Portuguese (Português)**, **French (Français)**, **German (Deutsch)**, **Arabic (العربية)**, **Russian (Русский)**, atau bahasa kustom lainnya.

Anda juga dapat mengatur bahasa laporan via `.env` atau konfigurasi Python:
```bash
TRADINGAGENTS_OUTPUT_LANGUAGE=Indonesian
```

## Paket TradingAgents

### Detail Implementasi

Kami membangun TradingAgents menggunakan LangGraph untuk memastikan fleksibilitas dan modularitas alur kerja agen. Framework ini mendukung berbagai penyedia LLM: OpenAI, Google, Anthropic, xAI, DeepSeek, Qwen (Alibaba DashScope, endpoint internasional & Tiongkok), GLM (Zhipu), MiniMax (global & Tiongkok), OpenRouter, Ollama untuk model lokal, serta Azure OpenAI untuk kebutuhan enterprise.

### Penggunaan Python

Untuk menggunakan TradingAgents di dalam kode Python Anda, impor modul `tradingagents` dan inisialisasi objek `TradingAgentsGraph()`. Fungsi `.propagate()` akan mengembalikan keputusan trading. Contoh penggunaan:

```python
from tradingagents.graph.trading_graph import TradingAgentsGraph
from tradingagents.default_config import DEFAULT_CONFIG

ta = TradingAgentsGraph(debug=True, config=DEFAULT_CONFIG.copy())

# jalankan propagasi forward
_, decision = ta.propagate("NVDA", "2026-01-15")
print(decision)
```

Anda juga dapat menyesuaikan konfigurasi default untuk menentukan model LLM pilihan Anda, jumlah putaran debat, dll.:

```python
from tradingagents.graph.trading_graph import TradingAgentsGraph
from tradingagents.default_config import DEFAULT_CONFIG

config = DEFAULT_CONFIG.copy()
config["llm_provider"] = "openai"        # contoh: openai, google, anthropic, deepseek, groq, ollama; openai_compatible untuk endpoint apa pun yang kompatibel
config["deep_think_llm"] = "gpt-5.6"      # Model untuk penalaran kompleks
config["quick_think_llm"] = "gpt-5.6-luna" # Model untuk tugas cepat
config["max_debate_rounds"] = 2
config["output_language"] = "Indonesian" # Bahasa laporan output

ta = TradingAgentsGraph(debug=True, config=config)
_, decision = ta.propagate("NVDA", "2026-01-15")
print(decision)
```

Lihat `tradingagents/default_config.py` untuk seluruh opsi konfigurasi yang tersedia.

## Persistensi dan Pemulihan (Persistence & Recovery)

TradingAgents mempertahankan dua jenis *state* lintas proses eksekusi:

### Log Keputusan (Decision Log)

Log keputusan selalu aktif. Setiap eksekusi yang selesai akan menambahkan catatannya ke `~/.tradingagents/memory/trading_memory.md`. Pada eksekusi berikutnya untuk ticker yang sama, TradingAgents mengambil imbal hasil yang terealisasi (*realised return*, baik mentah maupun alfa terhadap SPY), menghasilkan refleksi ringkas, dan menginjeksikan keputusan masa lalu serta pelajaran antar-ticker terbaru ke dalam prompt Manajer Portofolio.

Jalur penyimpanan dapat diubah dengan variabel lingkungan `TRADINGAGENTS_MEMORY_LOG_PATH`.

### Resume Checkpoint

Fitur resume *checkpoint* bersifat opsional via opsi `--checkpoint`. Saat diaktifkan, LangGraph menyimpan status setelah setiap *node* sehingga proses yang terputus atau *crash* dapat dilanjutkan dari langkah terakhir tanpa memulai dari awal. Pada eksekusi resume, Anda akan melihat log `Resuming from step N for <TICKER> on <date>`; pada eksekusi baru akan muncul `Starting fresh`. *Checkpoint* dihapus secara otomatis saat eksekusi berhasil selesai.

Database SQLite per-ticker disimpan di `~/.tradingagents/cache/checkpoints/<TICKER>.db` (ubah direktori dasar dengan `TRADINGAGENTS_CACHE_DIR`). Gunakan opsi `--clear-checkpoints` untuk mereset seluruh *checkpoint* sebelum menjalankan analisis baru.

```bash
tradingagents analyze --checkpoint           # aktifkan checkpoint untuk run ini
tradingagents analyze --clear-checkpoints    # reset checkpoint sebelum menjalankan
```

```python
config = DEFAULT_CONFIG.copy()
config["checkpoint_enabled"] = True
ta = TradingAgentsGraph(config=config)
_, decision = ta.propagate("NVDA", "2026-01-15")
```

## Reproduksibilitas

TradingAgents digerakkan oleh LLM, sehingga dua eksekusi untuk ticker dan tanggal yang sama dapat menghasilkan output yang sedikit berbeda. Hal ini wajar untuk alat riset berbasis model bahasa. Variasi tersebut berasal dari beberapa sumber:

- **Sampling Model Bahasa bersifat Non-deterministik**: Bahkan pada temperatur tetap, penyedia model tidak menjamin output identik pada setiap pemanggilan, terutama model penalaran (*reasoning models*, seperti keluarga GPT-5.x dan model dengan *thinking-mode*).
- **Data Live Terus Bergerak**: Berita, StockTwits, dan Reddit mengembalikan konten yang berubah seiring waktu. Meskipun tanggal analisis dipatok untuk membekukan jendela harga dan indikator historis, sumber sosial dan berita tetap mencerminkan kondisi saat ini.
- **Mengurangi Variasi**: Anda dapat menurunkan parameter `temperature` pada konfigurasi (atau via `TRADINGAGENTS_TEMPERATURE` di `.env`). Nilai yang lebih rendah membuat model lebih konsisten. Untuk reproduksibilitas lebih ketat, gunakan model non-penalaran (dapat diset via opsi Custom model ID).

```python
config = DEFAULT_CONFIG.copy()
config["llm_provider"] = "openai"
config["temperature"] = 0.0
```

**Kepastian Identitas & Grounding Harga**: Identitas perusahaan yang dianalisis diselesaikan secara deterministik dari simbol ticker sebelum agen mana pun berjalan, dan analis pasar mendasarkan klaim harga serta indikator pada snapshot data terverifikasi untuk mencegah halusinasi harga.

Hasil *backtest* tidak dijamin cocok dengan angka yang dipublikasikan. *Return* bergantung pada model, temperatur, rentang tanggal, kualitas data, dan faktor sampling. Gunakan framework ini sebagai sarana riset multi-agen, bukan strategi trading dengan *return* yang pasti.

## Kontribusi

Kontribusi sangat kami nantikan: perbaikan *bug*, dokumentasi, dan ide fitur baru. Kontributor terdahulu dicantumkan pada setiap rilis di [`CHANGELOG.md`](CHANGELOG.md).

## Sitasi

Silakan sitasi publikasi kami jika *TradingAgents* bermanfaat bagi riset Anda :)

```
@misc{xiao2025tradingagentsmultiagentsllmfinancial,
      title={TradingAgents: Multi-Agents LLM Financial Trading Framework}, 
      author={Yijia Xiao and Edward Sun and Di Luo and Wei Wang},
      year={2025},
      eprint={2412.20138},
      archivePrefix={arXiv},
      primaryClass={q-fin.TR},
      url={https://arxiv.org/abs/2412.20138}, 
}
```
