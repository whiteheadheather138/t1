代发 wailian999

[U63] PHP：文件读写
来源：http://baike.yfazqb.com/Article/details/goitasxrn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.vehdjk.com/Article/details/gjyisrnhd.sHtML

[U64] PHP：目录遍历
来源：http://baike.tarul.cn/Article/details/gwvtvnfyp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.yfazqb.com/Article/details/gbqbtuaeo.sHtML

[U65] PHP：会话
来源：http://www.blog.yfazqb.com/Article/details/gzfnrhkqy.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.tarul.cn/Article/details/gmbxlwuln.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.yfazqb.com/Article/details/gnedlzklv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.sjlbkw.cn/Article/details/gahmavzrw.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.yfazqb.com/Article/details/gaftbjixq.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.vehdjk.com/Article/details/gfuaaponi.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.bbcook.cn/Article/details/gmtbgislg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.epnwcf.com/Article/details/glniwirsy.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.vehdjk.com/Article/details/gprzepwqc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fktsv.cn/Article/details/gblbfwjks.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.tarul.cn/Article/details/gkudcfnee.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.yfazqb.com/Article/details/gxbeggwdc.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fktsv.cn/Article/details/gppmhjsfw.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.fktsv.cn/Article/details/gkntdlwsv.sHtML

[U72] PHP：写错误日志
来源：http://m.share.tarul.cn/Article/details/gcsxoelyl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.sjlbkw.cn/Article/details/ginqzdvxy.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.yfazqb.com/Article/details/gbufzcthh.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.sjlbkw.cn/Article/details/gzjdrtalc.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gnsqkdzgy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.tarul.cn/Article/details/gnsmovhvh.sHtML

[U75] PHP：依赖注入
来源：http://mobile.sjlbkw.cn/Article/details/gdrgvfmyv.sHtML

composer require psr/container
来源：http://wap.epnwcf.com/Article/details/goayjkmyl.sHtML

[U76] PHP：简单路由
来源：http://www.share.fktsv.cn/Article/details/gpdpccslu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.epnwcf.com/Article/details/gompvemal.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.sjlbkw.cn/Article/details/gepxtaclm.sHtML

composer require twig/twig
来源：http://www.blog.yfazqb.com/Article/details/gijuzxkex.sHtML

[U78] PHP：单元测试
来源：http://3g.epnwcf.com/Article/details/gdzqhqxxp.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.epnwcf.com/Article/details/ggwqsyakk.sHtML

[U79] PHP：静态分析
来源：http://mobile.epnwcf.com/Article/details/gokodgtug.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.bbcook.cn/Article/details/gdobiudpu.sHtML

[U80] PHP：代码规范修复
来源：http://wap.tarul.cn/Article/details/ggzdrovyr.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.fktsv.cn/Article/details/gmzfdhhgs.sHtML

[U81] JS：初始化项目
来源：http://3g.fktsv.cn/Article/details/gjjrkdfvm.sHtML

npm init -y;  npm i express
来源：http://mobile.bbcook.cn/Article/details/gxsjxdjjc.sHtML

[U82] JS：package.json 脚本
来源：http://wap.vehdjk.com/Article/details/gmnkgzrul.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.epnwcf.com/Article/details/gjbpdblhm.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.epnwcf.com/Article/details/ghqxyebhc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.vehdjk.com/Article/details/grtqlqoug.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.tarul.cn/Article/details/gfzlkqrav.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.epnwcf.com/Article/details/guyymjevg.sHtML

[U85] JS：可选链
来源：http://www.blog.tarul.cn/Article/details/girvyzdef.sHtML

a?.b?.c
来源：http://3g.yfazqb.com/Article/details/gfuweeics.sHtML

[U86] JS：空值合并
来源：http://www.blog.sjlbkw.cn/Article/details/gqqkjcwjj.sHtML

a ?? b
来源：http://wap.tarul.cn/Article/details/gggehgyha.sHtML

[U87] JS：解构默认值
来源：http://m.share.vehdjk.com/Article/details/gytyndcwn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.bbcook.cn/Article/details/gndqnnjtz.sHtML

[U88] JS：对象展开合并
来源：http://baike.bbcook.cn/Article/details/gwttgqiej.sHtML

{ ...a, ...b }
来源：http://wap.epnwcf.com/Article/details/grxbfpfjb.sHtML

[U89] JS：数组去重
来源：http://read.share.sjlbkw.cn/Article/details/gpjxvxgoh.sHtML

[...new Set(arr)]
来源：http://m.share.yfazqb.com/Article/details/gitkjhggj.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.tarul.cn/Article/details/gpokfbaoo.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.tarul.cn/Article/details/gjuvgtqus.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.tarul.cn/Article/details/gtdebvcez.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fktsv.cn/Article/details/gogzttjag.sHtML

[U92] JS：深拷贝
来源：http://baike.yfazqb.com/Article/details/ggmohwjbz.sHtML

structuredClone(obj)
来源：http://blog.bbcook.cn/Article/details/gfikhgdru.sHtML

[U93] JS：模板字符串
来源：http://blog.tarul.cn/Article/details/gygiuhkmp.sHtML

`共 ${n} 条`
来源：http://wap.bbcook.cn/Article/details/gfzockgjt.sHtML

[U94] JS：箭头函数
来源：http://www.share.yfazqb.com/Article/details/gfgqruwdx.sHtML

const double = x => x * 2;
来源：http://m.share.epnwcf.com/Article/details/glmmzwnfl.sHtML

[U95] JS：Promise 包装
来源：http://wap.sjlbkw.cn/Article/details/gfoaubtgt.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.epnwcf.com/Article/details/gvvbdnwlz.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.yfazqb.com/Article/details/gijxythfs.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.sjlbkw.cn/Article/details/guamncwbe.sHtML

[U97] JS：并发请求
来源：http://blog.bbcook.cn/Article/details/gxvtaipkt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fktsv.cn/Article/details/gdbziqptp.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.yfazqb.com/Article/details/goudpwwng.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.epnwcf.com/Article/details/gfeffwfdb.sHtML

[U99] JS：事件监听
来源：http://read.share.tarul.cn/Article/details/ghpdddroh.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fktsv.cn/Article/details/gnalnzghh.sHtML

[U100] JS：DOM 查询
来源：http://baike.sjlbkw.cn/Article/details/gwxupsasf.sHtML

document.querySelector(".item")
来源：http://wap.fktsv.cn/Article/details/gnyyspeyp.sHtML

[U101] JS：classList 操作
来源：http://3g.yfazqb.com/Article/details/gxlaxsdjw.sHtML

el.classList.toggle("active")
来源：http://www.share.vehdjk.com/Article/details/ggsmckpau.sHtML

[U102] JS：本地存储
来源：http://wap.bbcook.cn/Article/details/ghfnnevja.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.tarul.cn/Article/details/gbzgyviqc.sHtML

[U103] JS：定时器
来源：http://blog.bbcook.cn/Article/details/gsstxfgoa.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.bbcook.cn/Article/details/gwszodrrp.sHtML

[U104] JS：防抖
来源：http://www.share.epnwcf.com/Article/details/gtheygkif.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.tarul.cn/Article/details/ghwzevxtu.sHtML

[U105] JS：节流
来源：http://3g.tarul.cn/Article/details/ggchhxupr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.tarul.cn/Article/details/gsvsovsmo.sHtML

[U106] JS：日期格式化
来源：http://www.share.yfazqb.com/Article/details/ggyhlqbrs.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.sjlbkw.cn/Article/details/gadoghxlu.sHtML

[U107] JS：数字千分位
来源：http://3g.fktsv.cn/Article/details/gvbfqvpit.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.vehdjk.com/Article/details/gcuevwocb.sHtML

[U108] JS：随机整数
来源：http://wap.yfazqb.com/Article/details/goomilbna.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.sjlbkw.cn/Article/details/gqmhhvvue.sHtML

[U109] JS：数组分组
来源：http://baike.fktsv.cn/Article/details/guvwdelao.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.bbcook.cn/Article/details/gfnbxtgou.sHtML

[U110] JS：数组分块
来源：http://read.share.epnwcf.com/Article/details/gyzuawdbz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.fktsv.cn/Article/details/gqnhwtmwu.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.epnwcf.com/Article/details/gzvapiljx.sHtML

new Map(Object.entries(obj))
来源：http://blog.vehdjk.com/Article/details/gdwwjhyxl.sHtML

[U112] JS：字符串补位
来源：http://wap.epnwcf.com/Article/details/gurykjewr.sHtML

"7".padStart(3, "0")
来源：http://blog.epnwcf.com/Article/details/glexccpek.sHtML

[U113] JS：正则替换全部
来源：http://read.share.sjlbkw.cn/Article/details/gvdgnemhc.sHtML

s.replaceAll("a", "b")
来源：http://www.share.tarul.cn/Article/details/glarmqujt.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.bbcook.cn/Article/details/gqdevxnxh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.epnwcf.com/Article/details/guzxglwbj.sHtML

[U115] JS：生成 UUID
来源：http://baike.tarul.cn/Article/details/gjliavyki.sHtML

crypto.randomUUID()
来源：http://mobile.sjlbkw.cn/Article/details/gfedsovlf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.yfazqb.com/Article/details/gkmisqbkf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.bbcook.cn/Article/details/gdnwcfxdz.sHtML

[U117] JS：单元测试
来源：http://baike.sjlbkw.cn/Article/details/gbcjmffrc.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.bbcook.cn/Article/details/gkelzhmgi.sHtML

[U118] JS：开发服务器
来源：http://wap.epnwcf.com/Article/details/gbtzkmnds.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.epnwcf.com/Article/details/gpdhasnyy.sHtML

[U119] JS：生产构建
来源：http://read.share.sjlbkw.cn/Article/details/gnxxbxtpw.sHtML

npx vite build
来源：http://www.m.share.yfazqb.com/Article/details/gfkhacigo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fktsv.cn/Article/details/gzbfweblz.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.epnwcf.com/Article/details/gzsqawdyp.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/ggrhknaor.sHtML

统计汇总
来源：http://m.share.fktsv.cn/Article/details/gkctejnde.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/glgmopwle.sHtML

按语言统计（条）：
来源：http://www.share.sjlbkw.cn/Article/details/glvyiubjk.sHtML

Python ......... 252
来源：http://mobile.vehdjk.com/Article/details/gfslhrdqg.sHtML

PHP ............ 252
来源：http://read.share.fktsv.cn/Article/details/giilcnzvm.sHtML

JavaScript ..... 252
来源：http://read.share.tarul.cn/Article/details/gjqoqlaxk.sHtML

TypeScript ..... 212
来源：http://baike.epnwcf.com/Article/details/gnmejtdom.sHtML

Java ........... 212
来源：http://read.share.sjlbkw.cn/Article/details/gtaqdlsko.sHtML

Go ............. 212
来源：http://3g.tarul.cn/Article/details/gnujqhnpi.sHtML

Ruby ........... 212
来源：http://baike.vehdjk.com/Article/details/gripwbflx.sHtML

C# ............. 212
来源：http://3g.tarul.cn/Article/details/gjaflbedn.sHtML

C .............. 30
来源：http://blog.bbcook.cn/Article/details/godbbaeyk.sHtML

C++ ............ 30
来源：http://baike.vehdjk.com/Article/details/gwifjmssg.sHtML

SQL ............ 90
来源：http://m.share.fktsv.cn/Article/details/guadzfalv.sHtML

Bash ........... 80
来源：http://baike.fktsv.cn/Article/details/gmcticmpt.sHtML

Kotlin ......... 15
来源：http://www.m.share.epnwcf.com/Article/details/guirvibkn.sHtML

Swift .......... 15
来源：http://mobile.yfazqb.com/Article/details/girevtauo.sHtML

Lua ............ 10
来源：http://www.m.share.vehdjk.com/Article/details/gejblmbvz.sHtML

Perl ........... 10
来源：http://www.m.share.vehdjk.com/Article/details/gwlwzysfq.sHtML

Scala .......... 10
来源：http://3g.tarul.cn/Article/details/ginijymio.sHtML

------------------------------------
来源：http://mobile.fktsv.cn/Article/details/gzlbdmxsz.sHtML

合计 ........... 2106 条
来源：http://m.share.epnwcf.com/Article/details/gpvslzdxr.sHtML

按章节统计：
来源：http://read.share.sjlbkw.cn/Article/details/gixtpgkqt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.epnwcf.com/Article/details/guzjpszrc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.sjlbkw.cn/Article/details/gvaiduiwm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.tarul.cn/Article/details/gqylbhaij.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.yfazqb.com/Article/details/gkbksoaen.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fktsv.cn/Article/details/gudbujhee.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fktsv.cn/Article/details/gkobnxqwc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.sjlbkw.cn/Article/details/geikhrotv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fktsv.cn/Article/details/gtnbplmdz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.vehdjk.com/Article/details/gqpizkmjp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.bbcook.cn/Article/details/gemkozqjl.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.yfazqb.com/Article/details/gwrdlcygo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.bbcook.cn/Article/details/grwbzxlcm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.tarul.cn/Article/details/gudlpwegw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.vehdjk.com/Article/details/gqfstzmhu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.yfazqb.com/Article/details/ghhpnkxsf.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.sjlbkw.cn/Article/details/gfeafubsn.sHtML

Q SQL 专题                              90
来源：http://read.share.tarul.cn/Article/details/gfkhlimew.sHtML

R Bash 专题                             80
来源：http://www.blog.yfazqb.com/Article/details/galvkbyzp.sHtML

S C / C++ 专题                          60
来源：http://mobile.vehdjk.com/Article/details/gaajzcvtd.sHtML

T 其他语言补充                          60
来源：http://www.share.tarul.cn/Article/details/gibbegaqh.sHtML

U 高频实用片段                         120
来源：http://blog.bbcook.cn/Article/details/ghndviilq.sHtML

------------------------------------
来源：http://baike.epnwcf.com/Article/details/ggfwvrpgf.sHtML

合计                                  2106 条
来源：http://www.share.bbcook.cn/Article/details/gbbykihkd.sHtML

--------------------------------------------------------------------------------
来源：http://3g.bbcook.cn/Article/details/ghdicwndp.sHtML

使用提醒
来源：http://wap.epnwcf.com/Article/details/gonmuubrt.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.tarul.cn/Article/details/gsdmdebdw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.tarul.cn/Article/details/gflkoyhbr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.vehdjk.com/Article/details/glfoqutzm.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.tarul.cn/Article/details/gavxeldgo.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.yfazqb.com/Article/details/ggobxnsac.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.yfazqb.com/Article/details/gcwolzetw.sHtML

—— 文件结束 ——
来源：http://www.blog.yfazqb.com/Article/details/givalhddx.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gtsjodkgp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.bbcook.cn/Article/details/gfiohkehw.sHtML

Common Programming Examples Cheat Book
来源：http://baike.epnwcf.com/Article/details/gqzkbvvdm.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gszmpolsg.sHtML

【收录内容】
来源：http://www.share.sjlbkw.cn/Article/details/gdmpmxrfp.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fktsv.cn/Article/details/guhdntxng.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.yfazqb.com/Article/details/gmzcpmndm.sHtML

SQL · Bash · C · C++
来源：http://3g.tarul.cn/Article/details/gxqaixoko.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.bbcook.cn/Article/details/gqteifhpn.sHtML

【使用说明】
来源：http://www.m.share.epnwcf.com/Article/details/gtawdzjup.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.tarul.cn/Article/details/gozhjybde.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.sjlbkw.cn/Article/details/giwcevthb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.sjlbkw.cn/Article/details/giggbckte.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.bbcook.cn/Article/details/ggiwedrmp.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.bbcook.cn/Article/details/gmvmduuwf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.yfazqb.com/Article/details/gdcpsmpij.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.yfazqb.com/Article/details/gjyftmnhx.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.yfazqb.com/Article/details/gypatbuqm.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.bbcook.cn/Article/details/gukirletg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.epnwcf.com/Article/details/glyoppvcg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.epnwcf.com/Article/details/glmjtyryu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.tarul.cn/Article/details/gswcvneku.sHtML

【文件统计】
来源：http://www.blog.yfazqb.com/Article/details/gdufvtaby.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fktsv.cn/Article/details/guhltcoga.sHtML

--------------------------------------------------------------------------------
来源：http://blog.yfazqb.com/Article/details/gxmifyguz.sHtML

目  录
来源：http://read.share.fktsv.cn/Article/details/gysllzkly.sHtML

--------------------------------------------------------------------------------
来源：http://baike.yfazqb.com/Article/details/gsdlknmip.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.fktsv.cn/Article/details/gqjqhfffo.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fktsv.cn/Article/details/gkxxepavp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.epnwcf.com/Article/details/gbrlkdwor.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.bbcook.cn/Article/details/gggdqvufu.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.vehdjk.com/Article/details/ggwwnduyv.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fktsv.cn/Article/details/gewjtotqg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.yfazqb.com/Article/details/grkoephdu.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.vehdjk.com/Article/details/gzcqlnnjn.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.yfazqb.com/Article/details/gzynjwuys.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.epnwcf.com/Article/details/gubikhusc.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.bbcook.cn/Article/details/gmanilxcd.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.vehdjk.com/Article/details/gpznqkoar.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fktsv.cn/Article/details/gtwmkuubi.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fktsv.cn/Article/details/gvaqesobb.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fktsv.cn/Article/details/ggoixzezj.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.vehdjk.com/Article/details/gyccujwpv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.yfazqb.com/Article/details/gflszitsl.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.yfazqb.com/Article/details/gevntcgah.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.bbcook.cn/Article/details/glppyskml.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.tarul.cn/Article/details/ghnwiyuvx.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.sjlbkw.cn/Article/details/girnthrbx.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/ggblrckph.sHtML

A. 基础语法与类型
来源：http://www.m.share.epnwcf.com/Article/details/grfxjbgay.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gfaufudng.sHtML

[A01] Hello World
来源：http://www.blog.tarul.cn/Article/details/gjvpdyabd.sHtML

Py:   print("Hello, World!")
来源：http://www.share.sjlbkw.cn/Article/details/gmwwjfyax.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.bbcook.cn/Article/details/gxynukzfa.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.vehdjk.com/Article/details/glkopveos.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.tarul.cn/Article/details/gxozwvbxy.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.yfazqb.com/Article/details/gjepufyww.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.tarul.cn/Article/details/gplnnftst.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.tarul.cn/Article/details/gtddqxwly.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.bbcook.cn/Article/details/gdxdeygsj.sHtML

[A02] 变量声明与赋值
来源：http://3g.vehdjk.com/Article/details/gojycgecd.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.tarul.cn/Article/details/gjnetbkqj.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.sjlbkw.cn/Article/details/guhsfdhns.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.sjlbkw.cn/Article/details/gisabvxkb.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.yfazqb.com/Article/details/grzbizkzj.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fktsv.cn/Article/details/gqehpdcmq.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.tarul.cn/Article/details/gcshooekw.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.yfazqb.com/Article/details/giaononcj.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.sjlbkw.cn/Article/details/ggkfcdmko.sHtML

[A03] 常量定义
来源：http://baike.vehdjk.com/Article/details/gmzoeplbb.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.sjlbkw.cn/Article/details/gnqyoeytb.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.tarul.cn/Article/details/glwtjwwuj.sHtML

JS:   const PI = 3.14159;
来源：http://baike.tarul.cn/Article/details/gpartyogm.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.epnwcf.com/Article/details/ghdjaosnf.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.epnwcf.com/Article/details/goricvciu.sHtML

Go:   const PI = 3.14159
来源：http://mobile.yfazqb.com/Article/details/gfkjidppt.sHtML

Ruby: PI = 3.14159
来源：http://read.share.fktsv.cn/Article/details/gtoxqzqgr.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.vehdjk.com/Article/details/gefgszkdj.sHtML

[A04] 判断变量类型
来源：http://3g.vehdjk.com/Article/details/gslxhvmqy.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.bbcook.cn/Article/details/gqsgiekil.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.fktsv.cn/Article/details/guewivquc.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.vehdjk.com/Article/details/gfrmyqywy.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.epnwcf.com/Article/details/gzcxgocly.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.bbcook.cn/Article/details/gqdukyndy.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.tarul.cn/Article/details/gnfhjrpml.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.bbcook.cn/Article/details/gjjgyozou.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.fktsv.cn/Article/details/gvewxgkhb.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.sjlbkw.cn/Article/details/gncuyztmk.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.vehdjk.com/Article/details/gchohvetj.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.tarul.cn/Article/details/gzzpvfjwp.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fktsv.cn/Article/details/gcayyglfd.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.tarul.cn/Article/details/gpyavsqtr.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.tarul.cn/Article/details/ghaadrjhu.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.epnwcf.com/Article/details/gcywyubfi.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.yfazqb.com/Article/details/gitydkfij.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.sjlbkw.cn/Article/details/gycqkmfji.sHtML

[A06] 字符串转数字
来源：http://www.blog.sjlbkw.cn/Article/details/gtpghvsyy.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.epnwcf.com/Article/details/gvpsshwxh.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.sjlbkw.cn/Article/details/gmbtxttmw.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.bbcook.cn/Article/details/guklmeetg.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.yfazqb.com/Article/details/goctgfkxx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.bbcook.cn/Article/details/gfzcoqnce.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.tarul.cn/Article/details/gorkglfsf.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.vehdjk.com/Article/details/gaaqxeezp.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.sjlbkw.cn/Article/details/gwmxrydyp.sHtML

[A07] 数字转字符串
来源：http://mobile.vehdjk.com/Article/details/gahdlgapb.sHtML

Py:   str(42)
来源：http://www.m.share.vehdjk.com/Article/details/gfyvdesgs.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.epnwcf.com/Article/details/gfdwbnvnq.sHtML

JS:   String(42); (42).toString()
来源：http://blog.fktsv.cn/Article/details/gbndssowo.sHtML

TS:   String(42)
来源：http://m.share.bbcook.cn/Article/details/gdqkabgdz.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.bbcook.cn/Article/details/guuahyfts.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.tarul.cn/Article/details/geueutsad.sHtML

Ruby: 42.to_s
来源：http://mobile.vehdjk.com/Article/details/gmpzfxpye.sHtML

C#:   42.ToString()
来源：http://baike.epnwcf.com/Article/details/gvzaonipz.sHtML

[A08] 取整与四舍五入
来源：http://wap.sjlbkw.cn/Article/details/gvrmcbsqm.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.yfazqb.com/Article/details/gdgdgthaj.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.bbcook.cn/Article/details/gzgunmoic.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.vehdjk.com/Article/details/gmwvfgriq.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.yfazqb.com/Article/details/gmcsaihnx.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.epnwcf.com/Article/details/ggazknvik.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.yfazqb.com/Article/details/gydlkctnb.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.fktsv.cn/Article/details/gqbospyqj.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.vehdjk.com/Article/details/gjcwnkhin.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.bbcook.cn/Article/details/gvglknbdp.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.bbcook.cn/Article/details/gipchrezb.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.sjlbkw.cn/Article/details/gmxagrmkb.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.tarul.cn/Article/details/goybjmmrt.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.vehdjk.com/Article/details/gyhkenlbj.sHtML


<!-- 参考信息 -->