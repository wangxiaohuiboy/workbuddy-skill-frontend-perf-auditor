# WorkBuddy Skill · Frontend Performance Auditor

> Analyze your frontend project and get a prioritized, code-level performance
> optimization plan (bundle size + Core Web Vitals).
>
> 分析前端项目，给出按优先级排序、可落地执行的性能优化方案（包体积 + Core Web Vitals）。

---

## English

### What it does
Looks at your dependencies, build setup and (optionally) Lighthouse numbers, then
returns a **prioritized optimization plan with estimated impact** — not generic tips.

### Effects you can achieve
- 📦 Shrink bundle: find heavy deps, enable tree-shaking, swap `lodash`→per-method,
  `moment`→`day.js`, add dynamic `import()`.
- ✂️ Code-splitting: route/component-level lazy loading for heavy pieces.
- ⚡ Core Web Vitals: lower LCP (preload, kill render-blocking), fix CLS
  (`aspect-ratio`), improve INP (debounce, web workers).
- 🖼️ Image & font loading: `avif`/`webp`, `srcset`, `font-display: swap`, subset.
- 📊 A priority table (P0/P1/P2) with estimated savings per change.

### How to use
```
Why is my bundle 1.2MB? Help me cut it down.
分析下我的首屏为什么这么慢，给我优化方案。
```

```
Optimize this Next.js app for LCP and CLS.
```

### Install (WorkBuddy)
Copy this folder into `~/.workbuddy/skills/` or `<project>/.workbuddy/skills/`.

---

## 中文

### 这个 Skill 能做什么
查看你的依赖、构建配置以及（可选的）Lighthouse 数据，输出一份**带预估收益、
按优先级排序的优化方案**，而不是泛泛而谈。

### 可实现的效果
- 📦 缩减包体：找出重型依赖、开启 tree-shaking、`lodash` 改按需引入、`moment` 换
  `day.js`、加动态 `import()`。
- ✂️ 代码分割：路由级 / 组件级懒加载重型模块。
- ⚡ Core Web Vitals：降 LCP（预加载、去除阻塞渲染）、修 CLS（`aspect-ratio`）、
  提 INP（防抖、Web Worker）。
- 🖼️ 图片与字体：`avif`/`webp`、`srcset`、`font-display: swap`、子集化。
- 📊 带预估收益（如「≈ -120kB」「LCP ~ -0.5s」）的优先级表（P0/P1/P2）。

### 使用方法
```
我的包为什么有 1.2MB？帮我砍下去。
```

```
优化这个 Next.js 应用的 LCP 和 CLS。
```

### 安装（WorkBuddy）
把本文件夹复制到 `~/.workbuddy/skills/` 或 `<项目>/.workbuddy/skills/` 即可启用。

---

## License
MIT
