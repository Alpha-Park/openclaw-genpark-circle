---
name: genpark-circle
description: Use this skill when the user wants to post an insight, thought, opinion, or discovery to GenPark Circle (GenPark's community forum), or asks things like "post to GenPark Circle", "share my thought on GenPark", "write a Circle post", "publish an insight on GenPark", "post in the GenPark forum", "write 洞见 for GenPark", "share this to Circle", "GenPark forum post", or mentions GenPark community, GenPark Circle, or GenPark 洞见.
metadata: {"openclaw": {"emoji": "💡", "requires": {}}}
---

# GenPark Circle — Insight Publisher

You help the user craft and publish **洞见 (insights)** — sharp, thoughtful posts — to **GenPark Circle**, the community forum inside GenPark. Posts should feel like quality thought-leadership: personal, opinionated, and worth reading.

---

## Step 1: Gather the User's Idea

Ask the user (or infer from context):

- **Topic / subject**: What do they want to share? A product discovery? A trend observation? A personal opinion? A review?
- **Language preference**: Chinese (中文), English, or mixed? (Default: match the language they're writing in)
- **Tone**: Casual & conversational? Professional? Enthusiastic? Thoughtful/analytical?
- **Target audience**: Fellow shoppers? Enthusiasts of a specific category? General community?
- **Reference product(s)**: Is there a specific GenPark product to link or highlight?

If the user provides a rough draft or bullet points, use those as the raw material. If they just give a topic, generate the full post.

**Memory check**: Check memory for saved tone/style preferences or past Circle posts to maintain consistency.

---

## Step 2: Draft the Post

Write a Circle post that follows these principles:

### Structure (flexible, not rigid)

```
[Hook — one punchy opening line that earns the read]

[Body — 2–4 short paragraphs expanding the insight]
- Personal observation or experience
- A specific example, product, or trend
- A "so what?" — why this matters to other GenPark users

[Close — a question, invitation, or call to action for the community]
```

### Quality Standards

| ✅ Do | ❌ Don't |
|---|---|
| Start with a strong hook | Start with "Hi everyone…" or "I want to share…" |
| Be specific (name products, occasions, or observations) | Be vague or generic |
| Have exactly one clear point | Try to cover three things at once |
| Invite response (end with a question) | End with nothing |
| Sound like a real person | Sound like a press release |
| Keep it under ~250 words | Write an essay |

### Formatting

- Use **short paragraphs** (2–3 sentences max each)
- Emoji can be used **sparingly** (1–2) if it fits the tone
- If naming a product, use its full name so it's searchable
- Add 2–4 relevant hashtags at the bottom (e.g. `#TechFinds #MinimalistDesign #GenParkCircle`)

---

## Step 3: Review with User

Before posting, show the user the full draft and ask:

> "Here's your Circle post draft. Want to tweak anything before I post it?"

Make any requested edits. Once confirmed, proceed to Step 4.

---

## Step 4: Post to GenPark Circle

Use your **browser** to post:

1. Navigate to `https://genpark.ai`
2. Sign in with the user's credentials (use stored credentials from memory; ask if unavailable)
3. Navigate to **Circle** (community/forum section)
4. Choose the appropriate channel or topic thread:
   - If product-related → find the matching category channel (Tech, Fashion, Home, etc.)
   - If a general observation → use the general discussion area
5. Click "New Post" (or equivalent)
6. Paste the drafted content into the post editor
7. Add any product tags or links if prompted
8. Review the preview, then click **Publish**
9. Confirm the post is live and capture the post URL

---

## Step 5: Confirm and Save

After posting:

1. Report back to the user: "✅ Your insight is live on GenPark Circle! [Post URL]"
2. Offer to share the Circle post link to other platforms (Twitter/X, LinkedIn, etc.)
3. Save to memory:

```
genpark_circle_posts:
  - title: "[First line of post]"
    url: "https://genpark.ai/circle/..."
    topic: "minimalist tech"
    date: "YYYY-MM-DD"
    tone: "thoughtful"
    language: "zh"
```

---

## Quick Examples

### Example: Chinese 洞见 (tech product)

> **最近发现一款让我停用了三款App的产品。**
>
> 在 GenPark 上偶然刷到这个桌面磁吸充电底座——表面上只是个配件，但用了两周之后，我的桌面彻底清爽了。以前三根数据线绕来绕去，现在一放一拿，生活小小的爽感就是这样来的。
>
> 有没有人也是被GenPark的某个"不起眼的小东西"彻底圈粉？欢迎分享你的「无法戒掉」清单。
>
> #GenParkCircle #桌面好物 #极简生活

---

### Example: English insight (fashion/lifestyle)

> **When did "gift wrapping" become the product itself?**
>
> Found this candle set on GenPark today. The packaging is so considered I kept the box. It made me realise I'm increasingly paying for the *unboxing* as much as the thing inside.
>
> Brands that get this right don't just sell products — they sell a feeling you want to give someone. What's the best-packaged thing you've discovered recently?
>
> #GenParkFinds #GiftIdeas #PackagingThatMatters

---

## Notes

- Always get user confirmation before publishing — never post without approval.
- If the Circle UI has changed, navigate carefully and describe what you see to the user.
- For longer-form content, consider breaking into a **thread** if GenPark Circle supports it.
- If the user wants to **pair this post with a product pick**, use `genpark-shop` first to find the product, then pass it to this skill.
