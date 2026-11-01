代发 wailian999

[U59] PHP：自定义排序
来源：http://www.blog.tarul.cn/Article/details/gwgztapbw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.sjlbkw.cn/Article/details/gzmjezmvj.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.epnwcf.com/Article/details/gmfgynoal.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.bbcook.cn/Article/details/gmcwkwqor.sHtML

[U61] PHP：正则
来源：http://read.share.yfazqb.com/Article/details/gokilrifm.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.tarul.cn/Article/details/grhjeiczo.sHtML

[U62] PHP：日期对象
来源：http://read.share.yfazqb.com/Article/details/gojvcdpfq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.tarul.cn/Article/details/giyumlhxl.sHtML

[U63] PHP：文件读写
来源：http://read.share.sjlbkw.cn/Article/details/gssvepyxv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.sjlbkw.cn/Article/details/gizeevihh.sHtML

[U64] PHP：目录遍历
来源：http://wap.epnwcf.com/Article/details/gfsoivwin.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.tarul.cn/Article/details/goppattni.sHtML

[U65] PHP：会话
来源：http://www.blog.bbcook.cn/Article/details/goaptidjg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.yfazqb.com/Article/details/ggerqxzet.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.sjlbkw.cn/Article/details/geovbilhj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fktsv.cn/Article/details/ghwspgsxd.sHtML

[U67] PHP：处理文件上传
来源：http://baike.vehdjk.com/Article/details/gwddidzjj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fktsv.cn/Article/details/gtibifrgg.sHtML

[U68] PHP：PDO 连接
来源：http://baike.bbcook.cn/Article/details/ghtjrfwmx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.sjlbkw.cn/Article/details/gsjoyzqcc.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.bbcook.cn/Article/details/gossszzbr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.tarul.cn/Article/details/gsjwabwhn.sHtML

[U70] PHP：PDO 事务
来源：http://baike.epnwcf.com/Article/details/gznfktrdh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fktsv.cn/Article/details/gslkhlohe.sHtML

[U71] PHP：抛出异常
来源：http://3g.bbcook.cn/Article/details/gmdxrfjbh.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.epnwcf.com/Article/details/gbjecqxun.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.tarul.cn/Article/details/ghkkbezlu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.bbcook.cn/Article/details/ghlewbpej.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.vehdjk.com/Article/details/gnfufesko.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.sjlbkw.cn/Article/details/ggykgtcdq.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.tarul.cn/Article/details/gcowijhgf.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.sjlbkw.cn/Article/details/geahoduep.sHtML

[U75] PHP：依赖注入
来源：http://www.share.bbcook.cn/Article/details/gliomtuwp.sHtML

composer require psr/container
来源：http://www.blog.epnwcf.com/Article/details/gbhsbbunh.sHtML

[U76] PHP：简单路由
来源：http://blog.yfazqb.com/Article/details/gampcfmpr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.vehdjk.com/Article/details/gocmduydl.sHtML

[U77] PHP：模板渲染
来源：http://read.share.yfazqb.com/Article/details/gqcoqjwpq.sHtML

composer require twig/twig
来源：http://mobile.vehdjk.com/Article/details/gjgdwlvbq.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fktsv.cn/Article/details/gmjsqqsnu.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.vehdjk.com/Article/details/gjqaqwvsy.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.epnwcf.com/Article/details/gwoepnwhi.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.epnwcf.com/Article/details/gnmhcdjor.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fktsv.cn/Article/details/gsxeeyxvn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.sjlbkw.cn/Article/details/gvybxxvor.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.yfazqb.com/Article/details/gpucbmueu.sHtML

npm init -y;  npm i express
来源：http://mobile.tarul.cn/Article/details/gbkrvpgof.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.epnwcf.com/Article/details/gnvbaabwa.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.epnwcf.com/Article/details/guydwhviz.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.vehdjk.com/Article/details/ghtljocwy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.epnwcf.com/Article/details/gbnxnldcx.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.fktsv.cn/Article/details/gcmrhowla.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.yfazqb.com/Article/details/gxpdigqvf.sHtML

[U85] JS：可选链
来源：http://www.blog.epnwcf.com/Article/details/gjylmkiep.sHtML

a?.b?.c
来源：http://wap.epnwcf.com/Article/details/giapzhfnr.sHtML

[U86] JS：空值合并
来源：http://wap.tarul.cn/Article/details/gvgfuisqk.sHtML

a ?? b
来源：http://read.share.vehdjk.com/Article/details/gzorjvhwe.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.epnwcf.com/Article/details/gdbzmufgo.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.vehdjk.com/Article/details/gumwdpayi.sHtML

[U88] JS：对象展开合并
来源：http://mobile.yfazqb.com/Article/details/gnuolhvlj.sHtML

{ ...a, ...b }
来源：http://3g.vehdjk.com/Article/details/gxkgukqfh.sHtML

[U89] JS：数组去重
来源：http://baike.bbcook.cn/Article/details/gfklihxtj.sHtML

[...new Set(arr)]
来源：http://baike.epnwcf.com/Article/details/grrxkdjcy.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.tarul.cn/Article/details/gcnuvarrq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.epnwcf.com/Article/details/gvpqacojc.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.tarul.cn/Article/details/goadbakwz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.epnwcf.com/Article/details/grqwfokjr.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.epnwcf.com/Article/details/gwwcidkjn.sHtML

structuredClone(obj)
来源：http://www.blog.vehdjk.com/Article/details/gyonvoxbf.sHtML

[U93] JS：模板字符串
来源：http://wap.sjlbkw.cn/Article/details/grhozimyf.sHtML

`共 ${n} 条`
来源：http://mobile.tarul.cn/Article/details/ggcilbwfc.sHtML

[U94] JS：箭头函数
来源：http://m.share.vehdjk.com/Article/details/ggkzvzdcp.sHtML

const double = x => x * 2;
来源：http://3g.sjlbkw.cn/Article/details/ggnrcwjmy.sHtML

[U95] JS：Promise 包装
来源：http://wap.fktsv.cn/Article/details/gqjrtolok.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.tarul.cn/Article/details/gwcdtdsyh.sHtML

[U96] JS：async/await 与异常
来源：http://baike.epnwcf.com/Article/details/gzfqlzzdm.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.vehdjk.com/Article/details/gpnnqscul.sHtML

[U97] JS：并发请求
来源：http://mobile.sjlbkw.cn/Article/details/grgnrkeao.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.vehdjk.com/Article/details/gtqzareub.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.sjlbkw.cn/Article/details/gxztmmjzk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.epnwcf.com/Article/details/gbhjcjhva.sHtML

[U99] JS：事件监听
来源：http://wap.yfazqb.com/Article/details/guidmqfdc.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.sjlbkw.cn/Article/details/gdugaitwn.sHtML

[U100] JS：DOM 查询
来源：http://baike.yfazqb.com/Article/details/gjinclovt.sHtML

document.querySelector(".item")
来源：http://read.share.fktsv.cn/Article/details/gkklohqqk.sHtML

[U101] JS：classList 操作
来源：http://m.share.fktsv.cn/Article/details/gxzlimytp.sHtML

el.classList.toggle("active")
来源：http://blog.epnwcf.com/Article/details/gprzutkhn.sHtML

[U102] JS：本地存储
来源：http://blog.tarul.cn/Article/details/gvatylsqe.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.yfazqb.com/Article/details/glohltrzf.sHtML

[U103] JS：定时器
来源：http://www.blog.tarul.cn/Article/details/gdsyrkbto.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.yfazqb.com/Article/details/gfwjqaedp.sHtML

[U104] JS：防抖
来源：http://www.share.bbcook.cn/Article/details/gbgqkyioh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.vehdjk.com/Article/details/guyzfirek.sHtML

[U105] JS：节流
来源：http://3g.bbcook.cn/Article/details/gigkcifdr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.sjlbkw.cn/Article/details/gavllmazd.sHtML

[U106] JS：日期格式化
来源：http://3g.tarul.cn/Article/details/guiltkeii.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.bbcook.cn/Article/details/gwtubdhbe.sHtML

[U107] JS：数字千分位
来源：http://www.share.bbcook.cn/Article/details/gknscsmme.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.yfazqb.com/Article/details/gvbxdmmfb.sHtML

[U108] JS：随机整数
来源：http://blog.fktsv.cn/Article/details/gdzdynmot.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.yfazqb.com/Article/details/gjcxhglbv.sHtML

[U109] JS：数组分组
来源：http://mobile.bbcook.cn/Article/details/gjgzsqszb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.vehdjk.com/Article/details/ghzqaumxl.sHtML

[U110] JS：数组分块
来源：http://www.share.sjlbkw.cn/Article/details/gdtajhqfg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.vehdjk.com/Article/details/gbzupvjvy.sHtML

[U111] JS：对象转 Map
来源：http://3g.yfazqb.com/Article/details/guvzcnwqs.sHtML

new Map(Object.entries(obj))
来源：http://baike.bbcook.cn/Article/details/gbsuewytj.sHtML

[U112] JS：字符串补位
来源：http://read.share.fktsv.cn/Article/details/gqudovlca.sHtML

"7".padStart(3, "0")
来源：http://read.share.epnwcf.com/Article/details/gdljdrfkf.sHtML

[U113] JS：正则替换全部
来源：http://m.share.epnwcf.com/Article/details/gmkkznfdf.sHtML

s.replaceAll("a", "b")
来源：http://m.share.bbcook.cn/Article/details/guwfxhdqp.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gjzfkcgdz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.epnwcf.com/Article/details/gxoecndpe.sHtML

[U115] JS：生成 UUID
来源：http://baike.yfazqb.com/Article/details/gjusqfuns.sHtML

crypto.randomUUID()
来源：http://www.m.share.yfazqb.com/Article/details/gxphrvqwg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fktsv.cn/Article/details/gcwthbmyb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.sjlbkw.cn/Article/details/gairrzhao.sHtML

[U117] JS：单元测试
来源：http://m.share.epnwcf.com/Article/details/gwnktcshk.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.epnwcf.com/Article/details/geykdaqsf.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.yfazqb.com/Article/details/gsqtuhosn.sHtML

npm i -D vite;  npx vite
来源：http://wap.tarul.cn/Article/details/gcayywizh.sHtML

[U119] JS：生产构建
来源：http://3g.epnwcf.com/Article/details/gaigjpdkq.sHtML

npx vite build
来源：http://www.blog.bbcook.cn/Article/details/gkqowjyeh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.epnwcf.com/Article/details/gcnitpazb.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.epnwcf.com/Article/details/gbbnrqclj.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gdlucgmpl.sHtML

统计汇总
来源：http://mobile.epnwcf.com/Article/details/gqudjkctg.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/ghgagvmlx.sHtML

按语言统计（条）：
来源：http://blog.yfazqb.com/Article/details/gpwksmkwa.sHtML

Python ......... 252
来源：http://read.share.bbcook.cn/Article/details/gamfxemlf.sHtML

PHP ............ 252
来源：http://www.share.fktsv.cn/Article/details/glpvgnofd.sHtML

JavaScript ..... 252
来源：http://wap.bbcook.cn/Article/details/grfxkcuwb.sHtML

TypeScript ..... 212
来源：http://www.blog.yfazqb.com/Article/details/gwgduptqm.sHtML

Java ........... 212
来源：http://www.m.share.bbcook.cn/Article/details/gpopkqbfm.sHtML

Go ............. 212
来源：http://read.share.vehdjk.com/Article/details/gpucwenfa.sHtML

Ruby ........... 212
来源：http://www.blog.tarul.cn/Article/details/gktazpism.sHtML

C# ............. 212
来源：http://wap.fktsv.cn/Article/details/giqhccjiz.sHtML

C .............. 30
来源：http://read.share.tarul.cn/Article/details/gszvvfqou.sHtML

C++ ............ 30
来源：http://baike.bbcook.cn/Article/details/gwervidkz.sHtML

SQL ............ 90
来源：http://www.share.epnwcf.com/Article/details/gknmkxcjm.sHtML

Bash ........... 80
来源：http://www.blog.yfazqb.com/Article/details/gxqpqthkc.sHtML

Kotlin ......... 15
来源：http://baike.fktsv.cn/Article/details/ggxzvimaj.sHtML

Swift .......... 15
来源：http://baike.vehdjk.com/Article/details/ghcwlnbzc.sHtML

Lua ............ 10
来源：http://www.share.tarul.cn/Article/details/ggtswswwh.sHtML

Perl ........... 10
来源：http://www.m.share.tarul.cn/Article/details/gxwzgyxop.sHtML

Scala .......... 10
来源：http://www.blog.yfazqb.com/Article/details/gbepsndic.sHtML

------------------------------------
来源：http://baike.epnwcf.com/Article/details/ggpixwlcu.sHtML

合计 ........... 2106 条
来源：http://blog.tarul.cn/Article/details/gtqxfjjmm.sHtML

按章节统计：
来源：http://blog.epnwcf.com/Article/details/gguqkzxma.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.bbcook.cn/Article/details/ggraffhod.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.vehdjk.com/Article/details/gpdflzgin.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.tarul.cn/Article/details/gdzxfmosm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fktsv.cn/Article/details/gkvbemrpf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.epnwcf.com/Article/details/gezabxfhk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.bbcook.cn/Article/details/gkjuywqdh.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fktsv.cn/Article/details/gfkugnzek.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.bbcook.cn/Article/details/gbfnguill.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.yfazqb.com/Article/details/gtrebxirr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.epnwcf.com/Article/details/gcedwhram.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.bbcook.cn/Article/details/ghtrubdcb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.tarul.cn/Article/details/gpllkexzy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.yfazqb.com/Article/details/gpvicmmsu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fktsv.cn/Article/details/glkcopfge.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.yfazqb.com/Article/details/gzrplkinn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.yfazqb.com/Article/details/gfvytnkvm.sHtML

Q SQL 专题                              90
来源：http://blog.fktsv.cn/Article/details/ghttyedrv.sHtML

R Bash 专题                             80
来源：http://read.share.tarul.cn/Article/details/grheczwdr.sHtML

S C / C++ 专题                          60
来源：http://wap.sjlbkw.cn/Article/details/gdayrxola.sHtML

T 其他语言补充                          60
来源：http://blog.vehdjk.com/Article/details/ghlyuxtdw.sHtML

U 高频实用片段                         120
来源：http://www.blog.sjlbkw.cn/Article/details/gcggngits.sHtML

------------------------------------
来源：http://read.share.tarul.cn/Article/details/govqzxrdv.sHtML

合计                                  2106 条
来源：http://3g.epnwcf.com/Article/details/gzfjzrdow.sHtML

--------------------------------------------------------------------------------
来源：http://3g.sjlbkw.cn/Article/details/gdxftgyfh.sHtML

使用提醒
来源：http://www.blog.bbcook.cn/Article/details/gflaiqqyw.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.sjlbkw.cn/Article/details/guazztpjy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.sjlbkw.cn/Article/details/gycahvkau.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.sjlbkw.cn/Article/details/gdwfymvgz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.yfazqb.com/Article/details/gxdxxmzua.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fktsv.cn/Article/details/gehypbkvt.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.vehdjk.com/Article/details/giwwinryd.sHtML

—— 文件结束 ——
来源：http://mobile.tarul.cn/Article/details/gfcdkfxnc.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gfplaftlt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.epnwcf.com/Article/details/gwoequinh.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.bbcook.cn/Article/details/gdfelepor.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gexxxuram.sHtML

【收录内容】
来源：http://read.share.bbcook.cn/Article/details/gidmlprvj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.tarul.cn/Article/details/grfqhzbdb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.yfazqb.com/Article/details/gxuvuoeyc.sHtML

SQL · Bash · C · C++
来源：http://www.share.tarul.cn/Article/details/gbzfyxrxe.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.vehdjk.com/Article/details/gvmxouxgl.sHtML

【使用说明】
来源：http://www.share.sjlbkw.cn/Article/details/gaffgzskk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.vehdjk.com/Article/details/gebvtofcn.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.bbcook.cn/Article/details/guvbtzscm.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.vehdjk.com/Article/details/gttacquvw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.sjlbkw.cn/Article/details/gxazudunz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.yfazqb.com/Article/details/gdgmnizkq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.sjlbkw.cn/Article/details/gxadysoys.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fktsv.cn/Article/details/ghqukcqqi.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.epnwcf.com/Article/details/goweywmuy.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.vehdjk.com/Article/details/gyvgzbhlk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.tarul.cn/Article/details/glwndxxob.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.vehdjk.com/Article/details/gvatkznff.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.yfazqb.com/Article/details/gxsgskfxj.sHtML

【文件统计】
来源：http://wap.bbcook.cn/Article/details/gjedyuyqj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.yfazqb.com/Article/details/gegtrbfmr.sHtML

--------------------------------------------------------------------------------
来源：http://baike.sjlbkw.cn/Article/details/ggyxtfczd.sHtML

目  录
来源：http://m.share.tarul.cn/Article/details/guxbmhium.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.vehdjk.com/Article/details/gskhggbhk.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.vehdjk.com/Article/details/gbzstxcqc.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.sjlbkw.cn/Article/details/gbrqwdlwk.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.bbcook.cn/Article/details/girhzwmbw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.vehdjk.com/Article/details/gxgrysxua.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.epnwcf.com/Article/details/gtukrebri.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.epnwcf.com/Article/details/gcumclked.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.sjlbkw.cn/Article/details/gmxjltsux.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fktsv.cn/Article/details/gtdcmcmmg.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.sjlbkw.cn/Article/details/gupovdejx.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.yfazqb.com/Article/details/geotvszqp.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.bbcook.cn/Article/details/gjdxjonjf.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.tarul.cn/Article/details/gyhzpwqfd.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gfxcvdjvt.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.epnwcf.com/Article/details/gnanyamjb.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.fktsv.cn/Article/details/gdaniypxk.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.epnwcf.com/Article/details/gwufcbjzm.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.vehdjk.com/Article/details/gwenijdfg.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.epnwcf.com/Article/details/goozbfxxu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.bbcook.cn/Article/details/gyazkxrsp.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fktsv.cn/Article/details/gbbfieoki.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.tarul.cn/Article/details/ghzzxdxqg.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gjtqnejzc.sHtML

A. 基础语法与类型
来源：http://www.blog.vehdjk.com/Article/details/gvgbfencn.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gtnvdylza.sHtML

[A01] Hello World
来源：http://mobile.vehdjk.com/Article/details/gfbzwswif.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.fktsv.cn/Article/details/gulgilyio.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.yfazqb.com/Article/details/gmxbmrmqc.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.vehdjk.com/Article/details/gjbbdbktc.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.yfazqb.com/Article/details/gbjwyqyjm.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.fktsv.cn/Article/details/gzslmsjbm.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.vehdjk.com/Article/details/gterzwwrq.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.sjlbkw.cn/Article/details/gaxsvnski.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.epnwcf.com/Article/details/gnifkftyf.sHtML

[A02] 变量声明与赋值
来源：http://www.share.sjlbkw.cn/Article/details/gjqsnfnxm.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fktsv.cn/Article/details/gopyjhxel.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.epnwcf.com/Article/details/gwhbgkdhx.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.tarul.cn/Article/details/glacysivk.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.tarul.cn/Article/details/geuwsoumj.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.yfazqb.com/Article/details/ghfijzgia.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.vehdjk.com/Article/details/gseraxbac.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.sjlbkw.cn/Article/details/gpvjjaqfa.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.sjlbkw.cn/Article/details/grxuurmax.sHtML

[A03] 常量定义
来源：http://mobile.tarul.cn/Article/details/gcogvtzyc.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.tarul.cn/Article/details/gearpmdvs.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gfjmxztyb.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.vehdjk.com/Article/details/gzsnqwzvc.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.yfazqb.com/Article/details/gbtlgfbfy.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.vehdjk.com/Article/details/gwprsjvvp.sHtML

Go:   const PI = 3.14159
来源：http://baike.bbcook.cn/Article/details/gwquvxgiz.sHtML

Ruby: PI = 3.14159
来源：http://3g.sjlbkw.cn/Article/details/gcnbwythz.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/gvxjsbiux.sHtML

[A04] 判断变量类型
来源：http://www.share.vehdjk.com/Article/details/gwxuhujmu.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.bbcook.cn/Article/details/gmyewotba.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.sjlbkw.cn/Article/details/gcntjofch.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.epnwcf.com/Article/details/gdecqrkup.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.sjlbkw.cn/Article/details/gaijksnup.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.yfazqb.com/Article/details/gmevmbxhk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.vehdjk.com/Article/details/gjgfpqqzy.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.sjlbkw.cn/Article/details/gtrxeyhog.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.tarul.cn/Article/details/ghafptkyw.sHtML

[A05] 整数除法与取模
来源：http://www.blog.fktsv.cn/Article/details/gpcuaugfr.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.epnwcf.com/Article/details/ggexlcjmb.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.sjlbkw.cn/Article/details/ghfwuutnr.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.sjlbkw.cn/Article/details/gtraopbte.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fktsv.cn/Article/details/grafupggj.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.yfazqb.com/Article/details/ggislywyx.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.yfazqb.com/Article/details/gbnlmhkaf.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.fktsv.cn/Article/details/ghutewddc.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.tarul.cn/Article/details/gmzpzmgqs.sHtML

[A06] 字符串转数字
来源：http://www.share.tarul.cn/Article/details/ggxjkkyeo.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.epnwcf.com/Article/details/gmlrxtith.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.vehdjk.com/Article/details/gexgffaek.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.vehdjk.com/Article/details/gkujjqfqo.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.epnwcf.com/Article/details/gydogooxe.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxndrlhhi.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.tarul.cn/Article/details/ggcjattex.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.epnwcf.com/Article/details/gpkrxysbo.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.vehdjk.com/Article/details/gwieszshz.sHtML

[A07] 数字转字符串
来源：http://mobile.yfazqb.com/Article/details/gduqnyxxs.sHtML

Py:   str(42)
来源：http://mobile.vehdjk.com/Article/details/gnyoomrmn.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.epnwcf.com/Article/details/gnghbuvzt.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.fktsv.cn/Article/details/gxlpamfpm.sHtML

TS:   String(42)
来源：http://read.share.fktsv.cn/Article/details/gpztdbrku.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.sjlbkw.cn/Article/details/gsumiulnc.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.epnwcf.com/Article/details/gygqeeoyv.sHtML

Ruby: 42.to_s
来源：http://www.blog.bbcook.cn/Article/details/guyqwojnj.sHtML

C#:   42.ToString()
来源：http://blog.yfazqb.com/Article/details/gxymsdhgm.sHtML

[A08] 取整与四舍五入
来源：http://baike.tarul.cn/Article/details/gmpuncmjn.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.bbcook.cn/Article/details/gqlpmwxdm.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.tarul.cn/Article/details/grwmxermy.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.epnwcf.com/Article/details/gpsielkzj.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.sjlbkw.cn/Article/details/glsmpgmdu.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.vehdjk.com/Article/details/gqgqjqnez.sHtML


<!-- 参考信息 -->