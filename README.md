# AI-MeetingRoom（デジタルペルソナ会議室）

複数のAIペルソナが議論し、時代や領域を超えた多角的視点から
意思決定を支援するマルチエージェント型シミュレーションシステム。

🔗 **URL**: https://ai-meeting-room-production.up.railway.app/

---

## 開発意図
「異なる専門性の衝突こそが新たな示唆を生む」という仮説に基づき、
実際の会議では参加者の経験や立場に縛られて得られない視点を、
時代や領域を超えた人格を呼び出すことで低コストに引き出す。

## 主な特徴
- **マルチエージェント方式**：ペルソナごとに独立したコンテキストと
  知識ベースを保持。単一LLMに複数人格を持たせる方式と異なり、
  会話進行に伴う発言の均質化を防ぐ。
- **RAGによる知識補完**：各ペルソナの発言に外部データを根拠として付与。
- **成熟度スコアによる改善ループ**：知識量・会話精度・人格準拠度の
  3軸でペルソナ成熟度を定量評価。閾値未達のペルソナから優先的にプロンプトと
  知識ベースを改善するサイクルを運用。利用者評価もスコアに直接反映(会話精度・人格準拠度スコア)する設計とした。

## 技術スタック
- 言語：Python
- DB：PostgreSQL
- LLM：Claude API
- インフラ：Railway

## システム構成
（<img width="1082" height="510" alt="image" src="https://github.com/user-attachments/assets/7b6ff27f-b1d5-4d2c-9ffb-60ede8148359" />


## デモ
<img width="1919" height="985" alt="image" src="https://github.com/user-attachments/assets/d11bae40-401f-4b5b-91c6-038eaeff4f24" />
