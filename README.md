
# 无需人类演示即可解决奥林匹克几何问题


This repository contains the code necessary to
reproduce DDAR and AlphaGeometry,
the two geometry theorem provers
introduced in the [Nature 2024](https://www.nature.com/articles/s41586-023-06747-5) paper:

*<center>"Solving Olympiad Geometry without Human Demonstrations".</center>*


</br>


<center>
<img alt="fig1" width="800px" src="fig1.svg">
</center>


<div class="Box-sc-g0xbh4-0 bJMeLZ js-snippet-clipboard-copy-unpositioned" data-hpc="true"><article class="markdown-body entry-content container-lg" itemprop="text"><h1 tabindex="-1" dir="auto"><a id="user-content-solving-olympiad-geometry-without-human-demonstrations" class="anchor" aria-hidden="true" tabindex="-1" href="#solving-olympiad-geometry-without-human-demonstrations"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">无需人类演示即可解决奥林匹克几何问题</font></font></h1>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">该存储库包含重现 DDAR 和 AlphaGeometry 所需的代码，这两个几何定理证明器在</font></font><a href="https://www.nature.com/articles/s41586-023-06747-5" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Nature 2024</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">论文中介绍：</font></font></p>
<p dir="auto"><em></em></p><em><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">“无需人类演示即可解决奥林匹克几何问题”。</font></font></em><p dir="auto"></p>
<br>

<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/google-deepmind/alphageometry/blob/main/fig1.svg"><img alt="图。1" width="800px" src="/google-deepmind/alphageometry/raw/main/fig1.svg" style="max-width: 100%;"></a></p>

<h2 tabindex="-1" dir="auto"><a id="user-content-dependencies" class="anchor" aria-hidden="true" tabindex="-1" href="#dependencies"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">依赖关系</font></font></h2>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">对于下面提供的说明，我们使用 Python 3.10.9 以及依赖项，其确切版本号在 中列出</font></font><code>requirements.txt</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">我们的代码依赖于</font></font><code>meliad</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">, 这不是一个注册的包</font></font><code>pip</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font><font style="vertical-align: inherit;">有关如何手动安装的信息，请参阅下面的说明</font></font><code>meliad</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"></font><code>meliad</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">请注意，在没有和依赖项的</font><font style="vertical-align: inherit;">情况下，人们仍然可以运行 DDAR 求解器</font></font><code>sentencepiece</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></p>
<h2 tabindex="-1" dir="auto"><a id="user-content-run-the-instructions" class="anchor" aria-hidden="true" tabindex="-1" href="#run-the-instructions"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">运行指令</font></font></h2>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">其中的所有指令都</font></font><code>README.md</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">可以通过以下方式一次性运行：</font></font></p>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>bash run.sh
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="bash run.sh" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">下面，我们将逐步解释这些说明。</font></font></p>
<h2 tabindex="-1" dir="auto"><a id="user-content-install-dependencies-download-weights-and-vocabulary" class="anchor" aria-hidden="true" tabindex="-1" href="#install-dependencies-download-weights-and-vocabulary"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">安装依赖项，下载权重和词汇。</font></font></h2>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">安装是在虚拟环境中完成的：</font></font></p>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>virtualenv -p python3 .
source ./bin/activate
pip install --require-hashes -r requirements.txt
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="virtualenv -p python3 .
source ./bin/activate
pip install --require-hashes -r requirements.txt" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">下载权重和词汇：</font></font></p>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>bash download.sh
DATA=ag_ckpt_vocab
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="bash download.sh
DATA=ag_ckpt_vocab" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">最后，</font></font><code>meliad</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">单独安装，因为它没有注册</font></font><code>pip</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：</font></font></p>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>MELIAD_PATH=meliad_lib/meliad
mkdir -p $MELIAD_PATH
git clone https://github.com/google-research/meliad $MELIAD_PATH
export PYTHONPATH=$PYTHONPATH:$MELIAD_PATH
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="MELIAD_PATH=meliad_lib/meliad
mkdir -p $MELIAD_PATH
git clone https://github.com/google-research/meliad $MELIAD_PATH
export PYTHONPATH=$PYTHONPATH:$MELIAD_PATH" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<h2 tabindex="-1" dir="auto"><a id="user-content-set-up-common-flags" class="anchor" aria-hidden="true" tabindex="-1" href="#set-up-common-flags"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">设置通用标志</font></font></h2>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">在运行python脚本之前，我们首先准备一些常用的标志。</font><font style="vertical-align: inherit;">符号引擎需要定义和推导规则才能运行。</font><font style="vertical-align: inherit;">这些定义和规则在两个文本文件
</font></font><code>defs.txt</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">和</font></font><code>rules.txt</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">.</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>DDAR_ARGS=(
  --defs_file=<span class="pl-s"><span class="pl-pds">$(</span>pwd<span class="pl-pds">)</span></span>/defs.txt \
  --rules_file=<span class="pl-s"><span class="pl-pds">$(</span>pwd<span class="pl-pds">)</span></span>/rules.txt \
)<span class="pl-k">;</span></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="DDAR_ARGS=(
  --defs_file=$(pwd)/defs.txt \
  --rules_file=$(pwd)/rules.txt \
);" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">接下来，我们定义与证明搜索相关的标志。</font><font style="vertical-align: inherit;">为了重现下面的简单示例，我们使用轻量级值作为证明搜索参数：</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>BATCH_SIZE=2
BEAM_SIZE=2
DEPTH=2

SEARCH_ARGS=(
  --beam_size=<span class="pl-smi">$BEAM_SIZE</span>
  --search_depth=<span class="pl-smi">$DEPTH</span>
)</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="BATCH_SIZE=2
BEAM_SIZE=2
DEPTH=2

SEARCH_ARGS=(
  --beam_size=$BEAM_SIZE
  --search_depth=$DEPTH
)" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">注：我们论文中的结果可以通过设置 , 来获得
</font><font style="vertical-align: inherit;">，</font></font><code>BATCH_SIZE=32</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">如</font><font style="vertical-align: inherit;">
方法部分所述。</font><font style="vertical-align: inherit;">为了保持在 IMO 时间限制之内，需要 4 个 V100-GPU 和 250 个 CPU 工作线程，如扩展数据 - 图 1 所示。请注意，由于内部依赖性，我们还放弃了其他内存/速度优化，以提高代码清晰度。</font></font><code>BEAM_SIZE=512</code><font style="vertical-align: inherit;"></font><code>DEPTH=16</code><font style="vertical-align: inherit;"></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">假设下载的检查点和词汇表位于</font></font><code>DATA</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">，安装的</font></font><code>meliad</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">源代码位于</font></font><code>MELIAD_PATH</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font><font style="vertical-align: inherit;">我们遵循约定，利用该</font></font><code>gin</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">库来管理模型配置</font></font><code>meliad</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font><font style="vertical-align: inherit;">我们现在定义与语言模型相关的标志：</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>LM_ARGS=(
  --ckpt_path=<span class="pl-smi">$DATA</span> \
  --vocab_path=<span class="pl-smi">$DATA</span>/geometry.757.model
  --gin_search_paths=<span class="pl-smi">$MELIAD_PATH</span>/transformer/configs,<span class="pl-s"><span class="pl-pds">$(</span>pwd<span class="pl-pds">)</span></span> \
  --gin_file=base_htrans.gin \
  --gin_file=size/medium_150M.gin \
  --gin_file=options/positions_t5.gin \
  --gin_file=options/lr_cosine_decay.gin \
  --gin_file=options/seq_1024_nocache.gin \
  --gin_file=geometry_150M_generate.gin \
  --gin_param=DecoderOnlyLanguageModelGenerate.output_token_losses=True \
  --gin_param=TransformerTaskConfig.batch_size=<span class="pl-smi">$BATCH_SIZE</span> \
  --gin_param=TransformerTaskConfig.sequence_length=128 \
  --gin_param=Trainer.restore_state_variables=False
)<span class="pl-k">;</span></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="LM_ARGS=(
  --ckpt_path=$DATA \
  --vocab_path=$DATA/geometry.757.model
  --gin_search_paths=$MELIAD_PATH/transformer/configs,$(pwd) \
  --gin_file=base_htrans.gin \
  --gin_file=size/medium_150M.gin \
  --gin_file=options/positions_t5.gin \
  --gin_file=options/lr_cosine_decay.gin \
  --gin_file=options/seq_1024_nocache.gin \
  --gin_file=geometry_150M_generate.gin \
  --gin_param=DecoderOnlyLanguageModelGenerate.output_token_losses=True \
  --gin_param=TransformerTaskConfig.batch_size=$BATCH_SIZE \
  --gin_param=TransformerTaskConfig.sequence_length=128 \
  --gin_param=Trainer.restore_state_variables=False
);" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"></font><code>SEARCH_ARGS</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">提示：请注意，您仍然可以在不定义和 的</font><font style="vertical-align: inherit;">情况下运行 DDAR 求解器</font></font><code>LM_ARGS</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font><code>lm_inference</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">在这种情况下，只需禁用内部模块</font><font style="vertical-align: inherit;">的导入即可</font></font><code>alphageometry.py</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></p>
<h2 tabindex="-1" dir="auto"><a id="user-content-run-ddar" class="anchor" aria-hidden="true" tabindex="-1" href="#run-ddar"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">运行DDAR</font></font></h2>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">该脚本通过从文本文件中读取问题列表来加载问题，并根据其名称解决列表中的特定问题。</font></font><code>--problems_file</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">我们通过标志和</font><font style="vertical-align: inherit;">传递这两条信息
</font></font><code>--problem_name</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font><font style="vertical-align: inherit;">我们用</font></font><code>--mode=ddar</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">来表示我们想要使用 DDAR 求解器。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">下面我们展示了这个求解器求解 IMO 2000 P1：</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>python -m alphageometry \
--alsologtostderr \
--problems_file=<span class="pl-s"><span class="pl-pds">$(</span>pwd<span class="pl-pds">)</span></span>/imo_ag_30.txt \
--problem_name=translated_imo_2000_p1 \
--mode=ddar \
<span class="pl-s"><span class="pl-pds">"</span><span class="pl-smi">${DDAR_ARGS[@]}</span><span class="pl-pds">"</span></span></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="python -m alphageometry \
--alsologtostderr \
--problems_file=$(pwd)/imo_ag_30.txt \
--problem_name=translated_imo_2000_p1 \
--mode=ddar \
&quot;${DDAR_ARGS[@]}&quot;" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">期望以下输出</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>graph.py:468] translated_imo_2000_p1
graph.py:469] a b = segment a b<span class="pl-k">;</span> g1 = on_tline g1 a a b<span class="pl-k">;</span> g2 = on_tline g2 b b a<span class="pl-k">;</span> m = on_circle m g1 a, on_circle m g2 b<span class="pl-k">;</span> n = on_circle n g1 a, on_circle n g2 b<span class="pl-k">;</span> c = on_pline c m a b, on_circle c g1 a<span class="pl-k">;</span> d = on_pline d m a b, on_circle d g2 b<span class="pl-k">;</span> e = on_line e a c, on_line e b d<span class="pl-k">;</span> p = on_line p a n, on_line p c d<span class="pl-k">;</span> q = on_line q b n, on_line q c d <span class="pl-k">?</span> cong e p e q
ddar.py:41] Depth 1/1000 <span class="pl-k">time</span> = 1.7772269248962402
ddar.py:41] Depth 2/1000 <span class="pl-k">time</span> = 5.63526177406311
ddar.py:41] Depth 3/1000 <span class="pl-k">time</span> = 6.883412837982178
ddar.py:41] Depth 4/1000 <span class="pl-k">time</span> = 10.275688409805298
ddar.py:41] Depth 5/1000 <span class="pl-k">time</span> = 12.048273086547852
alphageometry.py:190]
==========================
 <span class="pl-k">*</span> From theorem premises:
A B G1 G2 M N C D E P Q <span class="pl-c1">:</span> Points
AG_1 ⟂ AB [00]
BA ⟂ G_2B [01]
G_2M = G_2B [02]
G_1M = G_1A [03]

...
[log omitted]
...

036. ∠QEB = ∠(QP-EA) [46] <span class="pl-k">&amp;</span> ∠(BE-QP) = ∠AEP [55] ⇒  ∠EQP = ∠QPE [56]
037. ∠PQE = ∠EPQ [56] ⇒  EP = EQ

==========================</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="graph.py:468] translated_imo_2000_p1
graph.py:469] a b = segment a b; g1 = on_tline g1 a a b; g2 = on_tline g2 b b a; m = on_circle m g1 a, on_circle m g2 b; n = on_circle n g1 a, on_circle n g2 b; c = on_pline c m a b, on_circle c g1 a; d = on_pline d m a b, on_circle d g2 b; e = on_line e a c, on_line e b d; p = on_line p a n, on_line p c d; q = on_line q b n, on_line q c d ? cong e p e q
ddar.py:41] Depth 1/1000 time = 1.7772269248962402
ddar.py:41] Depth 2/1000 time = 5.63526177406311
ddar.py:41] Depth 3/1000 time = 6.883412837982178
ddar.py:41] Depth 4/1000 time = 10.275688409805298
ddar.py:41] Depth 5/1000 time = 12.048273086547852
alphageometry.py:190]
==========================
 * From theorem premises:
A B G1 G2 M N C D E P Q : Points
AG_1 ⟂ AB [00]
BA ⟂ G_2B [01]
G_2M = G_2B [02]
G_1M = G_1A [03]

...
[log omitted]
...

036. ∠QEB = ∠(QP-EA) [46] &amp; ∠(BE-QP) = ∠AEP [55] ⇒  ∠EQP = ∠QPE [56]
037. ∠PQE = ∠EPQ [56] ⇒  EP = EQ

==========================" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">输出首先包含它使用的相关前提列表，然后是逐步构建证明的证明步骤。</font><font style="vertical-align: inherit;">所有谓词都经过编号，以跟踪它们是如何从前提导出的，并表明证明是完全合理的。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">提示：另外传递该标志</font></font><code>--out_file=path/to/output/text/file.txt</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">
会将证明写入文本文件。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">运行 中的所有问题</font></font><code>imo_ag_30.txt</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">将产生其中 14 个问题的解决方案，如我们论文中的表 1 所示。</font></font></p>
<h2 tabindex="-1" dir="auto"><a id="user-content-run-alphageometry" class="anchor" aria-hidden="true" tabindex="-1" href="#run-alphageometry"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">运行 AlphaGeometry：</font></font></h2>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">作为一个简单的例子，我们</font></font><code>--problem_name=orthocenter</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">
从加载</font></font><code>--problem_file=examples.txt</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font><font style="vertical-align: inherit;">这次，我们</font></font><code>--mode=alphageometry</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">使用 AlphaGeometry 解算器并传递</font></font><code>SEARCH_ARGS</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">和</font></font><code>LM_ARGS</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">标志。</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>python -m alphageometry \
--alsologtostderr \
--problems_file=<span class="pl-s"><span class="pl-pds">$(</span>pwd<span class="pl-pds">)</span></span>/examples.txt \
--problem_name=orthocenter \
--mode=alphageometry \
<span class="pl-s"><span class="pl-pds">"</span><span class="pl-smi">${DDAR_ARGS[@]}</span><span class="pl-pds">"</span></span> \
<span class="pl-s"><span class="pl-pds">"</span><span class="pl-smi">${SEARCH_ARGS[@]}</span><span class="pl-pds">"</span></span> \
<span class="pl-s"><span class="pl-pds">"</span><span class="pl-smi">${LM_ARGS[@]}</span><span class="pl-pds">"</span></span></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="python -m alphageometry \
--alsologtostderr \
--problems_file=$(pwd)/examples.txt \
--problem_name=orthocenter \
--mode=alphageometry \
&quot;${DDAR_ARGS[@]}&quot; \
&quot;${SEARCH_ARGS[@]}&quot; \
&quot;${LM_ARGS[@]}&quot;" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">预期输出如下：</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>...
[log omitted]
...
training_loop.py:725] Total parameters: 152072288
training_loop.py:739] Total state size: 0
training_loop.py:492] Training loop: creating task <span class="pl-k">for</span> mode beam_search

graph.py:468] orthocenter
graph.py:469] a b c = triangle a b c<span class="pl-k">;</span> d = on_tline d b a c, on_tline d c a b <span class="pl-k">?</span> perp a d b c
ddar.py:41] Depth 1/1000 <span class="pl-k">time</span> = 0.009987592697143555 branch = 4
ddar.py:41] Depth 2/1000 <span class="pl-k">time</span> = 0.00672602653503418 branch = 0
alphageometry.py:221] DD+AR failed to solve the problem.
alphageometry.py:457] Depth 0. There are 1 nodes to expand:
alphageometry.py:460] {S} a <span class="pl-c1">:</span> <span class="pl-k">;</span> b <span class="pl-c1">:</span> <span class="pl-k">;</span> c <span class="pl-c1">:</span> <span class="pl-k">;</span> d <span class="pl-c1">:</span> T a b c d 00 T a c b d 01 <span class="pl-k">?</span> T a d b c {F1} x00
alphageometry.py:465] Decoding from {S} a <span class="pl-c1">:</span> <span class="pl-k">;</span> b <span class="pl-c1">:</span> <span class="pl-k">;</span> c <span class="pl-c1">:</span> <span class="pl-k">;</span> d <span class="pl-c1">:</span> T a b c d 00 T a c b d 01 <span class="pl-k">?</span> T a d b c {F1} x00
...
[log omitted]
...
alphageometry.py:470] LM output (score=-1.102287): <span class="pl-s"><span class="pl-pds">"</span>e : C a c e 02 C b d e 03 ;<span class="pl-pds">"</span></span>
alphageometry.py:471] Translation: <span class="pl-s"><span class="pl-pds">"</span>e = on_line e a c, on_line e b d<span class="pl-pds">"</span></span>

alphageometry.py:480] Solving: <span class="pl-s"><span class="pl-pds">"</span>a b c = triangle a b c; d = on_tline d b a c, on_tline d c a b; e = on_line e a c, on_line e b d ? perp a d b c<span class="pl-pds">"</span></span>
graph.py:468]
graph.py:469] a b c = triangle a b c<span class="pl-k">;</span> d = on_tline d b a c, on_tline d c a b<span class="pl-k">;</span> e = on_line e a c, on_line e b d <span class="pl-k">?</span> perp a d b c
ddar.py:41] Depth 1/1000 <span class="pl-k">time</span> = 0.021120786666870117
ddar.py:41] Depth 2/1000 <span class="pl-k">time</span> = 0.033370018005371094
ddar.py:41] Depth 3/1000 <span class="pl-k">time</span> = 0.04297471046447754
alphageometry.py:140]
==========================
 <span class="pl-k">*</span> From theorem premises:
A B C D <span class="pl-c1">:</span> Points
BD ⟂ AC [00]
CD ⟂ AB [01]

 <span class="pl-k">*</span> Auxiliary Constructions:
E <span class="pl-c1">:</span> Points
E,B,D are collinear [02]
E,C,A are collinear [03]

 <span class="pl-k">*</span> Proof steps:
001. E,B,D are collinear [02] <span class="pl-k">&amp;</span> E,C,A are collinear [03] <span class="pl-k">&amp;</span> BD ⟂ AC [00] ⇒  ∠BEA = ∠CED [04]
002. E,B,D are collinear [02] <span class="pl-k">&amp;</span> E,C,A are collinear [03] <span class="pl-k">&amp;</span> BD ⟂ AC [00] ⇒  ∠BEC = ∠AED [05]
003. A,E,C are collinear [03] <span class="pl-k">&amp;</span> E,B,D are collinear [02] <span class="pl-k">&amp;</span> AC ⟂ BD [00] ⇒  EC ⟂ EB [06]
004. EC ⟂ EB [06] <span class="pl-k">&amp;</span> CD ⟂ AB [01] ⇒  ∠(EC-BA) = ∠(EB-CD) [07]
005. E,C,A are collinear [03] <span class="pl-k">&amp;</span> E,B,D are collinear [02] <span class="pl-k">&amp;</span> ∠(EC-BA) = ∠(EB-CD) [07] ⇒  ∠BAE = ∠CDE [08]
006. ∠BEA = ∠CED [04] <span class="pl-k">&amp;</span> ∠BAE = ∠CDE [08] (Similar Triangles)⇒  EB:EC = EA:ED [09]
007. EB:EC = EA:ED [09] <span class="pl-k">&amp;</span> ∠BEC = ∠AED [05] (Similar Triangles)⇒  ∠BCE = ∠ADE [10]
008. EB:EC = EA:ED [09] <span class="pl-k">&amp;</span> ∠BEC = ∠AED [05] (Similar Triangles)⇒  ∠EBC = ∠EAD [11]
009. ∠BCE = ∠ADE [10] <span class="pl-k">&amp;</span> E,C,A are collinear [03] <span class="pl-k">&amp;</span> E,B,D are collinear [02] <span class="pl-k">&amp;</span> ∠EBC = ∠EAD [11] ⇒  AD ⟂ BC
==========================

alphageometry.py:505] Solved.</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="...
[log omitted]
...
training_loop.py:725] Total parameters: 152072288
training_loop.py:739] Total state size: 0
training_loop.py:492] Training loop: creating task for mode beam_search

graph.py:468] orthocenter
graph.py:469] a b c = triangle a b c; d = on_tline d b a c, on_tline d c a b ? perp a d b c
ddar.py:41] Depth 1/1000 time = 0.009987592697143555 branch = 4
ddar.py:41] Depth 2/1000 time = 0.00672602653503418 branch = 0
alphageometry.py:221] DD+AR failed to solve the problem.
alphageometry.py:457] Depth 0. There are 1 nodes to expand:
alphageometry.py:460] {S} a : ; b : ; c : ; d : T a b c d 00 T a c b d 01 ? T a d b c {F1} x00
alphageometry.py:465] Decoding from {S} a : ; b : ; c : ; d : T a b c d 00 T a c b d 01 ? T a d b c {F1} x00
...
[log omitted]
...
alphageometry.py:470] LM output (score=-1.102287): &quot;e : C a c e 02 C b d e 03 ;&quot;
alphageometry.py:471] Translation: &quot;e = on_line e a c, on_line e b d&quot;

alphageometry.py:480] Solving: &quot;a b c = triangle a b c; d = on_tline d b a c, on_tline d c a b; e = on_line e a c, on_line e b d ? perp a d b c&quot;
graph.py:468]
graph.py:469] a b c = triangle a b c; d = on_tline d b a c, on_tline d c a b; e = on_line e a c, on_line e b d ? perp a d b c
ddar.py:41] Depth 1/1000 time = 0.021120786666870117
ddar.py:41] Depth 2/1000 time = 0.033370018005371094
ddar.py:41] Depth 3/1000 time = 0.04297471046447754
alphageometry.py:140]
==========================
 * From theorem premises:
A B C D : Points
BD ⟂ AC [00]
CD ⟂ AB [01]

 * Auxiliary Constructions:
E : Points
E,B,D are collinear [02]
E,C,A are collinear [03]

 * Proof steps:
001. E,B,D are collinear [02] &amp; E,C,A are collinear [03] &amp; BD ⟂ AC [00] ⇒  ∠BEA = ∠CED [04]
002. E,B,D are collinear [02] &amp; E,C,A are collinear [03] &amp; BD ⟂ AC [00] ⇒  ∠BEC = ∠AED [05]
003. A,E,C are collinear [03] &amp; E,B,D are collinear [02] &amp; AC ⟂ BD [00] ⇒  EC ⟂ EB [06]
004. EC ⟂ EB [06] &amp; CD ⟂ AB [01] ⇒  ∠(EC-BA) = ∠(EB-CD) [07]
005. E,C,A are collinear [03] &amp; E,B,D are collinear [02] &amp; ∠(EC-BA) = ∠(EB-CD) [07] ⇒  ∠BAE = ∠CDE [08]
006. ∠BEA = ∠CED [04] &amp; ∠BAE = ∠CDE [08] (Similar Triangles)⇒  EB:EC = EA:ED [09]
007. EB:EC = EA:ED [09] &amp; ∠BEC = ∠AED [05] (Similar Triangles)⇒  ∠BCE = ∠ADE [10]
008. EB:EC = EA:ED [09] &amp; ∠BEC = ∠AED [05] (Similar Triangles)⇒  ∠EBC = ∠EAD [11]
009. ∠BCE = ∠ADE [10] &amp; E,C,A are collinear [03] &amp; E,B,D are collinear [02] &amp; ∠EBC = ∠EAD [11] ⇒  AD ⟂ BC
==========================

alphageometry.py:505] Solved." tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">注意：点</font></font><code>H</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">会自动重命名为</font></font><code>D</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">，因为 LM 是针对综合问题进行训练的，其中点按字母顺序命名，因此在测试期间预计也是如此。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">注意：在 AlphaGeometry 的实现中，我们删除了所有依赖于内部基础设施的优化，例如，多 GPU 上的并行模型推理、多个 CPU 上的并行 DDAR、LM 和 DDAR 的并行执行、跨不同问题的 CPU 工作线程共享池、等等。我们还删除了一些内存/速度优化和代码抽象，以提高代码清晰度。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">从输出中可以看出，DDAR 最初未能解决该问题。</font><font style="vertical-align: inherit;">LM 提出了两个辅助结构（因为</font></font><code>BATCH_SIZE=2</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">）：</font></font></p>
<ul dir="auto">
<li><code>e = eqdistance e c a b, eqdistance e b a c</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">，即构造</font></font><code>E</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">为圆（中心=C，半径=AB）和圆（中心=B，半径=AC）的交集。</font><font style="vertical-align: inherit;">该建筑得分为</font></font><code>-1.186</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">.</font></font></li>
<li><code>e = on_line e a c, on_line e b d</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">，即
是</font><font style="vertical-align: inherit;">和</font></font><code>E</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">的交集</font><font style="vertical-align: inherit;">。</font><font style="vertical-align: inherit;">该结构比之前的</font><font style="vertical-align: inherit;">结构得分更高（ ）。</font></font><code>AC</code><font style="vertical-align: inherit;"></font><code>BD</code><font style="vertical-align: inherit;"></font><code>-1.102287</code><font style="vertical-align: inherit;"></font></li>
</ul>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">由于第二次构建得分较高，DDAR 首先尝试了第二次构建，并立即找到了解决方案。</font><font style="vertical-align: inherit;">因此证明搜索终止并且没有第二次迭代。</font></font></p>
<h2 tabindex="-1" dir="auto"><a id="user-content-results" class="anchor" aria-hidden="true" tabindex="-1" href="#results"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">结果</font></font></h2>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">在尝试重现我们论文中的 AlphaGeometry 数字之前，请确保通过准备的测试套件中的所有测试：</font></font></p>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>bash run_tests.sh
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="bash run_tests.sh" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"></font><code>--problem_file</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">然后，传递（列）和（行）</font><font style="vertical-align: inherit;">对应的值</font></font><code>--mode</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">，迭代所有问题，得到以下结果：</font></font></p>

<p dir="auto"><b><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">已解决问题数量：</font></font></b></p>
<table>
<thead>
<tr>
<th></th>
<th><code>imo_ag_30.txt</code></th>
<th><code>jgex_ag_231.txt</code></th>
</tr>
</thead>
<tbody>
<tr>
<td><code>ddar</code></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">14</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">198</font></font></td>
</tr>
<tr>
<td><code>alphageometry</code></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">25</font></font></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">228</font></font></td>
</tr>
</tbody>
</table>

<h2 tabindex="-1" dir="auto"><a id="user-content-source-code-description" class="anchor" aria-hidden="true" tabindex="-1" href="#source-code-description"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">源码说明</font></font></h2>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">此存储库中的文件包括运行解算器的 python 模块/脚本以及执行脚本所需的资源文件。</font><font style="vertical-align: inherit;">我们在下面列出了它们中的每一个及其描述。</font></font></p>
<table>
<thead>
<tr>
<th><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">文件名</font></font></th>
<th><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">描述</font></font></th>
</tr>
</thead>
<tbody>
<tr>
<td><code>geometry.py</code></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">在证明状态图中实现节点（点、线、圆等）。</font></font></td>
</tr>
<tr>
<td><code>numericals.py</code></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">在动态几何环境中实现数值引擎。</font></font></td>
</tr>
<tr>
<td><code>graph_utils.py</code></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">实现证明状态图的实用程序。</font></font></td>
</tr>
<tr>
<td><code>graph.py</code></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">实现证明状态图。</font></font></td>
</tr>
<tr>
<td><code>problem.py</code></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">实现表示问题前提、结论、DAG 节点的类。</font></font></td>
</tr>
<tr>
<td><code>dd.py</code></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">实现 DD 及其回溯。</font></font></td>
</tr>
<tr>
<td><code>ar.py</code></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">实现 AR 及其追溯。</font></font></td>
</tr>
<tr>
<td><code>trace_back.py</code></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">实现递归回溯和依赖差异算法。</font></font></td>
</tr>
<tr>
<td><code>ddar.py</code></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">实现DD+AR的组合。</font></font></td>
</tr>
<tr>
<td><code>beam_search.py</code></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">在 JAX 中实现语言模型的波束解码。</font></font></td>
</tr>
<tr>
<td><code>models.py</code></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">实现变压器模型。</font></font></td>
</tr>
<tr>
<td><code>transformer_layer.py</code></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">实现变压器层。</font></font></td>
</tr>
<tr>
<td><code>decoder_stack.py</code></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">实现变压器解码器堆栈。</font></font></td>
</tr>
<tr>
<td><code>lm_inference.py</code></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">实现一个经过训练的 LM 的接口来执行解码。</font></font></td>
</tr>
<tr>
<td><code>alphageometry.py</code></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">加载问题、调用 DD+AR 或 AlphaGeometry 求解器并打印解决方案的主脚本。</font></font></td>
</tr>
<tr>
<td><code>pretty.py</code></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">漂亮地格式化求解器输出的解决方案。</font></font></td>
</tr>
<tr>
<td><code>*_test.py</code></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">测试相应的模块。</font></font></td>
</tr>
<tr>
<td><code>download.sh</code></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">下载模型检查点和 LM 的脚本</font></font></td>
</tr>
<tr>
<td><code>run.sh</code></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">用于执行 README 中指令的脚本。</font></font></td>
</tr>
<tr>
<td><code>run_tests.sh</code></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">执行测试套件的脚本。</font></font></td>
</tr>
</tbody>
</table>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">资源文件：</font></font></p>
<table>
<thead>
<tr>
<th><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">资源文件名</font></font></th>
<th><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">描述</font></font></th>
</tr>
</thead>
<tbody>
<tr>
<td><code>defs.txt</code></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">不同几何构造动作的定义。</font></font></td>
</tr>
<tr>
<td><code>rules.txt</code></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">DD的扣除规则。</font></font></td>
</tr>
<tr>
<td><code>geometry_150M_generate.gin</code></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">在 meliad 中实现的 LM 的 Gin 配置。</font></font></td>
</tr>
<tr>
<td><code>imo_ag_30.txt</code></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">IMO-AG-30 中的问题。</font></font></td>
</tr>
<tr>
<td><code>jgex_ag_231.txt</code></td>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">JGEX-AG-231 中的问题。</font></font></td>
</tr>
</tbody>
</table>
<h2 tabindex="-1" dir="auto"><a id="user-content-citing-this-work" class="anchor" aria-hidden="true" tabindex="-1" href="#citing-this-work"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">引用这篇作品</font></font></h2>
<div class="highlight highlight-text-bibtex notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-k">@Article</span>{<span class="pl-en">AlphaGeometryTrinh2024</span>,
  <span class="pl-s">author</span>  = <span class="pl-s"><span class="pl-pds">{</span>Trinh, Trieu and Wu, Yuhuai and Le, Quoc and He, He and Luong, Thang<span class="pl-pds">}</span></span>,
  <span class="pl-s">journal</span> = <span class="pl-s"><span class="pl-pds">{</span>Nature<span class="pl-pds">}</span></span>,
  <span class="pl-s">title</span>   = <span class="pl-s"><span class="pl-pds">{</span>Solving Olympiad Geometry without Human Demonstrations<span class="pl-pds">}</span></span>,
  <span class="pl-s">year</span>    = <span class="pl-s"><span class="pl-pds">{</span>2024<span class="pl-pds">}</span></span>,
  <span class="pl-s">doi</span>     = <span class="pl-s"><span class="pl-pds">{</span>10.1038/s41586-023-06747-5<span class="pl-pds">}</span></span>
}</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="@Article{AlphaGeometryTrinh2024,
  author  = {Trinh, Trieu and Wu, Yuhuai and Le, Quoc and He, He and Luong, Thang},
  journal = {Nature},
  title   = {Solving Olympiad Geometry without Human Demonstrations},
  year    = {2024},
  doi     = {10.1038/s41586-023-06747-5}
}" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<h2 tabindex="-1" dir="auto"><a id="user-content-acknowledgements" class="anchor" aria-hidden="true" tabindex="-1" href="#acknowledgements"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">致谢</font></font></h2>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">这项研究是 Google Brain 团队（现 Google Deepmind）和纽约大学计算机科学系的合作成果。</font><font style="vertical-align: inherit;">我们感谢 Rif A. Saurous、Denny Zhou、Christian Szegedy、Delesley Hutchins、Thomas Kipf、Hieu Pham、Petar Veličković、Debidatta Dwibedi、Kunghyun Cho、Lerrel Pinto、Alfredo Canziani、Thomas Wies、He He 研究小组、Evan Chen（美国IMO 团队教练）、Mirek Olsak、Patrik Bak 以及所有三位 Nature 裁判的帮助和支持。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">AlphaGeometry 的代码与以下单独的库和包进行通信和/或引用：</font></font></p>
<ul dir="auto">
<li><a href="https://github.com/abseil/abseil-py"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">绳降</font></font></a></li>
<li><a href="https://github.com/google/jax/"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">贾克斯</font></font></a></li>
<li><a href="https://matplotlib.org/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">绘图库</font></font></a></li>
<li><a href="https://numpy.org" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">数值模拟</font></font></a></li>
<li><a href="https://scipy.org" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">科学Py</font></font></a></li>
<li><a href="https://github.com/tensorflow/tensorflow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">TensorFlow</font></font></a></li>
<li><a href="https://github.com/google-research/meliad"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">梅利亚德</font></font></a></li>
<li><a href="https://github.com/google/flax"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">亚麻</font></font></a></li>
<li><a href="https://github.com/google/gin-config"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">杜松子酒</font></font></a></li>
<li><a href="https://github.com/google-research/text-to-text-transfer-transformer"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">T5</font></font></a></li>
<li><a href="https://github.com/google/sentencepiece"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">句子片段</font></font></a></li>
</ul>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">我们感谢所有贡献者和维护者！</font></font></p>
<h2 tabindex="-1" dir="auto"><a id="user-content-disclaimer" class="anchor" aria-hidden="true" tabindex="-1" href="#disclaimer"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">免责声明</font></font></h2>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">这不是 Google 官方支持的产品。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">该研究代码“按原样”提供给更广泛的研究社区。</font><font style="vertical-align: inherit;">Google 不承诺以任何方式维护或以其他方式支持此代码。</font></font></p>
<h2 tabindex="-1" dir="auto"><a id="user-content-code-license" class="anchor" aria-hidden="true" tabindex="-1" href="#code-license"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">代码许可</font></font></h2>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">版权所有 2023 DeepMind 技术有限公司</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">所有软件均根据 Apache 许可证 2.0 版 (Apache 2.0) 获得许可；</font><font style="vertical-align: inherit;">除非遵守 Apache 2.0 许可证，否则您不得使用此文件。</font><font style="vertical-align: inherit;">您可以在以下位置获取 Apache 2.0 许可证的副本：
 https: </font></font><a href="https://www.apache.org/licenses/LICENSE-2.0" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">//www.apache.org/licenses/LICENSE-2.0</font></font></a></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">所有其他材料均根据知识共享署名 4.0 国际许可证 (CC-BY) 获得许可。</font><font style="vertical-align: inherit;">您可以通过以下网址获取 CC-BY 许可证副本：
 </font></font><a href="https://creativecommons.org/licenses/by/4.0/legalcode" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">https://creativecommons.org/licenses/by/4.0/legalcode</font></font></a></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">除非适用法律要求或书面同意，否则此处根据 Apache 2.0 或 CC-BY 许可分发的所有软件和材料均按“原样”分发，不附带任何明示或暗示的保证或条件。</font><font style="vertical-align: inherit;">请参阅特定语言的许可证，了解这些许可证下的权限和限制。</font></font></p>
<h2 tabindex="-1" dir="auto"><a id="user-content-model-parameters-license" class="anchor" aria-hidden="true" tabindex="-1" href="#model-parameters-license"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">型号 参数 许可证</font></font></h2>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">AlphaGeometry 检查点和词汇表根据 Creative Commons Attribution 4.0 International (CC BY 4.0) 许可证的条款提供。</font><font style="vertical-align: inherit;">您可以在以下位置找到详细信息：
 </font></font><a href="https://creativecommons.org/licenses/by/4.0/legalcode" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">https ://creativecommons.org/licenses/by/4.0/legalcode</font></font></a></p>
</article></div>
