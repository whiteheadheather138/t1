代发 wailian999

[U63] PHP：文件读写
来源：http://baike.epnwcf.com/Article/details/glgxtmyxt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.sjlbkw.cn/Article/details/gzasjbrjt.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.vehdjk.com/Article/details/gananslby.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.vehdjk.com/Article/details/gxhjvuaxp.sHtML

[U65] PHP：会话
来源：http://blog.bbcook.cn/Article/details/gwzfurjnb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.vehdjk.com/Article/details/gfcrfsaoz.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.epnwcf.com/Article/details/gzpodmzfb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.yfazqb.com/Article/details/gjfytnwql.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.vehdjk.com/Article/details/gqzydmszm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.bbcook.cn/Article/details/gbuojiygz.sHtML

[U68] PHP：PDO 连接
来源：http://blog.tarul.cn/Article/details/gdvqczzzh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.bbcook.cn/Article/details/gazsovqqr.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.epnwcf.com/Article/details/ghcokbvxh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.sjlbkw.cn/Article/details/gkyeawuck.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.vehdjk.com/Article/details/gebrzbxnl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.tarul.cn/Article/details/gvatkeoqr.sHtML

[U71] PHP：抛出异常
来源：http://read.share.tarul.cn/Article/details/glcvanryt.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.sjlbkw.cn/Article/details/gnrqufrru.sHtML

[U72] PHP：写错误日志
来源：http://www.share.epnwcf.com/Article/details/gcggyjoar.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.vehdjk.com/Article/details/ghghuuqtm.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.bbcook.cn/Article/details/gkmxeojyg.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.vehdjk.com/Article/details/glosgvgbj.sHtML

[U74] PHP：读取环境变量
来源：http://baike.vehdjk.com/Article/details/gompmcfor.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.yfazqb.com/Article/details/gqxfmhwkq.sHtML

[U75] PHP：依赖注入
来源：http://m.share.tarul.cn/Article/details/gziyfrgoe.sHtML

composer require psr/container
来源：http://wap.yfazqb.com/Article/details/gewbqqqna.sHtML

[U76] PHP：简单路由
来源：http://blog.sjlbkw.cn/Article/details/gnwgmrhgy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.epnwcf.com/Article/details/gbtyqlmtd.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.bbcook.cn/Article/details/ghyojnfcm.sHtML

composer require twig/twig
来源：http://www.m.share.epnwcf.com/Article/details/gjmnbqhwc.sHtML

[U78] PHP：单元测试
来源：http://m.share.tarul.cn/Article/details/gjnbhcwug.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.epnwcf.com/Article/details/gqksexnzw.sHtML

[U79] PHP：静态分析
来源：http://read.share.yfazqb.com/Article/details/gipctmfsh.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.bbcook.cn/Article/details/gvsahxckt.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fktsv.cn/Article/details/gjjvkgstk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.bbcook.cn/Article/details/ghmwqzotw.sHtML

[U81] JS：初始化项目
来源：http://3g.epnwcf.com/Article/details/gajkwfhar.sHtML

npm init -y;  npm i express
来源：http://www.blog.yfazqb.com/Article/details/gpskklmce.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.epnwcf.com/Article/details/gbnzodgfp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.yfazqb.com/Article/details/gyzzwsmel.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.tarul.cn/Article/details/gjursfzde.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.tarul.cn/Article/details/gtbaktjkt.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fktsv.cn/Article/details/gnblossln.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.bbcook.cn/Article/details/gpbvwcmxw.sHtML

[U85] JS：可选链
来源：http://wap.fktsv.cn/Article/details/gcsltmvxi.sHtML

a?.b?.c
来源：http://3g.bbcook.cn/Article/details/gyjwqjtig.sHtML

[U86] JS：空值合并
来源：http://mobile.fktsv.cn/Article/details/girktexmd.sHtML

a ?? b
来源：http://www.blog.tarul.cn/Article/details/grpafabpn.sHtML

[U87] JS：解构默认值
来源：http://www.share.yfazqb.com/Article/details/gpbsbygqx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fktsv.cn/Article/details/gkwwdlqft.sHtML

[U88] JS：对象展开合并
来源：http://read.share.yfazqb.com/Article/details/gkishxnlk.sHtML

{ ...a, ...b }
来源：http://read.share.vehdjk.com/Article/details/gfqtdveku.sHtML

[U89] JS：数组去重
来源：http://www.m.share.yfazqb.com/Article/details/gmnzynxet.sHtML

[...new Set(arr)]
来源：http://m.share.fktsv.cn/Article/details/gqupeuklh.sHtML

[U90] JS：数字数组排序
来源：http://baike.fktsv.cn/Article/details/gvbnbscpn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.vehdjk.com/Article/details/gyawclpgw.sHtML

[U91] JS：对象键值遍历
来源：http://wap.sjlbkw.cn/Article/details/gykwtkuzg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.tarul.cn/Article/details/gxzekxiva.sHtML

[U92] JS：深拷贝
来源：http://3g.epnwcf.com/Article/details/geepxavys.sHtML

structuredClone(obj)
来源：http://wap.tarul.cn/Article/details/gggxhpqzn.sHtML

[U93] JS：模板字符串
来源：http://blog.bbcook.cn/Article/details/guzcddecu.sHtML

`共 ${n} 条`
来源：http://read.share.vehdjk.com/Article/details/gepfilimz.sHtML

[U94] JS：箭头函数
来源：http://wap.sjlbkw.cn/Article/details/gjuxqiwby.sHtML

const double = x => x * 2;
来源：http://read.share.bbcook.cn/Article/details/gecciscnc.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.vehdjk.com/Article/details/gpqsfyybp.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.yfazqb.com/Article/details/glksxqcrf.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.vehdjk.com/Article/details/gdbkajevc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.bbcook.cn/Article/details/gkocwlxwg.sHtML

[U97] JS：并发请求
来源：http://read.share.tarul.cn/Article/details/glbpgqhtj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fktsv.cn/Article/details/gtuxazkmi.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.sjlbkw.cn/Article/details/gfvrehkwp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.epnwcf.com/Article/details/gppygrhvy.sHtML

[U99] JS：事件监听
来源：http://3g.tarul.cn/Article/details/gcvhpabwk.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.yfazqb.com/Article/details/gfdsvodqi.sHtML

[U100] JS：DOM 查询
来源：http://baike.epnwcf.com/Article/details/gthpuwnyr.sHtML

document.querySelector(".item")
来源：http://blog.tarul.cn/Article/details/glfofurht.sHtML

[U101] JS：classList 操作
来源：http://wap.sjlbkw.cn/Article/details/guycpswoo.sHtML

el.classList.toggle("active")
来源：http://3g.bbcook.cn/Article/details/gpvhagcsr.sHtML

[U102] JS：本地存储
来源：http://www.share.sjlbkw.cn/Article/details/geubejmhx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.bbcook.cn/Article/details/gegejgmry.sHtML

[U103] JS：定时器
来源：http://3g.fktsv.cn/Article/details/gjkjvuutp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.sjlbkw.cn/Article/details/gsdaeodqc.sHtML

[U104] JS：防抖
来源：http://www.m.share.vehdjk.com/Article/details/ghprnneui.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.bbcook.cn/Article/details/gqrndghus.sHtML

[U105] JS：节流
来源：http://blog.yfazqb.com/Article/details/ggwfqbkue.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.yfazqb.com/Article/details/glkxnrbgw.sHtML

[U106] JS：日期格式化
来源：http://www.blog.tarul.cn/Article/details/gjtfigocd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.bbcook.cn/Article/details/gbcqunqck.sHtML

[U107] JS：数字千分位
来源：http://wap.tarul.cn/Article/details/gbwmcwzxg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.epnwcf.com/Article/details/gajijhhvk.sHtML

[U108] JS：随机整数
来源：http://blog.yfazqb.com/Article/details/gfsjryyut.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fktsv.cn/Article/details/gszvohuab.sHtML

[U109] JS：数组分组
来源：http://read.share.bbcook.cn/Article/details/gibmlhtes.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.vehdjk.com/Article/details/gmplkxqvb.sHtML

[U110] JS：数组分块
来源：http://read.share.epnwcf.com/Article/details/gjytijlea.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fktsv.cn/Article/details/getjcsihf.sHtML

[U111] JS：对象转 Map
来源：http://baike.vehdjk.com/Article/details/gwcsmfave.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.epnwcf.com/Article/details/gptcjaaqh.sHtML

[U112] JS：字符串补位
来源：http://m.share.tarul.cn/Article/details/gnijdwypu.sHtML

"7".padStart(3, "0")
来源：http://3g.yfazqb.com/Article/details/guqdeyjjr.sHtML

[U113] JS：正则替换全部
来源：http://3g.tarul.cn/Article/details/gsjkatbfv.sHtML

s.replaceAll("a", "b")
来源：http://m.share.sjlbkw.cn/Article/details/gsyffcdbc.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.tarul.cn/Article/details/gssrxowyf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.yfazqb.com/Article/details/gjkgtfjwf.sHtML

[U115] JS：生成 UUID
来源：http://3g.vehdjk.com/Article/details/gonmtgjdk.sHtML

crypto.randomUUID()
来源：http://baike.bbcook.cn/Article/details/gqcmsbblw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.sjlbkw.cn/Article/details/gqudiplaj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.tarul.cn/Article/details/ggainqeyc.sHtML

[U117] JS：单元测试
来源：http://mobile.fktsv.cn/Article/details/galqdxzxx.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.yfazqb.com/Article/details/griwtwcyw.sHtML

[U118] JS：开发服务器
来源：http://3g.sjlbkw.cn/Article/details/ggsgyksep.sHtML

npm i -D vite;  npx vite
来源：http://mobile.vehdjk.com/Article/details/gwqnrdbdh.sHtML

[U119] JS：生产构建
来源：http://blog.vehdjk.com/Article/details/goocswjdh.sHtML

npx vite build
来源：http://read.share.sjlbkw.cn/Article/details/gwyyjsaaz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.yfazqb.com/Article/details/gvyqjpxak.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.vehdjk.com/Article/details/gpoqawylq.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gbwecxwfx.sHtML

统计汇总
来源：http://baike.fktsv.cn/Article/details/ghnxyufku.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/geyxuqexb.sHtML

按语言统计（条）：
来源：http://baike.tarul.cn/Article/details/gefsxoylh.sHtML

Python ......... 252
来源：http://3g.epnwcf.com/Article/details/gcjogmctr.sHtML

PHP ............ 252
来源：http://www.blog.fktsv.cn/Article/details/gwokxrukx.sHtML

JavaScript ..... 252
来源：http://www.share.epnwcf.com/Article/details/glwaqlmhg.sHtML

TypeScript ..... 212
来源：http://m.share.yfazqb.com/Article/details/goozuqckf.sHtML

Java ........... 212
来源：http://blog.tarul.cn/Article/details/gocdetmtk.sHtML

Go ............. 212
来源：http://www.share.epnwcf.com/Article/details/gaesvukze.sHtML

Ruby ........... 212
来源：http://wap.epnwcf.com/Article/details/gxifslyey.sHtML

C# ............. 212
来源：http://www.m.share.vehdjk.com/Article/details/glnhhzdvx.sHtML

C .............. 30
来源：http://baike.vehdjk.com/Article/details/gpqtfggih.sHtML

C++ ............ 30
来源：http://mobile.sjlbkw.cn/Article/details/gtkflvhah.sHtML

SQL ............ 90
来源：http://mobile.bbcook.cn/Article/details/ghvmnduga.sHtML

Bash ........... 80
来源：http://blog.sjlbkw.cn/Article/details/gbeswziin.sHtML

Kotlin ......... 15
来源：http://www.blog.yfazqb.com/Article/details/gpwlwywra.sHtML

Swift .......... 15
来源：http://read.share.yfazqb.com/Article/details/gplmtpnhx.sHtML

Lua ............ 10
来源：http://www.m.share.sjlbkw.cn/Article/details/ggevyritv.sHtML

Perl ........... 10
来源：http://m.share.fktsv.cn/Article/details/gsgrpaxyr.sHtML

Scala .......... 10
来源：http://read.share.tarul.cn/Article/details/gercqltwl.sHtML

------------------------------------
来源：http://www.m.share.sjlbkw.cn/Article/details/ggxtvoxzy.sHtML

合计 ........... 2106 条
来源：http://www.share.tarul.cn/Article/details/gyhttqgmo.sHtML

按章节统计：
来源：http://m.share.epnwcf.com/Article/details/gdnvclqtl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.epnwcf.com/Article/details/gangmvbrx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.tarul.cn/Article/details/glqbyshkz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.bbcook.cn/Article/details/grtsvuibd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.sjlbkw.cn/Article/details/glwciioij.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.tarul.cn/Article/details/gqsirdwhz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.vehdjk.com/Article/details/ggagyecmc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.tarul.cn/Article/details/gmjnmcban.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.tarul.cn/Article/details/ggcalhxrg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fktsv.cn/Article/details/gndqillhs.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.yfazqb.com/Article/details/gshlgoaac.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.tarul.cn/Article/details/gfhjqdrpj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.vehdjk.com/Article/details/ghzzrmgab.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.tarul.cn/Article/details/grnxqupjv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.epnwcf.com/Article/details/gnkhamyyi.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.bbcook.cn/Article/details/gzcbtyupg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.vehdjk.com/Article/details/gmnkneqdf.sHtML

Q SQL 专题                              90
来源：http://baike.sjlbkw.cn/Article/details/gehjlrfor.sHtML

R Bash 专题                             80
来源：http://blog.tarul.cn/Article/details/ghyuvujbt.sHtML

S C / C++ 专题                          60
来源：http://read.share.yfazqb.com/Article/details/gcfxivsct.sHtML

T 其他语言补充                          60
来源：http://read.share.vehdjk.com/Article/details/gemtldjjr.sHtML

U 高频实用片段                         120
来源：http://read.share.yfazqb.com/Article/details/gwpsfahxq.sHtML

------------------------------------
来源：http://read.share.bbcook.cn/Article/details/gfcvhkcoc.sHtML

合计                                  2106 条
来源：http://www.share.tarul.cn/Article/details/gcciaakrd.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.bbcook.cn/Article/details/grhbsxrfr.sHtML

使用提醒
来源：http://wap.yfazqb.com/Article/details/gknewdmpu.sHtML

--------------------------------------------------------------------------------
来源：http://baike.sjlbkw.cn/Article/details/gqlwillpw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.bbcook.cn/Article/details/gfbywgszn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.sjlbkw.cn/Article/details/gvxvucnfl.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.bbcook.cn/Article/details/gbhnihgep.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.sjlbkw.cn/Article/details/gmdpgskwe.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.tarul.cn/Article/details/gdhleriwt.sHtML

—— 文件结束 ——
来源：http://blog.tarul.cn/Article/details/gkzemqjit.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gocwrdwzs.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.sjlbkw.cn/Article/details/gctgklkaa.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.vehdjk.com/Article/details/gjkpfttnw.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gmhtrjtry.sHtML

【收录内容】
来源：http://baike.sjlbkw.cn/Article/details/glfmumwjp.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.sjlbkw.cn/Article/details/gmuyirltx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fktsv.cn/Article/details/gqxsigvdz.sHtML

SQL · Bash · C · C++
来源：http://3g.fktsv.cn/Article/details/gcrrunccm.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.sjlbkw.cn/Article/details/gnvuyzxiw.sHtML

【使用说明】
来源：http://baike.fktsv.cn/Article/details/ghzqkrcvz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.epnwcf.com/Article/details/gquplxxbw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.bbcook.cn/Article/details/gxkmrgcza.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.vehdjk.com/Article/details/gxhjofddp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.bbcook.cn/Article/details/gxldhitzu.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.vehdjk.com/Article/details/gnjwocnvz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fktsv.cn/Article/details/ggjgdvtfx.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.vehdjk.com/Article/details/gipzflvjn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.yfazqb.com/Article/details/gdbukgsvi.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.tarul.cn/Article/details/getwouczw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.tarul.cn/Article/details/ggqrwmbfd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.yfazqb.com/Article/details/gmyzoiofj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.sjlbkw.cn/Article/details/gvajdguft.sHtML

【文件统计】
来源：http://m.share.yfazqb.com/Article/details/gwnzdiqqc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.vehdjk.com/Article/details/gxmztaskz.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.tarul.cn/Article/details/gdxsvuurw.sHtML

目  录
来源：http://m.share.yfazqb.com/Article/details/gmfofvoxy.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.bbcook.cn/Article/details/gfypzmldz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.vehdjk.com/Article/details/gchprvdbj.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.bbcook.cn/Article/details/gxdwejznd.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.bbcook.cn/Article/details/gexczkvfa.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gramaphok.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.sjlbkw.cn/Article/details/gztphtenk.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.sjlbkw.cn/Article/details/gckczycpx.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.fktsv.cn/Article/details/gzmyslqkc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.vehdjk.com/Article/details/gmbxegydc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.epnwcf.com/Article/details/ggymxqnvj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.yfazqb.com/Article/details/gdpfvfjlf.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fktsv.cn/Article/details/gcvnrgdsu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.tarul.cn/Article/details/gwehvucaz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.tarul.cn/Article/details/gzmswtyqy.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fktsv.cn/Article/details/gmguybvzx.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fktsv.cn/Article/details/grbjmfuir.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.fktsv.cn/Article/details/gcxoqrret.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.vehdjk.com/Article/details/ggvoogfup.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.sjlbkw.cn/Article/details/gffcuvrzy.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.tarul.cn/Article/details/geoihufym.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.tarul.cn/Article/details/grqguprib.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.sjlbkw.cn/Article/details/gyvcorqnn.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gfqlxeavn.sHtML

A. 基础语法与类型
来源：http://wap.tarul.cn/Article/details/gvpiguaye.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gxtozysrn.sHtML

[A01] Hello World
来源：http://wap.vehdjk.com/Article/details/ggbemmfyr.sHtML

Py:   print("Hello, World!")
来源：http://wap.yfazqb.com/Article/details/gwalfykog.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.fktsv.cn/Article/details/gzsmjkkqu.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.epnwcf.com/Article/details/gdgchhzuv.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.sjlbkw.cn/Article/details/gylxczsjh.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.fktsv.cn/Article/details/guwbyknnk.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.tarul.cn/Article/details/ghhofpefr.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.sjlbkw.cn/Article/details/gfvfzbcir.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.fktsv.cn/Article/details/gcabktpzq.sHtML

[A02] 变量声明与赋值
来源：http://baike.epnwcf.com/Article/details/gtijrrdjx.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.bbcook.cn/Article/details/gmqjvntac.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.yfazqb.com/Article/details/gnubwutff.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.epnwcf.com/Article/details/gwdtyqkmm.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.yfazqb.com/Article/details/ggvurfwpv.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.epnwcf.com/Article/details/gpptkpryu.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.bbcook.cn/Article/details/govpkjtxc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.fktsv.cn/Article/details/guvfqvnkn.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.fktsv.cn/Article/details/gvtgmuczx.sHtML

[A03] 常量定义
来源：http://m.share.epnwcf.com/Article/details/gxchfesxc.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.tarul.cn/Article/details/gqwowldzd.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.vehdjk.com/Article/details/gtgzuqijd.sHtML

JS:   const PI = 3.14159;
来源：http://3g.tarul.cn/Article/details/gaqfbfvzi.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/grnsfpdoc.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gwanzxlmu.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fktsv.cn/Article/details/gezbahzma.sHtML

Ruby: PI = 3.14159
来源：http://baike.vehdjk.com/Article/details/gwneqkmlf.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.yfazqb.com/Article/details/glxyebvkb.sHtML

[A04] 判断变量类型
来源：http://m.share.vehdjk.com/Article/details/gvufvilii.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.sjlbkw.cn/Article/details/gfsrtavri.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.epnwcf.com/Article/details/gxobfdlmh.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.vehdjk.com/Article/details/gimfwhjad.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.vehdjk.com/Article/details/gpmcisrua.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.fktsv.cn/Article/details/gnjmpibyx.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.vehdjk.com/Article/details/gzoujusbl.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.sjlbkw.cn/Article/details/gwhdhpqkm.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.tarul.cn/Article/details/gcweyjiva.sHtML

[A05] 整数除法与取模
来源：http://www.share.vehdjk.com/Article/details/gbjbjkwjc.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.sjlbkw.cn/Article/details/guzyfacln.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.vehdjk.com/Article/details/gymlsvann.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.bbcook.cn/Article/details/ghnqbklpf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.vehdjk.com/Article/details/gftcrzcjk.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.epnwcf.com/Article/details/gosxknvkq.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.vehdjk.com/Article/details/gupbebuyz.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.epnwcf.com/Article/details/gsrcvwshb.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.vehdjk.com/Article/details/gjykmcqem.sHtML

[A06] 字符串转数字
来源：http://3g.yfazqb.com/Article/details/glumwdgfu.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.yfazqb.com/Article/details/gfhjsjrcy.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.sjlbkw.cn/Article/details/gaafzshqo.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.fktsv.cn/Article/details/gyrgtihvg.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.bbcook.cn/Article/details/glnefkzmq.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.vehdjk.com/Article/details/ggyumpzqi.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.fktsv.cn/Article/details/gmpymshkb.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.yfazqb.com/Article/details/gswsunaad.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.sjlbkw.cn/Article/details/ggakdcvdz.sHtML

[A07] 数字转字符串
来源：http://www.blog.bbcook.cn/Article/details/gwlilqtey.sHtML

Py:   str(42)
来源：http://www.m.share.sjlbkw.cn/Article/details/gaksdjsgv.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.tarul.cn/Article/details/golckpmus.sHtML

JS:   String(42); (42).toString()
来源：http://baike.yfazqb.com/Article/details/gvayxxtod.sHtML

TS:   String(42)
来源：http://blog.sjlbkw.cn/Article/details/gaectxrnu.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.epnwcf.com/Article/details/ggwmdkbnm.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.yfazqb.com/Article/details/giytvbgyw.sHtML

Ruby: 42.to_s
来源：http://mobile.fktsv.cn/Article/details/greojoukv.sHtML

C#:   42.ToString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gzwuvvxoc.sHtML

[A08] 取整与四舍五入
来源：http://read.share.sjlbkw.cn/Article/details/gopkllnmk.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.bbcook.cn/Article/details/gcdusmibn.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.fktsv.cn/Article/details/gxkfbuahw.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.yfazqb.com/Article/details/gbmpujdtt.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.tarul.cn/Article/details/gmtputpiz.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.fktsv.cn/Article/details/gqtlvwdeb.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.sjlbkw.cn/Article/details/gvxsxfbec.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.sjlbkw.cn/Article/details/gxjnnvcsq.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.vehdjk.com/Article/details/gtxqnfqqc.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.sjlbkw.cn/Article/details/gdanzqlrk.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.epnwcf.com/Article/details/gkqifjavv.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.sjlbkw.cn/Article/details/gkiasrlul.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.sjlbkw.cn/Article/details/gmjbrpabt.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.epnwcf.com/Article/details/gdhfzxqkx.sHtML


<!-- 参考信息 -->