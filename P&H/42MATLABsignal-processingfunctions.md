
|search|items|URL|
|:--|:--|:--|
|42 MATLAB signal-processing functions| 344|
|42 signal-processing functions|408|
|signal-processing functions|10787|
|Signal Processing Toolbox| 11543|https://jp.mathworks.com/help/signal/index.html?
|||s_tid=srchtitle_support_results_1_Signal%2520Processing%2520Toolbox|



|N.|function|description|
|:--|:--|:--|
||信号の生成、解析、および前処理 波形生成 波形
|1|sin	|ラジアン単位の引数の正弦|
|2|square	|矩形波|
||変調および量子化
|3|framesig|	Partition signal into frames (R2024a 以降)
||測定と特徴抽出 記述統計 Statistics
|4|cummax|	累積最大値
|5|cummin|	累積最小値
|6|envelope|	信号の包絡線
|7|メモ:max|	配列の最大要素
|8|メモ:mean|	配列の平均値
|9|メモ:median|	配列の中央値
|10|メモ:min|	配列の最小要素
|11|メモ:std|	標準偏差
|12|メモ:var	|分散
||特徴抽出
|13|メモ:findpeaks	局所的最大値
|14|refinepeaks	Refine peak value and location estimates (R2024b 以降)
|15|メモ:signalFrequencyFeatureExtractor	Streamline signal frequency feature extraction (R2021b 以降)
|16|メモ:signalTimeFeatureExtractor	Streamline signal time feature extraction
|17|メモ:signalTimeFrequencyFeatureExtractor	Streamline signal time-frequency feature extraction (R2024a 以降)
||信号のラベル付け
||18|framesig	Partition signal into frames (R2024a 以降)
||19|sigrangebinmask	Label signal samples with values within a specified range (R2023a 以降)
||スペクトル測定 パワーと帯域幅
メモ:signalFrequencyFeatureExtractor	Streamline signal frequency feature extraction (R2021b 以降)
メモ:signalTimeFrequencyFeatureExtractor	Streamline signal time-frequency feature extraction (R2024a 以降)
spectralCrest	Spectral crest for signals and spectrograms
spectralEntropy	Spectral entropy for signals and spectrograms
spectralFlatness	Spectral flatness for signals and spectrograms
spectralKurtosis	Spectral kurtosis for signals and spectrograms
spectralSkewness	Spectral skewness for signals and spectrograms
高調波測定
メモ:signalTimeFeatureExtractor	Streamline signal time feature extraction
変換、相関、およびモデリング
変換
離散フーリエ変換とコサイン変換
abs	絶対値と複素数の大きさ
angle	位相角
fft	高速フーリエ変換
fft2	2 次元の高速フーリエ変換
fftshift	ゼロ周波数成分をスペクトルの中心に移動
メモ:ifft	逆フーリエ高速変換
メモ:ifft2	2 次元逆高速フーリエ変換
ifftshift	逆ゼロ周波数シフト
ヒルベルト変換とウォルシュ・アダマール変換
envelope	信号の包絡線
hilbert	ヒルベルト変換を使用した離散時間解析信号
時間-周波数解析
メモ:dlistft	Deep learning inverse short-time Fourier transform (R2024a 以降)
メモ:dlstft	深層学習の短時間フーリエ変換
メモ:fsst	フーリエ シンクロスクイーズド変換
メモ:ifsst	逆フーリエ シンクロスクイーズド変換
メモ:istft	逆短時間フーリエ変換
メモ:istftLayer	Inverse short-time Fourier transform layer (R2024a 以降)
メモ:spectrogram	短時間フーリエ変換を使用したスペクトログラム
メモ:stft	短時間フーリエ変換
メモ:stftLayer	Short-time Fourier transform layer (R2021b 以降)
wvd	Wigner-Ville 分布と平滑化疑似 Wigner-Ville 分布
メモ:xspectrogram	短時間フーリエ変換を使用したクロス スペクトログラム
ビット反転
bitrevorder	データのビット反転順への並べ替え
相関と畳み込み
畳み込み
conv	畳み込みおよび多項式乗算
conv2	2 次元の畳み込み
デジタル フィルターとアナログ フィルター
デジタル フィルター解析
周波数領域応答
abs	絶対値と複素数の大きさ
angle	位相角
デジタル フィルター処理
フィルター関数
ctffilt	Cascaded transfer function filtering (R2024b 以降)
メモ:fftfilt	オーバーラップ加算法を使用した FFT ベースの FIR フィルター処理
メモ:filter	1 次元のデジタル フィルター
メモ:filtfilt	ゼロ位相デジタル フィルター処理
畳み込み
conv	畳み込みおよび多項式乗算
conv2	2 次元の畳み込み
線形システムの変換
ctf2zp	Convert cascaded transfer functions to zero-pole-gain form (R2024b 以降)
sos2ctf	Convert digital filter second-order section parameters to cascaded transfer function form (R2024a 以降)
zp2ctf	Convert zero-pole-gain filter parameters to cascaded transfer function form (R2024a 以降)
マルチレート信号処理
downsample	整数係数によるサンプル レートの低減
メモ:interp1	1 次データ内挿 (テーブル ルックアップ)
メモ:resample	均一または不均一なデータを新しい固定レートでリサンプリング
upsample	整数係数によるサンプル レートの増加
スペクトル解析
スペクトル推定
推定器
メモ:findpeaks	局所的最大値
periodogram	ピリオドグラム パワー スペクトル密度推定
pwelch	ウェルチのパワー スペクトル密度推定
refinepeaks	Refine peak value and location estimates (R2024b 以降)
spectralEntropy	Spectral entropy for signals and spectrograms
データ管理
メモ:paddata	Pad data by adding elements (R2023b 以降)
メモ:trimdata	Trim data by removing elements (R2023b 以降)
パラメトリック スペクトル推定
メモ:findpeaks	局所的最大値
refinepeaks	Refine peak value and location estimates (R2024b 以降)
ウィンドウ
スペクトル ウィンドウ
blackman	ブラックマン ウィンドウ
chebwin	チェビシェフ ウィンドウ
flattopwin	フラット トップ加重ウィンドウ
hamming	ハミング ウィンドウ
hann	ハン (ハニング) ウィンドウ
kaiser	カイザー ウィンドウ
時間-周波数解析
変換
メモ:dlistft	Deep learning inverse short-time Fourier transform (R2024a 以降)
メモ:dlstft	深層学習の短時間フーリエ変換
メモ:fsst	フーリエ シンクロスクイーズド変換
メモ:ifsst	逆フーリエ シンクロスクイーズド変換
メモ:istft	逆短時間フーリエ変換
メモ:istftLayer	Inverse short-time Fourier transform layer (R2024a 以降)
メモ:spectrogram	短時間フーリエ変換を使用したスペクトログラム
メモ:stft	短時間フーリエ変換
メモ:stftLayer	Short-time Fourier transform layer (R2021b 以降)
wvd	Wigner-Ville 分布と平滑化疑似 Wigner-Ville 分布
メモ:xspectrogram	短時間フーリエ変換を使用したクロス スペクトログラム
スペクトルの記述子
spectralCrest	Spectral crest for signals and spectrograms
spectralEntropy	Spectral entropy for signals and spectrograms
spectralFlatness	Spectral flatness for signals and spectrograms
spectralKurtosis	Spectral kurtosis for signals and spectrograms
spectralSkewness	Spectral skewness for signals and spectrograms
データ適応法
メモ:ewt	経験的ウェーブレット変換
ウェーブレットを使用した時間-周波数解析
メモ:cqt	Constant-Q nonstationary Gabor transform
メモ:cwt	連続 1 次元ウェーブレット変換
メモ:modwpt	Maximal overlap discrete wavelet packet transform
メモ:modwt	最大重複離散ウェーブレット変換
tqwt	Tunable Q-factor wavelet transform (R2021b 以降)
メモ:waveletScattering	Wavelet time scattering
メモ:wcoherence	ウェーブレット コヒーレンスとウェーブレット クロス スペクトル
信号向け AI
分類
データストア、特徴抽出器、および層
cwtLayer	Continuous wavelet transform layer (R2022b 以降)
icwtLayer	Inverse continuous wavelet transform layer (R2024b 以降)
メモ:istftLayer	Inverse short-time Fourier transform layer (R2024a 以降)
メモ:modwtLayer	Maximal overlap discrete wavelet transform layer (R2022b 以降)
メモ:signalFrequencyFeatureExtractor	Streamline signal frequency feature extraction (R2021b 以降)
メモ:signalTimeFeatureExtractor	Streamline signal time feature extraction
メモ:signalTimeFrequencyFeatureExtractor	Streamline signal time-frequency feature extraction (R2024a 以降)
メモ:stftLayer	Short-time Fourier transform layer (R2021b 以降)
メモ:waveletScattering	Wavelet time scattering
回帰
データストア、特徴抽出器、および層
cwtLayer	Continuous wavelet transform layer (R2022b 以降)
icwtLayer	Inverse continuous wavelet transform layer (R2024b 以降)
メモ:istftLayer	Inverse short-time Fourier transform layer (R2024a 以降)
メモ:modwtLayer	Maximal overlap discrete wavelet transform layer (R2022b 以降)
メモ:signalFrequencyFeatureExtractor	Streamline signal frequency feature extraction (R2021b 以降)
メモ:signalTimeFeatureExtractor	Streamline signal time feature extraction
メモ:signalTimeFrequencyFeatureExtractor	Streamline signal time-frequency feature extraction (R2024a 以降)
メモ:stftLayer	Short-time Fourier transform layer (R2021b 以降)
メモ:waveletScattering	Wavelet time scattering
前処理と特徴抽出
信号の前処理と測定
envelope	信号の包絡線
メモ:findpeaks	局所的最大値
refinepeaks	Refine peak value and location estimates (R2024b 以降)
データストアとデータの管理
メモ:paddata	Pad data by adding elements (R2023b 以降)
メモ:trimdata	Trim data by removing elements (R2023b 以降)
時間領域の特徴
メモ:mean	配列の平均値
メモ:signalTimeFeatureExtractor	Streamline signal time feature extraction
メモ:std	標準偏差
周波数領域の特徴
pwelch	ウェルチのパワー スペクトル密度推定
メモ:signalFrequencyFeatureExtractor	Streamline signal frequency feature extraction (R2021b 以降)
時間-周波数変換
メモ:cwt	連続 1 次元ウェーブレット変換
メモ:fsst	フーリエ シンクロスクイーズド変換
メモ:modwpt	Maximal overlap discrete wavelet packet transform
メモ:modwt	最大重複離散ウェーブレット変換
メモ:stft	短時間フーリエ変換
時間-周波数の特徴
メモ:signalTimeFrequencyFeatureExtractor	Streamline signal time-frequency feature extraction (R2024a 以降)
spectralCrest	Spectral crest for signals and spectrograms
spectralEntropy	Spectral entropy for signals and spectrograms
spectralFlatness	Spectral flatness for signals and spectrograms
spectralKurtosis	Spectral kurtosis for signals and spectrograms
spectralSkewness	Spectral skewness for signals and spectrograms
メモ:waveletScattering	Wavelet time scattering
微分可能な信号の処理
cwtLayer	Continuous wavelet transform layer (R2022b 以降)
dlcwt	Deep learning continuous wavelet transform (R2022b 以降)
dlicwt	Deep learning inverse continuous 1-D wavelet transform (R2024b 以降)
メモ:dlistft	Deep learning inverse short-time Fourier transform (R2024a 以降)
メモ:dlmodwt	Deep learning maximal overlap discrete wavelet transform and multiresolution analysis (R2022a 以降)
メモ:dlstft	深層学習の短時間フーリエ変換
icwtLayer	Inverse continuous wavelet transform layer (R2024b 以降)
メモ:istftLayer	Inverse short-time Fourier transform layer (R2024a 以降)
メモ:modwtLayer	Maximal overlap discrete wavelet transform layer (R2022b 以降)
メモ:stftLayer	Short-time Fourier transform layer (R2021b 以降)
特徴抽出ユーティリティ
framesig	Partition signal into frames (R2024a 以降)
信号のラベル付け
信号ラベル
framesig	Partition signal into frames (R2024a 以降)
信号の関心領域
sigrangebinmask	Label signal samples with values within a specified range (R2023a 以降)
異常検出
データストア、特徴抽出器、および層
cwtLayer	Continuous wavelet transform layer (R2022b 以降)
icwtLayer	Inverse continuous wavelet transform layer (R2024b 以降)
メモ:istftLayer	Inverse short-time Fourier transform layer (R2024a 以降)
メモ:modwtLayer	Maximal overlap discrete wavelet transform layer (R2022b 以降)
メモ:signalFrequencyFeatureExtractor	Streamline signal frequency feature extraction (R2021b 以降)
メモ:signalTimeFeatureExtractor	Streamline signal time feature extraction
メモ:signalTimeFrequencyFeatureExtractor	Streamline signal time-frequency feature extraction (R2024a 以降)
メモ:stftLayer	Short-time Fourier transform layer (R2021b 以降)
メモ:waveletScattering	Wavelet time scattering

