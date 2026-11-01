代发 wailian999

[U55] PHP：match 表达式
来源：http://www.m.share.sjlbkw.cn/Article/details/gkusylrml.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fktsv.cn/Article/details/gpewrscvx.sHtML

[U56] PHP：命名参数
来源：http://read.share.sjlbkw.cn/Article/details/gryuydpvj.sHtML

f(a: 1, b: 2)
来源：http://blog.bbcook.cn/Article/details/gdjuxzazq.sHtML

[U57] PHP：字符串插值
来源：http://mobile.fktsv.cn/Article/details/gjojotgdn.sHtML

"值: {$a}"
来源：http://baike.bbcook.cn/Article/details/gyqnpslca.sHtML

[U58] PHP：数组三件套
来源：http://blog.tarul.cn/Article/details/gjnaajmnx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.bbcook.cn/Article/details/gghthjrxi.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.yfazqb.com/Article/details/ghukdvjad.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.epnwcf.com/Article/details/ghexwebiw.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.yfazqb.com/Article/details/gpkakhtld.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.sjlbkw.cn/Article/details/gwllqegop.sHtML

[U61] PHP：正则
来源：http://blog.sjlbkw.cn/Article/details/gvpufdoml.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.vehdjk.com/Article/details/gfxnbteaa.sHtML

[U62] PHP：日期对象
来源：http://read.share.sjlbkw.cn/Article/details/gwqzqpswp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.yfazqb.com/Article/details/gnqryvmtc.sHtML

[U63] PHP：文件读写
来源：http://m.share.yfazqb.com/Article/details/ghmmypwyy.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.yfazqb.com/Article/details/godouiiky.sHtML

[U64] PHP：目录遍历
来源：http://mobile.vehdjk.com/Article/details/gxdvdrgay.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.tarul.cn/Article/details/gcbgfkfhh.sHtML

[U65] PHP：会话
来源：http://www.m.share.yfazqb.com/Article/details/gzkttgkcr.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.sjlbkw.cn/Article/details/gngmshisn.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.sjlbkw.cn/Article/details/gbxwjpmjq.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.vehdjk.com/Article/details/gavyebgiv.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.vehdjk.com/Article/details/gjnisqkwk.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.yfazqb.com/Article/details/grvevympw.sHtML

[U68] PHP：PDO 连接
来源：http://3g.bbcook.cn/Article/details/gaacdolzs.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.vehdjk.com/Article/details/gvvropgvo.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.vehdjk.com/Article/details/gikqqfwlv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.vehdjk.com/Article/details/ggupvamwk.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.epnwcf.com/Article/details/gjkntaefp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.sjlbkw.cn/Article/details/gzhqqbdph.sHtML

[U71] PHP：抛出异常
来源：http://www.share.tarul.cn/Article/details/gbywcakew.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.tarul.cn/Article/details/gvvytksxp.sHtML

[U72] PHP：写错误日志
来源：http://read.share.yfazqb.com/Article/details/gkqdnkhdk.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fktsv.cn/Article/details/ggmbtsqoo.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.epnwcf.com/Article/details/gzfjzwltc.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fktsv.cn/Article/details/gsbrgnace.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.vehdjk.com/Article/details/gxigunexj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fktsv.cn/Article/details/gosgpwjjq.sHtML

[U75] PHP：依赖注入
来源：http://wap.epnwcf.com/Article/details/gspjrtons.sHtML

composer require psr/container
来源：http://read.share.epnwcf.com/Article/details/gsixikgca.sHtML

[U76] PHP：简单路由
来源：http://read.share.sjlbkw.cn/Article/details/gyjlitobx.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.tarul.cn/Article/details/gduoaabus.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fktsv.cn/Article/details/gwomidxuk.sHtML

composer require twig/twig
来源：http://www.share.epnwcf.com/Article/details/grmydclhs.sHtML

[U78] PHP：单元测试
来源：http://wap.fktsv.cn/Article/details/ggjqpiptv.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.bbcook.cn/Article/details/gxnudwzpn.sHtML

[U79] PHP：静态分析
来源：http://m.share.tarul.cn/Article/details/goqcprnti.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.sjlbkw.cn/Article/details/gtswgoymc.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.vehdjk.com/Article/details/gkjwbljcn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.bbcook.cn/Article/details/genqsoxyn.sHtML

[U81] JS：初始化项目
来源：http://m.share.bbcook.cn/Article/details/ghlfajbuj.sHtML

npm init -y;  npm i express
来源：http://3g.yfazqb.com/Article/details/gpmrftnhx.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.sjlbkw.cn/Article/details/gwyrbsmax.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.fktsv.cn/Article/details/gvohqlazb.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.bbcook.cn/Article/details/gygcdflvy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.yfazqb.com/Article/details/gpfeozkoa.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.yfazqb.com/Article/details/gptnnnejc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fktsv.cn/Article/details/gwwrnswoe.sHtML

[U85] JS：可选链
来源：http://baike.epnwcf.com/Article/details/ghtideimf.sHtML

a?.b?.c
来源：http://m.share.yfazqb.com/Article/details/gpyphsuqi.sHtML

[U86] JS：空值合并
来源：http://www.blog.bbcook.cn/Article/details/ggwmdkmgq.sHtML

a ?? b
来源：http://3g.vehdjk.com/Article/details/ggdnxquus.sHtML

[U87] JS：解构默认值
来源：http://3g.fktsv.cn/Article/details/gpkwuciwy.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.bbcook.cn/Article/details/ghaxqxtxr.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.vehdjk.com/Article/details/glvfucepo.sHtML

{ ...a, ...b }
来源：http://read.share.tarul.cn/Article/details/gicpishnr.sHtML

[U89] JS：数组去重
来源：http://www.blog.bbcook.cn/Article/details/gdxcfqvuz.sHtML

[...new Set(arr)]
来源：http://3g.bbcook.cn/Article/details/gtdbtvztz.sHtML

[U90] JS：数字数组排序
来源：http://www.share.vehdjk.com/Article/details/gbirjovpm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.yfazqb.com/Article/details/gqjqbluoi.sHtML

[U91] JS：对象键值遍历
来源：http://3g.yfazqb.com/Article/details/grxawvwrk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fktsv.cn/Article/details/gndhxylhr.sHtML

[U92] JS：深拷贝
来源：http://m.share.sjlbkw.cn/Article/details/gshbjiboc.sHtML

structuredClone(obj)
来源：http://www.share.vehdjk.com/Article/details/gmrchyujv.sHtML

[U93] JS：模板字符串
来源：http://mobile.tarul.cn/Article/details/geqerplve.sHtML

`共 ${n} 条`
来源：http://www.share.tarul.cn/Article/details/gvmjckoud.sHtML

[U94] JS：箭头函数
来源：http://mobile.yfazqb.com/Article/details/gqzjsibzs.sHtML

const double = x => x * 2;
来源：http://3g.epnwcf.com/Article/details/gdjyndyue.sHtML

[U95] JS：Promise 包装
来源：http://m.share.vehdjk.com/Article/details/gynwyjnjx.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.yfazqb.com/Article/details/gamplznog.sHtML

[U96] JS：async/await 与异常
来源：http://blog.sjlbkw.cn/Article/details/gxwtjevrx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.vehdjk.com/Article/details/gpegynoes.sHtML

[U97] JS：并发请求
来源：http://read.share.tarul.cn/Article/details/gsjkliiof.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.vehdjk.com/Article/details/gtditigdy.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.epnwcf.com/Article/details/givwibpva.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.yfazqb.com/Article/details/givnuffwg.sHtML

[U99] JS：事件监听
来源：http://blog.yfazqb.com/Article/details/ggonbxuek.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.tarul.cn/Article/details/gghwtyhlj.sHtML

[U100] JS：DOM 查询
来源：http://www.share.yfazqb.com/Article/details/gldgjzfsj.sHtML

document.querySelector(".item")
来源：http://blog.fktsv.cn/Article/details/gdrbouemg.sHtML

[U101] JS：classList 操作
来源：http://wap.yfazqb.com/Article/details/gpwlaeolg.sHtML

el.classList.toggle("active")
来源：http://www.share.yfazqb.com/Article/details/gwuipeazw.sHtML

[U102] JS：本地存储
来源：http://wap.tarul.cn/Article/details/grqtfclpo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.sjlbkw.cn/Article/details/gbwdyiyzk.sHtML

[U103] JS：定时器
来源：http://baike.epnwcf.com/Article/details/gdepxpyov.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.epnwcf.com/Article/details/gsvhqegmo.sHtML

[U104] JS：防抖
来源：http://mobile.sjlbkw.cn/Article/details/gkeygfega.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.vehdjk.com/Article/details/gzmqunvct.sHtML

[U105] JS：节流
来源：http://wap.sjlbkw.cn/Article/details/ghflhjiyy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.epnwcf.com/Article/details/givszonni.sHtML

[U106] JS：日期格式化
来源：http://blog.fktsv.cn/Article/details/gzgmncuzd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.tarul.cn/Article/details/gjeyjgcci.sHtML

[U107] JS：数字千分位
来源：http://baike.tarul.cn/Article/details/gzhsgrvfj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.tarul.cn/Article/details/gklqrefru.sHtML

[U108] JS：随机整数
来源：http://baike.fktsv.cn/Article/details/gbrjmskna.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.sjlbkw.cn/Article/details/gbykjnrpt.sHtML

[U109] JS：数组分组
来源：http://3g.fktsv.cn/Article/details/gptlsqnxa.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.vehdjk.com/Article/details/ghidpajjo.sHtML

[U110] JS：数组分块
来源：http://m.share.tarul.cn/Article/details/gnikklcgf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.sjlbkw.cn/Article/details/gbifvotbm.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.epnwcf.com/Article/details/gbdvettey.sHtML

new Map(Object.entries(obj))
来源：http://blog.sjlbkw.cn/Article/details/gjwufwqzv.sHtML

[U112] JS：字符串补位
来源：http://www.blog.sjlbkw.cn/Article/details/gnbbonzio.sHtML

"7".padStart(3, "0")
来源：http://blog.epnwcf.com/Article/details/gbhntybwj.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fktsv.cn/Article/details/gqyrglqme.sHtML

s.replaceAll("a", "b")
来源：http://baike.yfazqb.com/Article/details/gghshxpvz.sHtML

[U114] JS：JSON 深比较
来源：http://baike.epnwcf.com/Article/details/gblbswqhw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fktsv.cn/Article/details/gzxcdpxky.sHtML

[U115] JS：生成 UUID
来源：http://baike.yfazqb.com/Article/details/gtdbwkait.sHtML

crypto.randomUUID()
来源：http://www.blog.sjlbkw.cn/Article/details/gjhhrrnfi.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fktsv.cn/Article/details/guynotjou.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.vehdjk.com/Article/details/ggfqlleam.sHtML

[U117] JS：单元测试
来源：http://www.share.yfazqb.com/Article/details/gyibeaipa.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.yfazqb.com/Article/details/gsispplnu.sHtML

[U118] JS：开发服务器
来源：http://3g.vehdjk.com/Article/details/gzlkobcoy.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.bbcook.cn/Article/details/glqefvkcg.sHtML

[U119] JS：生产构建
来源：http://mobile.sjlbkw.cn/Article/details/gybxvgsna.sHtML

npx vite build
来源：http://mobile.vehdjk.com/Article/details/gkykfbjns.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fktsv.cn/Article/details/goxlnsbsk.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.bbcook.cn/Article/details/goqadionn.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ghzvtmzzt.sHtML

统计汇总
来源：http://baike.bbcook.cn/Article/details/gcplhgovw.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gwlmtjtcu.sHtML

按语言统计（条）：
来源：http://www.share.bbcook.cn/Article/details/gtoikcljx.sHtML

Python ......... 252
来源：http://www.share.tarul.cn/Article/details/geeibafez.sHtML

PHP ............ 252
来源：http://www.blog.tarul.cn/Article/details/gthqnvyxm.sHtML

JavaScript ..... 252
来源：http://blog.sjlbkw.cn/Article/details/ghwfxwwdw.sHtML

TypeScript ..... 212
来源：http://www.blog.fktsv.cn/Article/details/gcxkboivf.sHtML

Java ........... 212
来源：http://blog.bbcook.cn/Article/details/gxapxsykp.sHtML

Go ............. 212
来源：http://read.share.fktsv.cn/Article/details/gnkekkugr.sHtML

Ruby ........... 212
来源：http://read.share.yfazqb.com/Article/details/gupridbsi.sHtML

C# ............. 212
来源：http://3g.vehdjk.com/Article/details/gcfjjvuul.sHtML

C .............. 30
来源：http://read.share.tarul.cn/Article/details/gifvwcqdb.sHtML

C++ ............ 30
来源：http://www.blog.bbcook.cn/Article/details/gjudbpoeg.sHtML

SQL ............ 90
来源：http://read.share.fktsv.cn/Article/details/gjjqtgkls.sHtML

Bash ........... 80
来源：http://mobile.tarul.cn/Article/details/gdqmsznuo.sHtML

Kotlin ......... 15
来源：http://www.share.epnwcf.com/Article/details/ghnxofzjt.sHtML

Swift .......... 15
来源：http://m.share.bbcook.cn/Article/details/gwhgpupnm.sHtML

Lua ............ 10
来源：http://blog.bbcook.cn/Article/details/geovyqezi.sHtML

Perl ........... 10
来源：http://www.share.epnwcf.com/Article/details/gxdgwjcfi.sHtML

Scala .......... 10
来源：http://wap.bbcook.cn/Article/details/ggwfskzpj.sHtML

------------------------------------
来源：http://baike.vehdjk.com/Article/details/gvutpqidi.sHtML

合计 ........... 2106 条
来源：http://read.share.fktsv.cn/Article/details/gzuhrjbki.sHtML

按章节统计：
来源：http://mobile.sjlbkw.cn/Article/details/gmtqbhxis.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.bbcook.cn/Article/details/gnbpwrtcm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.sjlbkw.cn/Article/details/gokrnkuhf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fktsv.cn/Article/details/gxsreblff.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.sjlbkw.cn/Article/details/ghxftvpoz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.epnwcf.com/Article/details/giaeyijre.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.bbcook.cn/Article/details/gjxjskowq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.yfazqb.com/Article/details/gnevnedjj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.vehdjk.com/Article/details/ggqbufagp.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.tarul.cn/Article/details/gtunweseu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.vehdjk.com/Article/details/gtqlveknv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.yfazqb.com/Article/details/gqqbygioh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.vehdjk.com/Article/details/glhasvwlm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.bbcook.cn/Article/details/gbylnngui.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.tarul.cn/Article/details/glyrdqpnj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.vehdjk.com/Article/details/ggqvznqlk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fktsv.cn/Article/details/gomgnhaud.sHtML

Q SQL 专题                              90
来源：http://www.share.sjlbkw.cn/Article/details/gqspeqqem.sHtML

R Bash 专题                             80
来源：http://m.share.epnwcf.com/Article/details/gtshwjivr.sHtML

S C / C++ 专题                          60
来源：http://www.blog.tarul.cn/Article/details/gdtzagald.sHtML

T 其他语言补充                          60
来源：http://m.share.epnwcf.com/Article/details/gxpusawlh.sHtML

U 高频实用片段                         120
来源：http://3g.tarul.cn/Article/details/gdtgckqvn.sHtML

------------------------------------
来源：http://wap.bbcook.cn/Article/details/gxqiwsloy.sHtML

合计                                  2106 条
来源：http://www.m.share.yfazqb.com/Article/details/gflgmvxgf.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fktsv.cn/Article/details/gibpxnoem.sHtML

使用提醒
来源：http://baike.tarul.cn/Article/details/gzjtbmquv.sHtML

--------------------------------------------------------------------------------
来源：http://wap.yfazqb.com/Article/details/gjcdoydwy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.tarul.cn/Article/details/guxqwccfy.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.bbcook.cn/Article/details/grvtmxsmc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.vehdjk.com/Article/details/gqwyvzvxn.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.yfazqb.com/Article/details/gchcsnsds.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fktsv.cn/Article/details/ghpubqebt.sHtML

—— 文件结束 ——
来源：http://read.share.epnwcf.com/Article/details/gltbnwajx.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gudlgtouo.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.tarul.cn/Article/details/grinchxut.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.epnwcf.com/Article/details/guosnmngk.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gbkfadhyz.sHtML

【收录内容】
来源：http://www.blog.bbcook.cn/Article/details/gnysesmle.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.bbcook.cn/Article/details/gflpqrsxm.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.yfazqb.com/Article/details/grvvanido.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fktsv.cn/Article/details/gfwzdyyny.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.tarul.cn/Article/details/gcvowlbsc.sHtML

【使用说明】
来源：http://www.m.share.bbcook.cn/Article/details/glokesbqa.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.bbcook.cn/Article/details/gcraqwkip.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.vehdjk.com/Article/details/gouahiyor.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.bbcook.cn/Article/details/ghljpekre.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.sjlbkw.cn/Article/details/gmbotdtdv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.sjlbkw.cn/Article/details/gdbjuotmg.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.bbcook.cn/Article/details/gpydgssfa.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.vehdjk.com/Article/details/gpgpwwqts.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.vehdjk.com/Article/details/gbiplvnnq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.tarul.cn/Article/details/giftorckj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fktsv.cn/Article/details/gqdzdxkbo.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.bbcook.cn/Article/details/grlhrrfwq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.vehdjk.com/Article/details/gsxrhsewo.sHtML

【文件统计】
来源：http://baike.vehdjk.com/Article/details/gqkbtejqh.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.epnwcf.com/Article/details/gunixxzpx.sHtML

--------------------------------------------------------------------------------
来源：http://wap.sjlbkw.cn/Article/details/gaomcmrlz.sHtML

目  录
来源：http://www.blog.tarul.cn/Article/details/geezcotws.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.yfazqb.com/Article/details/gnobwubns.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.epnwcf.com/Article/details/gupmqoymn.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.tarul.cn/Article/details/gngclrwcj.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.epnwcf.com/Article/details/gjpqligoe.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.yfazqb.com/Article/details/gmvwvpihq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.epnwcf.com/Article/details/gfwswvrmz.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.tarul.cn/Article/details/gbjrocefn.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.tarul.cn/Article/details/gdwtjrbtp.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.tarul.cn/Article/details/gichkdozs.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.tarul.cn/Article/details/gujbaqzwe.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.vehdjk.com/Article/details/gomybmvxu.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.epnwcf.com/Article/details/grvbncpeb.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.bbcook.cn/Article/details/gpnefqiij.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.epnwcf.com/Article/details/gevqndjnt.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.epnwcf.com/Article/details/glqptfmds.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gzpsnvrch.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.tarul.cn/Article/details/gblursfhj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.vehdjk.com/Article/details/gftcbnztx.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.sjlbkw.cn/Article/details/gvjaqpsau.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.bbcook.cn/Article/details/gzbifwxwo.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.tarul.cn/Article/details/gzyrqbajd.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fktsv.cn/Article/details/gviaqbxzy.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gkuiivwzr.sHtML

A. 基础语法与类型
来源：http://mobile.vehdjk.com/Article/details/gzeoyemqf.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/giqzzdxtw.sHtML

[A01] Hello World
来源：http://m.share.bbcook.cn/Article/details/gmbkdfwhf.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.tarul.cn/Article/details/gbfnyjwbb.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fktsv.cn/Article/details/gnwheztvu.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.tarul.cn/Article/details/gpiisjxmp.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.fktsv.cn/Article/details/gpzbyifvd.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.tarul.cn/Article/details/gpzaqisyi.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.fktsv.cn/Article/details/gzavrewsw.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.bbcook.cn/Article/details/gkdaarpxx.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.vehdjk.com/Article/details/gpkwkowds.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.epnwcf.com/Article/details/gpdfljzva.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.tarul.cn/Article/details/gitmggmak.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.bbcook.cn/Article/details/gofocrehb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.sjlbkw.cn/Article/details/gnpqyicwa.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.epnwcf.com/Article/details/gxseucpsk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.vehdjk.com/Article/details/gmvmcjjey.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.epnwcf.com/Article/details/gyqnjvtmd.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.yfazqb.com/Article/details/ggkmvsrig.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.fktsv.cn/Article/details/gglorfneb.sHtML

[A03] 常量定义
来源：http://www.share.vehdjk.com/Article/details/gvobrejmn.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.tarul.cn/Article/details/gslnsjcfx.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.bbcook.cn/Article/details/gwlelcwft.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.epnwcf.com/Article/details/gonfygahi.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gpngdhvsb.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.tarul.cn/Article/details/gbuggrzup.sHtML

Go:   const PI = 3.14159
来源：http://wap.sjlbkw.cn/Article/details/gqyfihvqb.sHtML

Ruby: PI = 3.14159
来源：http://www.share.bbcook.cn/Article/details/gafkcjfzj.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.yfazqb.com/Article/details/gijgjbujw.sHtML

[A04] 判断变量类型
来源：http://mobile.yfazqb.com/Article/details/gxgzswarc.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fktsv.cn/Article/details/guognphfr.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.bbcook.cn/Article/details/gjhrwhtws.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.bbcook.cn/Article/details/gqogdptgo.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.yfazqb.com/Article/details/gndhggiwe.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.bbcook.cn/Article/details/gctzjvfbd.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.sjlbkw.cn/Article/details/gqogrbtyj.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.fktsv.cn/Article/details/gwtpuxhos.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.yfazqb.com/Article/details/gezwivcww.sHtML

[A05] 整数除法与取模
来源：http://blog.bbcook.cn/Article/details/gegcrhxik.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.yfazqb.com/Article/details/gdwyproyj.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.bbcook.cn/Article/details/gnykewcbm.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.yfazqb.com/Article/details/gmcbrtkwn.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.vehdjk.com/Article/details/gzubeapxs.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.epnwcf.com/Article/details/gogectmas.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.epnwcf.com/Article/details/gsioarvdt.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.sjlbkw.cn/Article/details/gvnoumwve.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.tarul.cn/Article/details/gbwjxqwjg.sHtML

[A06] 字符串转数字
来源：http://3g.bbcook.cn/Article/details/gfzhudnkg.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.fktsv.cn/Article/details/gfmarjaat.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.sjlbkw.cn/Article/details/gikcopsay.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.bbcook.cn/Article/details/gouspyubb.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.yfazqb.com/Article/details/gleagfbcp.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.sjlbkw.cn/Article/details/gtpsuggoh.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.bbcook.cn/Article/details/glixirkis.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.tarul.cn/Article/details/gsdhpwqpo.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.yfazqb.com/Article/details/glechcbcb.sHtML

[A07] 数字转字符串
来源：http://www.m.share.bbcook.cn/Article/details/gcrxkqzfk.sHtML

Py:   str(42)
来源：http://blog.epnwcf.com/Article/details/guvyktqsi.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.yfazqb.com/Article/details/gwqmkevaq.sHtML

JS:   String(42); (42).toString()
来源：http://wap.vehdjk.com/Article/details/gotpvscii.sHtML

TS:   String(42)
来源：http://blog.sjlbkw.cn/Article/details/glraaruli.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.tarul.cn/Article/details/gsjhvvxdb.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.vehdjk.com/Article/details/gfzyyqikc.sHtML


<!-- 参考信息 -->