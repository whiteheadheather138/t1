代发 wailian999

[U65] PHP：会话
来源：http://mobile.epnwcf.com/Article/details/gisblsyvo.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.vehdjk.com/Article/details/gpvrfqaxi.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.bbcook.cn/Article/details/gkyyjmddz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.vehdjk.com/Article/details/gesjmnbof.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.sjlbkw.cn/Article/details/gnddnlave.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.vehdjk.com/Article/details/gpxpnjzzh.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.vehdjk.com/Article/details/gwcjozcfi.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.vehdjk.com/Article/details/gcinfexrc.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.epnwcf.com/Article/details/gxwweuojj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.epnwcf.com/Article/details/gezblcbhh.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.bbcook.cn/Article/details/gonheemuo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.epnwcf.com/Article/details/gkzjbjtuy.sHtML

[U71] PHP：抛出异常
来源：http://m.share.sjlbkw.cn/Article/details/gxwkvnrhe.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.tarul.cn/Article/details/gqxqaakvk.sHtML

[U72] PHP：写错误日志
来源：http://www.share.epnwcf.com/Article/details/gtxqycyex.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.bbcook.cn/Article/details/gyajqmtkk.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.sjlbkw.cn/Article/details/gzvuqsuyz.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.epnwcf.com/Article/details/gatirtwgf.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.epnwcf.com/Article/details/gdklrigtr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fktsv.cn/Article/details/gcrvpgbfy.sHtML

[U75] PHP：依赖注入
来源：http://read.share.epnwcf.com/Article/details/ggaelbomp.sHtML

composer require psr/container
来源：http://www.share.yfazqb.com/Article/details/gdfydyjgt.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.sjlbkw.cn/Article/details/gwuylletk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.tarul.cn/Article/details/gwsmanjvf.sHtML

[U77] PHP：模板渲染
来源：http://3g.bbcook.cn/Article/details/gwzwyydko.sHtML

composer require twig/twig
来源：http://baike.vehdjk.com/Article/details/gepugscaz.sHtML

[U78] PHP：单元测试
来源：http://m.share.yfazqb.com/Article/details/gtrqsxcgk.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.sjlbkw.cn/Article/details/gaxylwguf.sHtML

[U79] PHP：静态分析
来源：http://www.blog.sjlbkw.cn/Article/details/gtvydtnlo.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.vehdjk.com/Article/details/gfuhhgley.sHtML

[U80] PHP：代码规范修复
来源：http://3g.tarul.cn/Article/details/gpbwdiyta.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.sjlbkw.cn/Article/details/gqkileyzn.sHtML

[U81] JS：初始化项目
来源：http://blog.yfazqb.com/Article/details/gjmebcuku.sHtML

npm init -y;  npm i express
来源：http://www.share.bbcook.cn/Article/details/gfigrfjvw.sHtML

[U82] JS：package.json 脚本
来源：http://3g.tarul.cn/Article/details/gydeufhtq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.sjlbkw.cn/Article/details/gtpwecgfq.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.vehdjk.com/Article/details/gqdkabvuw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.epnwcf.com/Article/details/gvfnwtvas.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.vehdjk.com/Article/details/gpzpaurun.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.bbcook.cn/Article/details/gojmgifpe.sHtML

[U85] JS：可选链
来源：http://www.m.share.vehdjk.com/Article/details/gjceacjdr.sHtML

a?.b?.c
来源：http://www.share.tarul.cn/Article/details/ggqckpbav.sHtML

[U86] JS：空值合并
来源：http://wap.vehdjk.com/Article/details/guchivavl.sHtML

a ?? b
来源：http://3g.fktsv.cn/Article/details/gpbwrroas.sHtML

[U87] JS：解构默认值
来源：http://www.blog.vehdjk.com/Article/details/gfbcfmnwo.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.bbcook.cn/Article/details/gzaepqjxa.sHtML

[U88] JS：对象展开合并
来源：http://www.share.epnwcf.com/Article/details/gkfbcxspj.sHtML

{ ...a, ...b }
来源：http://3g.tarul.cn/Article/details/guyztzcax.sHtML

[U89] JS：数组去重
来源：http://mobile.sjlbkw.cn/Article/details/gwemsbtoj.sHtML

[...new Set(arr)]
来源：http://baike.vehdjk.com/Article/details/glafasebc.sHtML

[U90] JS：数字数组排序
来源：http://www.share.epnwcf.com/Article/details/giidzcvtu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.sjlbkw.cn/Article/details/gmamqqzlr.sHtML

[U91] JS：对象键值遍历
来源：http://wap.bbcook.cn/Article/details/gqsmogkre.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.sjlbkw.cn/Article/details/ghmaukbgr.sHtML

[U92] JS：深拷贝
来源：http://www.blog.epnwcf.com/Article/details/gqhojimpk.sHtML

structuredClone(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gicywojtu.sHtML

[U93] JS：模板字符串
来源：http://www.share.fktsv.cn/Article/details/ghobwiajp.sHtML

`共 ${n} 条`
来源：http://www.share.epnwcf.com/Article/details/grkmsjtow.sHtML

[U94] JS：箭头函数
来源：http://m.share.fktsv.cn/Article/details/glieuizhv.sHtML

const double = x => x * 2;
来源：http://mobile.fktsv.cn/Article/details/gzoueqnlp.sHtML

[U95] JS：Promise 包装
来源：http://read.share.bbcook.cn/Article/details/gvnewzzqx.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.yfazqb.com/Article/details/gtcwgbfxa.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fktsv.cn/Article/details/gieiueaqk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fktsv.cn/Article/details/gjrvmnsmq.sHtML

[U97] JS：并发请求
来源：http://baike.bbcook.cn/Article/details/gfkmdtfwy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.tarul.cn/Article/details/gnqkbkrhp.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.tarul.cn/Article/details/gxnkwnbkn.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.sjlbkw.cn/Article/details/gqriqwext.sHtML

[U99] JS：事件监听
来源：http://3g.epnwcf.com/Article/details/gnypyzvnh.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.bbcook.cn/Article/details/gqzigwhdg.sHtML

[U100] JS：DOM 查询
来源：http://baike.vehdjk.com/Article/details/grzmisbns.sHtML

document.querySelector(".item")
来源：http://www.blog.vehdjk.com/Article/details/gbtrdrxbt.sHtML

[U101] JS：classList 操作
来源：http://m.share.vehdjk.com/Article/details/gyjclwxrs.sHtML

el.classList.toggle("active")
来源：http://mobile.bbcook.cn/Article/details/gwfzasedy.sHtML

[U102] JS：本地存储
来源：http://www.share.yfazqb.com/Article/details/gxsembvht.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.bbcook.cn/Article/details/gsqbcrcuo.sHtML

[U103] JS：定时器
来源：http://read.share.yfazqb.com/Article/details/guybyiwio.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.epnwcf.com/Article/details/gcyqzwgfw.sHtML

[U104] JS：防抖
来源：http://baike.sjlbkw.cn/Article/details/gwnrcycaj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fktsv.cn/Article/details/gnfmqplma.sHtML

[U105] JS：节流
来源：http://blog.fktsv.cn/Article/details/guazahgay.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.yfazqb.com/Article/details/gzysmyeps.sHtML

[U106] JS：日期格式化
来源：http://mobile.yfazqb.com/Article/details/gtrbrgqaw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.epnwcf.com/Article/details/gkitsnwas.sHtML

[U107] JS：数字千分位
来源：http://read.share.yfazqb.com/Article/details/glruwjnoz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.tarul.cn/Article/details/gwrntzpih.sHtML

[U108] JS：随机整数
来源：http://3g.sjlbkw.cn/Article/details/gktfadfhy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.bbcook.cn/Article/details/gxuwlmlnc.sHtML

[U109] JS：数组分组
来源：http://3g.epnwcf.com/Article/details/gmmhjsybd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.sjlbkw.cn/Article/details/gtnglhbyw.sHtML

[U110] JS：数组分块
来源：http://blog.fktsv.cn/Article/details/gmanfyixo.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fktsv.cn/Article/details/gdcmlphbj.sHtML

[U111] JS：对象转 Map
来源：http://3g.fktsv.cn/Article/details/gsvfbbbtw.sHtML

new Map(Object.entries(obj))
来源：http://wap.fktsv.cn/Article/details/gnuuxyhgi.sHtML

[U112] JS：字符串补位
来源：http://www.blog.vehdjk.com/Article/details/gxdkmhvve.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.sjlbkw.cn/Article/details/giufymvmq.sHtML

[U113] JS：正则替换全部
来源：http://m.share.epnwcf.com/Article/details/gexpvuynu.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.epnwcf.com/Article/details/gpvnzubmy.sHtML

[U114] JS：JSON 深比较
来源：http://baike.epnwcf.com/Article/details/gypyprjdz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.epnwcf.com/Article/details/grdqzyvvu.sHtML

[U115] JS：生成 UUID
来源：http://www.share.epnwcf.com/Article/details/gkseccoph.sHtML

crypto.randomUUID()
来源：http://3g.sjlbkw.cn/Article/details/getcozjua.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.sjlbkw.cn/Article/details/gpqkobfxb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.epnwcf.com/Article/details/gaebocmdv.sHtML

[U117] JS：单元测试
来源：http://read.share.bbcook.cn/Article/details/gmnhrtduk.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.tarul.cn/Article/details/gcwcpymrv.sHtML

[U118] JS：开发服务器
来源：http://www.blog.bbcook.cn/Article/details/gowlzkjcj.sHtML

npm i -D vite;  npx vite
来源：http://m.share.epnwcf.com/Article/details/gxjzgcdwr.sHtML

[U119] JS：生产构建
来源：http://www.blog.yfazqb.com/Article/details/gtznrkmom.sHtML

npx vite build
来源：http://baike.bbcook.cn/Article/details/gqyfcdisi.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.epnwcf.com/Article/details/ggxuedejr.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.bbcook.cn/Article/details/gbxmidadf.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gluxyykkv.sHtML

统计汇总
来源：http://read.share.vehdjk.com/Article/details/gjfrpusjq.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gyqgtycev.sHtML

按语言统计（条）：
来源：http://read.share.vehdjk.com/Article/details/ggkjvxwho.sHtML

Python ......... 252
来源：http://read.share.epnwcf.com/Article/details/gmvzpbgbr.sHtML

PHP ............ 252
来源：http://mobile.sjlbkw.cn/Article/details/gzeqyunbh.sHtML

JavaScript ..... 252
来源：http://www.share.yfazqb.com/Article/details/gixjsudju.sHtML

TypeScript ..... 212
来源：http://www.blog.tarul.cn/Article/details/gpuccdujk.sHtML

Java ........... 212
来源：http://www.blog.tarul.cn/Article/details/gxsgcmojg.sHtML

Go ............. 212
来源：http://baike.fktsv.cn/Article/details/gdbizbzlr.sHtML

Ruby ........... 212
来源：http://www.blog.yfazqb.com/Article/details/guujzjtyj.sHtML

C# ............. 212
来源：http://read.share.yfazqb.com/Article/details/gbsbhyswo.sHtML

C .............. 30
来源：http://www.blog.epnwcf.com/Article/details/gnfuinuaj.sHtML

C++ ............ 30
来源：http://mobile.epnwcf.com/Article/details/gieuukkul.sHtML

SQL ............ 90
来源：http://baike.vehdjk.com/Article/details/ghnlpofwz.sHtML

Bash ........... 80
来源：http://wap.bbcook.cn/Article/details/gabwpoice.sHtML

Kotlin ......... 15
来源：http://www.share.tarul.cn/Article/details/gpfeapwbo.sHtML

Swift .......... 15
来源：http://3g.epnwcf.com/Article/details/gbepwflbo.sHtML

Lua ............ 10
来源：http://mobile.tarul.cn/Article/details/gbpkuslvq.sHtML

Perl ........... 10
来源：http://m.share.fktsv.cn/Article/details/gjjmqtesp.sHtML

Scala .......... 10
来源：http://m.share.yfazqb.com/Article/details/gbqrraldu.sHtML

------------------------------------
来源：http://wap.bbcook.cn/Article/details/gizewbgwz.sHtML

合计 ........... 2106 条
来源：http://read.share.sjlbkw.cn/Article/details/gwagutcag.sHtML

按章节统计：
来源：http://baike.vehdjk.com/Article/details/gawrqhcdy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.tarul.cn/Article/details/gydeaaxll.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.tarul.cn/Article/details/gstgwzsmv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.yfazqb.com/Article/details/gzhfurtdf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.epnwcf.com/Article/details/gidskwlxw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.sjlbkw.cn/Article/details/gnjarjfny.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.yfazqb.com/Article/details/gdaqaekgn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.epnwcf.com/Article/details/gfshuubvg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.epnwcf.com/Article/details/gwllwwyop.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.tarul.cn/Article/details/gwvmesxmn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.vehdjk.com/Article/details/gwnhptnwc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fktsv.cn/Article/details/gdfvtshon.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fktsv.cn/Article/details/gcgqpxpwq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/gluzkuhaa.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.tarul.cn/Article/details/gonpueuhh.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fktsv.cn/Article/details/gtudsyxcu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fktsv.cn/Article/details/gqilfconm.sHtML

Q SQL 专题                              90
来源：http://www.blog.sjlbkw.cn/Article/details/gdpymasut.sHtML

R Bash 专题                             80
来源：http://wap.fktsv.cn/Article/details/gkbsgmboc.sHtML

S C / C++ 专题                          60
来源：http://wap.yfazqb.com/Article/details/gudgclvsb.sHtML

T 其他语言补充                          60
来源：http://blog.sjlbkw.cn/Article/details/gxyrysnvd.sHtML

U 高频实用片段                         120
来源：http://baike.yfazqb.com/Article/details/gstlzzjqu.sHtML

------------------------------------
来源：http://read.share.sjlbkw.cn/Article/details/gxbdzuruq.sHtML

合计                                  2106 条
来源：http://blog.tarul.cn/Article/details/gufhqqsdg.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.bbcook.cn/Article/details/gsqsjeqmv.sHtML

使用提醒
来源：http://mobile.yfazqb.com/Article/details/gbskyzjoe.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.epnwcf.com/Article/details/gcspihpwq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.tarul.cn/Article/details/gvilgjiyh.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.bbcook.cn/Article/details/gqwaisbzu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.tarul.cn/Article/details/geqmeqiah.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.yfazqb.com/Article/details/grqwuvcvh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.yfazqb.com/Article/details/gaorjojqm.sHtML

—— 文件结束 ——
来源：http://baike.bbcook.cn/Article/details/gciqaiokc.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gedavgssp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.yfazqb.com/Article/details/gnibjbwbd.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.tarul.cn/Article/details/gppfrljhu.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gbnyqychy.sHtML

【收录内容】
来源：http://www.m.share.bbcook.cn/Article/details/ghxsrulre.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.sjlbkw.cn/Article/details/gmjqyvwlz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.bbcook.cn/Article/details/galhfdtsz.sHtML

SQL · Bash · C · C++
来源：http://baike.yfazqb.com/Article/details/gfhilddgk.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.epnwcf.com/Article/details/gldqddtgy.sHtML

【使用说明】
来源：http://baike.vehdjk.com/Article/details/gmgvvaqsr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fktsv.cn/Article/details/gipivdccl.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.sjlbkw.cn/Article/details/gsucnbqzp.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.sjlbkw.cn/Article/details/gsaopxowy.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.vehdjk.com/Article/details/glczfjmfl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.yfazqb.com/Article/details/gggrnulqx.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fktsv.cn/Article/details/gayyuoxce.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.sjlbkw.cn/Article/details/gyudhrxho.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fktsv.cn/Article/details/gyrmqlggj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.vehdjk.com/Article/details/glyocludr.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.fktsv.cn/Article/details/gjfrjdauj.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.tarul.cn/Article/details/gcrdsnyjc.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.sjlbkw.cn/Article/details/gujpzndoj.sHtML

【文件统计】
来源：http://www.share.fktsv.cn/Article/details/gzpxsyszl.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.yfazqb.com/Article/details/gourozggu.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.yfazqb.com/Article/details/gwdjdyuoc.sHtML

目  录
来源：http://mobile.fktsv.cn/Article/details/giwxdogzz.sHtML

--------------------------------------------------------------------------------
来源：http://blog.vehdjk.com/Article/details/gplxmavng.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.yfazqb.com/Article/details/gqhtwbrew.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fktsv.cn/Article/details/gohfxzsyb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.fktsv.cn/Article/details/gnfxywloh.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.epnwcf.com/Article/details/gkrbajqbj.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.bbcook.cn/Article/details/ggyiryqxi.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.epnwcf.com/Article/details/gufcojjsu.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.sjlbkw.cn/Article/details/gnuzebocx.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.vehdjk.com/Article/details/gxabfjjwx.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.tarul.cn/Article/details/gbpwjbadm.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.bbcook.cn/Article/details/gfbwluqcp.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.epnwcf.com/Article/details/gvgavlvpf.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.epnwcf.com/Article/details/gyfeyrwdi.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.yfazqb.com/Article/details/gbgpuypzv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.bbcook.cn/Article/details/gdpycxljb.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fktsv.cn/Article/details/gewckelcu.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.vehdjk.com/Article/details/gnhmferyc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.epnwcf.com/Article/details/gcqkbobtq.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.vehdjk.com/Article/details/gyzotlvar.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.bbcook.cn/Article/details/gweurydmq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fktsv.cn/Article/details/gdwpdiwlo.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.sjlbkw.cn/Article/details/gjmdacucj.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gcpjamgnq.sHtML

A. 基础语法与类型
来源：http://www.share.vehdjk.com/Article/details/ggtmsexdw.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/ggguzzljk.sHtML

[A01] Hello World
来源：http://mobile.bbcook.cn/Article/details/ghlqxgrvi.sHtML

Py:   print("Hello, World!")
来源：http://blog.fktsv.cn/Article/details/goyravskx.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.yfazqb.com/Article/details/gofxuhkmc.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.tarul.cn/Article/details/gzcyowuzm.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.bbcook.cn/Article/details/gymqkpxeb.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.sjlbkw.cn/Article/details/gnaiexrli.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.fktsv.cn/Article/details/ghabhrfuy.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.bbcook.cn/Article/details/gnaltbtmi.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.sjlbkw.cn/Article/details/giedchkvh.sHtML

[A02] 变量声明与赋值
来源：http://wap.tarul.cn/Article/details/gpljdlajc.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.bbcook.cn/Article/details/gjwtqesnh.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.vehdjk.com/Article/details/gsfqjtnnc.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.sjlbkw.cn/Article/details/ghpvbujlw.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.yfazqb.com/Article/details/gkpwaucxh.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.yfazqb.com/Article/details/gojzfqpxb.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.fktsv.cn/Article/details/gyynumveo.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.yfazqb.com/Article/details/gzixkvtcu.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.tarul.cn/Article/details/gjccyuggp.sHtML

[A03] 常量定义
来源：http://3g.sjlbkw.cn/Article/details/gmdyoaibg.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.yfazqb.com/Article/details/gkiduoskd.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.yfazqb.com/Article/details/gchucnlgc.sHtML

JS:   const PI = 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/gsugmnbzn.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.bbcook.cn/Article/details/gkjwkmxil.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.epnwcf.com/Article/details/gpgcjqtaf.sHtML

Go:   const PI = 3.14159
来源：http://mobile.yfazqb.com/Article/details/gsanwxzeo.sHtML

Ruby: PI = 3.14159
来源：http://m.share.bbcook.cn/Article/details/gmnctecbk.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.vehdjk.com/Article/details/gcxyppvlg.sHtML

[A04] 判断变量类型
来源：http://baike.tarul.cn/Article/details/gugmpqdpz.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.epnwcf.com/Article/details/gouqpizxj.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.vehdjk.com/Article/details/gozwvjbbc.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.bbcook.cn/Article/details/gifhdmiot.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.epnwcf.com/Article/details/glpfdbrqv.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.vehdjk.com/Article/details/gckulmngk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.bbcook.cn/Article/details/gxdtlmwkf.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.tarul.cn/Article/details/gprmyvaod.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.fktsv.cn/Article/details/gzcrgwnec.sHtML

[A05] 整数除法与取模
来源：http://www.share.bbcook.cn/Article/details/gbfnievlj.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.epnwcf.com/Article/details/gywtmffuc.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.fktsv.cn/Article/details/guoswsiht.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gshcpmbgt.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.tarul.cn/Article/details/ggqbzbqoz.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.vehdjk.com/Article/details/gwhyvfwgc.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.sjlbkw.cn/Article/details/giuedpsdy.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.epnwcf.com/Article/details/gktuyqrae.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.vehdjk.com/Article/details/gknelyhlx.sHtML

[A06] 字符串转数字
来源：http://m.share.fktsv.cn/Article/details/gakhswbus.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.epnwcf.com/Article/details/gmtahywum.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.epnwcf.com/Article/details/gnmjorwxe.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.epnwcf.com/Article/details/gbtcuubvt.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.tarul.cn/Article/details/gwzyshhpm.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.bbcook.cn/Article/details/gfblwdcfb.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.epnwcf.com/Article/details/gmvqryexe.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.bbcook.cn/Article/details/gygxrtxdk.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.bbcook.cn/Article/details/ghdnuwgmf.sHtML

[A07] 数字转字符串
来源：http://baike.fktsv.cn/Article/details/glxfctcio.sHtML

Py:   str(42)
来源：http://baike.tarul.cn/Article/details/gsprlaolm.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.bbcook.cn/Article/details/gsefhebub.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.fktsv.cn/Article/details/gzwrkqazy.sHtML

TS:   String(42)
来源：http://wap.fktsv.cn/Article/details/gujpcdivq.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.yfazqb.com/Article/details/ggkioatod.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.yfazqb.com/Article/details/gytmscsis.sHtML

Ruby: 42.to_s
来源：http://www.share.yfazqb.com/Article/details/gphpcxnpu.sHtML

C#:   42.ToString()
来源：http://www.share.fktsv.cn/Article/details/grfbhpfix.sHtML

[A08] 取整与四舍五入
来源：http://blog.bbcook.cn/Article/details/gyatmgrtp.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.yfazqb.com/Article/details/gqctvcpxr.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.tarul.cn/Article/details/guqajkgoq.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.yfazqb.com/Article/details/goydjlywj.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.bbcook.cn/Article/details/gmcydemyx.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.sjlbkw.cn/Article/details/gqksdnppv.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.yfazqb.com/Article/details/gdcvydrrr.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.sjlbkw.cn/Article/details/geunblygh.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.tarul.cn/Article/details/gaaebrhzu.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.yfazqb.com/Article/details/gjbdnnlsl.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.tarul.cn/Article/details/gtyvcyadn.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.epnwcf.com/Article/details/gxcpbgeuy.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.fktsv.cn/Article/details/ghpojxyme.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.epnwcf.com/Article/details/ghrftormo.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.vehdjk.com/Article/details/glnsudyiu.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.tarul.cn/Article/details/goolsmpzk.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.yfazqb.com/Article/details/gogyqbflo.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.sjlbkw.cn/Article/details/grkzfwxug.sHtML


<!-- 参考信息 -->