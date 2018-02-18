# 3 Days to WordPress.org

แนวทางการพัฒนา theme / plugin และอัพขึ้น [WordPress.org](https://wordpress.org/) ใน 3 วัน

## 1. Cover

ทำไมถึงอยากอัพขึ้น [WordPress.org](https://wordpress.org/)
- พัฒนาตัวเอง
- อยากรู้การทำงานของ Open source ใหญ่ๆ แบบนี้ว่า flow ในการทำงานเขาเป็นยังไงกัน
- เป็นช่องทางใน การพัฒนาโค้ด และส่งต่อไปยังผู้ใช้งาน

## 2. Speaker

ชื่อ ณัฐชัย ทองนิรันดร์ (โจ้), web developer

## 3. Timeline

```
| type   | name             | start    | submit         | first review   | approved       | all  |
|--------|------------------|----------|----------------|----------------|----------------|------|
| plugin | Auto Subpage Menu| 23/08/15 | 25/08/15 (+2d) | -              | 27/08/15 (+2d) | 5d   |
| theme  | Koa              | 24/05/16 | 31/07/16 (+2m) | 30/12/16 (+5m) | 16/01/17 (+2w) | 7.5m |
| plugin | Mobile Redirect..| 12/08/16 | 13/08/16 (+1d) | -              | 16/08/16 (+3d) | 5d   |
| plugin | Grayscale Body   | 14/10/16 | 14/10/16       | -              | 15/10/16 (+1d) | 2d   |
| plugin | Black Ribbon     | 24/10/16 | 24/10/16       | -              | 25/10/16 (+1d) | 2d   |
| theme  | Mediumm          | 11/01/16 | 13/04/17 (+15m)| 25/05/17 (+1m) | 19/06/17 (+1m) | 17m  |
| plugin | PromptPay        | 07/09/17 | 07/09/17       | -              | 10/09/17 (+3d) | 4d   |
| plugin | Mourning         | 02/10/17 | 04/10/17 (+2d) | -              | 05/10/17 (+1d) | 4d   |
```

ข้อสังเกต และประสบการณ์ที่พบเจอตอน submit และ review
- plugin แรกๆ ใช้เวลา 2-3 วันในการรออนุมัติ แต่หลังๆ แค่ 1 วัน
- หลังๆจะพัฒนาได้ไว เพราะ copy ของเก่ามา
- อย่าง PromptPay ที่ใช้เวลา 3 วันเพราะปัญหาอื่น คือ เราไม่ได้เป็นตัวแทนของ PromptPay, เขาก็เลยแนะนำให้ ใส่ชื่อแบรนด์เพิ่มเข้าไปเช่น jojoee-promptpay
- การส่ง plugin, ส่งแล้วรอ feedback (ถ้าไม่มีปัญหาอะไรเขาก็จะส่ง email มาอนุมัติเลย)

ตัวอย่าง Plugins ที่พัฒนา

- Auto Subpage Menu: Automatically add/remove top-level page to/from menus, [WordPress](https://wordpress.org/plugins/auto-subpage-menu/), [GitHub](https://github.com/jojoee/auto-subpage-menu), [SVN](http://plugins.svn.wordpress.org/auto-subpage-menu/)
- Black Ribbon: Automatically add black ribbon into sites corner, [WordPress](https://wordpress.org/plugins/black-ribbon/), [GitHub](https://github.com/jojoee/black-ribbon), [SVN](https://plugins.svn.wordpress.org/black-ribbon/)
- Grayscale Body: Automatically turn the site to grayscale, [WordPress](https://wordpress.org/plugins/grayscale-body/), [GitHub](https://github.com/jojoee/grayscale-body), [SVN](https://plugins.svn.wordpress.org/grayscale-body/)
- Mobile Redirect With Slug: Redirect mobile’s user to mobile site, [WordPress](https://wordpress.org/plugins/mobile-redirect-with-slug/), [GitHub](https://github.com/jojoee/mobile-redirect-with-slug), [SVN](https://plugins.svn.wordpress.org/mobile-redirect-with-slug/)
- Mourning: Add black ribbon and grey out the website, [WordPress](https://wordpress.org/plugins/mourning/), [GitHub](https://github.com/woodpeckerr/mourning), [SVN](https://plugins.svn.wordpress.org/mourning)
- PromptPay: PromptPay integration for WordPress, [WordPress](https://wordpress.org/plugins/wp-promptpay/), [GitHub](https://github.com/woodpeckerr/promptpay), [SVN](https://plugins.svn.wordpress.org/wp-promptpay/)

ตัวอย่าง Themes ที่พัฒนา

- Koa: Simple clean blog, [WordPress](https://wordpress.org/themes/koa), [GitHub](https://github.com/jojoee/wordpress-theme-koa), [Ticket](https://themes.trac.wordpress.org/ticket/35162)
- Mediumm, theme that's very inspired by medium.com, [WordPress](https://wordpress.org/themes/mediumm), [GitHub](https://github.com/jojoee/medium-clone), [Ticket 1](https://themes.trac.wordpress.org/ticket/41990), [Ticket 2](https://themes.trac.wordpress.org/ticket/43504)

## 4. Content

1. Web development standards, มาตรฐานการพัฒนาเว็บ ทั่วไป
2. WordPress development standards, มาตรฐานการพัฒนาร่วมกับ WordPress (เหมือนเราทำอยู่บน Framework ตัวนึง) เช่นเราทำ React, Symfony เราก็จะใช้ท่านี้ ทำแบบนี้
3. WordPress.org submitting standards, มาตรฐานในการอัพขึ้น WordPress.org, เหมือนกับเราส่งงาน ให้ Tester, PM หรือ ลูกค้า ตรวจสอบหรือดูคุณภาพของงาน

โดยใน session นี้จะเน้น 3 เป็นพิเศษ, เพราะว่าหัวข้อที่ 1 กับ 2 นั้นหาอ่านเอาในอินเทอร์เน็ตได้ง่ายกว่า

## 5. Why standards / best practice

1. Avoid common problem เช่น
- เราโหลด css ก่อน เพื่อให้เวลาเปิด page แล้ว layout มันแสดงผลได้ถูกต้อง
- เราใช้ `wp_enqueue_script` ในการโหลดไฟล์ ทำให้เวลามันเรียกใช้ library เดียวกันมันก็จะไปเรียกตัวเดียวกัน แทนที่จะเป็นการ include เข้ามาซ้ำกัน
2. Avoid future problem เช่น
- การหลีกเลี่ยง deprecated method, เวลาเขาไม่ support method พวกนี้แล้วเนี่ย เราก็จะได้ไม่มีปัญหา
3. On the same page, เข้าใจไปในทิศทางเดียวกัน เช่น 
- เรียกใช้ไฟล์ผ่าน `wp_enqueue_script` เพื่อลดการใช้งาน common library ที่ซ้ำซ้อน
4. Save time
5. etc.

## 6. Web development standards

1. [Coding standard](https://make.wordpress.org/core/handbook/best-practices/coding-standards/)
2. DRY, อะไรที่ซ้ำๆกัน แยกออกมา เวลาจะเปลี่ยนแปลงจะได้เปลี่ยนแปลงที่เดียว
3. [Design pattern](https://code.tutsplus.com/series/design-patterns-in-wordpress--wp-33841)
4. Test e.g. unit, acceptance, responsive, browser compatibility
5. Others เช่น Git, Security, SEO, UX, CSS architecture, Software development life cycle, etc

## 7. WordPress development standards

จุดประสงค์ก็เพื่อให้ทำงานร่วมกับ Framework และ Plguin ตัวอื่นๆได้

1. [Template tags](https://codex.wordpress.org/Template_Tags) เช่น `get_header()`, `get_footer()`
2. [Template hierarchy](https://developer.wordpress.org/themes/basics/template-hierarchy/)
3. [Localization](https://developer.wordpress.org/themes/functionality/localization/) ช่วยสนันสนุนการทำแปลภาษา เช่น `__( 'Primary Navigation', 'mediumm' )`
4. [Taxonomy](https://codex.wordpress.org/Taxonomies)
5. [Child Themes](https://codex.wordpress.org/Child_Themes)
6. [The Loop](https://codex.wordpress.org/The_Loop)
ใช้ในการ display posts

```php
if ( have_posts() ) {
  while ( have_posts() ) {
    the_post(); ?>
    <a href="<?php the_permalink(); ?>">
      <?php the_title(); ?>
    </a>
    <div class="entry">
      <?php the_content(); ?>
    </div>
    <?php
  }
} else { ?>
  <p>
    <?php esc_html_e( 'Sorry, no posts matched your criteria.' ); ?>
  </p>
  <?php
}
```

7. [Hooks](https://codex.wordpress.org/Plugin_API/Hooks) ([Action](https://codex.wordpress.org/Plugin_API/Action_Reference) / [Filter](https://codex.wordpress.org/Plugin_API/Filter_Reference))

```php
function hook_css() { ?>
  <style>
  .wp_head_example {
    background-color : #f1f1f1;
  }
  </style>
  <?php
}
add_action( 'wp_head', 'hook_css' )
```
Action, เป็นเหมือนทำอะไรสักอย่าง เช่นอันนี้จะเป็นการเพิ่ม `<style>` เข้าไปที่ส่วน `<head>`

```php
function custom_excerpt_more( $more ) {
  return 'Read More';
}
add_filter( 'excerpt_more', 'custom_excerpt_more' );
```
เป็นเหมือนกรองหรือเปลี่ยนแปลง อะไรสักอย่าง เช่น อันนี้จะเป็นการเปลี่ยนส่วนของ excerpt (เวลาเนื้อหายาวเกินไปแล้วมักจะมี ... ต่อหลัง ซึ่งอาจจะเปลี่ยนเป็น "อ่านต่อ" หรืออะไรก็แล้วแต่)

8. [Settings API](https://codex.wordpress.org/Settings_API) (Setting page)
9. [Shortcode](https://codex.wordpress.org/Shortcode_API) มีประโยชน์ในหน้า content editor

## 8. WordPress.org submitting standards

### 8.1 Plugin

#### 8.1.1 Process

1. Login WordPress.org
2. `readme.txt` validation, แนะนำให้เขียนละเอียดๆ, [ตัวอย่าง readme.txt](https://github.com/jojoee/grayscale-body/blob/master/readme.txt)
3. Submit
4. Wait (manually reviewed)
5. Once approved, upload plugin to WordPress SVN
6. Misc
- After, upload to SVN, automatically displayed in the [plugins browser](https://wordpress.org/plugins/)
- เคยเจอ user run บน PHP 5.4 ทำให้ syntax จากการใช้อาเรย์ (ต้องใช้ `array()` แทน `[]`)
- แนะนำในการทำ zip file ก่อน submit, [ตัวอย่าง gulpfile.js](https://github.com/woodpeckerr/promptpay/blob/master/gulpfile.js)

```js
const gulp = require('gulp');
const zip = require('gulp-zip');
const clean = require('gulp-clean');
const fs = require('fs');

const mainFile = 'mourning.php';
const mainFileContent = fs.readFileSync(mainFile, 'utf8');
const pluginVersion = /^Version.*$/igm.exec(mainFileContent)[0].substring(9).trim();
const pluginName = /^Plugin Name.*$/igm.exec(mainFileContent)[0].substring(13).trim().toLowerCase();
const packageFolderName = pluginName + '-' + pluginVersion;

gulp.task('clean', function () {
  return gulp.src(pluginName + '-*', {read: false})
    .pipe(clean());
});

gulp.task('pack', ['clean'], function () {
  return gulp.src([
    'css/**',
    'image/**',
    'mourning.php',
    'readme.txt',
    'screenshot-1.jpg',
    'screenshot-2.jpg'
  ], {base: '.'})
    .pipe(gulp.dest(packageFolderName));
});

gulp.task('pack.zip', ['pack'], function () {
  return gulp.src(packageFolderName + '/**')
    .pipe(zip(packageFolderName + '.zip'))
    .pipe(gulp.dest('./'));
});
```

#### 8.1.2 Review (บางข้อ)

1. License, GPLv2 or later, ตรวจสอบทุกไฟล์ (code, design, image, etc.)
2. Code must be human readable, ป้องกันพวก malicious code เช่น backdoors หรือ tracking
3. Trialware is not permitted, ห้าม plugin พวกทดลองใช้

### 8.2 Theme

#### 8.2.1 Process

1. Upload
2. Queue, wait for reviewer
3. Reviewer check
4. Reviewer create ticket and add add issues
5. No 7 days feedback from author, ticket may be closed
6. Once approved, reviewer will do the final review
7. Reviewer found new issue, reopened ticket
8. No issues found, ticket is marked live
9. All updates to it from then on are done in the update queue

#### 8.2.2 Review

1. [Recommended](https://make.wordpress.org/themes/handbook/review/recommended/) (optional) เช่นพวก `readme.txt`, `changelog.txt`
2. [Accessibility](https://make.wordpress.org/themes/handbook/review/accessibility) (optional), แนวๆพวก web accessibility เช่น
- ควรใช้ header tag ให้ถูกต้อง
- ไม่ควรใช้สีที่หลากหลายเกินไป เพราะจะทำให้คนที่ตาบอดสีเข้าใจเนื้อหาได้ยากขึ้น
3. [Required](https://make.wordpress.org/themes/handbook/review/required/)
- Code
  - No PHP or JS notices.
  - Provide a unique prefix
  - Pass [Theme Check](https://make.wordpress.org/themes/handbook/review/required/theme-check-plugin/)
- Core Functionality and Features
  - WordPress functionality (if available) เช่น Sidebars, Navigation Menus, Post Thumbnails
  - Child theme ready
  - 3 major WordPress versions backwards compatible
- Language, Localization ready
- Licensing, 100% GPL-compatible licensed สำหรับทุกไฟล์เช่น code, design, image
- Plugins
  - Cannot include plugins
  - Cannot require plugins to work
  - May use TGM Plugin Activation to recommend plugins
- Others
  - Include `comments.php`
  - Dont block admin bar
  - Any custom features, template should be explained
  - Documentation, any custom features, template should be explained
  - แนะนำการทดสอบ layout ด้วย Theme unit test เช่น [Theme Unit Test](https://codex.wordpress.org/Theme_Unit_Test), [WP Test - The Best Tests for WordPress](http://wptest.io/)

## 9. Recap

เป้าหมายคือผมต้องการให้ได้รับอนุมัติไวๆ และด้วย reviewer เขาก็เป็นอาสาสมัคร ผมจึงคิดว่าถ้าทำ code ให้ อ่านง่าย, ได้มาตรฐาน และเขียนอธิบายละเอียดๆ จะทำให้เขา review ได้ง่าย จึงเกิดเป็นวิธีการซึ่งประกอบไปด้วย 3 หัวข้อหลักนี้

1. Web development standards เช่น lint check, code style
2. WordPress development standards เช่น เราอยากจะทำอย่างนี้เราต้องใช้อะไร ท่าไหนที่เหมาะสม
3. WordPress.org submitting standards คล้ายๆการตรวจสอบและทำเอกสารส่งมอบไปยัง tester, PM, client เพื่อทำการตรวจสอบ

## 10. Thank you & QA

ท้ายนี้ผมเชื่อว่ามีหลายคนที่อยากจะอัพขึ้น [WordPress.org](https://wordpress.org/) แต่บางที ไม่แน่ใจว่า process เป็นยังไง, นานไหม, ต้องทำอะไรบ้าง คราวนี้ก็พอจะทราบกันแล้วว่าไม่ยากและขั้นตอนไม่นาน ก็อยากเชิญชวนให้มาลอง มาช่วยๆกันเยอะๆนะครับ, ขอบคุณครับ

## Other references

- [PHP Code Checker](https://phpcodechecker.com/)
- [WP-CLI](http://wp-cli.org/)
- [wp_cron](https://codex.wordpress.org/Function_Reference/wp_cron)
- [ESLint](https://eslint.org/) สำหรับ Javascript
- [PHP_CodeSniffer](https://github.com/WordPress-Coding-Standards/WordPress-Coding-Standards) สำหรับ WordPress

### Boilerplate / Starter

- [WordPress Plugin Boilerplate](https://github.com/DevinVinson/WordPress-Plugin-Boilerplate)
- [WordPress Plugin Boilerplate Generator](https://wppb.me/)
- [WordPress Widget Boilerplate](https://github.com/tommcfarlin/WordPress-Widget-Boilerplate)
- [Underscores | A Starter Theme for WordPress](https://underscores.me/)
- [Sage | WordPress Starter Theme](https://roots.io/sage/)

### Shortcode
- [Shortcodes included with WooCommerce - WooCommerce Docs](https://docs.woocommerce.com/document/woocommerce-shortcodes/)
- [Shortcode API](https://codex.wordpress.org/Shortcode_API)

### Plugin
- [Make WordPress Plugins](https://make.wordpress.org/plugins/)
- [Developer Information](https://wordpress.org/plugins/developers/)
- [WordPress Plugin Directory readme.txt standard](https://wordpress.org/plugins/about/readme.txt)
- [A readme.txt validator](https://wordpress.org/plugins/about/validator/)
- [Using Subversion with the WordPress Plugins Directory](https://wordpress.org/plugins/about/svn/)
- [Detailed Plugin Guidelines](https://developer.wordpress.org/plugins/wordpress-org/detailed-plugin-guidelines/)
- [How Your Readme.txt Works](https://developer.wordpress.org/plugins/wordpress-org/how-your-readme-txt-works/)
- [How Your Plugin Assets Work](https://developer.wordpress.org/plugins/wordpress-org/plugin-assets/)
- [How to Use Subversion](https://developer.wordpress.org/plugins/wordpress-org/how-to-use-subversion/)
- [Plugin Developer FAQ](https://developer.wordpress.org/plugins/wordpress-org/plugin-developer-faq/)

### Theme
- [Submit Your Theme or Theme Update to the Directory](https://wordpress.org/themes/upload/)
- [Theme Directory](https://wordpress.org/themes/getting-started/)
- [Theme Review Team](https://make.wordpress.org/themes/)
- [Review Process](https://make.wordpress.org/themes/handbook/review/)
- [Become a Reviewer](https://make.wordpress.org/themes/handbook/get-involved/become-a-reviewer/)
- [Theme Handbook](https://developer.wordpress.org/themes/)
