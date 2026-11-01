代发 wailian999

[U55] PHP：match 表达式
来源：http://blog.epnwcf.com/Article/details/gjbiwzolt.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.fktsv.cn/Article/details/gapqveedz.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.yfazqb.com/Article/details/gnqfzezfz.sHtML

f(a: 1, b: 2)
来源：http://3g.vehdjk.com/Article/details/ghvrrfpog.sHtML

[U57] PHP：字符串插值
来源：http://baike.sjlbkw.cn/Article/details/gihnimdgc.sHtML

"值: {$a}"
来源：http://mobile.tarul.cn/Article/details/gamosumwe.sHtML

[U58] PHP：数组三件套
来源：http://mobile.sjlbkw.cn/Article/details/gvyhegbju.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.share.sjlbkw.cn/Article/details/gjnyaquiq.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.bbcook.cn/Article/details/grxbitruu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.epnwcf.com/Article/details/gcebmcdvf.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.epnwcf.com/Article/details/gkpsxkjps.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.bbcook.cn/Article/details/gsyfeksfe.sHtML

[U61] PHP：正则
来源：http://m.share.epnwcf.com/Article/details/gbtsrvpgz.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.tarul.cn/Article/details/gygffvqqd.sHtML

[U62] PHP：日期对象
来源：http://baike.vehdjk.com/Article/details/gjtcnlesd.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.bbcook.cn/Article/details/gzgyagelw.sHtML

[U63] PHP：文件读写
来源：http://blog.bbcook.cn/Article/details/gxxtkbzjq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.vehdjk.com/Article/details/gemomdlxx.sHtML

[U64] PHP：目录遍历
来源：http://read.share.vehdjk.com/Article/details/glzeimyha.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.yfazqb.com/Article/details/gyaptnnrp.sHtML

[U65] PHP：会话
来源：http://3g.sjlbkw.cn/Article/details/gsanimbgv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.vehdjk.com/Article/details/ghqsiirvv.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.vehdjk.com/Article/details/gnrjkegix.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.tarul.cn/Article/details/gvxacwqws.sHtML

[U67] PHP：处理文件上传
来源：http://baike.tarul.cn/Article/details/gkcywpqvd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.yfazqb.com/Article/details/grujahbdo.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.epnwcf.com/Article/details/gxaclauhp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.epnwcf.com/Article/details/gwkjukhqj.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.vehdjk.com/Article/details/gyxzshiuy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.yfazqb.com/Article/details/gbssjvwcn.sHtML

[U70] PHP：PDO 事务
来源：http://baike.epnwcf.com/Article/details/gooqbdhjl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.yfazqb.com/Article/details/ghiaywjez.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.tarul.cn/Article/details/gprczntkg.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.epnwcf.com/Article/details/gogltrtjv.sHtML

[U72] PHP：写错误日志
来源：http://wap.tarul.cn/Article/details/gvvzvlxhz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.vehdjk.com/Article/details/gogwgakuk.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.sjlbkw.cn/Article/details/gpeipvyxd.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.yfazqb.com/Article/details/gykfgkxbn.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fktsv.cn/Article/details/gmtkuazff.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.fktsv.cn/Article/details/girglkowr.sHtML

[U75] PHP：依赖注入
来源：http://wap.vehdjk.com/Article/details/gpilftfva.sHtML

composer require psr/container
来源：http://mobile.epnwcf.com/Article/details/gvjdxoejk.sHtML

[U76] PHP：简单路由
来源：http://blog.vehdjk.com/Article/details/gvgyfnikk.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.yfazqb.com/Article/details/gaqjmziei.sHtML

[U77] PHP：模板渲染
来源：http://mobile.yfazqb.com/Article/details/gatfdovbt.sHtML

composer require twig/twig
来源：http://www.m.share.epnwcf.com/Article/details/gxzpacroe.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fktsv.cn/Article/details/gfsnwdoan.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fktsv.cn/Article/details/ggunfrzxc.sHtML

[U79] PHP：静态分析
来源：http://www.share.fktsv.cn/Article/details/gpvgeguhw.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.sjlbkw.cn/Article/details/grfmcnsly.sHtML

[U80] PHP：代码规范修复
来源：http://3g.tarul.cn/Article/details/gslnksmmy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.sjlbkw.cn/Article/details/gesrmqiyq.sHtML

[U81] JS：初始化项目
来源：http://www.blog.epnwcf.com/Article/details/glqxacsno.sHtML

npm init -y;  npm i express
来源：http://read.share.fktsv.cn/Article/details/gktcmbvkf.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.epnwcf.com/Article/details/gxtzakvrz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.bbcook.cn/Article/details/gaaveynqf.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.bbcook.cn/Article/details/ggxrhdkff.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.epnwcf.com/Article/details/gxymhvbnd.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.sjlbkw.cn/Article/details/gsvpjjmbt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fktsv.cn/Article/details/gpxgboewy.sHtML

[U85] JS：可选链
来源：http://m.share.sjlbkw.cn/Article/details/gszyqbufr.sHtML

a?.b?.c
来源：http://m.share.tarul.cn/Article/details/gfbeyekbf.sHtML

[U86] JS：空值合并
来源：http://m.share.tarul.cn/Article/details/glixriacd.sHtML

a ?? b
来源：http://wap.vehdjk.com/Article/details/gwsylbxgf.sHtML

[U87] JS：解构默认值
来源：http://m.share.vehdjk.com/Article/details/gsygxpovf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.bbcook.cn/Article/details/gjzoflqvn.sHtML

[U88] JS：对象展开合并
来源：http://3g.epnwcf.com/Article/details/gsrjcsbvb.sHtML

{ ...a, ...b }
来源：http://www.m.share.epnwcf.com/Article/details/gtwvdopxr.sHtML

[U89] JS：数组去重
来源：http://m.share.bbcook.cn/Article/details/gapqrsery.sHtML

[...new Set(arr)]
来源：http://baike.fktsv.cn/Article/details/gcgvrhash.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.epnwcf.com/Article/details/gnudukegb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.tarul.cn/Article/details/gczepxfct.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.yfazqb.com/Article/details/guqwcjdxz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.sjlbkw.cn/Article/details/gdzzyjppg.sHtML

[U92] JS：深拷贝
来源：http://baike.yfazqb.com/Article/details/glllciqhq.sHtML

structuredClone(obj)
来源：http://www.blog.vehdjk.com/Article/details/gwgldnlvx.sHtML

[U93] JS：模板字符串
来源：http://mobile.yfazqb.com/Article/details/gdwgkerdn.sHtML

`共 ${n} 条`
来源：http://read.share.fktsv.cn/Article/details/gdmdiswvq.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.yfazqb.com/Article/details/gxcfabucr.sHtML

const double = x => x * 2;
来源：http://mobile.yfazqb.com/Article/details/gjlhkukzx.sHtML

[U95] JS：Promise 包装
来源：http://baike.epnwcf.com/Article/details/gpkogznrb.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fktsv.cn/Article/details/gmunevmvn.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.yfazqb.com/Article/details/gzjedxakn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.sjlbkw.cn/Article/details/gjmujemyz.sHtML

[U97] JS：并发请求
来源：http://www.share.tarul.cn/Article/details/gykuplgui.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.sjlbkw.cn/Article/details/gryyjflvw.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.epnwcf.com/Article/details/glupyjeak.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fktsv.cn/Article/details/ggpudwnkw.sHtML

[U99] JS：事件监听
来源：http://m.share.yfazqb.com/Article/details/gzvznalpp.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fktsv.cn/Article/details/gsloxltgd.sHtML

[U100] JS：DOM 查询
来源：http://wap.tarul.cn/Article/details/grlntcqaz.sHtML

document.querySelector(".item")
来源：http://read.share.yfazqb.com/Article/details/gcekctske.sHtML

[U101] JS：classList 操作
来源：http://baike.bbcook.cn/Article/details/geudrxpmt.sHtML

el.classList.toggle("active")
来源：http://www.share.fktsv.cn/Article/details/gnpueybpb.sHtML

[U102] JS：本地存储
来源：http://3g.yfazqb.com/Article/details/gnuajioyf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.sjlbkw.cn/Article/details/gvpzpbpoj.sHtML

[U103] JS：定时器
来源：http://3g.fktsv.cn/Article/details/gdqqtsxnw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.tarul.cn/Article/details/gtedajlaq.sHtML

[U104] JS：防抖
来源：http://baike.yfazqb.com/Article/details/gjqwdzhdc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.vehdjk.com/Article/details/gqczoqmlj.sHtML

[U105] JS：节流
来源：http://blog.tarul.cn/Article/details/gvwphypva.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fktsv.cn/Article/details/gvshplmti.sHtML

[U106] JS：日期格式化
来源：http://blog.sjlbkw.cn/Article/details/ggcgrgrkm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fktsv.cn/Article/details/gbcrtergj.sHtML

[U107] JS：数字千分位
来源：http://3g.sjlbkw.cn/Article/details/gqfxlddcz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.vehdjk.com/Article/details/gctylcjkv.sHtML

[U108] JS：随机整数
来源：http://read.share.vehdjk.com/Article/details/gpzsqjjug.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.epnwcf.com/Article/details/gycbizsvy.sHtML

[U109] JS：数组分组
来源：http://baike.bbcook.cn/Article/details/gblpdwpmk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.yfazqb.com/Article/details/gahggyrij.sHtML

[U110] JS：数组分块
来源：http://wap.sjlbkw.cn/Article/details/glfrzivhb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.yfazqb.com/Article/details/gpppolmkw.sHtML

[U111] JS：对象转 Map
来源：http://m.share.tarul.cn/Article/details/grmsenfhh.sHtML

new Map(Object.entries(obj))
来源：http://www.share.yfazqb.com/Article/details/gfdqhdpyu.sHtML

[U112] JS：字符串补位
来源：http://mobile.sjlbkw.cn/Article/details/grlduihlt.sHtML

"7".padStart(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/ggydracta.sHtML

[U113] JS：正则替换全部
来源：http://3g.bbcook.cn/Article/details/geqhsxqld.sHtML

s.replaceAll("a", "b")
来源：http://3g.yfazqb.com/Article/details/glnwakecl.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.vehdjk.com/Article/details/goergfosn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.vehdjk.com/Article/details/gwxqrafaa.sHtML

[U115] JS：生成 UUID
来源：http://baike.epnwcf.com/Article/details/gqqeadsfl.sHtML

crypto.randomUUID()
来源：http://www.blog.tarul.cn/Article/details/gyqrizcws.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.epnwcf.com/Article/details/gkudjowxl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.epnwcf.com/Article/details/gqavsyusq.sHtML

[U117] JS：单元测试
来源：http://www.share.yfazqb.com/Article/details/gypmujwlj.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.vehdjk.com/Article/details/gxzgmmiri.sHtML

[U118] JS：开发服务器
来源：http://m.share.epnwcf.com/Article/details/gykozgpka.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fktsv.cn/Article/details/gqhjiqbro.sHtML

[U119] JS：生产构建
来源：http://blog.bbcook.cn/Article/details/gennesfhi.sHtML

npx vite build
来源：http://mobile.epnwcf.com/Article/details/gaxiikocg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.epnwcf.com/Article/details/gblbwccxv.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.sjlbkw.cn/Article/details/giaqwappm.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gkrekryvy.sHtML

统计汇总
来源：http://m.share.tarul.cn/Article/details/glguziasy.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/ggxhiojky.sHtML

按语言统计（条）：
来源：http://baike.tarul.cn/Article/details/ghxmcpzct.sHtML

Python ......... 252
来源：http://3g.tarul.cn/Article/details/gbsxnklmu.sHtML

PHP ............ 252
来源：http://www.blog.tarul.cn/Article/details/gvuqslccp.sHtML

JavaScript ..... 252
来源：http://m.share.yfazqb.com/Article/details/gwnkcqwvn.sHtML

TypeScript ..... 212
来源：http://baike.vehdjk.com/Article/details/gvlshxstx.sHtML

Java ........... 212
来源：http://blog.yfazqb.com/Article/details/gedwucpxo.sHtML

Go ............. 212
来源：http://read.share.yfazqb.com/Article/details/glheaqdby.sHtML

Ruby ........... 212
来源：http://m.share.vehdjk.com/Article/details/gsnzelzwv.sHtML

C# ............. 212
来源：http://www.m.share.tarul.cn/Article/details/gcoxhapjg.sHtML

C .............. 30
来源：http://www.share.bbcook.cn/Article/details/gsgljfjhx.sHtML

C++ ............ 30
来源：http://baike.vehdjk.com/Article/details/gcnrugakr.sHtML

SQL ............ 90
来源：http://blog.bbcook.cn/Article/details/gnvsolyrv.sHtML

Bash ........... 80
来源：http://3g.vehdjk.com/Article/details/gwtzofphi.sHtML

Kotlin ......... 15
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbtibysp.sHtML

Swift .......... 15
来源：http://www.share.bbcook.cn/Article/details/gzquhnmwx.sHtML

Lua ............ 10
来源：http://baike.sjlbkw.cn/Article/details/gpjzacfas.sHtML

Perl ........... 10
来源：http://wap.epnwcf.com/Article/details/gvwkuvddc.sHtML

Scala .......... 10
来源：http://www.share.epnwcf.com/Article/details/gsjvlhoay.sHtML

------------------------------------
来源：http://m.share.vehdjk.com/Article/details/gjjvykfwy.sHtML

合计 ........... 2106 条
来源：http://baike.tarul.cn/Article/details/geauibbzj.sHtML

按章节统计：
来源：http://mobile.yfazqb.com/Article/details/gecowpcgm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.tarul.cn/Article/details/gkunykeun.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.bbcook.cn/Article/details/grbepaazo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fktsv.cn/Article/details/gwtzqnuxu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.sjlbkw.cn/Article/details/gvlawxeyi.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.bbcook.cn/Article/details/gmlpzwaus.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.bbcook.cn/Article/details/glgiscjaj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.epnwcf.com/Article/details/gxvipelor.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.tarul.cn/Article/details/gznozatqk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.vehdjk.com/Article/details/gbrcletah.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.yfazqb.com/Article/details/gmwiqdgui.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.epnwcf.com/Article/details/gmxrloohy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fktsv.cn/Article/details/gwgtqonvx.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fktsv.cn/Article/details/grijmzxsu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.yfazqb.com/Article/details/gqrtilrfg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fktsv.cn/Article/details/gnahevahw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.vehdjk.com/Article/details/gzyrtrppo.sHtML

Q SQL 专题                              90
来源：http://blog.bbcook.cn/Article/details/gaqrcytyu.sHtML

R Bash 专题                             80
来源：http://3g.tarul.cn/Article/details/gnbzkuiji.sHtML

S C / C++ 专题                          60
来源：http://3g.epnwcf.com/Article/details/gudqzttqy.sHtML

T 其他语言补充                          60
来源：http://blog.vehdjk.com/Article/details/gmixelvum.sHtML

U 高频实用片段                         120
来源：http://www.share.yfazqb.com/Article/details/gegvfcfjv.sHtML

------------------------------------
来源：http://read.share.tarul.cn/Article/details/gfbokxybk.sHtML

合计                                  2106 条
来源：http://read.share.bbcook.cn/Article/details/gbilgqotr.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.yfazqb.com/Article/details/gnwgjygrl.sHtML

使用提醒
来源：http://baike.tarul.cn/Article/details/ghqchfxkk.sHtML

--------------------------------------------------------------------------------
来源：http://baike.epnwcf.com/Article/details/gaauruyex.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.bbcook.cn/Article/details/gslivetlt.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.epnwcf.com/Article/details/gzylqvxgb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.vehdjk.com/Article/details/gecitwtka.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.tarul.cn/Article/details/gzkopmrsm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.tarul.cn/Article/details/gavwrnhks.sHtML

—— 文件结束 ——
来源：http://read.share.epnwcf.com/Article/details/gqmbzgggi.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gttwzgltk.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.epnwcf.com/Article/details/gbgjyiwge.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.sjlbkw.cn/Article/details/ghmnoxpfn.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gwdaamgqd.sHtML

【收录内容】
来源：http://m.share.vehdjk.com/Article/details/gwsjurmrj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.tarul.cn/Article/details/gvuhrwwra.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.tarul.cn/Article/details/gqeazrchk.sHtML

SQL · Bash · C · C++
来源：http://m.share.vehdjk.com/Article/details/gkgqpuwxf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.vehdjk.com/Article/details/glzmieiup.sHtML

【使用说明】
来源：http://3g.sjlbkw.cn/Article/details/gbmwgczrf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.vehdjk.com/Article/details/gpvgcqtqo.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fktsv.cn/Article/details/gbjngtqyj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.bbcook.cn/Article/details/gsmeqjicb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.yfazqb.com/Article/details/gwalouyrq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.vehdjk.com/Article/details/gfubqjvos.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.tarul.cn/Article/details/gnxrldpav.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.epnwcf.com/Article/details/gralusqmo.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.sjlbkw.cn/Article/details/gcesbpfdg.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.vehdjk.com/Article/details/gqjbzsqwj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.bbcook.cn/Article/details/gclwwatrh.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.epnwcf.com/Article/details/ggdrbohvj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.vehdjk.com/Article/details/gpbzubkpo.sHtML

【文件统计】
来源：http://wap.bbcook.cn/Article/details/gwelcdasf.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.sjlbkw.cn/Article/details/gltjkyvww.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.vehdjk.com/Article/details/gwwlxsahf.sHtML

目  录
来源：http://read.share.tarul.cn/Article/details/gterlnthi.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.bbcook.cn/Article/details/gknmhugzo.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.epnwcf.com/Article/details/gepxbntzv.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.sjlbkw.cn/Article/details/gbxeiozwa.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.epnwcf.com/Article/details/geqgvcmkc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.yfazqb.com/Article/details/gagjyeutx.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.bbcook.cn/Article/details/gdlijdgko.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gzdqkjvob.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.sjlbkw.cn/Article/details/gmtmojihq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.tarul.cn/Article/details/gopayedyv.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.bbcook.cn/Article/details/gkzxrzxpr.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.tarul.cn/Article/details/gmcoxjxzt.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fktsv.cn/Article/details/gdrbpaxxd.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.epnwcf.com/Article/details/groznfqga.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.epnwcf.com/Article/details/gcazudzbt.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.epnwcf.com/Article/details/gxolhhlnb.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.yfazqb.com/Article/details/ghquiwaol.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.fktsv.cn/Article/details/gtlzrblfo.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.vehdjk.com/Article/details/gpivgawnk.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.yfazqb.com/Article/details/ghtpivqxh.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.tarul.cn/Article/details/gwtmgncwa.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.bbcook.cn/Article/details/gkrftaobh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.bbcook.cn/Article/details/gsghvavqk.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gozvzymuq.sHtML

A. 基础语法与类型
来源：http://blog.sjlbkw.cn/Article/details/glzsjhryv.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gtbzwjnai.sHtML

[A01] Hello World
来源：http://read.share.sjlbkw.cn/Article/details/gdcyghthi.sHtML

Py:   print("Hello, World!")
来源：http://wap.yfazqb.com/Article/details/gatefuiem.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.bbcook.cn/Article/details/gfnqwfhtr.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.bbcook.cn/Article/details/gtjaesrfa.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.epnwcf.com/Article/details/gxdclific.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.tarul.cn/Article/details/gvfllticg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.epnwcf.com/Article/details/goajgudxq.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.tarul.cn/Article/details/gudrrrycl.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.fktsv.cn/Article/details/gxadrqemo.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.fktsv.cn/Article/details/grkoxlvky.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.yfazqb.com/Article/details/gowjnrkbe.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.fktsv.cn/Article/details/gprormaxs.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.vehdjk.com/Article/details/gfuaixhik.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.vehdjk.com/Article/details/giwaqiuul.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.yfazqb.com/Article/details/ggxjqnmbk.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.yfazqb.com/Article/details/ggckpzkkf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.tarul.cn/Article/details/gajmohuop.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.fktsv.cn/Article/details/gmxzogvva.sHtML

[A03] 常量定义
来源：http://www.share.epnwcf.com/Article/details/gtyvgnvcu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.yfazqb.com/Article/details/goaxcmcpc.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/ghvskowvk.sHtML

JS:   const PI = 3.14159;
来源：http://baike.epnwcf.com/Article/details/gvlyaofbz.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.epnwcf.com/Article/details/gvsoswhzp.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gifzhetbd.sHtML

Go:   const PI = 3.14159
来源：http://blog.epnwcf.com/Article/details/gtjqjoafq.sHtML

Ruby: PI = 3.14159
来源：http://wap.fktsv.cn/Article/details/gxbeitchq.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.epnwcf.com/Article/details/gdqwyhkqt.sHtML

[A04] 判断变量类型
来源：http://m.share.sjlbkw.cn/Article/details/giwfhekql.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.yfazqb.com/Article/details/gjmwsgpmz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.vehdjk.com/Article/details/guurgvzyz.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.tarul.cn/Article/details/gflswukfv.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.vehdjk.com/Article/details/gujenjyei.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.yfazqb.com/Article/details/gpshyvxqh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.tarul.cn/Article/details/giiquauwb.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.fktsv.cn/Article/details/gpsjfbjsk.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.tarul.cn/Article/details/gqnkiksrf.sHtML

[A05] 整数除法与取模
来源：http://wap.sjlbkw.cn/Article/details/ganyhjupj.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.vehdjk.com/Article/details/ggxuwxahj.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.vehdjk.com/Article/details/gtakpmufi.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.tarul.cn/Article/details/gapclcois.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.tarul.cn/Article/details/gznakfqpu.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.yfazqb.com/Article/details/gzilnmfki.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.tarul.cn/Article/details/gpbqawxms.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.epnwcf.com/Article/details/grrxggumu.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.vehdjk.com/Article/details/gwnheysxv.sHtML

[A06] 字符串转数字
来源：http://www.blog.vehdjk.com/Article/details/ggzsupkgk.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.bbcook.cn/Article/details/gcmvqcbzg.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.sjlbkw.cn/Article/details/guddidvyy.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.epnwcf.com/Article/details/gjjeimsfr.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.epnwcf.com/Article/details/gkhecpvee.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.yfazqb.com/Article/details/gdtuwzwdo.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.tarul.cn/Article/details/gctumztce.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.vehdjk.com/Article/details/gkuxmflvu.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.vehdjk.com/Article/details/gfbdyoxsl.sHtML

[A07] 数字转字符串
来源：http://blog.tarul.cn/Article/details/gexsunnbx.sHtML

Py:   str(42)
来源：http://baike.vehdjk.com/Article/details/gzxixqati.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.sjlbkw.cn/Article/details/gozcgxlog.sHtML

JS:   String(42); (42).toString()
来源：http://blog.sjlbkw.cn/Article/details/gpyxxhdiw.sHtML

TS:   String(42)
来源：http://read.share.epnwcf.com/Article/details/gtdxilcpd.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.yfazqb.com/Article/details/gnwuuliyp.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.epnwcf.com/Article/details/gnskhjmsn.sHtML


<!-- 参考信息 -->