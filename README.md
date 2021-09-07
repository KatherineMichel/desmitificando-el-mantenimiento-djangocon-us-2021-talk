# Desmitificando el Mantenimiento- DjangoCon US 2021 Talk

## Table of Contents

- [About](#about)
- [Slides and Script Table of Contents](#slides-and-script-table-of-contents)
- [Slides and Script](#slides-and-script) 
- [Attribution](#attribution)
- [Contact Kati](#contact-kati)
- [Copyright](#copyright)

<hr>

## About

Slides and script for a talk Katherine "Kati" Michel ([Twitter](https://twitter.com/KatiMichel), [GitHub](https://github.com/KatherineMichel)) gave at DjangoCon US Saturday, October 23, 2021.
 
Conference Page
* [DjangoCon US 2021](https://2021.djangocon.us/)

Slide Deck and Video Recording
* [Original slide deck](https://docs.google.com/presentation/d/17UG5OwojhiHYAaFjVJLncDdqMGHQAjk_W0rLoEgIp8Q/edit?usp=sharing)
* ["Desmitificando el Mantenimiento"]()
* [Video recording](https://www.youtube.com/watch?v=jTc2MRg3f0I)

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>




## Slides and Script Table of Contents

- [Get a Jumpstart on Collaboration and Code Review in GitHub](#get-a-jumpstart-on-collaboration-and-code-review-in-github)
- [Welcome](#welcome)
- [About Me](#about-me)
- [Talk Goal](#talk-goal)
- [Good News](#good-news)
- [More Good News](#more-good-news)
- [More Good News- Hacktoberfest](#more-good-news-hacktoberfest)
- [Announcing TacoFancy](#announcing-tacofancy)
- [One Life Changing Question](#one-life-changing-question)
- [My First Pull Request](#my-first-pull-request)
- [DjangoCon US Website as Example Project](#djangocon-us-website-as-example-project)
- [Prerequisites for Getting Started](#prerequisites-for-getting-started)
- [Housekeeping](#housekeeping)
- [What are Git and GitHub?](#what-are-git-and-github)
- [Social Network](#social-network)
- [Repositories](#repositories)
- [Local Development Environment Example](#local-development-environment-example)
- [Workflow Overview](#workflow-overview)
- [The Two Collaborative Development Models](#the-two-collaborative-development-models)
- [The Two Types of Accounts](#the-two-types-of-accounts)
- [Write Permission](#write-permission)
- [Examples of What Write Permission Will Allow You to Do](#examples-of-what-write-permission-will-allow-you-to-do)
- [Why We Need Write Permission](#why-we-need-write-permission)
- [Write Permission and Collaboration Examples](#write-permission-and-collaboration-examples)
- [How to Fork a Repo](#how-to-fork-a-repo)
- [Forked Repo](#forked-repo)
- [Workflow Overview](#workflow-overview)
- [Collaboration and Code Review Best Practice Workflow Using Branches](#collaboration-and-code-review-best-practice-workflow-using-branches)
- [Working on a File in GitHub](#working-on-a-file-in-github)
- [Reasons for Using Branches](#reasons-for-using-branches)
- [Branches](#branches)
- [How to Create a Branch](#how-to-create-a-branch)
- [Workflow Overview](#workflow-overview)
- [Fork and Pull Model](#fork-and-pull-model)
- [Shared Repository Model](#shared-repository-model)
- [Bash Commands](#bash-commands)
- [Local Development Environment](#local-development-environment)
- [Cloning](#cloning)
- [Changing Directory](#changing-directory)
- [GitHub Repo Versus Local Directory](#github-repo-versus-local-directory)
- [Verifying Branch](#verifying-branch)
- [Creating a New Branch](#creating-a-new-branch)
- [Working on a File Locally](#working-on-a-file-locally)
- [Adding and Committing](#adding-and-committing)
- [Pushing](#pushing)
- [New Branch](#new-branch)
- [Workflow Overview](#workflow-overview)
- [Pull Request Review Process](#pull-request-review-process)
- [Pull Request Command Line](#pull-request-command-line)
- [Pull Request Review](#pull-request-review)
- [Workflow Overview](#workflow-overview)
- [Sandboxing](#sandboxing)
- [Simple, But Effective](#simple-but-effective)
- [Pushing Commits to a Pull Request](#pushing-commits-to-a-pull-request)
- [Triaging](#triaging)
- [Finding Community Projects Versus Via GitHub Search](#finding-community-projects-versus-via-github-search)
- [When You Locate a Project](#when-you-locate-a-project)
- [Documentation](#documentation)
- [Newcomer Perspective is Valuable](#newcomer-perspective-is-valuable)
- [When You Get Stuck](#when-you-get-stuck)
- [Thank You](#thank-you)

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

## Slides and Script

The script is a general outline and varies somewhat from what was said during the talk.

<table>

<tr><td width="30%">

![Slide 1](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_0.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 2](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_1.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 3](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_2.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 4](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_3.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 5](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_4.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 6](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_5.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 7](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_6.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 8](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_7.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 9](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_8.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 10](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_9.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 11](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_10.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 12](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_11.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 13](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_12.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 14](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_13.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 15](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_14.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 16](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_15.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 17](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_16.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 18](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_17.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 19](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_18.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 20](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_19.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 21](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_20.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 22](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_21.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 23](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_22.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 24](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_23.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 25](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_24.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 26](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_25.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 27](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_26.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 28](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_27.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 29](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_28.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 30](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_29.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 31](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_30.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 32](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_31.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 33](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_32.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 34](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_33.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 35](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_34.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 36](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_35.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 37](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_36.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 38](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_37.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 39](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_38.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 40](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_39.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 41](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_40.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 42](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_41.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 43](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_42.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 44](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_43.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 45](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_44.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 46](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_45.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 47](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_46.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 48](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_47.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 49](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_48.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 50](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_49.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 51](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_50.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 52](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_51.jpg)

</td><td>
    
### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 53](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_52.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 54](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_53.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 55](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_54.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 56](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_55.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 57](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_56.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 58](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_57.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 59](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_58.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 60](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_59.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 61](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_60.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 62](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_61.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 63](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_62.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 64](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_63.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 65](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_64.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 66](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_65.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 67](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_66.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 68](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_67.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 69](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_68.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 70](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_69.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 71](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_70.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 72](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_71.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 73](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_72.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 74](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_73.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 75](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_74.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 76](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_75.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 77](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_76.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 78](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_77.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 79](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_78.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 80](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_79.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 81](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_80.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 82](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_81.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 83](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_82.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 84](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_83.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 85](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_84.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 86](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_85.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 87](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_86.jpg)

</td><td>

### 
  
</td></tr>


<table>

<tr><td width="30%">

![Slide 88](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_87.jpg)

</td><td>

### 
  
</td></tr>

  
<table>

<tr><td width="30%">

![Slide 89](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_88.jpg)

</td><td>

### 
  
</td></tr>
  
  
<table>

<tr><td width="30%">

![Slide 90](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_89.jpg)

</td><td>

### 
  
</td></tr>
      
  
<table>

<tr><td width="30%">

![Slide 91](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_90.jpg)

</td><td>

### 
  
</td></tr>
  
  
<table>

<tr><td width="30%">

![Slide 92](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_91.jpg)

</td><td>

### 
  
</td></tr>
  
  
<table>

<tr><td width="30%">

![Slide 93](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_92.jpg)

</td><td>

### 
  
</td></tr>
  
  
<table>

<tr><td width="30%">

![Slide 94](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_93.jpg)

</td><td>

### 
  
</td></tr>
  
  
<table>

<tr><td width="30%">

![Slide 95](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_94.jpg)

</td><td>

### 
  
</td></tr>
  
  
<table>

<tr><td width="30%">

![Slide 96](https://speakerd.s3.amazonaws.com/presentations/c7426fbdf98547df99270ec45e047634/slide_95.jpg)

</td><td>

### 
  
</td></tr>
  
</table>

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

## Attribution

The style of this transcript is heavily inspired by:

* Ana Balica's ([Twitter](https://twitter.com/anabalica), [GitHub](https://github.com/ana-balica)) transcript of her [Humanizing among coders](https://ana-balica.github.io/2017/05/28/humanizing-among-coders/) keynote for [PyCon CZ 2016](https://cz.pycon.org/2016). 
* Honza Javorek's ([Twitter](https://twitter.com/honzajavorek), [GitHub](https://github.com/honzajavorek)) transcript of Anna Ossowski's ([Twitter](https://twitter.com/OssAnna16), [GitHub](https://github.com/OssAnna16)) keynote [Be(Come) A Mentor! Help Others Succeed!](https://github.com/honzajavorek/become-mentor) for [PyCon CZ 2017](https://cz.pycon.org/2017/). 

Thank you!

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

## Contact Kati

* Email: kthrnmichel@gmail.com
* GitHub: https://github.com/KatherineMichel
* Twitter: https://twitter.com/KatiMichel

:top: <sub>[**back to top**](#table-of-contents)</sub>

<hr>

## Copyright

© 2021 to Present Katherine Michel. All Rights Reserved.
