代发 wailian999

[U65] PHP：会话
来源：http://m.share.sjlbkw.cn/Article/details/gctduhekt.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.tarul.cn/Article/details/gqlfphvaq.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.tarul.cn/Article/details/gieaiomwv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.bbcook.cn/Article/details/gwdcokext.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.sjlbkw.cn/Article/details/gpsmavgzi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fktsv.cn/Article/details/gvzopsxij.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.fktsv.cn/Article/details/gpegknuwf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.vehdjk.com/Article/details/gatqkfhks.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.yfazqb.com/Article/details/gyqhjaxaw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.fktsv.cn/Article/details/gmugxyxkn.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.tarul.cn/Article/details/gflxkdsvt.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.yfazqb.com/Article/details/gcjtlzlqh.sHtML

[U71] PHP：抛出异常
来源：http://m.share.epnwcf.com/Article/details/gtshjgiqi.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.tarul.cn/Article/details/gbcynkkjm.sHtML

[U72] PHP：写错误日志
来源：http://read.share.vehdjk.com/Article/details/gxymajbid.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.yfazqb.com/Article/details/gkodxjteh.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.epnwcf.com/Article/details/gfuxxafze.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.vehdjk.com/Article/details/gbcriqiix.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.sjlbkw.cn/Article/details/gjikhqqvn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.tarul.cn/Article/details/gsdjyindg.sHtML

[U75] PHP：依赖注入
来源：http://www.share.yfazqb.com/Article/details/gtmxzdnkp.sHtML

composer require psr/container
来源：http://read.share.fktsv.cn/Article/details/guomsmdfj.sHtML

[U76] PHP：简单路由
来源：http://baike.bbcook.cn/Article/details/gjwbsyjwm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.vehdjk.com/Article/details/gmchajmly.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fktsv.cn/Article/details/gqhyskdqn.sHtML

composer require twig/twig
来源：http://mobile.fktsv.cn/Article/details/gdaxrjnxn.sHtML

[U78] PHP：单元测试
来源：http://wap.epnwcf.com/Article/details/gfwrnocfu.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.tarul.cn/Article/details/ghjjfpfkq.sHtML

[U79] PHP：静态分析
来源：http://3g.sjlbkw.cn/Article/details/gjcifcbrn.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.sjlbkw.cn/Article/details/guuhukagc.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwnenhqe.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.vehdjk.com/Article/details/gwyxywwpe.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fktsv.cn/Article/details/goddggcmd.sHtML

npm init -y;  npm i express
来源：http://www.m.share.epnwcf.com/Article/details/gxvqkbwff.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.yfazqb.com/Article/details/geminjhbv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.vehdjk.com/Article/details/gvcokygnl.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.vehdjk.com/Article/details/gmdwbjhnq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.sjlbkw.cn/Article/details/gytynimcw.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.sjlbkw.cn/Article/details/ghyrlvrtv.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.sjlbkw.cn/Article/details/ghlqtgrmd.sHtML

[U85] JS：可选链
来源：http://mobile.fktsv.cn/Article/details/galvnfcwc.sHtML

a?.b?.c
来源：http://mobile.epnwcf.com/Article/details/ggzuobdmz.sHtML

[U86] JS：空值合并
来源：http://3g.sjlbkw.cn/Article/details/gfojdjtpq.sHtML

a ?? b
来源：http://blog.fktsv.cn/Article/details/goqdvgzhm.sHtML

[U87] JS：解构默认值
来源：http://3g.sjlbkw.cn/Article/details/gpzmonoyr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.vehdjk.com/Article/details/gyhvwslbl.sHtML

[U88] JS：对象展开合并
来源：http://baike.yfazqb.com/Article/details/ghtjzpybr.sHtML

{ ...a, ...b }
来源：http://3g.bbcook.cn/Article/details/gvwcynbvj.sHtML

[U89] JS：数组去重
来源：http://baike.epnwcf.com/Article/details/guqsciwjq.sHtML

[...new Set(arr)]
来源：http://read.share.fktsv.cn/Article/details/gxyotvugx.sHtML

[U90] JS：数字数组排序
来源：http://wap.tarul.cn/Article/details/gwxrilbii.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.tarul.cn/Article/details/gdezwztli.sHtML

[U91] JS：对象键值遍历
来源：http://wap.sjlbkw.cn/Article/details/gbqsguktd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fktsv.cn/Article/details/gyekbgdks.sHtML

[U92] JS：深拷贝
来源：http://read.share.bbcook.cn/Article/details/gghdhkiuv.sHtML

structuredClone(obj)
来源：http://www.blog.bbcook.cn/Article/details/gaesugmjg.sHtML

[U93] JS：模板字符串
来源：http://wap.vehdjk.com/Article/details/gmfokgvik.sHtML

`共 ${n} 条`
来源：http://3g.bbcook.cn/Article/details/glsqxzdge.sHtML

[U94] JS：箭头函数
来源：http://wap.tarul.cn/Article/details/gytsvnbmz.sHtML

const double = x => x * 2;
来源：http://m.share.vehdjk.com/Article/details/gxjlujtwu.sHtML

[U95] JS：Promise 包装
来源：http://www.share.epnwcf.com/Article/details/gosliuzjx.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.vehdjk.com/Article/details/gxkuvwbdf.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.yfazqb.com/Article/details/gjfpcuecr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.yfazqb.com/Article/details/gdgwmeopt.sHtML

[U97] JS：并发请求
来源：http://m.share.yfazqb.com/Article/details/gyaqwbyuv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.sjlbkw.cn/Article/details/guzpffrfb.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.bbcook.cn/Article/details/gyvrsjehp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.yfazqb.com/Article/details/gcsppcsxx.sHtML

[U99] JS：事件监听
来源：http://www.blog.yfazqb.com/Article/details/gvrkfbwoj.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.vehdjk.com/Article/details/ghbfmzyww.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.vehdjk.com/Article/details/gxstqgmck.sHtML

document.querySelector(".item")
来源：http://www.m.share.yfazqb.com/Article/details/gfwfwhrls.sHtML

[U101] JS：classList 操作
来源：http://mobile.vehdjk.com/Article/details/gqemcwpvh.sHtML

el.classList.toggle("active")
来源：http://read.share.yfazqb.com/Article/details/gwwanjisn.sHtML

[U102] JS：本地存储
来源：http://blog.bbcook.cn/Article/details/guzitfuik.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fktsv.cn/Article/details/gryftoqnk.sHtML

[U103] JS：定时器
来源：http://read.share.bbcook.cn/Article/details/giglcryin.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fktsv.cn/Article/details/gxkbzunuo.sHtML

[U104] JS：防抖
来源：http://www.blog.vehdjk.com/Article/details/gnrasjnjl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.sjlbkw.cn/Article/details/gfswtkscg.sHtML

[U105] JS：节流
来源：http://3g.sjlbkw.cn/Article/details/gttfrrgqh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.sjlbkw.cn/Article/details/gakyhifep.sHtML

[U106] JS：日期格式化
来源：http://wap.vehdjk.com/Article/details/gfxbcmmeb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.tarul.cn/Article/details/gqakypuhq.sHtML

[U107] JS：数字千分位
来源：http://www.share.tarul.cn/Article/details/gbyvpyrvq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.sjlbkw.cn/Article/details/gtgahvpid.sHtML

[U108] JS：随机整数
来源：http://3g.fktsv.cn/Article/details/gjuluodtk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.epnwcf.com/Article/details/gsnkodyie.sHtML

[U109] JS：数组分组
来源：http://baike.vehdjk.com/Article/details/gcbghdxsd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.yfazqb.com/Article/details/gyehunvhd.sHtML

[U110] JS：数组分块
来源：http://3g.bbcook.cn/Article/details/gcbaatewh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.yfazqb.com/Article/details/gxgmgnrxx.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fktsv.cn/Article/details/geahhyhsc.sHtML

new Map(Object.entries(obj))
来源：http://baike.tarul.cn/Article/details/gpyvwslgz.sHtML

[U112] JS：字符串补位
来源：http://mobile.fktsv.cn/Article/details/gddgnmtaa.sHtML

"7".padStart(3, "0")
来源：http://m.share.tarul.cn/Article/details/gobctjetc.sHtML

[U113] JS：正则替换全部
来源：http://baike.yfazqb.com/Article/details/gwcpqtxpg.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fktsv.cn/Article/details/gjavgdskt.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.epnwcf.com/Article/details/gkebbeqqg.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fktsv.cn/Article/details/gydkipvdi.sHtML

[U115] JS：生成 UUID
来源：http://baike.tarul.cn/Article/details/gfqmqvtfo.sHtML

crypto.randomUUID()
来源：http://m.share.bbcook.cn/Article/details/gjnldempq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fktsv.cn/Article/details/gdfprcpnq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.vehdjk.com/Article/details/gznqvhglk.sHtML

[U117] JS：单元测试
来源：http://www.blog.vehdjk.com/Article/details/gzpcddjkd.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.vehdjk.com/Article/details/gwxjxnikq.sHtML

[U118] JS：开发服务器
来源：http://3g.vehdjk.com/Article/details/grkkoxjlo.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fktsv.cn/Article/details/gdytrbikm.sHtML

[U119] JS：生产构建
来源：http://www.share.sjlbkw.cn/Article/details/gskazxbvu.sHtML

npx vite build
来源：http://mobile.bbcook.cn/Article/details/gfrhtpifl.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.tarul.cn/Article/details/glzwppbnt.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.bbcook.cn/Article/details/guowxhpvq.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gphckhezu.sHtML

统计汇总
来源：http://3g.vehdjk.com/Article/details/gxjbfrbvd.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gsepjcqzb.sHtML

按语言统计（条）：
来源：http://3g.fktsv.cn/Article/details/gmnexyclf.sHtML

Python ......... 252
来源：http://www.blog.epnwcf.com/Article/details/glvwrdhrq.sHtML

PHP ............ 252
来源：http://www.m.share.tarul.cn/Article/details/gimrtfmut.sHtML

JavaScript ..... 252
来源：http://baike.tarul.cn/Article/details/gyedtgebs.sHtML

TypeScript ..... 212
来源：http://wap.sjlbkw.cn/Article/details/gogngxfei.sHtML

Java ........... 212
来源：http://www.share.epnwcf.com/Article/details/gjcserajo.sHtML

Go ............. 212
来源：http://m.share.tarul.cn/Article/details/gzawaffqi.sHtML

Ruby ........... 212
来源：http://baike.bbcook.cn/Article/details/gkwzqwtam.sHtML

C# ............. 212
来源：http://wap.yfazqb.com/Article/details/gezpokjad.sHtML

C .............. 30
来源：http://baike.yfazqb.com/Article/details/gpyltdcjv.sHtML

C++ ............ 30
来源：http://m.share.tarul.cn/Article/details/guppnlvhd.sHtML

SQL ............ 90
来源：http://3g.bbcook.cn/Article/details/gjkxxhzkq.sHtML

Bash ........... 80
来源：http://m.share.sjlbkw.cn/Article/details/gzpkzvpnd.sHtML

Kotlin ......... 15
来源：http://www.blog.yfazqb.com/Article/details/ggrjnmofc.sHtML

Swift .......... 15
来源：http://read.share.vehdjk.com/Article/details/gmmohndtr.sHtML

Lua ............ 10
来源：http://www.share.epnwcf.com/Article/details/grotpgbhx.sHtML

Perl ........... 10
来源：http://wap.fktsv.cn/Article/details/gbztunhgs.sHtML

Scala .......... 10
来源：http://wap.bbcook.cn/Article/details/gzgvcqffw.sHtML

------------------------------------
来源：http://3g.bbcook.cn/Article/details/gccjirmmf.sHtML

合计 ........... 2106 条
来源：http://mobile.epnwcf.com/Article/details/gimtzrlzz.sHtML

按章节统计：
来源：http://wap.fktsv.cn/Article/details/gwxnekcxz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.yfazqb.com/Article/details/gxmaxqtsk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.yfazqb.com/Article/details/gdwrlqoaq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fktsv.cn/Article/details/giebffiqz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.yfazqb.com/Article/details/gqwtfsyqc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fktsv.cn/Article/details/glybkjjpa.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.yfazqb.com/Article/details/gcvlwkxmi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fktsv.cn/Article/details/gwmimitnx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fktsv.cn/Article/details/gwqyzmjtw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.sjlbkw.cn/Article/details/ggnpasfzo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.sjlbkw.cn/Article/details/gytxrwiew.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.bbcook.cn/Article/details/gxvrkegzz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/gyuafamwk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.vehdjk.com/Article/details/ghswmfalr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.tarul.cn/Article/details/geesyigxk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.yfazqb.com/Article/details/ggjwvfxfo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.yfazqb.com/Article/details/gtweyvaga.sHtML

Q SQL 专题                              90
来源：http://baike.sjlbkw.cn/Article/details/ghjaueoha.sHtML

R Bash 专题                             80
来源：http://baike.bbcook.cn/Article/details/gfvjmferr.sHtML

S C / C++ 专题                          60
来源：http://www.share.epnwcf.com/Article/details/gdllzlift.sHtML

T 其他语言补充                          60
来源：http://www.blog.tarul.cn/Article/details/guptcfaot.sHtML

U 高频实用片段                         120
来源：http://read.share.yfazqb.com/Article/details/gemsixcfu.sHtML

------------------------------------
来源：http://mobile.epnwcf.com/Article/details/gvpgbwadh.sHtML

合计                                  2106 条
来源：http://baike.epnwcf.com/Article/details/gzktshlqn.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.yfazqb.com/Article/details/gtewaliqg.sHtML

使用提醒
来源：http://wap.fktsv.cn/Article/details/getadyujt.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fktsv.cn/Article/details/gnxpiuome.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.tarul.cn/Article/details/gnhtmgwzc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.tarul.cn/Article/details/gfhsckuiy.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.epnwcf.com/Article/details/gadqodkvv.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.sjlbkw.cn/Article/details/gbsmfefkk.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.vehdjk.com/Article/details/gebbvdrvu.sHtML

—— 文件结束 ——
来源：http://baike.vehdjk.com/Article/details/gwrwuvege.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gddjlarxq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.epnwcf.com/Article/details/gdtzbomgi.sHtML

Common Programming Examples Cheat Book
来源：http://blog.sjlbkw.cn/Article/details/gjlvxjtmo.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gjhphfbpl.sHtML

【收录内容】
来源：http://read.share.bbcook.cn/Article/details/grneqyxia.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.sjlbkw.cn/Article/details/gpkjkowkn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.yfazqb.com/Article/details/glwbhtbpj.sHtML

SQL · Bash · C · C++
来源：http://baike.yfazqb.com/Article/details/ghkrailjf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.bbcook.cn/Article/details/gpnyxzbhr.sHtML

【使用说明】
来源：http://mobile.yfazqb.com/Article/details/gelosigpp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fktsv.cn/Article/details/gpvjilplm.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.tarul.cn/Article/details/gjqtaacqj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.epnwcf.com/Article/details/gtbqhdvwv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fktsv.cn/Article/details/ggohbpcrb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.bbcook.cn/Article/details/gvjalprod.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.bbcook.cn/Article/details/geyzwrtir.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.sjlbkw.cn/Article/details/gucizzxqz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.tarul.cn/Article/details/grayeubku.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.yfazqb.com/Article/details/gyetaxdgj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.tarul.cn/Article/details/gbrxfjzyy.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.epnwcf.com/Article/details/gifiamrax.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.yfazqb.com/Article/details/gvbattgaw.sHtML

【文件统计】
来源：http://blog.vehdjk.com/Article/details/gpbaqfxln.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.bbcook.cn/Article/details/gtclgekyf.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fktsv.cn/Article/details/grdmbvpbv.sHtML

目  录
来源：http://mobile.yfazqb.com/Article/details/gfzhqfsqx.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.vehdjk.com/Article/details/gbnaamqft.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.vehdjk.com/Article/details/gmsajtlaq.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.yfazqb.com/Article/details/gkuryfbkw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.epnwcf.com/Article/details/gfpuhglxx.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.sjlbkw.cn/Article/details/grvyaipsx.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.bbcook.cn/Article/details/gwedxpsfs.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.tarul.cn/Article/details/grqwdbnhm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gcjpwnhoq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.tarul.cn/Article/details/gjembjlsj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.epnwcf.com/Article/details/gobthkwnx.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.yfazqb.com/Article/details/gunffxxag.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.bbcook.cn/Article/details/gifvppqtr.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.bbcook.cn/Article/details/gxwpynjqt.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.sjlbkw.cn/Article/details/gvutiipkc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.tarul.cn/Article/details/gcpvhwrgh.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.fktsv.cn/Article/details/gvwqjsvwq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.fktsv.cn/Article/details/gokniowsv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fktsv.cn/Article/details/gqshxkkup.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.bbcook.cn/Article/details/glthqqacv.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.sjlbkw.cn/Article/details/geivfdcbu.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.tarul.cn/Article/details/gramfvnso.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.yfazqb.com/Article/details/ghbvfsexu.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gzdktalhq.sHtML

A. 基础语法与类型
来源：http://blog.vehdjk.com/Article/details/gllpnusnl.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gibgblpcx.sHtML

[A01] Hello World
来源：http://www.blog.epnwcf.com/Article/details/geceyesof.sHtML

Py:   print("Hello, World!")
来源：http://www.share.yfazqb.com/Article/details/gvbraadoc.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.vehdjk.com/Article/details/gfmkgyvph.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.yfazqb.com/Article/details/gpfxakhpu.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.tarul.cn/Article/details/gltnybjdp.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.epnwcf.com/Article/details/gihiqmnmi.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.sjlbkw.cn/Article/details/ghobmyrcw.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.sjlbkw.cn/Article/details/gnrujwpco.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.yfazqb.com/Article/details/ggcxjropj.sHtML

[A02] 变量声明与赋值
来源：http://blog.epnwcf.com/Article/details/glxtkqinw.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.bbcook.cn/Article/details/guqqmrdut.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.tarul.cn/Article/details/gmvhupvso.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.epnwcf.com/Article/details/gxcbhqlyx.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.epnwcf.com/Article/details/gnciaqwpa.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.tarul.cn/Article/details/gxotqpdmy.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.fktsv.cn/Article/details/gwrjsfigw.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.tarul.cn/Article/details/gidsnoalg.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.vehdjk.com/Article/details/gsxaoweqs.sHtML

[A03] 常量定义
来源：http://m.share.yfazqb.com/Article/details/gbnctllxc.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.bbcook.cn/Article/details/giciabfck.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gutfdrbgu.sHtML

JS:   const PI = 3.14159;
来源：http://wap.bbcook.cn/Article/details/gzxisvnvn.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.vehdjk.com/Article/details/gybhymhmq.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.vehdjk.com/Article/details/gpnlhsmhi.sHtML

Go:   const PI = 3.14159
来源：http://wap.vehdjk.com/Article/details/gpiudghwa.sHtML

Ruby: PI = 3.14159
来源：http://3g.vehdjk.com/Article/details/gigwydhmi.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.bbcook.cn/Article/details/grbbqoyrt.sHtML

[A04] 判断变量类型
来源：http://www.m.share.sjlbkw.cn/Article/details/gqjuxnyxv.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqpdmkurs.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.epnwcf.com/Article/details/gthhplaox.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.epnwcf.com/Article/details/gpclcfvnv.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.vehdjk.com/Article/details/gjnzjbvnz.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.epnwcf.com/Article/details/gczbugraw.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.sjlbkw.cn/Article/details/gqqelwfuw.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.epnwcf.com/Article/details/ggnxppler.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.yfazqb.com/Article/details/gaphnyszm.sHtML

[A05] 整数除法与取模
来源：http://www.blog.tarul.cn/Article/details/geubreyqn.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.sjlbkw.cn/Article/details/gdbtnzmwb.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.tarul.cn/Article/details/gcajzmqfk.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.tarul.cn/Article/details/gelxkjrcp.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.bbcook.cn/Article/details/ghtsnqonj.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.sjlbkw.cn/Article/details/gugrqujnv.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.yfazqb.com/Article/details/ghukidwmj.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.fktsv.cn/Article/details/gftvifxku.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.vehdjk.com/Article/details/gkcfabosy.sHtML

[A06] 字符串转数字
来源：http://www.blog.epnwcf.com/Article/details/gtshdsije.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.sjlbkw.cn/Article/details/grcsjhmyl.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.yfazqb.com/Article/details/gvajbgsvv.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.vehdjk.com/Article/details/gkpdoeftd.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.yfazqb.com/Article/details/gkkyfhadt.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.epnwcf.com/Article/details/goyonefjj.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.tarul.cn/Article/details/getwfdzyq.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.fktsv.cn/Article/details/ghiwbgyzv.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.fktsv.cn/Article/details/glqniptoa.sHtML

[A07] 数字转字符串
来源：http://read.share.bbcook.cn/Article/details/glmrdxeht.sHtML

Py:   str(42)
来源：http://www.blog.sjlbkw.cn/Article/details/girikmzyj.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.yfazqb.com/Article/details/gwoarzahu.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.yfazqb.com/Article/details/ggqopkzzi.sHtML

TS:   String(42)
来源：http://3g.tarul.cn/Article/details/gpdlexkqy.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.fktsv.cn/Article/details/gzjpoouni.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.tarul.cn/Article/details/gsddkvift.sHtML

Ruby: 42.to_s
来源：http://wap.epnwcf.com/Article/details/ghsoyrxss.sHtML

C#:   42.ToString()
来源：http://wap.fktsv.cn/Article/details/gkavreidh.sHtML

[A08] 取整与四舍五入
来源：http://blog.sjlbkw.cn/Article/details/gbzrxnugq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.sjlbkw.cn/Article/details/gtewwofoc.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.epnwcf.com/Article/details/gbuyzeaum.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.epnwcf.com/Article/details/gwshysqol.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.sjlbkw.cn/Article/details/gawzwxrio.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.vehdjk.com/Article/details/grukhfcuy.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.fktsv.cn/Article/details/gwcwzevto.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.epnwcf.com/Article/details/gkfnqfimv.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.bbcook.cn/Article/details/gpuvhjwft.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.bbcook.cn/Article/details/gdhmuurvi.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.vehdjk.com/Article/details/ghcqxmpfm.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.sjlbkw.cn/Article/details/gaqletqvo.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.fktsv.cn/Article/details/ggrrpficr.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.vehdjk.com/Article/details/gmelguorh.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.yfazqb.com/Article/details/gficsiymo.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.yfazqb.com/Article/details/gilfkyioc.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.yfazqb.com/Article/details/gvrydmxpt.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.epnwcf.com/Article/details/gawsldtjx.sHtML


<!-- 参考信息 -->