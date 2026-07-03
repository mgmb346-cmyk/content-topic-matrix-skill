---
name: content-topic-matrix
description: Turn a content mother topic into a reusable short-video topic workflow for creators in any niche, including female growth, study, workplace, AI, personal IP, self-media, Douyin, Xiaohongshu, Bilibili, and 视频号. Use when the user wants to create, expand, screen, or schedule video topics with a two-axis topic matrix. The skill expands topics by content depth and presentation form, scores them with five screening questions, prevents account-positioning drift, and recommends the best topics to shoot this week.
---

# Content Topic Matrix

Use this skill to turn one vague mother topic into a structured short-video topic pool, then screen it into a practical weekly shooting list.

Core idea: AI should not randomly decide what to shoot. AI should execute the creator's topic system: matrix expansion first, five-question screening second, weekly execution last. This is a general creator workflow, not an AI-creator-only workflow.

## Required Inputs

If the user does not provide these, infer safely and state assumptions:

- Account niche: e.g. female growth, study, workplace, AI tools, content creation, brand IP, creator growth.
- Account style: e.g. rational, warm, sharp, diary-like, practical, story-driven, professional.
- Mother topic: the topic to expand, e.g. "NotebookLM 找选题".
- Platform: Douyin, Xiaohongshu, Bilibili, 视频号, or general short video.
- Target audience: e.g. beginner creators, women in self-growth, students, workers, AI beginners, solopreneurs.
- Goal: traffic, followers, saves, comments, leads, or balanced.
- Available proof: real test, case, data, screenshots, personal story, or only an idea.

## The Matrix

Use this exact two-axis matrix unless the user explicitly changes it.

Content depth:

1. 新手入门
2. 进阶技巧
3. 趋势判断
4. 避坑指南
5. 决策共鸣

Presentation form:

1. 干货教程
2. 故事案例
3. 观点解读
4. 互动话题

The 5 × 4 matrix gives 20 topic drawers. Each drawer should be treated as a topic pool, not a single title.

## Modes

Choose the mode that matches the user's request.

### Mode A: Mother Topic Expansion

Use when the user gives one mother topic and wants ideas.

Output 20 candidate topics, one for each matrix cell. For each candidate include:

- Matrix cell: e.g. 新手入门 × 干货教程
- Short-video title
- Opening hook
- Core point
- Why people would click
- Best goal: 流量 / 涨粉 / 收藏 / 评论 / 转化

### Mode B: Drawer Deep Dive

Use when the user names one matrix cell, e.g. "新手入门 × 干货教程".

Output 10-20 titles inside that drawer. Keep them distinct by audience, scenario, pain point, proof type, or platform keyword.

### Mode C: Weekly Shooting List

Use when the user wants execution.

Start from candidate topics, score each using the five questions, then recommend 3 topics to shoot this week. Include:

- Recommended shooting order
- Why this topic now
- Proof needed
- Suggested CTA
- What to measure after publishing

### Mode D: Title Optimization

Use when the user wants titles to be more clickable, less generic, or less "AI-flavored."

Keep the matrix cell and topic angle unchanged, but rewrite titles with:

- Platform-search keywords
- User pain points
- Concrete numbers or time cues
- Emotional click hooks
- The account's identity and promised value

For title optimization in any niche, read `references/title-keyword-framework.md`. If the user provides a niche-specific keyword bank, use it as reference material, not as a mandatory word list. If no keyword bank is provided, infer a small tentative keyword bank from the niche and label it as an assumption.

## Five-Question Screening

Score each candidate:

- 是 = 1
- 可改 = 0.5
- 否 = 0

Questions:

1. 新鲜度：这个选题有没有最近才值得讲的理由？
2. 可实测：我能不能真的操作一遍，并拿出结果？
3. 可讲清：这条能不能在 60-120 秒内讲明白？
4. 可互动：用户看完有没有话可以回？
5. 可延展：如果数据好，我能不能继续拍 3-10 条？

Decision rule:

- 5 分：优先拍
- 4 分：可拍
- 3 分：改角度后再拍
- 2 分以下：先放素材池

## Anti-Drift Rule

Protect the account's main identity.

Allow popular keywords to attract clicks, but make the angle return to the account niche, style, and promised value.

Examples:

### Female growth account

- Attraction keywords: 情绪稳定, 内耗, 高敏感, 亲密关系, 原生家庭, 自我成长.
- Return angle: personal experience, emotional awareness, self-repair, boundaries, women's growth.

### Study account

- Attraction keywords: 学习方法, 自律, 拖延, 记忆力, 复习, 高效学习.
- Return angle: executable study method, real study record, review system, learning workflow.

### Workplace account

- Attraction keywords: 职场, 沟通, 领导, 汇报, 提效, 升职.
- Return angle: practical workplace method, realistic case, communication template, decision advice.

### AI creator account

- Attraction keywords: 选题, 爆款, 小红书, 抖音, 用户痛点, 副业, 自媒体, 工具, 工作流.
- Return angle: AI real test, AI workflow, how AI completes a task, whether the method is reusable.

Avoid making the title look like the account has become a pure ecommerce, course-selling, or money-making account unless the user explicitly wants that.

Example:

- Too drifting: 《用户在吐槽，你在赚大钱》
- Better: 《我用 AI 拆了 10 条用户吐槽，整理出一份选题报告》

General rule:

- Popular keyword = door handle.
- Account identity = room people enter.
- If the title attracts the wrong audience, rewrite it.

## Output Style

Use concise Chinese. Prefer short-video language over course language.

Good titles are specific, clickable, and not over-inflated:

- Use concrete objects: 情绪稳定, 学习计划, 职场汇报, NotebookLM, 视频字幕, 选题库, 小红书.
- Use concrete results: 20 个方向, 3 条本周可拍, 一份复盘, 一套流程, 一个真实案例.
- Avoid empty abstractions: 赋能, 范式重构, 价值百万, 底层逻辑 unless the user asks for a dramatic style.

Title rule:

- Do not make titles sound like "AI wrote this."
- Prefer user-facing outcomes over technical descriptions.
- Use niche keywords as searchable objects, not as abstract concepts.
- Combine at most 2-3 high-frequency hook words per title. Do not stack keywords mechanically.
- Different niches need different keyword banks. Do not apply AI niche words to female growth, study, lifestyle, workplace, beauty, or other niches unless the user explicitly connects the topic to AI.

Example:

- Too AI-flavored: 《AI 如何基于矩阵生成内容选题》
- Better: 《不知道拍什么？我做了个选题 Skill，3 分钟拆出 20 个方向》

## Default Final Structure

When the user asks for a complete output, use:

1. Brief diagnosis of the mother topic.
2. 20-topic matrix table.
3. Five-question scoring table for the top candidates.
4. Recommended 3 topics for this week.
5. One next action.
