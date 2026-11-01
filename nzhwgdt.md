代发 wailian999

[U69] PHP：PDO 预处理
来源：http://www.share.epnwcf.com/Article/details/gxckmrraz.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.epnwcf.com/Article/details/gamxlpias.sHtML

[U70] PHP：PDO 事务
来源：http://baike.vehdjk.com/Article/details/gptafqyhw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.bbcook.cn/Article/details/gwzosxwbx.sHtML

[U71] PHP：抛出异常
来源：http://www.share.sjlbkw.cn/Article/details/gqhdapmce.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.tarul.cn/Article/details/gvyspjihx.sHtML

[U72] PHP：写错误日志
来源：http://baike.fktsv.cn/Article/details/gjcdhwqzx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.vehdjk.com/Article/details/gifpxmdok.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.sjlbkw.cn/Article/details/gzcrmrpbk.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.epnwcf.com/Article/details/gdzhustdd.sHtML

[U74] PHP：读取环境变量
来源：http://blog.epnwcf.com/Article/details/ggqcvyqod.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.yfazqb.com/Article/details/gvcpmuhim.sHtML

[U75] PHP：依赖注入
来源：http://www.share.bbcook.cn/Article/details/gknyhmnbu.sHtML

composer require psr/container
来源：http://mobile.sjlbkw.cn/Article/details/gqwspwrml.sHtML

[U76] PHP：简单路由
来源：http://mobile.bbcook.cn/Article/details/goflnmvbh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.bbcook.cn/Article/details/gyrjzsdhz.sHtML

[U77] PHP：模板渲染
来源：http://wap.epnwcf.com/Article/details/gpcwfvutr.sHtML

composer require twig/twig
来源：http://www.m.share.vehdjk.com/Article/details/gcxilxlmc.sHtML

[U78] PHP：单元测试
来源：http://3g.vehdjk.com/Article/details/gunmccuex.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.sjlbkw.cn/Article/details/gozwjtrzt.sHtML

[U79] PHP：静态分析
来源：http://wap.fktsv.cn/Article/details/gzzreqfkk.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.yfazqb.com/Article/details/gdumistcy.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.vehdjk.com/Article/details/gafuqddoh.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.bbcook.cn/Article/details/gnkwrsrau.sHtML

[U81] JS：初始化项目
来源：http://mobile.sjlbkw.cn/Article/details/gzpcbmqhy.sHtML

npm init -y;  npm i express
来源：http://www.m.share.tarul.cn/Article/details/gfhsynlrn.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.epnwcf.com/Article/details/gqwpgutmu.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.bbcook.cn/Article/details/grnysabih.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.vehdjk.com/Article/details/gakecovlp.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.epnwcf.com/Article/details/gfodmcvrz.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.bbcook.cn/Article/details/gixdkjxwq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.bbcook.cn/Article/details/gyivppfow.sHtML

[U85] JS：可选链
来源：http://read.share.epnwcf.com/Article/details/gmapiwsev.sHtML

a?.b?.c
来源：http://blog.sjlbkw.cn/Article/details/gubbflrpo.sHtML

[U86] JS：空值合并
来源：http://www.blog.fktsv.cn/Article/details/gvycruwra.sHtML

a ?? b
来源：http://read.share.yfazqb.com/Article/details/gxtaneiux.sHtML

[U87] JS：解构默认值
来源：http://mobile.bbcook.cn/Article/details/gaeveemno.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.epnwcf.com/Article/details/gcapqrhdu.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.epnwcf.com/Article/details/ghckopdcr.sHtML

{ ...a, ...b }
来源：http://www.share.epnwcf.com/Article/details/gbgrisdbd.sHtML

[U89] JS：数组去重
来源：http://wap.fktsv.cn/Article/details/gfnhbcnli.sHtML

[...new Set(arr)]
来源：http://wap.sjlbkw.cn/Article/details/gnhxbgcwh.sHtML

[U90] JS：数字数组排序
来源：http://read.share.yfazqb.com/Article/details/grhanbrnc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fktsv.cn/Article/details/gtbqdyhzt.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.sjlbkw.cn/Article/details/gbsksxbkg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.yfazqb.com/Article/details/gkjzbckrp.sHtML

[U92] JS：深拷贝
来源：http://www.share.sjlbkw.cn/Article/details/ghiltogop.sHtML

structuredClone(obj)
来源：http://blog.fktsv.cn/Article/details/gqapjdyoy.sHtML

[U93] JS：模板字符串
来源：http://www.share.yfazqb.com/Article/details/gygydtcfg.sHtML

`共 ${n} 条`
来源：http://www.m.share.bbcook.cn/Article/details/gqlcigdcy.sHtML

[U94] JS：箭头函数
来源：http://baike.vehdjk.com/Article/details/gpeeffxfm.sHtML

const double = x => x * 2;
来源：http://mobile.fktsv.cn/Article/details/gscvhmjwe.sHtML

[U95] JS：Promise 包装
来源：http://m.share.epnwcf.com/Article/details/gqhjwaqgw.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.vehdjk.com/Article/details/gzoxqsyqw.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.vehdjk.com/Article/details/gusascgyp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.bbcook.cn/Article/details/gjqndxlze.sHtML

[U97] JS：并发请求
来源：http://3g.sjlbkw.cn/Article/details/gdletnwwi.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.yfazqb.com/Article/details/glpzrtgrd.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.epnwcf.com/Article/details/ghkwwilfo.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fktsv.cn/Article/details/gujehcvtj.sHtML

[U99] JS：事件监听
来源：http://baike.sjlbkw.cn/Article/details/gjzfpfcyz.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.tarul.cn/Article/details/gdfrkdspi.sHtML

[U100] JS：DOM 查询
来源：http://wap.bbcook.cn/Article/details/ggiqtlpaj.sHtML

document.querySelector(".item")
来源：http://baike.sjlbkw.cn/Article/details/gsobtoshy.sHtML

[U101] JS：classList 操作
来源：http://wap.yfazqb.com/Article/details/gxsytgmrv.sHtML

el.classList.toggle("active")
来源：http://baike.bbcook.cn/Article/details/gmyxvcomv.sHtML

[U102] JS：本地存储
来源：http://blog.vehdjk.com/Article/details/glfqhjvls.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.epnwcf.com/Article/details/gzlcftppp.sHtML

[U103] JS：定时器
来源：http://www.blog.sjlbkw.cn/Article/details/gdejaytvb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.sjlbkw.cn/Article/details/gkjcwujes.sHtML

[U104] JS：防抖
来源：http://www.share.tarul.cn/Article/details/gktjfqwvi.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.bbcook.cn/Article/details/gnialstlp.sHtML

[U105] JS：节流
来源：http://mobile.bbcook.cn/Article/details/gdtoobsxu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.sjlbkw.cn/Article/details/gjzojrqvz.sHtML

[U106] JS：日期格式化
来源：http://www.share.bbcook.cn/Article/details/gpuwpvztg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.vehdjk.com/Article/details/gruyozelh.sHtML

[U107] JS：数字千分位
来源：http://mobile.bbcook.cn/Article/details/gadxwufrv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.tarul.cn/Article/details/gyukmfrgq.sHtML

[U108] JS：随机整数
来源：http://3g.sjlbkw.cn/Article/details/gmmkdjrkb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.tarul.cn/Article/details/gemslaqid.sHtML

[U109] JS：数组分组
来源：http://read.share.yfazqb.com/Article/details/gbmlconmr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fktsv.cn/Article/details/gdgirlbuj.sHtML

[U110] JS：数组分块
来源：http://www.blog.fktsv.cn/Article/details/gbhxbdytx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fktsv.cn/Article/details/gkekawwqc.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fktsv.cn/Article/details/gfkizrtah.sHtML

new Map(Object.entries(obj))
来源：http://m.share.tarul.cn/Article/details/getibrfti.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.epnwcf.com/Article/details/gvnuqqffq.sHtML

"7".padStart(3, "0")
来源：http://www.blog.bbcook.cn/Article/details/glhjthdgb.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.sjlbkw.cn/Article/details/gbtkrwsuj.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.vehdjk.com/Article/details/gvmipbbjj.sHtML

[U114] JS：JSON 深比较
来源：http://blog.epnwcf.com/Article/details/gtuutuuqr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.bbcook.cn/Article/details/gggibyqik.sHtML

[U115] JS：生成 UUID
来源：http://3g.fktsv.cn/Article/details/gwfegnetf.sHtML

crypto.randomUUID()
来源：http://blog.fktsv.cn/Article/details/gwlblezaj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.epnwcf.com/Article/details/gdhrunckv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.tarul.cn/Article/details/gbqgqjxzv.sHtML

[U117] JS：单元测试
来源：http://m.share.vehdjk.com/Article/details/grvtwujho.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.epnwcf.com/Article/details/gkltppsis.sHtML

[U118] JS：开发服务器
来源：http://read.share.sjlbkw.cn/Article/details/gvfkvkpha.sHtML

npm i -D vite;  npx vite
来源：http://www.share.sjlbkw.cn/Article/details/gvaeierqd.sHtML

[U119] JS：生产构建
来源：http://mobile.fktsv.cn/Article/details/gedawyrva.sHtML

npx vite build
来源：http://www.share.epnwcf.com/Article/details/gvonodtgv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.tarul.cn/Article/details/gjpipbsdd.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.tarul.cn/Article/details/grerpvgsm.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gxizchmgr.sHtML

统计汇总
来源：http://www.share.bbcook.cn/Article/details/gytlpletc.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/geiwswnkm.sHtML

按语言统计（条）：
来源：http://www.m.share.bbcook.cn/Article/details/gbkibimma.sHtML

Python ......... 252
来源：http://read.share.tarul.cn/Article/details/gcsvefeoo.sHtML

PHP ............ 252
来源：http://m.share.tarul.cn/Article/details/grpqsgxry.sHtML

JavaScript ..... 252
来源：http://baike.epnwcf.com/Article/details/guzsugzvq.sHtML

TypeScript ..... 212
来源：http://3g.yfazqb.com/Article/details/gpwrqqrbx.sHtML

Java ........... 212
来源：http://blog.vehdjk.com/Article/details/gkhrkrivv.sHtML

Go ............. 212
来源：http://www.blog.yfazqb.com/Article/details/gnhovtyty.sHtML

Ruby ........... 212
来源：http://www.m.share.fktsv.cn/Article/details/gorwcnxcq.sHtML

C# ............. 212
来源：http://read.share.bbcook.cn/Article/details/gwqfoqkis.sHtML

C .............. 30
来源：http://www.m.share.fktsv.cn/Article/details/gwvynvvhp.sHtML

C++ ............ 30
来源：http://baike.epnwcf.com/Article/details/gxvhagcjt.sHtML

SQL ............ 90
来源：http://baike.fktsv.cn/Article/details/gzsvktnga.sHtML

Bash ........... 80
来源：http://m.share.fktsv.cn/Article/details/gtnsvkoco.sHtML

Kotlin ......... 15
来源：http://www.m.share.bbcook.cn/Article/details/gommnqaxb.sHtML

Swift .......... 15
来源：http://blog.tarul.cn/Article/details/gwwyowyld.sHtML

Lua ............ 10
来源：http://www.blog.yfazqb.com/Article/details/gvjljiont.sHtML

Perl ........... 10
来源：http://3g.fktsv.cn/Article/details/givdnbzpj.sHtML

Scala .......... 10
来源：http://baike.vehdjk.com/Article/details/gphjsrvsw.sHtML

------------------------------------
来源：http://blog.fktsv.cn/Article/details/gdbbexhni.sHtML

合计 ........... 2106 条
来源：http://blog.epnwcf.com/Article/details/gthvssgqd.sHtML

按章节统计：
来源：http://blog.tarul.cn/Article/details/ghxzfolwj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fktsv.cn/Article/details/gwdzxgmxi.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.yfazqb.com/Article/details/goxeevhqa.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.sjlbkw.cn/Article/details/gykibccpj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.sjlbkw.cn/Article/details/gjklbbzvo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.bbcook.cn/Article/details/gjwdiktcx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.tarul.cn/Article/details/ggirgtrbt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fktsv.cn/Article/details/gmnoffjrj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.vehdjk.com/Article/details/grjrfrzdy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fktsv.cn/Article/details/gkctjwgjd.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.tarul.cn/Article/details/geklnewsy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.bbcook.cn/Article/details/gzedfwmyk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.vehdjk.com/Article/details/gzehkkrrs.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.yfazqb.com/Article/details/gqdxreuah.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.epnwcf.com/Article/details/ggfqermek.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.bbcook.cn/Article/details/gkknycmxc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.bbcook.cn/Article/details/gesxpjlno.sHtML

Q SQL 专题                              90
来源：http://www.m.share.vehdjk.com/Article/details/ggnxjnehi.sHtML

R Bash 专题                             80
来源：http://m.share.tarul.cn/Article/details/ghusatdfl.sHtML

S C / C++ 专题                          60
来源：http://3g.yfazqb.com/Article/details/gglxbbmdg.sHtML

T 其他语言补充                          60
来源：http://baike.epnwcf.com/Article/details/gmtmvndbt.sHtML

U 高频实用片段                         120
来源：http://mobile.fktsv.cn/Article/details/gqponekpk.sHtML

------------------------------------
来源：http://3g.tarul.cn/Article/details/gdmvcyqhb.sHtML

合计                                  2106 条
来源：http://m.share.bbcook.cn/Article/details/giiknkpyj.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fktsv.cn/Article/details/gjkcdkjzo.sHtML

使用提醒
来源：http://www.m.share.vehdjk.com/Article/details/gjwrycbxr.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fktsv.cn/Article/details/gvgecyddj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fktsv.cn/Article/details/gegvcdfvb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.bbcook.cn/Article/details/gniddjlzx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.yfazqb.com/Article/details/gjyfjjiza.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.epnwcf.com/Article/details/gntophuzv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.bbcook.cn/Article/details/gcnbhdhez.sHtML

—— 文件结束 ——
来源：http://www.blog.vehdjk.com/Article/details/gddlkxdee.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/grtojjzro.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.yfazqb.com/Article/details/gblutredh.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.epnwcf.com/Article/details/gnbgapdzm.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gnletgver.sHtML

【收录内容】
来源：http://blog.tarul.cn/Article/details/gwlcruyld.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.yfazqb.com/Article/details/gpwngqlgh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.vehdjk.com/Article/details/gyelxpiky.sHtML

SQL · Bash · C · C++
来源：http://baike.tarul.cn/Article/details/gofshxfko.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.tarul.cn/Article/details/glzxjnmyt.sHtML

【使用说明】
来源：http://baike.vehdjk.com/Article/details/gceimqgkg.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.bbcook.cn/Article/details/gyaplolqe.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.epnwcf.com/Article/details/gdwoepnqy.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.bbcook.cn/Article/details/gicsulhhn.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.bbcook.cn/Article/details/gtqrhleye.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.tarul.cn/Article/details/gvsxyairv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.epnwcf.com/Article/details/geclpmval.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.fktsv.cn/Article/details/gtadqkudy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.tarul.cn/Article/details/grljsyugf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.sjlbkw.cn/Article/details/gkdftalel.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.tarul.cn/Article/details/gddjjtkhs.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.epnwcf.com/Article/details/gudqnsuro.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.vehdjk.com/Article/details/glfcngneu.sHtML

【文件统计】
来源：http://read.share.epnwcf.com/Article/details/gscsjnuth.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.tarul.cn/Article/details/glynktvvj.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.yfazqb.com/Article/details/gazpauxnv.sHtML

目  录
来源：http://baike.epnwcf.com/Article/details/gatmbttcf.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/ggybopohb.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.yfazqb.com/Article/details/gnbhrvshx.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.vehdjk.com/Article/details/ghvfswjwo.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.bbcook.cn/Article/details/gzufcluxc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.tarul.cn/Article/details/gktqvfdps.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.vehdjk.com/Article/details/gjpeygemn.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.epnwcf.com/Article/details/ganqdctox.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.tarul.cn/Article/details/gosgwaxso.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.vehdjk.com/Article/details/ggkkpsqdr.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.tarul.cn/Article/details/gweczkbyn.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.bbcook.cn/Article/details/gxssjugtu.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.tarul.cn/Article/details/gearbbsgv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.vehdjk.com/Article/details/gnapdnqbo.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.epnwcf.com/Article/details/ghhfddtkm.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.bbcook.cn/Article/details/gyijiadye.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.tarul.cn/Article/details/gnjxzobji.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.yfazqb.com/Article/details/grrbtwdii.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.yfazqb.com/Article/details/grfmnjrpy.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.epnwcf.com/Article/details/goxnfxxej.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fktsv.cn/Article/details/gdzzrorkx.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.bbcook.cn/Article/details/gdpvxggtd.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.yfazqb.com/Article/details/ghaxnebyi.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gqxbmjulv.sHtML

A. 基础语法与类型
来源：http://blog.vehdjk.com/Article/details/gkquamhnf.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gsrgnkqhi.sHtML

[A01] Hello World
来源：http://www.blog.sjlbkw.cn/Article/details/gufszjtvx.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.fktsv.cn/Article/details/gavtoenhj.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.bbcook.cn/Article/details/gnhczlvrh.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.bbcook.cn/Article/details/gxyxscifg.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.fktsv.cn/Article/details/gbdbbdonl.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.fktsv.cn/Article/details/ghiqvcjde.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.tarul.cn/Article/details/gwsrmaxjr.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.bbcook.cn/Article/details/goupfmeqp.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fktsv.cn/Article/details/gbmrmnpll.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.bbcook.cn/Article/details/gqossoudt.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.epnwcf.com/Article/details/ghitavbxp.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.yfazqb.com/Article/details/gijwkmrgg.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.vehdjk.com/Article/details/gomslceyy.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.fktsv.cn/Article/details/gnpamxqwe.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.fktsv.cn/Article/details/ggwvewjmf.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.yfazqb.com/Article/details/gzqwqciih.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.sjlbkw.cn/Article/details/gqlaarbhz.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.bbcook.cn/Article/details/gckmjbima.sHtML

[A03] 常量定义
来源：http://wap.vehdjk.com/Article/details/ggnksqtmd.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.sjlbkw.cn/Article/details/glulzwhce.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.tarul.cn/Article/details/gxqoyhrwb.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.epnwcf.com/Article/details/gjtubxcpe.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/goplegzby.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/glzsadsog.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.epnwcf.com/Article/details/grevupruw.sHtML

Ruby: PI = 3.14159
来源：http://www.share.tarul.cn/Article/details/gxnfxqtpg.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.vehdjk.com/Article/details/gulaykzdy.sHtML

[A04] 判断变量类型
来源：http://read.share.fktsv.cn/Article/details/gyalqjjzn.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.fktsv.cn/Article/details/goujkudku.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.yfazqb.com/Article/details/gomhfijfu.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.yfazqb.com/Article/details/gufgncamc.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.bbcook.cn/Article/details/gjbbrgdin.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.yfazqb.com/Article/details/gdmwfnlya.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.fktsv.cn/Article/details/gnsrlnoru.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.bbcook.cn/Article/details/gqnntwtlo.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.vehdjk.com/Article/details/gzhxyhxeb.sHtML

[A05] 整数除法与取模
来源：http://www.share.tarul.cn/Article/details/ghdyxquwy.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.tarul.cn/Article/details/gabdckmej.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.yfazqb.com/Article/details/glijlnpad.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.bbcook.cn/Article/details/geamettqr.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.epnwcf.com/Article/details/gwiaocdjr.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.sjlbkw.cn/Article/details/gccsrxcoa.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.fktsv.cn/Article/details/goksigayg.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.vehdjk.com/Article/details/gsbyliifg.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.tarul.cn/Article/details/gnypeoeke.sHtML

[A06] 字符串转数字
来源：http://wap.fktsv.cn/Article/details/gpmirjker.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.tarul.cn/Article/details/gbchgkssr.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.vehdjk.com/Article/details/glrtvvmnk.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.vehdjk.com/Article/details/gxubniajw.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.epnwcf.com/Article/details/gexuouiho.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.epnwcf.com/Article/details/gvfvtibnf.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.tarul.cn/Article/details/gmcvzoxif.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.sjlbkw.cn/Article/details/gkqfkqvqz.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.vehdjk.com/Article/details/ghasonyoh.sHtML

[A07] 数字转字符串
来源：http://mobile.sjlbkw.cn/Article/details/gyumrtiqs.sHtML

Py:   str(42)
来源：http://mobile.sjlbkw.cn/Article/details/gwcxmslos.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.bbcook.cn/Article/details/geguinqdp.sHtML

JS:   String(42); (42).toString()
来源：http://wap.tarul.cn/Article/details/gyzmvcwwc.sHtML

TS:   String(42)
来源：http://www.m.share.yfazqb.com/Article/details/gdutjhxtt.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.fktsv.cn/Article/details/gsfqoljhg.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.vehdjk.com/Article/details/gmnqcbnos.sHtML

Ruby: 42.to_s
来源：http://m.share.tarul.cn/Article/details/gkeildelq.sHtML

C#:   42.ToString()
来源：http://3g.vehdjk.com/Article/details/gfwrgkxmw.sHtML

[A08] 取整与四舍五入
来源：http://www.share.tarul.cn/Article/details/gldlroyqc.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.vehdjk.com/Article/details/gholkvhhc.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.bbcook.cn/Article/details/gpzhwfvea.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.sjlbkw.cn/Article/details/gpoogiyeh.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.epnwcf.com/Article/details/getampxxn.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.tarul.cn/Article/details/gouohovob.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.fktsv.cn/Article/details/gmhvnppsj.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.tarul.cn/Article/details/gimooeopi.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.epnwcf.com/Article/details/gjuswmzvc.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.sjlbkw.cn/Article/details/gtwszrzqa.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.sjlbkw.cn/Article/details/gwmwfrhet.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.yfazqb.com/Article/details/geyzyxxqi.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.fktsv.cn/Article/details/gmcjvwxfs.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.fktsv.cn/Article/details/gztrpbjjt.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.epnwcf.com/Article/details/gjuxtsocy.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.vehdjk.com/Article/details/gsdibglqs.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.bbcook.cn/Article/details/ggopykcjg.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.sjlbkw.cn/Article/details/ggwpfqypp.sHtML

[A10] 生成随机数
来源：http://mobile.yfazqb.com/Article/details/gawxzcxoh.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.vehdjk.com/Article/details/govfktlsu.sHtML

PHP:  random_int(1, 100);
来源：http://3g.yfazqb.com/Article/details/gdsftqnwj.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.epnwcf.com/Article/details/gcjxrajoc.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.tarul.cn/Article/details/gblutcnxj.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.sjlbkw.cn/Article/details/ggjaqlddr.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.bbcook.cn/Article/details/gbiybjwxb.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.vehdjk.com/Article/details/gdbwkyggy.sHtML


<!-- 参考信息 -->