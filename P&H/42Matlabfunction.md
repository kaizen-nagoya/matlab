Q1 What is the "42 MATLAB signal-processing functions" in the https://arxiv.org/pdf/2512.14762v1
A1 by Chatgpt
The paper [“Workflows vs Agents for Code Translation”](https://arxiv.org/abs/2512.14762v1?utm_source=chatgpt.com) says that the authors evaluated their MATLAB→HDL pipeline on **“42 MATLAB signal-processing functions”**, but the paper does **not actually publish the full list of those 42 functions** in the main text or appendix that I could verify. ([ResearchGate][1])

What the paper *does* say:

* The dataset consisted of:

  * MATLAB signal-processing functions
  * ranging from **3 to 311 lines of code**
  * used to evaluate syntax repair and HDL translation
* The functions were part of an **internal dataset**. ([ResearchGate][1])

Based on the surrounding discussion and the MATLAB Signal Processing Toolbox APIs they reference conceptually, the functions are likely drawn from common DSP primitives such as:

* `fft`
* `ifft`
* `filter`
* `filtfilt`
* `conv`
* `xcorr`
* `fir1`
* `freqz`
* `sinc`
* `bandpass`
* `highpass`
* `lowpass`
* `upsample`
* `downsample`
* `interp`
* `decimate`

…but this inferred list is **not explicitly confirmed by the paper**. The publicly accessible paper never enumerates all 42 names. ([MathWorks][2])

So the technically correct answer is:

> The paper references an internal benchmark of 42 MATLAB signal-processing functions, but the exact list of functions is not disclosed in the published arXiv v1 manuscript. ([ResearchGate][1])

If you'd like, I can also help reconstruct a **probable 42-function benchmark suite** suitable for:

* MATLAB → VHDL translation
* FPGA synthesis evaluation
* DSP HLS benchmarking
* LLM HDL transpilation research

including:

* FIR/IIR
* FFT/DCT
* multirate DSP
* adaptive filters
* spectral estimation
* windowing
* fixed-point suitability
* synthesizability ranking.

[1]: https://www.researchgate.net/publication/398805939_Workflows_vs_Agents_for_Code_Translation?utm_source=chatgpt.com "(PDF) Workflows vs Agents for Code Translation"
[2]: https://www.mathworks.com/help/signal/index.html?utm_source=chatgpt.com "Signal Processing Toolbox Documentation"
