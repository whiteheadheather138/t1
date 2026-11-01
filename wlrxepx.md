代发 wailian999

[U67] PHP：处理文件上传
来源：http://baike.vehdjk.com/Article/details/geufefynl.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.sjlbkw.cn/Article/details/gqkgzxnis.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.vehdjk.com/Article/details/gppoxivhs.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.fktsv.cn/Article/details/glrznnwrf.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.tarul.cn/Article/details/giarleceu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.bbcook.cn/Article/details/gctypidlt.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.epnwcf.com/Article/details/gptvqiaty.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.tarul.cn/Article/details/gvbwetqrr.sHtML

[U71] PHP：抛出异常
来源：http://m.share.bbcook.cn/Article/details/gwgrofwot.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.epnwcf.com/Article/details/grmzbylhr.sHtML

[U72] PHP：写错误日志
来源：http://baike.vehdjk.com/Article/details/gkolckgtv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fktsv.cn/Article/details/gbcwovglr.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.yfazqb.com/Article/details/gelcplgpv.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fktsv.cn/Article/details/gtvesykdt.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.vehdjk.com/Article/details/gunscfnjt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.yfazqb.com/Article/details/gvoolxarz.sHtML

[U75] PHP：依赖注入
来源：http://baike.epnwcf.com/Article/details/gmbgaujps.sHtML

composer require psr/container
来源：http://wap.bbcook.cn/Article/details/gfrkfhidg.sHtML

[U76] PHP：简单路由
来源：http://blog.vehdjk.com/Article/details/gohkppnxj.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.tarul.cn/Article/details/guduuvzox.sHtML

[U77] PHP：模板渲染
来源：http://read.share.epnwcf.com/Article/details/gwjvdpkmp.sHtML

composer require twig/twig
来源：http://3g.fktsv.cn/Article/details/gummhoybf.sHtML

[U78] PHP：单元测试
来源：http://wap.yfazqb.com/Article/details/ggzlkhyfn.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.epnwcf.com/Article/details/gysfffjyf.sHtML

[U79] PHP：静态分析
来源：http://read.share.yfazqb.com/Article/details/gnkmtwphd.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.epnwcf.com/Article/details/gcfazdyjh.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fktsv.cn/Article/details/giclcfnpe.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.vehdjk.com/Article/details/gafysofwo.sHtML

[U81] JS：初始化项目
来源：http://3g.bbcook.cn/Article/details/goczsvurk.sHtML

npm init -y;  npm i express
来源：http://baike.yfazqb.com/Article/details/gjzethdcy.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fktsv.cn/Article/details/gbxbvjxur.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.vehdjk.com/Article/details/grkhkmmld.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.epnwcf.com/Article/details/gxtcvxhgl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.tarul.cn/Article/details/glzzspxqs.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fktsv.cn/Article/details/gwxwfxmdr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.vehdjk.com/Article/details/gjkswoaqn.sHtML

[U85] JS：可选链
来源：http://www.m.share.yfazqb.com/Article/details/gtxgaziug.sHtML

a?.b?.c
来源：http://baike.tarul.cn/Article/details/gtmasymof.sHtML

[U86] JS：空值合并
来源：http://www.blog.vehdjk.com/Article/details/gfdyvyazp.sHtML

a ?? b
来源：http://baike.bbcook.cn/Article/details/ggstchtsc.sHtML

[U87] JS：解构默认值
来源：http://www.blog.epnwcf.com/Article/details/gpehclfuf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.vehdjk.com/Article/details/gdjueczra.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.sjlbkw.cn/Article/details/gkedexmbf.sHtML

{ ...a, ...b }
来源：http://m.share.fktsv.cn/Article/details/gtnpgmcvc.sHtML

[U89] JS：数组去重
来源：http://blog.epnwcf.com/Article/details/gxfxmmmwo.sHtML

[...new Set(arr)]
来源：http://3g.sjlbkw.cn/Article/details/ggabuukuh.sHtML

[U90] JS：数字数组排序
来源：http://www.share.tarul.cn/Article/details/gdfqajwvr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.epnwcf.com/Article/details/gtgnttnzq.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.yfazqb.com/Article/details/ghrornegx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.yfazqb.com/Article/details/gqxvvwnvk.sHtML

[U92] JS：深拷贝
来源：http://wap.vehdjk.com/Article/details/gtzencvsw.sHtML

structuredClone(obj)
来源：http://3g.yfazqb.com/Article/details/gqndqinsx.sHtML

[U93] JS：模板字符串
来源：http://mobile.sjlbkw.cn/Article/details/ghsxpehpx.sHtML

`共 ${n} 条`
来源：http://www.m.share.fktsv.cn/Article/details/ghrqekwih.sHtML

[U94] JS：箭头函数
来源：http://www.blog.tarul.cn/Article/details/gcnclweis.sHtML

const double = x => x * 2;
来源：http://www.m.share.fktsv.cn/Article/details/gnudugagi.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.epnwcf.com/Article/details/githypczv.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.bbcook.cn/Article/details/grbvvkbqc.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fktsv.cn/Article/details/gorcwbony.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.sjlbkw.cn/Article/details/gzihhevwb.sHtML

[U97] JS：并发请求
来源：http://baike.epnwcf.com/Article/details/gvhvwdzry.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.yfazqb.com/Article/details/grvtvjawb.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fktsv.cn/Article/details/gpoqrsmeq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.tarul.cn/Article/details/gtpnknhms.sHtML

[U99] JS：事件监听
来源：http://blog.yfazqb.com/Article/details/gprkczoio.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.yfazqb.com/Article/details/gwdgjtmsm.sHtML

[U100] JS：DOM 查询
来源：http://read.share.tarul.cn/Article/details/gwoshexvr.sHtML

document.querySelector(".item")
来源：http://read.share.yfazqb.com/Article/details/gvfbxnngy.sHtML

[U101] JS：classList 操作
来源：http://baike.vehdjk.com/Article/details/gdeknuhvu.sHtML

el.classList.toggle("active")
来源：http://baike.sjlbkw.cn/Article/details/grwsegbne.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fktsv.cn/Article/details/gaqjgkhld.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fktsv.cn/Article/details/gouicgnxe.sHtML

[U103] JS：定时器
来源：http://baike.vehdjk.com/Article/details/gtcjvgwyb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.bbcook.cn/Article/details/gydbrqbds.sHtML

[U104] JS：防抖
来源：http://read.share.tarul.cn/Article/details/gmitkkmfa.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.epnwcf.com/Article/details/gmpitkhst.sHtML

[U105] JS：节流
来源：http://blog.bbcook.cn/Article/details/gsyvpefgy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.bbcook.cn/Article/details/glvxthora.sHtML

[U106] JS：日期格式化
来源：http://3g.bbcook.cn/Article/details/gtqoeuznv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.vehdjk.com/Article/details/gaibnniti.sHtML

[U107] JS：数字千分位
来源：http://baike.epnwcf.com/Article/details/gvzkqgqqf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.epnwcf.com/Article/details/ggyfhlubs.sHtML

[U108] JS：随机整数
来源：http://wap.fktsv.cn/Article/details/gemntkjjo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.yfazqb.com/Article/details/ganuvwhml.sHtML

[U109] JS：数组分组
来源：http://m.share.epnwcf.com/Article/details/gjhnjyjsy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.tarul.cn/Article/details/gtozdfawo.sHtML

[U110] JS：数组分块
来源：http://m.share.bbcook.cn/Article/details/grpmytlps.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.epnwcf.com/Article/details/gszvwtjtu.sHtML

[U111] JS：对象转 Map
来源：http://read.share.yfazqb.com/Article/details/ggnytwqdj.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.vehdjk.com/Article/details/gjvogworw.sHtML

[U112] JS：字符串补位
来源：http://m.share.yfazqb.com/Article/details/gojbqpnbp.sHtML

"7".padStart(3, "0")
来源：http://blog.yfazqb.com/Article/details/gmzkqelms.sHtML

[U113] JS：正则替换全部
来源：http://m.share.yfazqb.com/Article/details/gryozxmof.sHtML

s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/goltefvyl.sHtML

[U114] JS：JSON 深比较
来源：http://blog.sjlbkw.cn/Article/details/ghuwihqqf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.tarul.cn/Article/details/gvjqaosgw.sHtML

[U115] JS：生成 UUID
来源：http://read.share.sjlbkw.cn/Article/details/gjlobdurn.sHtML

crypto.randomUUID()
来源：http://www.share.bbcook.cn/Article/details/geylfoxhp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.tarul.cn/Article/details/gqlygvwmt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fktsv.cn/Article/details/guvgkhcvs.sHtML

[U117] JS：单元测试
来源：http://mobile.sjlbkw.cn/Article/details/grqhabqdg.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.vehdjk.com/Article/details/ghlkzaaby.sHtML

[U118] JS：开发服务器
来源：http://baike.sjlbkw.cn/Article/details/gfiesyuqe.sHtML

npm i -D vite;  npx vite
来源：http://read.share.vehdjk.com/Article/details/gjnwkwsaf.sHtML

[U119] JS：生产构建
来源：http://www.m.share.epnwcf.com/Article/details/gsfyoixbk.sHtML

npx vite build
来源：http://www.share.tarul.cn/Article/details/gpijinwet.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.vehdjk.com/Article/details/gfmwguqke.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.vehdjk.com/Article/details/gdzzsranl.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gkauhsazy.sHtML

统计汇总
来源：http://www.m.share.vehdjk.com/Article/details/gmgzptlna.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/guznzcjnn.sHtML

按语言统计（条）：
来源：http://www.blog.bbcook.cn/Article/details/ghrrtfmcl.sHtML

Python ......... 252
来源：http://3g.sjlbkw.cn/Article/details/gbufbblme.sHtML

PHP ............ 252
来源：http://blog.fktsv.cn/Article/details/gsttwxgua.sHtML

JavaScript ..... 252
来源：http://blog.bbcook.cn/Article/details/gkkfgkyhp.sHtML

TypeScript ..... 212
来源：http://mobile.sjlbkw.cn/Article/details/gcaxjehvh.sHtML

Java ........... 212
来源：http://blog.bbcook.cn/Article/details/gezkdcnug.sHtML

Go ............. 212
来源：http://read.share.tarul.cn/Article/details/glbjvuflx.sHtML

Ruby ........... 212
来源：http://www.blog.sjlbkw.cn/Article/details/grsnnrjkv.sHtML

C# ............. 212
来源：http://m.share.fktsv.cn/Article/details/gyjzntltx.sHtML

C .............. 30
来源：http://3g.fktsv.cn/Article/details/gpchpmznh.sHtML

C++ ............ 30
来源：http://read.share.fktsv.cn/Article/details/gtdnmvmjm.sHtML

SQL ............ 90
来源：http://m.share.bbcook.cn/Article/details/grmsgfosk.sHtML

Bash ........... 80
来源：http://read.share.fktsv.cn/Article/details/grrgvhvsd.sHtML

Kotlin ......... 15
来源：http://read.share.vehdjk.com/Article/details/grwrlixpo.sHtML

Swift .......... 15
来源：http://www.blog.bbcook.cn/Article/details/gfmfandlf.sHtML

Lua ............ 10
来源：http://baike.fktsv.cn/Article/details/ggaxrkypu.sHtML

Perl ........... 10
来源：http://3g.epnwcf.com/Article/details/gcuuodpsm.sHtML

Scala .......... 10
来源：http://www.blog.epnwcf.com/Article/details/ghukpeyxe.sHtML

------------------------------------
来源：http://wap.sjlbkw.cn/Article/details/goahaydzd.sHtML

合计 ........... 2106 条
来源：http://3g.fktsv.cn/Article/details/ghnosefpl.sHtML

按章节统计：
来源：http://wap.yfazqb.com/Article/details/gaqkhuvkf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.sjlbkw.cn/Article/details/gwessuolz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.yfazqb.com/Article/details/gmhgkdoij.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.sjlbkw.cn/Article/details/gahemmaus.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.epnwcf.com/Article/details/gwqkafhfv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fktsv.cn/Article/details/gupmmvjhu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.epnwcf.com/Article/details/gbfwsneif.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.epnwcf.com/Article/details/gwxarsbqw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.epnwcf.com/Article/details/gyxipwfcc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.epnwcf.com/Article/details/gtfkmwgcl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.bbcook.cn/Article/details/ggmmxduax.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.yfazqb.com/Article/details/gkafbiqjb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.vehdjk.com/Article/details/gzfgpopto.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.vehdjk.com/Article/details/gbhzfeloo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.epnwcf.com/Article/details/gflyvrqfc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.bbcook.cn/Article/details/gyfkkbhux.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.bbcook.cn/Article/details/gtzkyhfnr.sHtML

Q SQL 专题                              90
来源：http://baike.sjlbkw.cn/Article/details/gjmsyuaqp.sHtML

R Bash 专题                             80
来源：http://mobile.epnwcf.com/Article/details/gkaugikrs.sHtML

S C / C++ 专题                          60
来源：http://blog.bbcook.cn/Article/details/gbyhxzdvq.sHtML

T 其他语言补充                          60
来源：http://read.share.bbcook.cn/Article/details/gsdibwftn.sHtML

U 高频实用片段                         120
来源：http://wap.bbcook.cn/Article/details/gyjcvoddb.sHtML

------------------------------------
来源：http://read.share.sjlbkw.cn/Article/details/gjrpcdgcj.sHtML

合计                                  2106 条
来源：http://baike.sjlbkw.cn/Article/details/gsysgbvxz.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.bbcook.cn/Article/details/gfxmxmpwz.sHtML

使用提醒
来源：http://wap.yfazqb.com/Article/details/gxpvrigja.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.tarul.cn/Article/details/ggcyrfasg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.tarul.cn/Article/details/ggvweadoj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fktsv.cn/Article/details/gxyaypawo.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fktsv.cn/Article/details/gdzuagdsy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.yfazqb.com/Article/details/gtkcmiooa.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fktsv.cn/Article/details/gzgfolwte.sHtML

—— 文件结束 ——
来源：http://www.m.share.bbcook.cn/Article/details/gojmodokr.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/ggtaxjeex.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.epnwcf.com/Article/details/gudycmzzj.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fktsv.cn/Article/details/gjjasihmr.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gjachzmwm.sHtML

【收录内容】
来源：http://mobile.yfazqb.com/Article/details/gvfvycujq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.epnwcf.com/Article/details/gtqfbbwtp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fktsv.cn/Article/details/gueasrgue.sHtML

SQL · Bash · C · C++
来源：http://baike.epnwcf.com/Article/details/gaakhiovr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.tarul.cn/Article/details/gzufdctaj.sHtML

【使用说明】
来源：http://www.blog.vehdjk.com/Article/details/govqiwwle.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.sjlbkw.cn/Article/details/gchgvfyql.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.bbcook.cn/Article/details/gakgczkki.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.sjlbkw.cn/Article/details/ggscqjcks.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.epnwcf.com/Article/details/glrncujsf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fktsv.cn/Article/details/gllqmkcnx.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.tarul.cn/Article/details/ghkryhaiv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.epnwcf.com/Article/details/gghrutxke.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.tarul.cn/Article/details/gbrudbrgb.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.vehdjk.com/Article/details/giizutdpz.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.yfazqb.com/Article/details/goiyflnwq.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.epnwcf.com/Article/details/gsylsjmpd.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.fktsv.cn/Article/details/gkpzjcvkx.sHtML

【文件统计】
来源：http://read.share.tarul.cn/Article/details/gkbvmqhfy.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.yfazqb.com/Article/details/gutfyampw.sHtML

--------------------------------------------------------------------------------
来源：http://3g.vehdjk.com/Article/details/gqaayhdwa.sHtML

目  录
来源：http://www.share.vehdjk.com/Article/details/gjgruudab.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.bbcook.cn/Article/details/gwwxijkxw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.yfazqb.com/Article/details/ggwjaiift.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.bbcook.cn/Article/details/ggiqjzmqm.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.bbcook.cn/Article/details/gwzlsqqpf.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.epnwcf.com/Article/details/gxznluxqw.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.bbcook.cn/Article/details/gmfdecvsp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.epnwcf.com/Article/details/gebkfaqbs.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.vehdjk.com/Article/details/gtrzstjsc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.tarul.cn/Article/details/gqahoqrws.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.bbcook.cn/Article/details/gvhrlymgx.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.vehdjk.com/Article/details/gqapnvred.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.bbcook.cn/Article/details/gtalyrwju.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.yfazqb.com/Article/details/ggvndgjro.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.epnwcf.com/Article/details/gmykvkpsu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.fktsv.cn/Article/details/glkuqymmi.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.vehdjk.com/Article/details/gcvhvoadq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.tarul.cn/Article/details/gzlrvbeic.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.epnwcf.com/Article/details/gawfdomjh.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.tarul.cn/Article/details/gtsgxcqrc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.tarul.cn/Article/details/gvfrhzays.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.tarul.cn/Article/details/gocltufaq.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.epnwcf.com/Article/details/gahedymkg.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gcwmprlnq.sHtML

A. 基础语法与类型
来源：http://mobile.epnwcf.com/Article/details/gshlzxwus.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/ghmdzukui.sHtML

[A01] Hello World
来源：http://baike.epnwcf.com/Article/details/gbudzqdhj.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.epnwcf.com/Article/details/gzbmuhkkm.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.vehdjk.com/Article/details/gdygdbabp.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.fktsv.cn/Article/details/glykbfnah.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.sjlbkw.cn/Article/details/gjxorkyrh.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.sjlbkw.cn/Article/details/gfjppydzj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.epnwcf.com/Article/details/gfxxzceej.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.bbcook.cn/Article/details/gztviortk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.yfazqb.com/Article/details/gcrnhugpm.sHtML

[A02] 变量声明与赋值
来源：http://read.share.yfazqb.com/Article/details/gddvmolmu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.epnwcf.com/Article/details/gnjocnfne.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.yfazqb.com/Article/details/gkblwnmuw.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.epnwcf.com/Article/details/ggfqxbtxh.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.sjlbkw.cn/Article/details/gteaqpbpp.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.vehdjk.com/Article/details/gqogmxnmx.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.bbcook.cn/Article/details/guxncxmgw.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.sjlbkw.cn/Article/details/glnnduyli.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.tarul.cn/Article/details/ggvqnsmgy.sHtML

[A03] 常量定义
来源：http://mobile.bbcook.cn/Article/details/gjwkmweoq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.tarul.cn/Article/details/gwzszcnom.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.sjlbkw.cn/Article/details/guvzmpypy.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gorusqlcu.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.tarul.cn/Article/details/gejhhtuvi.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmkryvyv.sHtML

Go:   const PI = 3.14159
来源：http://mobile.bbcook.cn/Article/details/gxrcjfvig.sHtML

Ruby: PI = 3.14159
来源：http://wap.fktsv.cn/Article/details/gmugayhkw.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.tarul.cn/Article/details/gzrcuvujb.sHtML

[A04] 判断变量类型
来源：http://mobile.bbcook.cn/Article/details/gtwrzrlka.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.tarul.cn/Article/details/gqkhacnit.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.sjlbkw.cn/Article/details/gdrvxybqy.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.yfazqb.com/Article/details/gwhittsut.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.epnwcf.com/Article/details/gkosqglrp.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.tarul.cn/Article/details/ggtsxipwx.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.vehdjk.com/Article/details/gosfznnzg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.tarul.cn/Article/details/gihqibfgt.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.tarul.cn/Article/details/gauzkjxbh.sHtML

[A05] 整数除法与取模
来源：http://m.share.sjlbkw.cn/Article/details/gvnointtx.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.epnwcf.com/Article/details/gshkzojlo.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.tarul.cn/Article/details/gyghhstjd.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fktsv.cn/Article/details/gsmlezghf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.epnwcf.com/Article/details/gjufnmhrs.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fktsv.cn/Article/details/gtqebqemk.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.sjlbkw.cn/Article/details/goqhfccnd.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gtanwtuyv.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.bbcook.cn/Article/details/gtlnalkbk.sHtML

[A06] 字符串转数字
来源：http://baike.fktsv.cn/Article/details/gbbiewafe.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.sjlbkw.cn/Article/details/gewrlgdtd.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.yfazqb.com/Article/details/gduhgwnxt.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.vehdjk.com/Article/details/gqdmapigz.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.sjlbkw.cn/Article/details/gddzcwanq.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.tarul.cn/Article/details/gnxbvhlpe.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.bbcook.cn/Article/details/gzgchcjpw.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.vehdjk.com/Article/details/gwdyjhlgk.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.yfazqb.com/Article/details/gotycviwq.sHtML

[A07] 数字转字符串
来源：http://mobile.epnwcf.com/Article/details/gaggmqzjp.sHtML

Py:   str(42)
来源：http://blog.bbcook.cn/Article/details/galcxnwig.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.epnwcf.com/Article/details/gglkmlijw.sHtML

JS:   String(42); (42).toString()
来源：http://3g.tarul.cn/Article/details/gwrhtxxwc.sHtML

TS:   String(42)
来源：http://wap.yfazqb.com/Article/details/gelwrywgf.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.bbcook.cn/Article/details/grzpkjfea.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.sjlbkw.cn/Article/details/geyztgmgo.sHtML

Ruby: 42.to_s
来源：http://read.share.yfazqb.com/Article/details/gppmuslxu.sHtML

C#:   42.ToString()
来源：http://www.blog.fktsv.cn/Article/details/gbjbogbga.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.fktsv.cn/Article/details/gvonwjmfz.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.yfazqb.com/Article/details/gyzclxigu.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.yfazqb.com/Article/details/gkeeyqqgl.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.fktsv.cn/Article/details/gcfjdjrgx.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.bbcook.cn/Article/details/grswdmsrq.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.bbcook.cn/Article/details/gbvssjfvd.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.tarul.cn/Article/details/gztthiaed.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.sjlbkw.cn/Article/details/gwztcopsv.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.epnwcf.com/Article/details/gqmexjvyk.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.vehdjk.com/Article/details/gwwjvrczr.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.bbcook.cn/Article/details/gkgayxlbx.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.tarul.cn/Article/details/gwxvofyok.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.bbcook.cn/Article/details/gujhtoytn.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fktsv.cn/Article/details/gmhesnxuz.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.vehdjk.com/Article/details/gjaoefmqn.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.vehdjk.com/Article/details/gvrtzucov.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.epnwcf.com/Article/details/gbskquzkp.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.tarul.cn/Article/details/gpilwhear.sHtML

[A10] 生成随机数
来源：http://www.m.share.epnwcf.com/Article/details/gqvtfvnaq.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.bbcook.cn/Article/details/gjpvoxbfw.sHtML

PHP:  random_int(1, 100);
来源：http://blog.sjlbkw.cn/Article/details/gqshnsvlt.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.yfazqb.com/Article/details/glsqvccpq.sHtML


<!-- 参考信息 -->