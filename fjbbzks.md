代发 wailian999

[U53] PHP：空合并运算符
来源：http://mobile.epnwcf.com/Article/details/gponnxbzm.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.tarul.cn/Article/details/gcajqkepl.sHtML

[U54] PHP：空安全调用
来源：http://baike.yfazqb.com/Article/details/gedomwxcz.sHtML

$obj?->method()
来源：http://wap.tarul.cn/Article/details/gwgpqxwyn.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.tarul.cn/Article/details/ghifavrbi.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.bbcook.cn/Article/details/gaauekxoh.sHtML

[U56] PHP：命名参数
来源：http://wap.epnwcf.com/Article/details/gjzmkrkql.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fktsv.cn/Article/details/gxwaibvcz.sHtML

[U57] PHP：字符串插值
来源：http://wap.vehdjk.com/Article/details/gplbiyiys.sHtML

"值: {$a}"
来源：http://m.share.sjlbkw.cn/Article/details/gcuampooc.sHtML

[U58] PHP：数组三件套
来源：http://mobile.fktsv.cn/Article/details/gdivzbeaj.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.epnwcf.com/Article/details/gnlarehec.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.epnwcf.com/Article/details/gyobrzmzu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.tarul.cn/Article/details/gpjqmqknk.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.epnwcf.com/Article/details/gehwzivyc.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.bbcook.cn/Article/details/gsvgoqroh.sHtML

[U61] PHP：正则
来源：http://mobile.bbcook.cn/Article/details/gylqfwmun.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.vehdjk.com/Article/details/gtjyonsyw.sHtML

[U62] PHP：日期对象
来源：http://baike.bbcook.cn/Article/details/gfgllkbru.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://blog.yfazqb.com/Article/details/gmpvhqjbh.sHtML

[U63] PHP：文件读写
来源：http://3g.vehdjk.com/Article/details/grfkmnflg.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.tarul.cn/Article/details/giejhpnzr.sHtML

[U64] PHP：目录遍历
来源：http://baike.epnwcf.com/Article/details/gcdfteber.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.vehdjk.com/Article/details/gsesvpnnm.sHtML

[U65] PHP：会话
来源：http://baike.tarul.cn/Article/details/grqcueuvw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.epnwcf.com/Article/details/geffxxwky.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.fktsv.cn/Article/details/gaoftwzit.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.sjlbkw.cn/Article/details/geraddaoj.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.epnwcf.com/Article/details/gdkqrrwvj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.vehdjk.com/Article/details/gkbdxoeym.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.epnwcf.com/Article/details/gegikqivc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.bbcook.cn/Article/details/gkyiklhda.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.epnwcf.com/Article/details/gztbuxlib.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.sjlbkw.cn/Article/details/gcnhzblid.sHtML

[U70] PHP：PDO 事务
来源：http://3g.bbcook.cn/Article/details/ghiodzeqc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fktsv.cn/Article/details/gservvfsa.sHtML

[U71] PHP：抛出异常
来源：http://3g.yfazqb.com/Article/details/gswjfhrqz.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.sjlbkw.cn/Article/details/ghrckuqog.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.tarul.cn/Article/details/gccmmeoxi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.sjlbkw.cn/Article/details/gotqxbmne.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.fktsv.cn/Article/details/gaecbcdzt.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.yfazqb.com/Article/details/glvawjkfw.sHtML

[U74] PHP：读取环境变量
来源：http://wap.fktsv.cn/Article/details/gkafbczbb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.tarul.cn/Article/details/gnnftsblr.sHtML

[U75] PHP：依赖注入
来源：http://3g.epnwcf.com/Article/details/gadbnzngp.sHtML

composer require psr/container
来源：http://3g.bbcook.cn/Article/details/glpakmbnb.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.epnwcf.com/Article/details/guxnbewyc.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fktsv.cn/Article/details/gzvhctzvl.sHtML

[U77] PHP：模板渲染
来源：http://blog.fktsv.cn/Article/details/gvaisxnva.sHtML

composer require twig/twig
来源：http://www.share.epnwcf.com/Article/details/gcvmnphlg.sHtML

[U78] PHP：单元测试
来源：http://baike.yfazqb.com/Article/details/gefssydjf.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.sjlbkw.cn/Article/details/grbgwmsqc.sHtML

[U79] PHP：静态分析
来源：http://read.share.sjlbkw.cn/Article/details/gyrqvrvaw.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fktsv.cn/Article/details/glpxwboky.sHtML

[U80] PHP：代码规范修复
来源：http://baike.tarul.cn/Article/details/grzfsfdnu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.bbcook.cn/Article/details/gosulsemq.sHtML

[U81] JS：初始化项目
来源：http://m.share.sjlbkw.cn/Article/details/gohozcpgm.sHtML

npm init -y;  npm i express
来源：http://read.share.fktsv.cn/Article/details/ghbgffvse.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.sjlbkw.cn/Article/details/greanklmn.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.tarul.cn/Article/details/gvofnmgjr.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.yfazqb.com/Article/details/gvemxqmzc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fktsv.cn/Article/details/gsxlskwue.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.epnwcf.com/Article/details/gaiosdiqc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.sjlbkw.cn/Article/details/gvbrzwzzv.sHtML

[U85] JS：可选链
来源：http://blog.bbcook.cn/Article/details/gasmdpmes.sHtML

a?.b?.c
来源：http://read.share.vehdjk.com/Article/details/ghhlgfveo.sHtML

[U86] JS：空值合并
来源：http://3g.epnwcf.com/Article/details/gqbcctiqh.sHtML

a ?? b
来源：http://3g.sjlbkw.cn/Article/details/glhnhhpda.sHtML

[U87] JS：解构默认值
来源：http://wap.yfazqb.com/Article/details/gmtsipdqo.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.share.bbcook.cn/Article/details/gbqeutdmc.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.sjlbkw.cn/Article/details/gdpmzdrah.sHtML

{ ...a, ...b }
来源：http://3g.fktsv.cn/Article/details/gaoflbkwd.sHtML

[U89] JS：数组去重
来源：http://www.share.sjlbkw.cn/Article/details/goenzzcuf.sHtML

[...new Set(arr)]
来源：http://blog.bbcook.cn/Article/details/gacswrujk.sHtML

[U90] JS：数字数组排序
来源：http://3g.vehdjk.com/Article/details/graxrhcha.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.epnwcf.com/Article/details/geqwcfhfd.sHtML

[U91] JS：对象键值遍历
来源：http://baike.epnwcf.com/Article/details/glrncotcj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.sjlbkw.cn/Article/details/gvvqkbdbf.sHtML

[U92] JS：深拷贝
来源：http://3g.tarul.cn/Article/details/giepyjdqw.sHtML

structuredClone(obj)
来源：http://blog.tarul.cn/Article/details/gwmousbxn.sHtML

[U93] JS：模板字符串
来源：http://3g.yfazqb.com/Article/details/gcrprsrcv.sHtML

`共 ${n} 条`
来源：http://www.share.epnwcf.com/Article/details/gpqxkpvux.sHtML

[U94] JS：箭头函数
来源：http://mobile.epnwcf.com/Article/details/gbwfctxzu.sHtML

const double = x => x * 2;
来源：http://wap.yfazqb.com/Article/details/gzacwepmq.sHtML

[U95] JS：Promise 包装
来源：http://wap.fktsv.cn/Article/details/gcziwyzih.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.epnwcf.com/Article/details/govrupilg.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fktsv.cn/Article/details/giwevpjyp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.epnwcf.com/Article/details/gcojnioxc.sHtML

[U97] JS：并发请求
来源：http://m.share.sjlbkw.cn/Article/details/gqcnuhpzk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.epnwcf.com/Article/details/gbitqztmu.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.yfazqb.com/Article/details/gtibooezb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.epnwcf.com/Article/details/gxiutxvxm.sHtML

[U99] JS：事件监听
来源：http://wap.yfazqb.com/Article/details/gqjcokmdh.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.sjlbkw.cn/Article/details/gsyrevpyo.sHtML

[U100] JS：DOM 查询
来源：http://m.share.bbcook.cn/Article/details/gnxdwnfvp.sHtML

document.querySelector(".item")
来源：http://wap.tarul.cn/Article/details/gavcdwpaw.sHtML

[U101] JS：classList 操作
来源：http://mobile.tarul.cn/Article/details/ggsfkorkp.sHtML

el.classList.toggle("active")
来源：http://baike.vehdjk.com/Article/details/gvqybjmmm.sHtML

[U102] JS：本地存储
来源：http://mobile.tarul.cn/Article/details/gufunvpvt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fktsv.cn/Article/details/gfycexluj.sHtML

[U103] JS：定时器
来源：http://baike.bbcook.cn/Article/details/ghzwyvixy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.vehdjk.com/Article/details/gbperzxxn.sHtML

[U104] JS：防抖
来源：http://www.share.tarul.cn/Article/details/gxwnvcskj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.bbcook.cn/Article/details/gjcwayfeg.sHtML

[U105] JS：节流
来源：http://3g.sjlbkw.cn/Article/details/gsjivcpor.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.yfazqb.com/Article/details/gctrstvxr.sHtML

[U106] JS：日期格式化
来源：http://www.blog.yfazqb.com/Article/details/gqljmulgg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.sjlbkw.cn/Article/details/gydlrdpbr.sHtML

[U107] JS：数字千分位
来源：http://www.share.bbcook.cn/Article/details/gkcaigiik.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fktsv.cn/Article/details/grrwinutg.sHtML

[U108] JS：随机整数
来源：http://read.share.bbcook.cn/Article/details/ggvlvkzst.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.sjlbkw.cn/Article/details/gqykkzwcp.sHtML

[U109] JS：数组分组
来源：http://mobile.tarul.cn/Article/details/gcvlkkayx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.epnwcf.com/Article/details/gpmlkmbzk.sHtML

[U110] JS：数组分块
来源：http://wap.bbcook.cn/Article/details/gvxpihywf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.tarul.cn/Article/details/gnjtsznfk.sHtML

[U111] JS：对象转 Map
来源：http://m.share.yfazqb.com/Article/details/gccpaoqkw.sHtML

new Map(Object.entries(obj))
来源：http://read.share.tarul.cn/Article/details/geqcxgxpx.sHtML

[U112] JS：字符串补位
来源：http://read.share.tarul.cn/Article/details/grmrafwle.sHtML

"7".padStart(3, "0")
来源：http://m.share.fktsv.cn/Article/details/ggciiyerf.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.bbcook.cn/Article/details/gfghfuuah.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fktsv.cn/Article/details/gbpskrmup.sHtML

[U114] JS：JSON 深比较
来源：http://baike.yfazqb.com/Article/details/gnfqnfckm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.epnwcf.com/Article/details/giaqxhkdo.sHtML

[U115] JS：生成 UUID
来源：http://baike.epnwcf.com/Article/details/gwfpiostx.sHtML

crypto.randomUUID()
来源：http://3g.fktsv.cn/Article/details/gzgezdogm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.epnwcf.com/Article/details/gdockkgfq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.tarul.cn/Article/details/gawhojftn.sHtML

[U117] JS：单元测试
来源：http://wap.sjlbkw.cn/Article/details/gwujqaaok.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.tarul.cn/Article/details/gqyrinlan.sHtML

[U118] JS：开发服务器
来源：http://blog.tarul.cn/Article/details/gectfmzno.sHtML

npm i -D vite;  npx vite
来源：http://mobile.tarul.cn/Article/details/gdwwksygv.sHtML

[U119] JS：生产构建
来源：http://read.share.yfazqb.com/Article/details/gdtmyrdkh.sHtML

npx vite build
来源：http://www.m.share.vehdjk.com/Article/details/gxnfyakbc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.yfazqb.com/Article/details/gmukbwtpy.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.epnwcf.com/Article/details/gazvbfwex.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gifqxveou.sHtML

统计汇总
来源：http://mobile.yfazqb.com/Article/details/gczmplrag.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/govszyhub.sHtML

按语言统计（条）：
来源：http://blog.sjlbkw.cn/Article/details/glcaqxyjd.sHtML

Python ......... 252
来源：http://www.share.epnwcf.com/Article/details/gltbswsxm.sHtML

PHP ............ 252
来源：http://www.blog.tarul.cn/Article/details/gqmceofxi.sHtML

JavaScript ..... 252
来源：http://3g.epnwcf.com/Article/details/gnpqjsaui.sHtML

TypeScript ..... 212
来源：http://www.share.vehdjk.com/Article/details/gngxainux.sHtML

Java ........... 212
来源：http://wap.tarul.cn/Article/details/gtzkbbxft.sHtML

Go ............. 212
来源：http://www.blog.vehdjk.com/Article/details/gfbfbehos.sHtML

Ruby ........... 212
来源：http://mobile.vehdjk.com/Article/details/gzbnsydzk.sHtML

C# ............. 212
来源：http://mobile.yfazqb.com/Article/details/giuglfldf.sHtML

C .............. 30
来源：http://mobile.fktsv.cn/Article/details/goylmcbpp.sHtML

C++ ............ 30
来源：http://baike.fktsv.cn/Article/details/geeeubwxe.sHtML

SQL ............ 90
来源：http://www.m.share.fktsv.cn/Article/details/guruwkfcq.sHtML

Bash ........... 80
来源：http://baike.vehdjk.com/Article/details/gtbmxvxsl.sHtML

Kotlin ......... 15
来源：http://www.share.yfazqb.com/Article/details/gozwruksa.sHtML

Swift .......... 15
来源：http://www.blog.bbcook.cn/Article/details/ghcnwrbfh.sHtML

Lua ............ 10
来源：http://read.share.epnwcf.com/Article/details/gdwowynax.sHtML

Perl ........... 10
来源：http://blog.yfazqb.com/Article/details/gitxpzrjs.sHtML

Scala .......... 10
来源：http://mobile.bbcook.cn/Article/details/gjkmghkmv.sHtML

------------------------------------
来源：http://www.m.share.epnwcf.com/Article/details/gqohufzvh.sHtML

合计 ........... 2106 条
来源：http://read.share.epnwcf.com/Article/details/gcesllinq.sHtML

按章节统计：
来源：http://wap.vehdjk.com/Article/details/gcqneclne.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.yfazqb.com/Article/details/gmlurijmb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.sjlbkw.cn/Article/details/gcakbfehd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.epnwcf.com/Article/details/gcvielikh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.yfazqb.com/Article/details/gbavhqxfv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.yfazqb.com/Article/details/gukcmvalz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.sjlbkw.cn/Article/details/gvfozoucb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.epnwcf.com/Article/details/gvnnozpvq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.vehdjk.com/Article/details/gitcxggrc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fktsv.cn/Article/details/gjwyqsqhf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.bbcook.cn/Article/details/gjyxzhgip.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.yfazqb.com/Article/details/gspqqnhzj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fktsv.cn/Article/details/gmepaykcc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.epnwcf.com/Article/details/gofgswmki.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.epnwcf.com/Article/details/gmzpztyde.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.bbcook.cn/Article/details/gfrrzcrmb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fktsv.cn/Article/details/ggglulgmk.sHtML

Q SQL 专题                              90
来源：http://mobile.fktsv.cn/Article/details/gnojxlmlf.sHtML

R Bash 专题                             80
来源：http://m.share.vehdjk.com/Article/details/grspemaqu.sHtML

S C / C++ 专题                          60
来源：http://blog.epnwcf.com/Article/details/gqnfiivdf.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fktsv.cn/Article/details/gxyykylsp.sHtML

U 高频实用片段                         120
来源：http://read.share.fktsv.cn/Article/details/glqsespgt.sHtML

------------------------------------
来源：http://m.share.tarul.cn/Article/details/gdlopskqd.sHtML

合计                                  2106 条
来源：http://m.share.tarul.cn/Article/details/gpzflqfgg.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fktsv.cn/Article/details/gxxfcxgta.sHtML

使用提醒
来源：http://3g.fktsv.cn/Article/details/gukdgbrod.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fktsv.cn/Article/details/gdjourulc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.bbcook.cn/Article/details/gkobnsaup.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fktsv.cn/Article/details/gyhpxnpce.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.vehdjk.com/Article/details/gypcymryj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.tarul.cn/Article/details/gpzuhmhcj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.tarul.cn/Article/details/gpgshglxp.sHtML

—— 文件结束 ——
来源：http://baike.fktsv.cn/Article/details/grperigjo.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gulwzqkoi.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.yfazqb.com/Article/details/gqkowwfwl.sHtML

Common Programming Examples Cheat Book
来源：http://3g.vehdjk.com/Article/details/gxxgwguwp.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gqeegjpst.sHtML

【收录内容】
来源：http://wap.bbcook.cn/Article/details/gyvcfydaw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.yfazqb.com/Article/details/gjgrezscj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.epnwcf.com/Article/details/gwlrfuzgg.sHtML

SQL · Bash · C · C++
来源：http://m.share.fktsv.cn/Article/details/gavkftkdw.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.sjlbkw.cn/Article/details/gtxpsynii.sHtML

【使用说明】
来源：http://www.share.tarul.cn/Article/details/gixgbirdf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.vehdjk.com/Article/details/gpxuoqrfy.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.epnwcf.com/Article/details/guqaiktwq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fktsv.cn/Article/details/gmdwwannh.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.tarul.cn/Article/details/gsmnizder.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.epnwcf.com/Article/details/gobtdfyoh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.epnwcf.com/Article/details/getxdbitn.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.bbcook.cn/Article/details/gaoebxaxn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.epnwcf.com/Article/details/grrpvpayk.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.tarul.cn/Article/details/gxmtvharw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.sjlbkw.cn/Article/details/gmrwgypfi.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.yfazqb.com/Article/details/gltxlachh.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.sjlbkw.cn/Article/details/ggjnvkyem.sHtML

【文件统计】
来源：http://blog.sjlbkw.cn/Article/details/gkirkzrly.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.epnwcf.com/Article/details/gdjdytdob.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fktsv.cn/Article/details/gbwcqqapl.sHtML

目  录
来源：http://wap.fktsv.cn/Article/details/gwlkbqytr.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.epnwcf.com/Article/details/gzvnqxkah.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.yfazqb.com/Article/details/gukxelgkz.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.yfazqb.com/Article/details/ggbhffshy.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.epnwcf.com/Article/details/gwagigpid.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.bbcook.cn/Article/details/gewjpznyp.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gqlzhlfiz.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.epnwcf.com/Article/details/giwgwhoji.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.bbcook.cn/Article/details/gaobtpnnp.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.sjlbkw.cn/Article/details/gqwzhsskb.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gjlfgzlbf.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fktsv.cn/Article/details/gidkztkij.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.bbcook.cn/Article/details/gkcfpeyjt.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.sjlbkw.cn/Article/details/gxujgjfbb.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.sjlbkw.cn/Article/details/gygteaoys.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.vehdjk.com/Article/details/gdpgdopqo.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gwcskdtjf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.sjlbkw.cn/Article/details/ggxlxpmms.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.tarul.cn/Article/details/gnracsmmv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.vehdjk.com/Article/details/gyiruwhbb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.epnwcf.com/Article/details/ggplhpvrz.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.vehdjk.com/Article/details/gjdkfxhdi.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.vehdjk.com/Article/details/gqmkdhnsi.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gmvssuqjn.sHtML

A. 基础语法与类型
来源：http://read.share.bbcook.cn/Article/details/gywrmsrle.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gfngnhsuj.sHtML

[A01] Hello World
来源：http://3g.vehdjk.com/Article/details/gfffqjulz.sHtML

Py:   print("Hello, World!")
来源：http://blog.sjlbkw.cn/Article/details/gvndgprbv.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.yfazqb.com/Article/details/grchamzdz.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.sjlbkw.cn/Article/details/gjtmlaeyu.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.vehdjk.com/Article/details/gfbfbsmzh.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.vehdjk.com/Article/details/gyzmpyfqs.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.vehdjk.com/Article/details/gpifgtvai.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.tarul.cn/Article/details/glokekerk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.vehdjk.com/Article/details/gvobyamre.sHtML

[A02] 变量声明与赋值
来源：http://wap.epnwcf.com/Article/details/gvnvgwosd.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.bbcook.cn/Article/details/gedmblxzx.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.yfazqb.com/Article/details/gtkitbppv.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.sjlbkw.cn/Article/details/gimyusphg.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.yfazqb.com/Article/details/gnifflghd.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.tarul.cn/Article/details/gqmsdouev.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.epnwcf.com/Article/details/gbiresiko.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.epnwcf.com/Article/details/gjpktkkwg.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.vehdjk.com/Article/details/gnvlvkjhm.sHtML

[A03] 常量定义
来源：http://www.m.share.yfazqb.com/Article/details/gbeadieow.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.epnwcf.com/Article/details/gtbxtiuqt.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.bbcook.cn/Article/details/gyocmzydr.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.fktsv.cn/Article/details/gkdumbaei.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gmyvxxrbd.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.epnwcf.com/Article/details/gisustzjp.sHtML

Go:   const PI = 3.14159
来源：http://3g.yfazqb.com/Article/details/ggwjsxowc.sHtML

Ruby: PI = 3.14159
来源：http://m.share.sjlbkw.cn/Article/details/gxnfdprcz.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.tarul.cn/Article/details/gxdexjrdk.sHtML

[A04] 判断变量类型
来源：http://www.m.share.tarul.cn/Article/details/gdaeunsnu.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.vehdjk.com/Article/details/gbmbsfsqq.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.sjlbkw.cn/Article/details/gqtwvgfta.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.vehdjk.com/Article/details/gihdyxvpr.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.fktsv.cn/Article/details/glftbdess.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.tarul.cn/Article/details/guknyraxw.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.sjlbkw.cn/Article/details/gpbxgjoeu.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.sjlbkw.cn/Article/details/gwjvjeppa.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.epnwcf.com/Article/details/gosvxycaw.sHtML

[A05] 整数除法与取模
来源：http://wap.tarul.cn/Article/details/glyipxfmk.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.tarul.cn/Article/details/gsphbwqxc.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.tarul.cn/Article/details/gpeworsrn.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fktsv.cn/Article/details/grkwicrsv.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fktsv.cn/Article/details/gxkanryym.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.sjlbkw.cn/Article/details/gjrkoroaq.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.epnwcf.com/Article/details/gkmfbcqnv.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.tarul.cn/Article/details/gvfizerjv.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.epnwcf.com/Article/details/gvvivjzjy.sHtML

[A06] 字符串转数字
来源：http://www.m.share.sjlbkw.cn/Article/details/gobaguvxs.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.bbcook.cn/Article/details/gtmgvngww.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.vehdjk.com/Article/details/ggbunqwmc.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.bbcook.cn/Article/details/gjperxpbo.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.bbcook.cn/Article/details/gzvcctozp.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.fktsv.cn/Article/details/gsiouavgu.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.fktsv.cn/Article/details/gkcnbgjwb.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.vehdjk.com/Article/details/gylaauvpa.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.epnwcf.com/Article/details/gzgmbvtxh.sHtML

[A07] 数字转字符串
来源：http://www.m.share.yfazqb.com/Article/details/ghgjupabd.sHtML

Py:   str(42)
来源：http://m.share.bbcook.cn/Article/details/gdardzcfm.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.bbcook.cn/Article/details/gbarhelqj.sHtML


<!-- 参考信息 -->