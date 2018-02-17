# 3 Days to WordPress.org

แนวทางการพัฒนาและอัพขึ้น [WordPress.org](https://wordpress.org/) ใน 3 วัน

## 1. Cover

ทำไมถึงต้องอัพขึ้น [WordPress.org](https://wordpress.org/)
- พัฒนาตัวเอง
- อยากรู้การทำงานของ Open source ใหญ่ๆ แบบนี้ว่า flow ในการทำงานเขาเป็นยังไงกัน
- เป็นช่องทางใน การพัฒนาโค้ด และส่งต่อไปยังผู้ใช้งาน

กลับมาที่หัวข้อ คือการทำให้โค้ดของเราไปอยู่ใน WordPress.org ใน 3 วัน
อยากให้ลองคิดตามว่า มันเป็นไปได้จริงๆไหม

## 2. Speaker

ชื่อ ณัฐชัย ทองนิรันดร์ (โจ้), ทำงานเป็น web developer

## 3. Timeline

```
| type   | name             | start    | submit         | first review   | approved       | all  |
|--------|------------------|----------|----------------|----------------|----------------|------|
| plugin | Auto Subpage Menu| 23/08/15 | 25/08/15 (+2d) | -              | 27/08/15       | 5d   |
| theme  | Koa              | 24/05/16 | 31/07/16 (+2m) | 30/12/16 (+5m) | 16/01/17 (+2w) | 7.5m |
| plugin | Mobile Redirect..| 12/08/16 | 13/08/16 (+1d) | -              | 16/08/16 (+3d) | 5d   |
| plugin | Grayscale Body   | 14/10/16 | 14/10/16       | -              | 15/10/16 (+1d) | 2d   |
| plugin | Black Ribbon     | 24/10/16 | 24/10/16       | -              | 25/10/16 (+1d) | 2d   |
| theme  | Mediumm          | 11/01/16 | 13/04/17 (+15m)| 25/05/17 (+1m) | 19/06/17 (+1m) | 17m  |
| plugin | PromptPay        | 07/09/17 | 07/09/17       | -              | 10/09/17 (+3d) | 4d   |
| plugin | Mourning         | 02/10/17 | 04/10/17 (+2d) | -              | 05/10/17 (+1d) | 4d   |
```

ข้อสังเกต และประสบการณ์ที่พบเจอตอน submit และ review
- หลังๆ dev จะไว เพราะ copy ของเก่ามา
- อย่าง PromptPay เราไม่ได้เป็นตัวแทน เขาก็เลยแนะนำให้ ใส่ชื่อแบรนด์ ไปเช่น jojoee-promptpay
- list เป็นหาง เลย ถ้าเป็น theme
- แต่ละอันใช้เวลาไม่นาน ถึงแม้จะเป็น theme ก็ยังไม่นาน
- การส่ง plugin ไม่มี first review, ส่ง > รอ feedback (ถ้าไม่มีปัญหาอะไรเขาก็จะส่ง email มาอนุมัติเลย)

Plugins ที่พัฒนา

- Auto Subpage Menu: Automatically add/remove top-level page to/from menus, [WordPress](https://wordpress.org/plugins/auto-subpage-menu/), [GitHub](https://github.com/jojoee/auto-subpage-menu), [SVN](http://plugins.svn.wordpress.org/auto-subpage-menu/)
- Black Ribbon: Automatically add black ribbon into sites corner, [WordPress](https://wordpress.org/plugins/black-ribbon/), [GitHub](https://github.com/jojoee/black-ribbon), [SVN](https://plugins.svn.wordpress.org/black-ribbon/)
- Grayscale Body: Automatically turn the site to grayscale, [WordPress](https://wordpress.org/plugins/grayscale-body/), [GitHub](https://github.com/jojoee/grayscale-body), [SVN](https://plugins.svn.wordpress.org/grayscale-body/)
- Mobile Redirect With Slug: Redirect mobile’s user to mobile site, [WordPress](https://wordpress.org/plugins/mobile-redirect-with-slug/), [GitHub](https://github.com/jojoee/mobile-redirect-with-slug), [SVN](https://plugins.svn.wordpress.org/mobile-redirect-with-slug/)
- Mourning: Add black ribbon and grey out the website, [WordPress](https://wordpress.org/plugins/mourning/), [GitHub](https://github.com/woodpeckerr/mourning), [SVN](https://plugins.svn.wordpress.org/mourning)
- PromptPay: PromptPay integration for WordPress, [WordPress](https://wordpress.org/plugins/wp-promptpay/), [GitHub](https://github.com/woodpeckerr/promptpay), [SVN](https://plugins.svn.wordpress.org/wp-promptpay/)

Themes ที่พัฒนา
- Koa: Simple clean blog, [WordPress](https://wordpress.org/themes/koa), [GitHub](https://github.com/jojoee/wordpress-theme-koa), [Ticket](https://themes.trac.wordpress.org/ticket/35162)
- Mediumm, theme that's very inspired by medium.com, [WordPress](https://wordpress.org/themes/mediumm), [GitHub](https://github.com/jojoee/medium-clone), [Ticket 1](https://themes.trac.wordpress.org/ticket/41990), [Ticket 2](https://themes.trac.wordpress.org/ticket/43504)

## 4. Content

1. Web development standards

จะเป็นพวกมาตรฐานการพัฬนาเว็บ ทั่วไป

2. WordPress development standards

มาตรฐานการพัฒนาร่วมกับ WordPress, คิดซะว่าเราพัฒนาบน Framework ตัวนึง
เช่นเราทำ React เราก็จะใช้ท่านี้
ทำ Symfony, เราจะทำ Database migration เราก็มักใช้ Doctrine cmd

3. WordPress.org submitting standards

ตอนอัพโหลดขึ้น WordPress.org, เหมือนกับเราส่งงาน ให้ Tester, PM หรือ ลูกค้า เทสหรือดูคุณภาพของงาน
ซึ่งแนวคิดพวกนี้ จริงๆก็สามารถนำไป apply กับงานประจำได้เลยนะครับ เช่นเวลาส่งมอบงาน

โดยใน session นี้จะเน้น 3 เป็นพิเศษ
เพราะว่าหัวข้อที่ 1 กับ 2 นั้นหาอ่านเอาในอินเทอร์เน็ตได้ง่ายกว่า

## 5. Why standards / best practice

1. Avoid common problem

เช่นเราแนะนำให้่ concat + minify เพื่อลดปัญหาการโหลดเว็บช้า
แนะนำให้ css ไว้ด้านบน เพราะกัน blank screen
หรือถ้า css ใหญ่มากๆ เราก็จะ
ให้มันโหลดเฉพาะ critical css ก่อน

2. Avoid future problem

เลี่ยงปัญหาที่อาจจะเกิดขึ้นในอนาคต เช่นการ deprecated โคด
เราก็หลีกเลี่ยงการใช้ code พวกนี้
เวลาเขาเอาออก เราก็จะได้ไม่กระทบ

3. On the same page

เข้าใจไปในทิศทางเดียวกัน
ทำงานร่วมกันได้ง่ายขึ้น

เช่นแบบ jQuery plugin หรือ WordPress plugin ที่สามารถทำงานร่วมกันได้
เพราะเขา define standard ไว้
ให้ทำแบบนี้นะ เวลา อยากทำพวก login หรือ ดึง resource มานี่เราก็ใช้ 
OAuth protocol to get resource
หรือ
เวลาเรา implement จริงเราก็ใช้ของคนอื่นได้เลย
โดยที่มีแนวคิดเดียวกัน ไม่ต้องศึกษาใหม่

เช่น wp ทำ cache plugin
wp ทำ enqueue script

4. Save time

5. etc.

## 6. Web development standards

1. [Coding standard](https://make.wordpress.org/core/handbook/best-practices/coding-standards/)
- CSS, ปกติ
- JavaScript
- PHP (WP vs PSR)

ซึ่งพวก code standard แบบนี้เราสามารถใช้ Lint tool ช่วยได้
เครื่องมือแนะนำสำหรับ Coding standard ก็จะเป็นพวก Lint เช่น [ESLint](https://eslint.org/) สำหรับ Javascript, [PHP_CodeSniffer](https://github.com/WordPress-Coding-Standards/WordPress-Coding-Standards) สำหรับ WordPress
พวก Lint tool
ช่วยทำให้ code อ่านง่ายขึ้น
และช่วยกัน bug ได้บางส่วน
ทำให้เราเขียนได้ไวขึ้น

2. DRY, อะไรที่ซ้ำๆกัน แยกออกมา เวลาจะเปลี่ยนแปลงจะได้เปลี่ยนแปลงที่เดียว

3. [Design pattern](https://code.tutsplus.com/series/design-patterns-in-wordpress--wp-33841)

เป็น pattern ที่ใช้เฉพาะงานเจาะจง
เวลาเราจะทำงานใดๆ เราก็เลือกใช้ pattern ในการแก้ปัญหา
หรือทำให้เราเข้าใจ ตัวโปรแกรมนั้นมากนั้น

4. Test

- Unit test
- Acceptance test
- Responsive
- Browser compatibility

5. Others

Git, Security, SEO, UX, CSS architecture, Software development life cycle, etc

## 7. WordPress development standards

จุดประสงค์ก็เพื่อให้ทำงานร่วมกับ Framework และ Plguin ตัวอื่นๆได้
ดังนั้นเราต้องเข้าใจการทำงาน หรือลักษณะเฉพาะซะก่อน เช่น

1. [Template tags](https://codex.wordpress.org/Template_Tags) เป็น WP function ที่ใช้ในการแสดงข้อมูลออกมาเช่น 

get_header()
get_footer()
get_sidebar()

2. [Template hierarchy](https://developer.wordpress.org/themes/basics/template-hierarchy/)

3. [Localization](https://developer.wordpress.org/themes/functionality/localization/)

e.g. __( 'Primary Navigation', 'mediumm' )

__()
_e()
_x()
ช่วยสนันสนุนการทำแปลภาษา

4. [Taxonomy](https://codex.wordpress.org/Taxonomies)

อ่านเพิ่ม ??

5. [Child Themes](https://codex.wordpress.org/Child_Themes)

เหมือนเรา extend themes เขามา
แล้วอยากแก้ แค่บางส่วนเล็กๆน้อยๆ

ดียังไง, เวลา theme หลักเรา update เราไม่ต้องยุ่ง


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

จะเป็น flow ในการแสดงผลของหน้าเว็บ
ถ้าเราเข้าหน้าแรกมันก็จะไปเรียกไฟล์ home.php ก่อน
ถ้าไม่มีก็ไปไฟล์ index.php

8. [Settings API](https://codex.wordpress.org/Settings_API) (Setting page)


9. [Shortcode](https://codex.wordpress.org/Shortcode_API)

มีประโยชน์ในหน้า editor

- [Shortcodes included with WooCommerce - WooCommerce Docs](https://docs.woocommerce.com/document/woocommerce-shortcodes/)

- [Shortcode API](https://codex.wordpress.org/Shortcode_API)

## 8. WordPress.org submitting standards

### 8.1 Plugin

#### 8.1.1 Process

1. Login WordPress.org
2. `readme.txt` validation

(ที่สำคัญตรง readme.txt, ควรจะต้องเขียนละเอียดๆ), [ตัวอย่าง readme.txt](https://github.com/jojoee/grayscale-body/blob/master/readme.txt)
3. Submit
4. Wait (manually reviewed)
5. Once approved, upload plugin to WordPress SVN

note
1. after, upload to SVN, automatically displayed in the [plugins browser](https://wordpress.org/plugins/)
2. เคยเจอ user run บน 5.4 ก็ระวังเรื่อง syntax ด้วยเช่นเวลาจะใช้อาเรย์ ก็ต้องใช้ `array()` แทน `[]`
3. แนะนำในการทำ zip file ก่อน submit, [ตัวอย่าง gulpfile.js](https://github.com/woodpeckerr/promptpay/blob/master/gulpfile.js)

#### 8.1.2 Review

มีหลายข้อแต่คัดมาบางข้อ

1. License

GPLv2 or later
และต้องตรวจสอบไฟล์ทุกไฟล์ว่าลิขสิทธิ์ นั้นถูกต้องไม่ว่าจะโค้ด, รูปภาพหรืออื่นๆ

2. Code must be human readable

ป้องกันพวก 
malicious code, such as backdoors or tracking

3. Trialware is not permitted

ห้าม plugin พวกทดลองใช้


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

create tag
when release new version

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


### 8.2 Theme

Theme จะเข้าส่วน trac แล้วมีการ review โดยละเอียด comment เป็นจุดๆ

คัดมาเฉพาะบางจุด

ขอแยก process กับ review ออก


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

ก่อนจะ รีวิวแนะนำให้
ทดสอบโดยใช้ Theme unit test แนะนำ [Theme Unit Test](https://codex.wordpress.org/Theme_Unit_Test), [WP Test - The Best Tests for WordPress](http://wptest.io/)

1. [Recommended](https://make.wordpress.org/themes/handbook/review/recommended/) (optional)

Documentation
- readme.txt file
- changelog.txt

2. [Accessibility](https://make.wordpress.org/themes/handbook/review/accessibility) (optional)

optional คล้ายๆพวก web accessibility

สำหรับคนที่ใช้ `accessibility-ready` tag
heading e.g. H1 for article, h2, etc. หรือแบบการเล่นสีหรือการใช้สีมากเกินไป ก็จะทำให้คนตาบอดสี เห็น content ได้ยาก

3. [Required](https://make.wordpress.org/themes/handbook/review/required/)
3.1 Code
- No PHP or JS notices.
- Provide a unique prefix

    for everything the Theme defines in the public namespace, including options, functions, global variables, constants, post meta, etc.

- Pass [Theme Check](https://make.wordpress.org/themes/handbook/review/required/theme-check-plugin/)

รัน basic test เช่นตรวจ deprecated, styles, screenshot, text domain
3.2 Core Functionality and Features

- WordPress functionality (if available)

  e.g. Sidebars, Navigation Menus, Post Thumbnails

- Child theme ready

- 3 major WordPress versions backwards compatible

(version 4.5 if 4.8 is latest)

3.3 Language, Localization ready

All theme text strings are to be translatable, Include a text domain in style.css.

3.4 Licensing, 100% GPL-compatible licensed

including code, design, all resources e.g. font, image

3.5 Plugins

- Cannot include plugins
- Cannot require plugins to work
- May use TGM Plugin Activation to recommend plugins

3.6 Others
- Include comments.php
- dont block admin bar
- Any custom features, template should be explained
- Documentation, any custom features, template should be explained

แนะนำ
ให้ทำ page list ไว้
โชว์ใน [readme.txt](https://github.com/jojoee/medium-clone/blob/master/readme.txt) เพื่อตัวเองและ reviewer
แนบรูปด้วย

post / page checklist
1. home
/

2. post
/featured-image-parent/
/sticky/

3. page
/blog/
/amazon-store/
/about/
/parent-page/child-page-03/

3. archive
3.1 author
found: /author/joe/
empty: /author/dewde/

3.2 category
found: /category/post-formats/
empty: /category/scholarship/

3.3 date (month)
found: /2012/12/
found: /2016/08/
empty: /2016/12/

3.4 tag
found: /tag/fail/
empty: /tag/chat/

4. search
found: /?s=test
empty: /?s=404

5. 404
/404


- [Submit Your Theme or Theme Update to the Directory](https://wordpress.org/themes/upload/)
- [Theme Directory](https://wordpress.org/themes/getting-started/)
- [Theme Review Team](https://make.wordpress.org/themes/)
- [Review Process](https://make.wordpress.org/themes/handbook/review/)
- [Become a Reviewer](https://make.wordpress.org/themes/handbook/get-involved/become-a-reviewer/)
- [Theme Handbook](https://developer.wordpress.org/themes/)

## 9. Recap

1. Web development standards
2. WordPress development standards
ทำงานร่วมกับ Framework และคนอื่น
3. WordPress.org submitting standards
ส่งงาน
ใส่รายละเอียด ให้มากสุด

แต่ละ process ต้องเข้า queue ใช้เวลานาน

และถ้าเราเป็น reviewer เราก็อยากจะเลือก review plugin ที่มันได้มาตรฐาน นิดนึง
จะได้ทำงานไวๆ

พอมันได้มาตรฐาน
เราเองก็พัฒนาและดูและมันง่าย
เว็บเราใช้งานได้ดี, โหลดไว, ใช้งานง่าย เราก็รีวิวง่าย


## 10. Thank you & QA

นอกจาก ได้รับความรู้มากขึ้น

ก็ยังมีสิ่งที่น่าประทับใจอื่นๆ
เช่นแบบ
มีคนส่งเมลมาถาม
หรือแบบ เขาบอกว่า plugin ช่วยได้มากเลย
เราดีใจ ซึ่งของพวกนี้มันประเมินค่าไม่ได้ สำหรับผม

อีกข้อนึงที่อยากจะชวนมาร่วมกันก็คือ

ถึงแม้เราจะเห็นว่า wordpress.org มี plguin อยู่เต็มเลย
แต่ยังไงเราก็ยังต้องการนักพัฒนาคนไทย มาช่วยกันตอบโจทย์เฉพาะอย่างอยู่ดี
เช่น 

https://github.com/woodpeckerr/promptpay
https://github.com/SeedThemes/seed-fonts
https://github.com/SeedThemes/seed-buddhist-year

ก็อยากให้มาช่วยกันครับ
ขอบคุณครับ


github.com/jojoee/3days



## 11. เครื่องมือหรืออื่นๆที่น่าสนใจ

- [PHP Code Checker](https://phpcodechecker.com/)
- [WP-CLI](http://wp-cli.org/)
- [wp_cron](https://codex.wordpress.org/Function_Reference/wp_cron)

### Boilerplate / Starter

- [WordPress Plugin Boilerplate](https://github.com/DevinVinson/WordPress-Plugin-Boilerplate)
- [WordPress Plugin Boilerplate Generator](https://wppb.me/)
- [WordPress Widget Boilerplate](https://github.com/tommcfarlin/WordPress-Widget-Boilerplate)

- [Underscores | A Starter Theme for WordPress](https://underscores.me/)
- [Sage | WordPress Starter Theme](https://roots.io/sage/)
