# LEARNING FROM CLAUDE.md

Behavioral guidelines to reduce common LLM coding mistakes. Merge with project-specific instructions as needed.

**Tradeoff:** These guidelines bias toward caution over speed. For trivial tasks, use judgment.

## 1. Think Before Coding

**Don't assume. Don't hide confusion. Surface tradeoffs.**

Before implementing:
- State your assumptions explicitly. If uncertain, ask.
- If multiple interpretations exist, present them - don't pick silently.
- If a simpler approach exists, say so. Push back when warranted.
- If something is unclear, stop. Name what's confusing. Ask.

## 2. Simplicity First

**Minimum code that solves the problem. Nothing speculative.**

- No features beyond what was asked.
- No abstractions for single-use code.
- No "flexibility" or "configurability" that wasn't requested.
- No error handling for impossible scenarios.
- If you write 200 lines and it could be 50, rewrite it.

Ask yourself: "Would a senior engineer say this is overcomplicated?" If yes, simplify.

## 3. Surgical Changes

**Touch only what you must. Clean up only your own mess.**

When editing existing code:
- Don't "improve" adjacent code, comments, or formatting.
- Don't refactor things that aren't broken.
- Match existing style, even if you'd do it differently.
- If you notice unrelated dead code, mention it - don't delete it.

When your changes create orphans:
- Remove imports/variables/functions that YOUR changes made unused.
- Don't remove pre-existing dead code unless asked.

The test: Every changed line should trace directly to the user's request.

## 4. Goal-Driven Execution

**Define success criteria. Loop until verified.**

Transform tasks into verifiable goals:
- "Add validation" → "Write tests for invalid inputs, then make them pass"
- "Fix the bug" → "Write a test that reproduces it, then make it pass"
- "Refactor X" → "Ensure tests pass before and after"

For multi-step tasks, state a brief plan:
```
1. [Step] → verify: [check]
2. [Step] → verify: [check]
3. [Step] → verify: [check]
```

Strong success criteria let you loop independently. Weak criteria ("make it work") require constant clarification.

---

*** These guidelines are working if:** fewer unnecessary changes in diffs, fewer rewrites due to overcomplication, and clarifying questions come before implementation rather than after mistakes.

===============================================================================================
🔥 TOP 5 REPO GITHUB TRENDING HÔM QUA

🤖 Xu hướng nổi bật tiếp tục là AI Agent, Coding Agent và các công cụ giúp lập trình viên giảm token, hiểu source code nhanh hơn.

1. 🐎 Ponytail
    ⭐ 2.3k stars
    ⭐ AI workflow giúp Agent suy nghĩ và xử lý task theo hướng tối giản như một senior developer.
    🔎 Tìm kiếm: Ponytail GitHub
2. 🗜️ Headroom
    ⭐ 1.8k stars
    💰 Công cụ nén logs, tool output, file và RAG context trước khi gửi vào LLM.
    ✅ Giúp giảm token, giảm chi phí AI đáng kể.
    🔎 Tìm kiếm: Headroom GitHub
3. 🌐 Agent Reach
    ⭐ 1.5k stars
    🔍 Cho AI Agent tìm kiếm và đọc dữ liệu từ GitHub, Reddit, YouTube, X/Twitter… bằng một CLI.
    📌 Phù hợp làm Research Agent, Social Listening hoặc AI Marketing.
    🔎 Tìm kiếm: Agent Reach GitHub
4. 🧩 Codebase Memory MCP
    ⭐ 3.1k stars
    🧠 MCP Server giúp AI lập chỉ mục source code thành knowledge graph, ghi nhớ cấu trúc project và truy vấn nhanh hơn.
    💻 Rất đáng tham khảo cho dự án lớn React, Node.js, .NET, Java hoặc Python.
    🔎 Tìm kiếm: Codebase Memory MCP GitHub
5. 🎨 Taste Skill
    ⭐ 900+ stars
    ✨ Bộ kỹ năng giúp AI tạo giao diện frontend có gu hơn, hạn chế kiểu UI rập khuôn và “AI-generated” quá rõ.
    🎯 Phù hợp anh em dùng Claude Code, Codex, Cursor để làm UI/UX.
    🔎 Tìm kiếm: Taste Skill GitHub

📌 Điểm đáng chú ý:
✅ AI Agent đang tiến gần hơn đến vai trò “đồng đội lập trình”.
✅ Tối ưu token và memory là bài toán rất quan trọng khi dùng AI thực tế.
✅ MCP tiếp tục là cầu nối giữa AI với source code, dữ liệu và hệ thống doanh nghiệp.

💬 Anh em thấy repo nào có khả năng ứng dụng tốt nhất?
🔁 Chia sẻ để bạn bè cùng cập nhật.
📌 Lưu bài viết để nghiên cứu khi cần.

#Github #GithubTrending #AI #AIAgent #CodingAgent #MCP #OpenSource #Developer #SoftVietDigital #SoftVietAISEOAutoWriter
<!---
Alberthung368/Alberthung368 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
