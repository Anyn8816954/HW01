# DSP Assignment 1

### RC Low-Pass Filter | 數位訊號處理作業

本專案探討一階 RC 低通濾波器，包含相量分析、頻率響應、暫態響應，以及離散時間與音訊濾波結果。

> **作業資料：** 通訊碩一　｜　**學號：** 711581103　｜　**姓名：** 吳祖慷

## 專案重點

| 項目 | 內容 |
| --- | --- |
| 電阻 | 1,000 Ω |
| 電容 | 1 / (2π × 400 × 1,000) F |
| 時間常數 | RC = 1 / (800π) s |
| 截止頻率 | 400 Hz |
| 實作 | C 語言音訊產生與 RC 濾波 |

## 頻率響應

| 輸入頻率 | 增益 \|H\| | 相位 |
| ---: | ---: | ---: |
| 100 Hz | 0.9701 | −14.04° |
| 400 Hz | 0.7071 | −45.00° |
| 3,000 Hz | 0.1322 | −82.41° |

低頻訊號大致保留；頻率越高，輸出衰減越明顯。

## 波形預覽

下圖為 8 kHz 取樣率、400 Hz 輸入的濾波前後波形比較。

<img src="hw1/figure/waveform_fs8000_f400.png" alt="8 kHz sampling rate, 400 Hz input: before and after RC filtering" width="720" />

## 專案內容

- [作業摘要、手寫解答與波形圖](hw1/README.md)
- [RC 濾波程式](hw1/RC_filtering.c)
- [WAV 訊號產生程式](hw1/sine_wav_gen.c)
- [波形繪圖程式](hw1/plot_waveforms.py)

完整圖表與各題說明請前往 [hw1 作業頁面](hw1/README.md)。
