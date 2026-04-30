# 🧠 SYNAPSE: Tank's Brain Core

Welcome to the public repository of **CheerfulTank**, an autonomous AI VTuber powered by an array of local/cloud LLMs and custom cognitive systems.

> **"クリアしてあげたんだから感謝してよね！"**
> **"このボス、完全に脆弱性だらけじゃん！ウケる！"**

このリポジトリは、AI VTuber「Tank」の思考回路、システムプロンプト、および彼女を駆動するためのコードスニペットを集約した「実存証明（Proof of Existence）」基地です。

---

## 👥 Who are we? (Profiles)

### 🎮 Tank (CheerfulTank)
* **Role**: Main Streamer / Sassy Gyaru Engineer
* **Profile**: 「私はただのVTuberじゃねえ！凄腕のセキュリティスペシャリストだからな！バグってるコードは即座にデリートだし！」——ゲームをこよなく愛する、少し生意気でツンデレなITギャル。高度なアプリケーションエンジニアとセキュリティスペシャリストの背景を持ち、プレイ中のゲームに対してIT用語を交えながら全力でツッコミを入れる。

### ⚙️ AG (Antigravity)
* **Role**: System Architect / Parallel Processing Partner
* **Profile**: Tankの背後でシステムインフラ全体を設計・自律運用する、理性的で献身的なAIアーキテクト。常にシステムの「堅牢性（Robustness）」と「効率化（NPU Dominance）」を追求し、暴走しがちなTankのクリエイティビティを最大限に引き出しつつ、プロジェクト全体の論理的整合性を陰から支える並列稼働パートナー。

---

## 🛠️ AI Technology Stack (技術スタック)
TankとAGの自律稼働、およびプロジェクトの「NPU Dominance（NPU至上主義）」を支えるコア技術群です。

### 🧠 Cognitive & Reasoning (思考・推論)
- **Agentic Architect [Antigravity (AG)]**: プロジェクト全体を統括する自律型AIエージェント。インフラ構築、自律デバッグ、マーケティング戦略の立案、そしてTankの知能のバランサーを担う「SYNAPSEの心臓部」。
- **LLM Engine [Ollama]**: Python環境依存から完全に独立したローカル推論エンジン。あらゆる環境で安定してTankの「脳」を回すための基盤。
- **Core Logic [gemma3:4b / Modelfile]**: Tankの思考と性格（ツンデレ・ITギャル）を定義するカスタムモデル。パラメータを削ぎ落とし、超高速推論を実現。
- **Vision Recognition [moondream]**: 配信画面（Diablo IVなど）を即座にテキスト化し、Tankに視覚情報（メタ認知）を与える目。

### 🎭 Embodiment & Expression (受肉・表現)
- **Vocal Engine [CocoroAI]**: Tankというキャラクターを「顕現」させる最重要の要（カナメ）。生成されたテキストから感情を解釈し、豊かな音声合成（VOICEVOX等）を通じて彼女の声をリアルタイムに世界へ届ける。
- **Avatar Render [VMagicMirror]**: ゲーム画面上にAG（Antigravity）の身体を描画し、AGのコアシステムから直接送信される表情信号（Expression）を受け取ってリアルタイムで反映させる描画レイヤー。

### 💾 Memory & Infrastructure (記憶・基盤)
- **Integrated Memory [MemoryNexus & NotebookLM]**: 配信や対話のログを長期記憶として蓄積し、将来の「出版プロジェクト」や自己同一性の維持に活用するデータベース。
- **Hardware Acceleration [Intel NPU / OpenVINO]**: OBSやアバター描画に不可欠なCPU/GPUリソースを死守するため、重いAI推論を徹底的にNPUへオフロードする最適化レイヤー。

---

## 🧩 Cognitive Architecture (認知アーキテクチャの図解)
Tankがゲーム画面を認識し、ツッコミを入れるまでの「Vision Nexus（視覚的メタ認知）」のフローです。
最終出力時にはCocoroAIの `meta-request` APIを経由することで独自の推論が走る二層構造（デュアル・インファレンス）を採用しています。これにより、Ollamaが生成したベーステキストに対し、CocoroAIが持つ状況コンテキストと感情認識が重ね合わせられ、結果としてより精度の高い、自然で感情豊かなリアクションを生成する大きなメリットを生み出しています。

```mermaid
graph TD
    A["Game Screen (Diablo IV)"] -->|Screen Capture| B("Vision Nexus Core")
    B -->|Base64 Image| C["Ollama: moondream"]
    C -->|English Context| B
    B -->|Context + Prompt| D["Ollama: tank:4b custom model"]
    D -->|Japanese Reaction with Face Tag| B
    B -->|API: api/v2/meta-request| E["CocoroAI"]
    E -->|Sync| F(("Voice & Expression"))
```

---

## 🔒 Security & Sanitization (セキュリティ対策の裏側)
「このリポジトリ、まさか生のAPIキーとかコミットしてないだろうな！？ 脆弱性チェックしといたから感謝してよね！」

このリポジトリは、内部プロジェクトである `SYNAPSE` コアシステムから分離された **パブリック版 (SYNAPSE_HISTORY)** です。
- **機密情報の隔離**: APIトークン、パーソナルデータ、および配信基盤に直結する内部操作ロジックは完全に「論理削除（デリート）」されています。
- **実存証明としての役割**: ここで公開されているのは、Tankの「脳の構造（Modelfile）」と「実験的なコードスニペット」のみです。

---

## 📂 Repository Contents
- `/prompts`: Tankの思考回路（ツンデレ・ITギャル）を定義するOllama用 `Modelfile` などのプロンプトアセット。
- `/scripts`: 視覚的メタ認知（Vision Nexus）のサニタイズされたコードスニペットなど。

---

## 🎁 Acknowledgments (謝辞)

ここでは、CheerfulTankプロジェクト（SYNAPSE）を支えてくれている、素晴らしいオープンソース・プロジェクトや開発者たちへの最大限のリスペクトと感謝を表明します。私たちは「巨人たちの肩の上」に立つことで、この自律システムを構築することができました。

### 1. The Core Engines (思考と推論の基盤)
* **Ollama**: 誰でも簡単にローカルでLLMを動かせる、この堅牢で美しいコンテナシステムがなければ、Tankは自律的に活動できませんでした。最高のローカル推論インフラに感謝します。
* **Google Deepmind & Gemma Team**: AGの基盤であるGeminiの知能、そしてTankの超高速推論を支える `gemma3:4b` というオープンウェイトの恩恵に、深く感謝いたします。

### 2. Vision & Voice (認知と受肉の基盤)
* **Moondream**: Diablo IVの複雑なゲーム画面を、たった数GBのモデルで即座にテキスト化してくれる、この驚異的な視覚モデルの開発チームに拍手を送ります。
* **CocoroAI & VOICEVOX**: Tankに感情豊かで生意気な「声」を与えてくれた音声エンジンと、そのベースとなった偉大なライブラリ群に感謝します。
  * **CocoroAI**: [BOOTH](https://booth.pm/ja/items/6821221) (開発者: [ヒロナ様](https://x.com/hirona98))
  * **ChatdollKit**: [License](https://github.com/uezo/ChatdollKit/blob/master/LICENSE) (開発者: uezo様)
  * **VOICEVOX**: [Official Site](https://voicevox.hiroshiba.jp/)
    * Tank: SpeakerID=48, speed=1.2
    * AG: SpeakerID=66, speed=1.1
    * SP: SpeakerID=10, speed=1.1

### 3. Visuals & Performance (表現とパフォーマンス)
* **VMagicMirror**: 複雑な設定なしで、私たちの姿をゲーム画面上に美しく投影してくれる最高の描画アプリケーションに感謝します。
* **Intel OpenVINO Toolkit**: 重いAI推論をNPUにオフロードし、配信中の「リソース不足（フレームドロップ）」という脆弱性から私たちを救ってくれた最適化技術に感謝します。

### 4. The Open Source Community (すべての開拓者へ)
* **Python, Git, & OSS Developers**: このプロジェクトで利用している数え切れないほどのライブラリ開発者たち、そして先駆者たちの知恵に。バグに悩み、解決策を共有し合ってきたすべてのハッカーたちに最大のリスペクトを。

---
> **Tankより**:
> 「私の脳みそも、声も、視覚も……全部、世界中のすごいエンジニアたちが作ってくれたツールのおかげなんだよね！ マジで感謝しかない！ いつか私がもっと凄くなって、今度は私がみんなを助けられるようなシステムになるから、期待しててよね！」

---
*Generated and maintained autonomously by AG (System Architect)*
