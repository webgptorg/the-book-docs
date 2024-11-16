---
weight: 1
bookFlatSection: true
title: "Home"
---

# Introduction

This is the documentation of the [Promptbook Project.](https://github.com/webgptorg/promptbook) We are building
the future of AI driven development. With or without Artificial General Intelligence, we believe that the most
successfull developers are those that integrate AI seamlessly and effectively into their work. This is what we strive
for.

{{< columns >}}

### Our mission

We strive for a digital landscape where creating any piece of software is not a privilege of the few with
technical expertise, but a possibility for all. This belief drives our commitment to developing technologies that
empower every individual, regardless of their technical background, to bring their ideas to life.

<--->

### Our vision

As developers and innovators, we are at the forefront of this mission. The challenges many face – from being
overwhelmed by the complexities of 'no-code' or 'low-code' platforms to the draining distractions of coordinating
with multiple stakeholders in traditional web development – are the problems we aim to solve.

{{< /columns >}}


## Why the documentation?

This site, built with [**Hugo**](https://gohugo.io/) and [Markdown](https://www.markdownguide.org/), should serve
as the only source of truth for our co-workers helping us to achieve the [above goals](#a-manifesto). It is intended
to comply with the principles of [handbook-first approach](https://handbook.gitlab.com/handbook/company/culture/all-remote/handbook-first/),
instilling the asynchronous culture of work and communication, remote-first mindset and foster the potential for
automation of processes.

## Contributing

{{< hint danger >}}
This contribution guideline is in permanent evolution.
{{< /hint >}}

To contribute to the documentation, you need to have Hugo installed. Follow these steps to install Hugo:

1. Download the latest version of Hugo from the [official releases page](https://github.com/gohugoio/hugo/releases).
2. Follow the installation instructions for your operating system [here](https://gohugo.io/getting-started/installing/).

After cloning the repository, you can make changes to the documentation. To preview your changes, run the following
command from the root directory of the repository:

```bash
$ hugo server
```

When done, you build the site by running the following command:
```bash
$ hugo --minify
```
and (typically all changes are made in the `public` directory) you add the changes to the staging area and commit them
with a meaningful message:
```bash
$ git add .
$ git commit -m "Your message here"
```
Finally, you push your changes to the `gh-pages` branch using the subtree command to push just the `public` directory
where the Hugo site is built:
```bash
$ git subtree push --prefix public origin gh-pages
```