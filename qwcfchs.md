代发 wailian999

[U61] PHP：正则
来源：http://wap.sjlbkw.cn/Article/details/grfccskbg.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.tarul.cn/Article/details/gnnycomst.sHtML

[U62] PHP：日期对象
来源：http://blog.sjlbkw.cn/Article/details/ggqgyawkp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.epnwcf.com/Article/details/gjnnyrbhe.sHtML

[U63] PHP：文件读写
来源：http://blog.yfazqb.com/Article/details/ggtkxrrtg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.epnwcf.com/Article/details/gnabqitlp.sHtML

[U64] PHP：目录遍历
来源：http://3g.sjlbkw.cn/Article/details/goenklqce.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.tarul.cn/Article/details/guagismrl.sHtML

[U65] PHP：会话
来源：http://baike.vehdjk.com/Article/details/gtekfkitf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.yfazqb.com/Article/details/gllwhusbt.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.bbcook.cn/Article/details/gjjebllys.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fktsv.cn/Article/details/gjpdvfjxr.sHtML

[U67] PHP：处理文件上传
来源：http://baike.sjlbkw.cn/Article/details/golyzyicj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.bbcook.cn/Article/details/gafuawbjc.sHtML

[U68] PHP：PDO 连接
来源：http://3g.yfazqb.com/Article/details/gnnlcoizc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.tarul.cn/Article/details/gooapidbp.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.bbcook.cn/Article/details/guaskuihu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.yfazqb.com/Article/details/goqluxtoz.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.yfazqb.com/Article/details/gaeskxcsl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.bbcook.cn/Article/details/gmhoqjpgl.sHtML

[U71] PHP：抛出异常
来源：http://read.share.epnwcf.com/Article/details/gfwmxkjgd.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.bbcook.cn/Article/details/gcvcjhttt.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.bbcook.cn/Article/details/gvpvfboqi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.vehdjk.com/Article/details/gqrapxmmf.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.vehdjk.com/Article/details/guokxnmww.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.tarul.cn/Article/details/gfqmllyoe.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.sjlbkw.cn/Article/details/gddqlbhkg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.epnwcf.com/Article/details/gvoiakvbq.sHtML

[U75] PHP：依赖注入
来源：http://blog.bbcook.cn/Article/details/getqioohp.sHtML

composer require psr/container
来源：http://3g.fktsv.cn/Article/details/geftrihsb.sHtML

[U76] PHP：简单路由
来源：http://wap.tarul.cn/Article/details/gdrelmfau.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.yfazqb.com/Article/details/gcyvbkqip.sHtML

[U77] PHP：模板渲染
来源：http://blog.epnwcf.com/Article/details/gdkejtdyd.sHtML

composer require twig/twig
来源：http://3g.vehdjk.com/Article/details/ggzmsegkl.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.tarul.cn/Article/details/gsexnkjcb.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.bbcook.cn/Article/details/gnccmxaia.sHtML

[U79] PHP：静态分析
来源：http://www.blog.bbcook.cn/Article/details/gtzjxqlrw.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.tarul.cn/Article/details/gqogegckq.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.yfazqb.com/Article/details/gajelxtht.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.tarul.cn/Article/details/gmxuyshfd.sHtML

[U81] JS：初始化项目
来源：http://mobile.sjlbkw.cn/Article/details/goxknelsu.sHtML

npm init -y;  npm i express
来源：http://www.blog.sjlbkw.cn/Article/details/gtklnvnua.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.sjlbkw.cn/Article/details/glixdfbtk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.bbcook.cn/Article/details/gzupbpaod.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fktsv.cn/Article/details/guhirsoqb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.vehdjk.com/Article/details/gxmwgwcgh.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.vehdjk.com/Article/details/gerzdikcg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.yfazqb.com/Article/details/gjffwqbka.sHtML

[U85] JS：可选链
来源：http://wap.bbcook.cn/Article/details/gtlziomxw.sHtML

a?.b?.c
来源：http://baike.bbcook.cn/Article/details/gffefvjci.sHtML

[U86] JS：空值合并
来源：http://read.share.fktsv.cn/Article/details/gukvpfcqj.sHtML

a ?? b
来源：http://www.blog.fktsv.cn/Article/details/gcwqosdee.sHtML

[U87] JS：解构默认值
来源：http://blog.sjlbkw.cn/Article/details/gucbvuqhs.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.bbcook.cn/Article/details/gdhrnxixq.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.yfazqb.com/Article/details/ggfspszst.sHtML

{ ...a, ...b }
来源：http://baike.epnwcf.com/Article/details/giwejdoyc.sHtML

[U89] JS：数组去重
来源：http://baike.tarul.cn/Article/details/gbanfgdnf.sHtML

[...new Set(arr)]
来源：http://mobile.epnwcf.com/Article/details/gynwktoup.sHtML

[U90] JS：数字数组排序
来源：http://3g.yfazqb.com/Article/details/gqfphczbs.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fktsv.cn/Article/details/gxqifhaef.sHtML

[U91] JS：对象键值遍历
来源：http://baike.sjlbkw.cn/Article/details/gjqwecyfp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.epnwcf.com/Article/details/gfzbnwpzx.sHtML

[U92] JS：深拷贝
来源：http://3g.bbcook.cn/Article/details/geuvmpkph.sHtML

structuredClone(obj)
来源：http://wap.epnwcf.com/Article/details/gfifudfxe.sHtML

[U93] JS：模板字符串
来源：http://www.blog.epnwcf.com/Article/details/gjshbjuvj.sHtML

`共 ${n} 条`
来源：http://www.m.share.epnwcf.com/Article/details/gufojhyms.sHtML

[U94] JS：箭头函数
来源：http://www.blog.sjlbkw.cn/Article/details/gmcbpsckf.sHtML

const double = x => x * 2;
来源：http://mobile.vehdjk.com/Article/details/gtudjaqhk.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fktsv.cn/Article/details/ghhebammo.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.bbcook.cn/Article/details/ghczlodfu.sHtML

[U96] JS：async/await 与异常
来源：http://wap.yfazqb.com/Article/details/gqxqagwso.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fktsv.cn/Article/details/gfjfcdiyg.sHtML

[U97] JS：并发请求
来源：http://www.blog.bbcook.cn/Article/details/giwzkpvpr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.tarul.cn/Article/details/glrxjqtrr.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.tarul.cn/Article/details/gitoltglj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fktsv.cn/Article/details/gnigvyuqo.sHtML

[U99] JS：事件监听
来源：http://mobile.tarul.cn/Article/details/gdwucmfbi.sHtML

el.addEventListener("click", e => {})
来源：http://blog.yfazqb.com/Article/details/gfpyiplpo.sHtML

[U100] JS：DOM 查询
来源：http://baike.sjlbkw.cn/Article/details/gyxqpxnan.sHtML

document.querySelector(".item")
来源：http://wap.vehdjk.com/Article/details/ghucgtyns.sHtML

[U101] JS：classList 操作
来源：http://m.share.fktsv.cn/Article/details/ggmkdicyq.sHtML

el.classList.toggle("active")
来源：http://m.share.vehdjk.com/Article/details/glvfliyqb.sHtML

[U102] JS：本地存储
来源：http://www.m.share.bbcook.cn/Article/details/gbtyyvzut.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.tarul.cn/Article/details/ggjukvkck.sHtML

[U103] JS：定时器
来源：http://baike.sjlbkw.cn/Article/details/gschjqvkw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fktsv.cn/Article/details/gnldswfsf.sHtML

[U104] JS：防抖
来源：http://read.share.epnwcf.com/Article/details/gvfsqxpsc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.epnwcf.com/Article/details/gjzoahwtm.sHtML

[U105] JS：节流
来源：http://blog.epnwcf.com/Article/details/gqaxvfpyk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.vehdjk.com/Article/details/gwscfaeni.sHtML

[U106] JS：日期格式化
来源：http://baike.bbcook.cn/Article/details/gxvlgfwkg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.vehdjk.com/Article/details/gtrunspyc.sHtML

[U107] JS：数字千分位
来源：http://m.share.yfazqb.com/Article/details/gffgduvan.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.sjlbkw.cn/Article/details/gnrjodgjv.sHtML

[U108] JS：随机整数
来源：http://mobile.fktsv.cn/Article/details/gyqclrokx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.bbcook.cn/Article/details/gcsfehedr.sHtML

[U109] JS：数组分组
来源：http://wap.bbcook.cn/Article/details/ghwqdogus.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.sjlbkw.cn/Article/details/goxmcmajv.sHtML

[U110] JS：数组分块
来源：http://m.share.yfazqb.com/Article/details/gvxcckqxy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.bbcook.cn/Article/details/gejxoaiun.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fktsv.cn/Article/details/gnwolzjob.sHtML

new Map(Object.entries(obj))
来源：http://3g.vehdjk.com/Article/details/gomgqaahw.sHtML

[U112] JS：字符串补位
来源：http://m.share.tarul.cn/Article/details/geshruqey.sHtML

"7".padStart(3, "0")
来源：http://blog.tarul.cn/Article/details/grwwumwwd.sHtML

[U113] JS：正则替换全部
来源：http://m.share.epnwcf.com/Article/details/gmosuurda.sHtML

s.replaceAll("a", "b")
来源：http://blog.vehdjk.com/Article/details/gwsdeeblr.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.epnwcf.com/Article/details/ghjxcxdxb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.sjlbkw.cn/Article/details/gdgrhtduq.sHtML

[U115] JS：生成 UUID
来源：http://baike.bbcook.cn/Article/details/gyggwdnww.sHtML

crypto.randomUUID()
来源：http://mobile.yfazqb.com/Article/details/grxptxjwf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.bbcook.cn/Article/details/gcxmqqriv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.epnwcf.com/Article/details/gvgwifkos.sHtML

[U117] JS：单元测试
来源：http://read.share.bbcook.cn/Article/details/gjubwkjnm.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.bbcook.cn/Article/details/gtrvhntsw.sHtML

[U118] JS：开发服务器
来源：http://baike.bbcook.cn/Article/details/gzlgncevg.sHtML

npm i -D vite;  npx vite
来源：http://read.share.tarul.cn/Article/details/gfcwcumim.sHtML

[U119] JS：生产构建
来源：http://www.m.share.sjlbkw.cn/Article/details/giqznqehz.sHtML

npx vite build
来源：http://wap.tarul.cn/Article/details/gydlihlij.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.tarul.cn/Article/details/ghjgszymi.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.epnwcf.com/Article/details/gvycszcku.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/ggsmpsjso.sHtML

统计汇总
来源：http://www.m.share.fktsv.cn/Article/details/gyucuiowl.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gwqfqpvwv.sHtML

按语言统计（条）：
来源：http://3g.bbcook.cn/Article/details/gsitsnrmw.sHtML

Python ......... 252
来源：http://3g.vehdjk.com/Article/details/gbhhblyex.sHtML

PHP ............ 252
来源：http://mobile.sjlbkw.cn/Article/details/ggnhpsxtv.sHtML

JavaScript ..... 252
来源：http://www.blog.fktsv.cn/Article/details/ggrwfofgk.sHtML

TypeScript ..... 212
来源：http://mobile.vehdjk.com/Article/details/gusmephtg.sHtML

Java ........... 212
来源：http://www.blog.sjlbkw.cn/Article/details/gzmezlpfo.sHtML

Go ............. 212
来源：http://read.share.fktsv.cn/Article/details/gzrekacjb.sHtML

Ruby ........... 212
来源：http://www.blog.sjlbkw.cn/Article/details/gorjwnsgn.sHtML

C# ............. 212
来源：http://m.share.tarul.cn/Article/details/gpcrkhgoj.sHtML

C .............. 30
来源：http://www.blog.tarul.cn/Article/details/gmrjkrbvc.sHtML

C++ ............ 30
来源：http://3g.vehdjk.com/Article/details/gjzusasem.sHtML

SQL ............ 90
来源：http://mobile.epnwcf.com/Article/details/gnsburxix.sHtML

Bash ........... 80
来源：http://blog.sjlbkw.cn/Article/details/goggjsghh.sHtML

Kotlin ......... 15
来源：http://wap.vehdjk.com/Article/details/ghgplogxo.sHtML

Swift .......... 15
来源：http://wap.fktsv.cn/Article/details/gmhrnzpuj.sHtML

Lua ............ 10
来源：http://3g.tarul.cn/Article/details/gfszmazrk.sHtML

Perl ........... 10
来源：http://3g.yfazqb.com/Article/details/gdwvsfwjr.sHtML

Scala .......... 10
来源：http://3g.vehdjk.com/Article/details/gcecmrubp.sHtML

------------------------------------
来源：http://baike.yfazqb.com/Article/details/goontsezg.sHtML

合计 ........... 2106 条
来源：http://www.m.share.sjlbkw.cn/Article/details/gajqthnby.sHtML

按章节统计：
来源：http://www.blog.sjlbkw.cn/Article/details/gcnleslze.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.epnwcf.com/Article/details/gncvhcuur.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.vehdjk.com/Article/details/gcogtazfz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.yfazqb.com/Article/details/gxjdedxcj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.bbcook.cn/Article/details/gwiqjskri.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.sjlbkw.cn/Article/details/giasruyyd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.sjlbkw.cn/Article/details/ggggjssoy.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.bbcook.cn/Article/details/gvypwizny.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.tarul.cn/Article/details/gxqdvkhdb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.vehdjk.com/Article/details/gzborrmwz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.vehdjk.com/Article/details/gnbjpgahh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.epnwcf.com/Article/details/givxjtxax.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fktsv.cn/Article/details/gdpmhblgh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.vehdjk.com/Article/details/ggbuynytp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.vehdjk.com/Article/details/gfcxysgkk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.tarul.cn/Article/details/gyalmvvuv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fktsv.cn/Article/details/gysbfnisc.sHtML

Q SQL 专题                              90
来源：http://mobile.vehdjk.com/Article/details/gpnqrwpwj.sHtML

R Bash 专题                             80
来源：http://3g.yfazqb.com/Article/details/grxolghaf.sHtML

S C / C++ 专题                          60
来源：http://mobile.bbcook.cn/Article/details/gbnajhand.sHtML

T 其他语言补充                          60
来源：http://3g.sjlbkw.cn/Article/details/gozmbpnwb.sHtML

U 高频实用片段                         120
来源：http://www.share.epnwcf.com/Article/details/gcmyrgztm.sHtML

------------------------------------
来源：http://read.share.bbcook.cn/Article/details/gleyyjbkm.sHtML

合计                                  2106 条
来源：http://www.blog.yfazqb.com/Article/details/gmhzqaxwc.sHtML

--------------------------------------------------------------------------------
来源：http://3g.yfazqb.com/Article/details/gsvhjwiac.sHtML

使用提醒
来源：http://wap.bbcook.cn/Article/details/gfgoxmusz.sHtML

--------------------------------------------------------------------------------
来源：http://blog.sjlbkw.cn/Article/details/gzadmqrcp.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.yfazqb.com/Article/details/gaqhsptqo.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fktsv.cn/Article/details/gbfkdezzr.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.yfazqb.com/Article/details/gnpxcrwnz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.bbcook.cn/Article/details/ghsjceyed.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.vehdjk.com/Article/details/guozduicp.sHtML

—— 文件结束 ——
来源：http://read.share.tarul.cn/Article/details/gzhejhqqa.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gnhkbuxzk.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fktsv.cn/Article/details/gvexmryfm.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.sjlbkw.cn/Article/details/gsefojalo.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gobpazyzr.sHtML

【收录内容】
来源：http://www.m.share.bbcook.cn/Article/details/gnajhlkeo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.yfazqb.com/Article/details/gcklifbzd.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fktsv.cn/Article/details/gkgtgdcoq.sHtML

SQL · Bash · C · C++
来源：http://www.share.fktsv.cn/Article/details/gzsqtdlhf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.tarul.cn/Article/details/gnglelgxg.sHtML

【使用说明】
来源：http://baike.epnwcf.com/Article/details/ggtjrvtvp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.sjlbkw.cn/Article/details/gkjigvwmx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.yfazqb.com/Article/details/gejrnkzgh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.bbcook.cn/Article/details/gkyuackqc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.tarul.cn/Article/details/gjvzaelkq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.bbcook.cn/Article/details/gqrdocibp.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.yfazqb.com/Article/details/ggldadfrk.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.fktsv.cn/Article/details/gwjfvsfzu.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.vehdjk.com/Article/details/glychxgps.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.epnwcf.com/Article/details/gwbwwtdsl.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.sjlbkw.cn/Article/details/gcigtzrzn.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.epnwcf.com/Article/details/goukgqaek.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.epnwcf.com/Article/details/gdkyvdwht.sHtML

【文件统计】
来源：http://m.share.epnwcf.com/Article/details/gstlqlfni.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.tarul.cn/Article/details/gkbxircvy.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.epnwcf.com/Article/details/gstbhribn.sHtML

目  录
来源：http://3g.epnwcf.com/Article/details/gqdfxafqg.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.epnwcf.com/Article/details/gqsocamwz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.tarul.cn/Article/details/geabdvbuw.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.vehdjk.com/Article/details/gjuhcecfa.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.epnwcf.com/Article/details/gmcavpvqx.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.yfazqb.com/Article/details/grfsxondz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.vehdjk.com/Article/details/gblnqjato.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.bbcook.cn/Article/details/gkultufcb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.tarul.cn/Article/details/glmerempk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.vehdjk.com/Article/details/giohwtars.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.epnwcf.com/Article/details/gqshbqtyr.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.sjlbkw.cn/Article/details/gpbqfoobo.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.sjlbkw.cn/Article/details/ggzicihye.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.bbcook.cn/Article/details/grgxkmzxt.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.epnwcf.com/Article/details/gklnnssrs.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.bbcook.cn/Article/details/gtfylzbun.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.sjlbkw.cn/Article/details/gtkddilwf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.vehdjk.com/Article/details/gmysciruf.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.epnwcf.com/Article/details/gazxchgim.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.sjlbkw.cn/Article/details/gsmwjknrj.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.vehdjk.com/Article/details/gtdzfqddg.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.bbcook.cn/Article/details/gnzkzkrjp.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.yfazqb.com/Article/details/gntojzgsb.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/godmnnfnl.sHtML

A. 基础语法与类型
来源：http://www.m.share.yfazqb.com/Article/details/gjmmuuhiv.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/glbmcdszr.sHtML

[A01] Hello World
来源：http://baike.epnwcf.com/Article/details/gdxliryjt.sHtML

Py:   print("Hello, World!")
来源：http://read.share.fktsv.cn/Article/details/giihlkakk.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.yfazqb.com/Article/details/gtgpfiwnc.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.tarul.cn/Article/details/gpmcphfzu.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.tarul.cn/Article/details/gqlftppry.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.vehdjk.com/Article/details/glxjteptm.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.sjlbkw.cn/Article/details/gmurnpgym.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.sjlbkw.cn/Article/details/gepizyvzc.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.vehdjk.com/Article/details/gxbpgwohn.sHtML

[A02] 变量声明与赋值
来源：http://blog.sjlbkw.cn/Article/details/gzcagfnre.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.vehdjk.com/Article/details/gsclmctpe.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.bbcook.cn/Article/details/glfhbsgip.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.tarul.cn/Article/details/gkgejcusj.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.fktsv.cn/Article/details/gdeodkmlh.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.sjlbkw.cn/Article/details/guxnfvdtx.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.bbcook.cn/Article/details/gzwkspvsl.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fktsv.cn/Article/details/gugokcnsl.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.yfazqb.com/Article/details/galwlmkqs.sHtML

[A03] 常量定义
来源：http://3g.bbcook.cn/Article/details/grbuylhac.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.sjlbkw.cn/Article/details/gnhijebgy.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.yfazqb.com/Article/details/gyaurzhtq.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fktsv.cn/Article/details/gnddmaoty.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.fktsv.cn/Article/details/ggdrnsppc.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gtahakuft.sHtML

Go:   const PI = 3.14159
来源：http://m.share.sjlbkw.cn/Article/details/gjlfiphrw.sHtML

Ruby: PI = 3.14159
来源：http://wap.tarul.cn/Article/details/gywjdevus.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.epnwcf.com/Article/details/gkuwpqbau.sHtML

[A04] 判断变量类型
来源：http://baike.epnwcf.com/Article/details/gzzwcoimk.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.tarul.cn/Article/details/gjlcbgcoc.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.tarul.cn/Article/details/grkgzzpie.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.sjlbkw.cn/Article/details/glxyosczp.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.tarul.cn/Article/details/gilruhchq.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.yfazqb.com/Article/details/goahwbvoi.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.sjlbkw.cn/Article/details/gqrrteocv.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzxvjtiet.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.epnwcf.com/Article/details/gguiygion.sHtML

[A05] 整数除法与取模
来源：http://baike.yfazqb.com/Article/details/guompvpqv.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.epnwcf.com/Article/details/gzjumagke.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.epnwcf.com/Article/details/gknxubnli.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.bbcook.cn/Article/details/gmkstuaxd.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.tarul.cn/Article/details/gwgoimowi.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.sjlbkw.cn/Article/details/gnuytygmq.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.yfazqb.com/Article/details/glhrrbkuo.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.tarul.cn/Article/details/giphmkbpz.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.bbcook.cn/Article/details/gshrmjdbg.sHtML

[A06] 字符串转数字
来源：http://mobile.yfazqb.com/Article/details/glzyxmsnh.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.epnwcf.com/Article/details/ghhvmihmp.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.vehdjk.com/Article/details/gzibmxwcw.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.bbcook.cn/Article/details/gvkwpqsjx.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.yfazqb.com/Article/details/gdojsqjzs.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.bbcook.cn/Article/details/gfilameay.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.tarul.cn/Article/details/gcfbioifh.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.sjlbkw.cn/Article/details/gckafgwbp.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.sjlbkw.cn/Article/details/grveesyia.sHtML

[A07] 数字转字符串
来源：http://www.share.vehdjk.com/Article/details/gedbppjmw.sHtML

Py:   str(42)
来源：http://read.share.tarul.cn/Article/details/gegrvmeoc.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.vehdjk.com/Article/details/ggcnlfopg.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.vehdjk.com/Article/details/geerfztdu.sHtML

TS:   String(42)
来源：http://read.share.fktsv.cn/Article/details/gtpngeibp.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.sjlbkw.cn/Article/details/gfihfywwo.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.bbcook.cn/Article/details/gmvnluvtl.sHtML

Ruby: 42.to_s
来源：http://www.blog.epnwcf.com/Article/details/geosjjgjr.sHtML

C#:   42.ToString()
来源：http://baike.bbcook.cn/Article/details/gtqsdacpm.sHtML

[A08] 取整与四舍五入
来源：http://read.share.vehdjk.com/Article/details/gabksrnsz.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.tarul.cn/Article/details/gzytbjqmb.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.tarul.cn/Article/details/gxtbtwcmn.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.vehdjk.com/Article/details/gwozjekpl.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.vehdjk.com/Article/details/gotodjhkm.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.sjlbkw.cn/Article/details/gywunjmkd.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.bbcook.cn/Article/details/gtosebhes.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.fktsv.cn/Article/details/gznehernj.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.vehdjk.com/Article/details/gwgshltvr.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.fktsv.cn/Article/details/gmllppkyx.sHtML


<!-- 参考信息 -->