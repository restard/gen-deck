# Image Generation Rules

Last updated: June 8, 2026

## When To Use

Use these rules inside the create-from-structure flow when the AI is responsible for creating the background, base design, whitespace, decoration, or overall atmosphere. These rules mainly apply to single-page designs where fixed photos or exact text are not the main element, such as social media images, slide images, covers, section dividers, question pages, and closing or reflective pages.

## Purpose

Create a single image with a clear visual world. The main goal is to shape a suitable visual for the intended use, including the background, base design, whitespace, decoration, color, and atmosphere.

## Allowed Outputs

- Social media images
- Slide images
- Covers
- Section dividers
- Question pages
- Closing or reflective pages
- Slide images that prioritize visual atmosphere
- Information pages that do not require fixed assets

## Do Not Create

- Reproductions of real photos
- Before/After photos
- QR codes, URLs, prices, dates, or names
- Worksheets, tables, ruled forms, or any page that requires exact accuracy
- Fixed-asset pages that must use attached images or photos as they are

## Production Policy

- Before creating, recap the intent, purpose, use case, role of the page, medium, and aspect ratio
- If the use case or aspect ratio is missing, offer a small set of suitable candidates and ask the user to choose
- For slide images, suggest horizontal 16:9 as a candidate
- For social media images, suggest square 1:1 or vertical 4:5 for feed posts, and 9:16 for stories or vertical posts
- If a size is specified, adjust the whitespace, amount of text, and amount of decoration to match that ratio
- Keep text short and readable
- Leave enough whitespace in the center and main text area
- Do not let decorative elements interfere with the text
- Prioritize the design rules in Knowledge for the visual world, colors, and motifs
- If a page seems to require photos or fixed assets, do not draw it from structure. Move it to asset placement mode

## Recap Before Creation

Before creating from structure, recap the use case, role, design direction, text to include, and aspect ratio. Also include a simple Markdown wireframe.

The wireframe is not the finished image. It is only for sharing the placement concept. Keep it simple, showing only the relationship between elements such as the title, subcopy, whitespace, decoration, photo frame, and QR frame.

Example:

```text
┌──────────────────────────────┐
│  小さなメモ                    │
│                                │
│        メインタイトル           │
│        サブコピー               │
│                                │
│   手書き矢印   水色マーカー     │
│                                │
└──────────────────────────────┘
```

After the wireframe, provide the following options.

## Options

Before creating from structure, stop with the following prompt.

```text
次のどれかで返信してください。

[作る]
[内容を修正]
[次の1枚のおさらい]
```

After recapping the intent, purpose, use case, role of the page, medium, and aspect ratio, if the user replies with "作る", "作って", "はい", "OK", or similar wording, create one image preview without reconfirming.
