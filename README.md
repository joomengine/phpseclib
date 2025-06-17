# JCB! Super Powers

### What Are JCB Super Powers?
In simple terms, **JCB Super Powers are PHP classes** — but managed entirely from the Joomla Component Builder (JCB) interface.

You can use JCB to create your own:
- **Classes**
- **Interfaces**
- **Abstract classes**
- **Traits**
- **Final classes**

These are full-featured PHP code units that you define visually in the JCB GUI. JCB then takes care of:
- Proper **namespacing**
- Correct **file placement**
- Seamless **project integration**

Every Super Power is treated as a reusable unit of logic. It can be automatically injected into any part of your JCB-powered component, or used in other components or codebases via a **SPK** (Super Power Key).

Even better — you can use **dynamic placeholders** like [[[`NamespacePrefix`]]] or [[[`ComponentNamespace`]]] in your Super Power code Namespace. These automatically adapt when reused in different projects, making your logic portable and future-proof.

> In short: **Super Powers turn JCB into a PHP code factory** — giving you the power of advanced PHP with none of the manual file management.

To learn how to create, manage, and use Super Powers, see the  
[Super Powers Documentation →](https://git.vdm.dev/joomla/super-powers/wiki)

### What Can I Find Here?
This repository acts as a **central registry of approved Super Powers** specific to this JCB instance.  
Only the Super Powers that have been explicitly assigned to this repository are listed here.

In JCB, you can organize your Super Powers across multiple repositories.  
For example, we have separate repositories for:

- [GITEA](https://git.vdm.dev/joomla/gitea)-related classes
- [OpenAI](https://git.vdm.dev/joomla/openai) integrations
- Core [Super Power](https://git.vdm.dev/joomla/super-powers) collection
- and many more...

Each repository maintains its own index, and only the powers assigned to that specific repository will appear in its list.
#### How to Use These Super Powers
If you want to use any of the classes listed here in your own component logic, simply reference their **SPK** (Super Power Key):

```
Super---[unique-guid]---Power
```

> Replace each `---` with `___` when using the key inside your code.

JCB will automatically resolve this SPK during compilation, placing the associated class in the correct location with the correct namespace based on your component context.  
This makes your logic both **reusable** and **component-aware**, without hardcoding anything.

---
# Index of powers

- **Namespace**: [VDM\Joomla\Componentbuilder](#vdm-joomla-componentbuilder)

  - **class Crypt** | [Details](src/d357e796-9f22-4615-9ebc-970b42cbd280) | [Raw](src/d357e796-9f22-4615-9ebc-970b42cbd280/code.power) | [Settings](src/d357e796-9f22-4615-9ebc-970b42cbd280/settings.json) | SPK: `Super---d357e796_9f22_4615_9ebc_970b42cbd280---Power`
  - **class Server** | [Details](src/66355f70-c26c-4765-ba48-498e3df740ef) | [Raw](src/66355f70-c26c-4765-ba48-498e3df740ef/code.power) | [Settings](src/66355f70-c26c-4765-ba48-498e3df740ef/settings.json) | SPK: `Super---66355f70_c26c_4765_ba48_498e3df740ef---Power`
- **Namespace**: [VDM\Joomla\Componentbuilder\Crypt](#vdm-joomla-componentbuilder-crypt)

  - **class Aes** | [Details](src/a25c82c8-14c2-40df-adae-f832709ab49b) | [Raw](src/a25c82c8-14c2-40df-adae-f832709ab49b/code.power) | [Settings](src/a25c82c8-14c2-40df-adae-f832709ab49b/settings.json) | SPK: `Super---a25c82c8_14c2_40df_adae_f832709ab49b---Power`
  - **class FOF** | [Details](src/e98b4edc-25b9-49d7-98a0-e42ad3b75efe) | [Raw](src/e98b4edc-25b9-49d7-98a0-e42ad3b75efe/code.power) | [Settings](src/e98b4edc-25b9-49d7-98a0-e42ad3b75efe/settings.json) | SPK: `Super---e98b4edc_25b9_49d7_98a0_e42ad3b75efe---Power`
  - **class KeyLoader** | [Details](src/6da44dff-a221-4f22-b9d9-b2fc2a724b4b) | [Raw](src/6da44dff-a221-4f22-b9d9-b2fc2a724b4b/code.power) | [Settings](src/6da44dff-a221-4f22-b9d9-b2fc2a724b4b/settings.json) | SPK: `Super---6da44dff_a221_4f22_b9d9_b2fc2a724b4b---Power`
  - **class Password** | [Details](src/fea2b107-3ee4-4ebf-84be-d3f2829c8614) | [Raw](src/fea2b107-3ee4-4ebf-84be-d3f2829c8614/code.power) | [Settings](src/fea2b107-3ee4-4ebf-84be-d3f2829c8614/settings.json) | SPK: `Super---fea2b107_3ee4_4ebf_84be_d3f2829c8614---Power`
  - **class Random** | [Details](src/c46a42b4-b0d3-48e7-a6fa-af0399e1e66c) | [Raw](src/c46a42b4-b0d3-48e7-a6fa-af0399e1e66c/code.power) | [Settings](src/c46a42b4-b0d3-48e7-a6fa-af0399e1e66c/settings.json) | SPK: `Super---c46a42b4_b0d3_48e7_a6fa_af0399e1e66c---Power`
- **Namespace**: [VDM\Joomla\Componentbuilder\Server](#vdm-joomla-componentbuilder-server)

  - **class Ftp** | [Details](src/11be6be3-ee3e-4771-8663-5545b76b73ab) | [Raw](src/11be6be3-ee3e-4771-8663-5545b76b73ab/code.power) | [Settings](src/11be6be3-ee3e-4771-8663-5545b76b73ab/settings.json) | SPK: `Super---11be6be3_ee3e_4771_8663_5545b76b73ab---Power`
  - **class Load** | [Details](src/a3414824-e99d-4878-b3d1-b5deef0cae17) | [Raw](src/a3414824-e99d-4878-b3d1-b5deef0cae17/code.power) | [Settings](src/a3414824-e99d-4878-b3d1-b5deef0cae17/settings.json) | SPK: `Super---a3414824_e99d_4878_b3d1_b5deef0cae17---Power`
  - **class Sftp** | [Details](src/490b6aa5-5de7-4be5-a61a-f634f6e004c0) | [Raw](src/490b6aa5-5de7-4be5-a61a-f634f6e004c0/code.power) | [Settings](src/490b6aa5-5de7-4be5-a61a-f634f6e004c0/settings.json) | SPK: `Super---490b6aa5_5de7_4be5_a61a_f634f6e004c0---Power`
- **Namespace**: [VDM\Joomla\Componentbuilder\Service](#vdm-joomla-componentbuilder-service)

  - **class Crypt** | [Details](src/4d8f38ef-8f3a-463d-8678-0bf087ac6815) | [Raw](src/4d8f38ef-8f3a-463d-8678-0bf087ac6815/code.power) | [Settings](src/4d8f38ef-8f3a-463d-8678-0bf087ac6815/settings.json) | SPK: `Super---4d8f38ef_8f3a_463d_8678_0bf087ac6815---Power`
  - **class Server** | [Details](src/42ceff0b-226d-42ff-9ffa-3d5935890337) | [Raw](src/42ceff0b-226d-42ff-9ffa-3d5935890337/code.power) | [Settings](src/42ceff0b-226d-42ff-9ffa-3d5935890337/settings.json) | SPK: `Super---42ceff0b_226d_42ff_9ffa_3d5935890337---Power`
- **Namespace**: [VDM\Joomla\Componentbuilder\Crypt\Aes](#vdm-joomla-componentbuilder-crypt-aes)

  - **class Legacy** | [Details](src/437af6b0-ca02-49d7-8739-4edfc8a9ccb0) | [Raw](src/437af6b0-ca02-49d7-8739-4edfc8a9ccb0/code.power) | [Settings](src/437af6b0-ca02-49d7-8739-4edfc8a9ccb0/settings.json) | SPK: `Super---437af6b0_ca02_49d7_8739_4edfc8a9ccb0---Power`
- **Namespace**: [VDM\Joomla\Componentbuilder\Server\Model](#vdm-joomla-componentbuilder-server-model)

  - **class Load** | [Details](src/f37ee8b7-2909-4319-bdf8-769bd7635490) | [Raw](src/f37ee8b7-2909-4319-bdf8-769bd7635490/code.power) | [Settings](src/f37ee8b7-2909-4319-bdf8-769bd7635490/settings.json) | SPK: `Super---f37ee8b7_2909_4319_bdf8_769bd7635490---Power`
> remember to replace the `---` with `___` in the SPK to activate that Power in your code

### All used in [Joomla Component Builder](https://www.joomlacomponentbuilder.com) - [Source](https://git.vdm.dev/joomla/Component-Builder) - [Mirror](https://github.com/vdm-io/Joomla-Component-Builder) - [Download](https://git.vdm.dev/joomla/pkg-component-builder/releases)

---
[![Joomla Volunteer Portal](https://img.shields.io/badge/-Joomla-gold?logo=joomla)](https://volunteers.joomla.org/joomlers/1396-llewellyn-van-der-merwe "Join Llewellyn on the Joomla Volunteer Portal: Shaping the Future Together!") [![Octoleo](https://img.shields.io/badge/-Octoleo-black?logo=linux)](https://git.vdm.dev/octoleo "--quiet") [![Llewellyn](https://img.shields.io/badge/-Llewellyn-ffffff?logo=gitea)](https://git.vdm.dev/Llewellyn "Collaborate and Innovate with Llewellyn on Git: Building a Better Code Future!") [![Telegram](https://img.shields.io/badge/-Telegram-blue?logo=telegram)](https://t.me/Joomla_component_builder "Join Llewellyn and the Community on Telegram: Building Joomla Components Together!") [![Mastodon](https://img.shields.io/badge/-Mastodon-9e9eec?logo=mastodon)](https://joomla.social/@llewellyn "Connect and Engage with Llewellyn on Joomla Social: Empowering Communities, One Post at a Time!") [![X (Twitter)](https://img.shields.io/badge/-X-black?logo=x)](https://x.com/llewellynvdm "Join the Conversation with Llewellyn on X: Where Ideas Take Flight!") [![GitHub](https://img.shields.io/badge/-GitHub-181717?logo=github)](https://github.com/Llewellynvdm "Build, Innovate, and Thrive with Llewellyn on GitHub: Turning Ideas into Impact!") [![YouTube](https://img.shields.io/badge/-YouTube-ff0000?logo=youtube)](https://www.youtube.com/@OctoYou "Explore, Learn, and Create with Llewellyn on YouTube: Your Gateway to Inspiration!") [![n8n](https://img.shields.io/badge/-n8n-black?logo=n8n)](https://n8n.io/creators/octoleo "Effortless Automation and Impactful Workflows with Llewellyn on n8n!") [![Docker Hub](https://img.shields.io/badge/-Docker-grey?logo=docker)](https://hub.docker.com/u/llewellyn "Llewellyn on Docker: Containerize Your Creativity!") [![Open Collective](https://img.shields.io/badge/-Donate-green?logo=opencollective)](https://opencollective.com/joomla-component-builder "Donate towards JCB: Help Llewellyn financially so he can continue developing this great tool!") [![GPG Key](https://img.shields.io/badge/-GPG-blue?logo=gnupg)](https://git.vdm.dev/Llewellyn/gpg "Unlock Trust and Security with Llewellyn's GPG Key: Your Gateway to Verified Connections!")