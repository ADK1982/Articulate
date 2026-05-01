---
title: How Courses Work
course: getting-started
order: 2
duration: 5 min
---

Each course on this site is made up of a series of lessons like this one.

## Navigating lessons

Lessons are listed in order in the sidebar. The one you're currently viewing is highlighted. You can jump to any lesson at any time — there's no strict lock-step requirement unless the course description says otherwise.

## Adding a video

If you want to embed a video in a lesson, add a `video_url` field to the lesson's front matter:

```yaml
---
title: My Lesson
course: my-course
order: 1
video_url: https://www.youtube.com/embed/your-video-id
---
```

The video will appear at the top of the lesson, above the written content.

## You're all set

That's all there is to it. Head back to [Courses]({{ '/courses/' | relative_url }}) to find something to learn.
