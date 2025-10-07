# roBa × moNa2 Compatible ZMK Firmware

kumakey さんの **roBa** ハードを、**moNa2 として認識**させる ZMK ファームです。  
BLE/USB の **デバイス名だけを moNa2 に“偽装（masquerade）”** し、配線は roBa 準拠。  
作者の皆さまへ敬意を込めた、遊び心あるプロジェクトです。

## ✨ 特徴
- roBa（kumakey） / Seeed XIAO nRF52840 ×2（左右）
- BLE split（左=Central / 右=Peripheral）
- PMW3610（右トラックボール）
- Choc V2（ホットスワップ）、LEDなし
- 表示名: **moNa2 / moNa2-P**（※VID/PIDは変更しません）

## 🚀 GitHub Actions で UF2 を自動生成
1. このフォルダ一式を GitHub の新規リポジトリへアップロード  
2. 「Actions」タブ → “Build ZMK Firmware” が自動で実行  
3. 完了後、**Artifacts** から `zmk-uf2` をダウンロード  
4. `left.uf2` / `right.uf2` を XIAO にコピー

> USB名も moNa2 にしたい場合は、ビルドに `-DDTC_OVERLAY_FILE=docs/usbd_masq_mona.overlay` を追加。

## 🙌 クレジット
- Hardware: **roBa** by kumakey  
- Firmware Inspiration: **moNa2** by pooh_polo  
- PMW3610 Driver: **badjeff**  
- Firmware Base: **ZMK Project**  
- Integration: **saru (2025)**
