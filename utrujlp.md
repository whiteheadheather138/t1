代发 wailian999

[U65] PHP：会话
来源：http://3g.epnwcf.com/Article/details/grapptlna.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.epnwcf.com/Article/details/glrysdikl.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fktsv.cn/Article/details/gxcxirfus.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.yfazqb.com/Article/details/gtjfvgagt.sHtML

[U67] PHP：处理文件上传
来源：http://baike.tarul.cn/Article/details/ghrnmyued.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.vehdjk.com/Article/details/gwlhskbpb.sHtML

[U68] PHP：PDO 连接
来源：http://blog.tarul.cn/Article/details/grpvyxqbj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.sjlbkw.cn/Article/details/gutnfnghp.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.vehdjk.com/Article/details/gsxcphbbo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.epnwcf.com/Article/details/gblopkpgj.sHtML

[U70] PHP：PDO 事务
来源：http://blog.yfazqb.com/Article/details/gggrmfwwg.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.vehdjk.com/Article/details/gxmgrvfhy.sHtML

[U71] PHP：抛出异常
来源：http://wap.vehdjk.com/Article/details/gasnyeqag.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.tarul.cn/Article/details/ggggxpzjg.sHtML

[U72] PHP：写错误日志
来源：http://wap.bbcook.cn/Article/details/gcvltwmcw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.vehdjk.com/Article/details/gkiuxsdza.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.epnwcf.com/Article/details/gwicbollv.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.yfazqb.com/Article/details/gkymtniif.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.yfazqb.com/Article/details/gwxadydwk.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.bbcook.cn/Article/details/gwyibvmfd.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fktsv.cn/Article/details/gsngtahfa.sHtML

composer require psr/container
来源：http://www.share.epnwcf.com/Article/details/gaaxpccfy.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqitpzyp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.sjlbkw.cn/Article/details/gyagzspxc.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.epnwcf.com/Article/details/gsvovftiw.sHtML

composer require twig/twig
来源：http://www.blog.epnwcf.com/Article/details/guggfypoe.sHtML

[U78] PHP：单元测试
来源：http://wap.sjlbkw.cn/Article/details/gkrnelqad.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.bbcook.cn/Article/details/gqqnxwvyq.sHtML

[U79] PHP：静态分析
来源：http://read.share.yfazqb.com/Article/details/gwtlwerem.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.yfazqb.com/Article/details/guvykwlvb.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.sjlbkw.cn/Article/details/gmxrufqfp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.yfazqb.com/Article/details/gtjzgxizl.sHtML

[U81] JS：初始化项目
来源：http://www.share.vehdjk.com/Article/details/gmytjcpju.sHtML

npm init -y;  npm i express
来源：http://m.share.sjlbkw.cn/Article/details/gobfrpftc.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.sjlbkw.cn/Article/details/goymyhdbv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.sjlbkw.cn/Article/details/ggmdbqjld.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.epnwcf.com/Article/details/gvsbteaba.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.bbcook.cn/Article/details/giqedbnwa.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.tarul.cn/Article/details/grxjwybwz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.vehdjk.com/Article/details/gteibhrpo.sHtML

[U85] JS：可选链
来源：http://www.m.share.tarul.cn/Article/details/gzlehyspk.sHtML

a?.b?.c
来源：http://mobile.vehdjk.com/Article/details/gthswurgv.sHtML

[U86] JS：空值合并
来源：http://m.share.yfazqb.com/Article/details/ghwrvvexi.sHtML

a ?? b
来源：http://www.m.share.tarul.cn/Article/details/gzxwvvvsk.sHtML

[U87] JS：解构默认值
来源：http://read.share.tarul.cn/Article/details/gzmiudygv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fktsv.cn/Article/details/grpcrndup.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.epnwcf.com/Article/details/gachldvlg.sHtML

{ ...a, ...b }
来源：http://read.share.vehdjk.com/Article/details/ggzcfoylw.sHtML

[U89] JS：数组去重
来源：http://read.share.epnwcf.com/Article/details/grjvmsxee.sHtML

[...new Set(arr)]
来源：http://blog.sjlbkw.cn/Article/details/gbrtmlksp.sHtML

[U90] JS：数字数组排序
来源：http://m.share.epnwcf.com/Article/details/gwyezacud.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.yfazqb.com/Article/details/grcbwknmn.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.bbcook.cn/Article/details/gpzwrtcnb.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.bbcook.cn/Article/details/gksstznes.sHtML

[U92] JS：深拷贝
来源：http://m.share.epnwcf.com/Article/details/gyvokotot.sHtML

structuredClone(obj)
来源：http://read.share.tarul.cn/Article/details/gnihgyzuk.sHtML

[U93] JS：模板字符串
来源：http://wap.yfazqb.com/Article/details/gcmvtqddm.sHtML

`共 ${n} 条`
来源：http://baike.epnwcf.com/Article/details/gpkgovlse.sHtML

[U94] JS：箭头函数
来源：http://3g.sjlbkw.cn/Article/details/gnqsgzrgp.sHtML

const double = x => x * 2;
来源：http://www.share.yfazqb.com/Article/details/gagwkbzkt.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fktsv.cn/Article/details/gyhohoovo.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.bbcook.cn/Article/details/gsbjqufvj.sHtML

[U96] JS：async/await 与异常
来源：http://3g.vehdjk.com/Article/details/gtgjylvfv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxkoqakfw.sHtML

[U97] JS：并发请求
来源：http://baike.epnwcf.com/Article/details/gttyytxuu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.vehdjk.com/Article/details/gqqamqjtg.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.yfazqb.com/Article/details/gyeyvuraq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fktsv.cn/Article/details/gzzdmmvkq.sHtML

[U99] JS：事件监听
来源：http://mobile.sjlbkw.cn/Article/details/grivnqlye.sHtML

el.addEventListener("click", e => {})
来源：http://wap.yfazqb.com/Article/details/gxllfekba.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fktsv.cn/Article/details/gmnmpokqq.sHtML

document.querySelector(".item")
来源：http://wap.bbcook.cn/Article/details/gjiaarpyl.sHtML

[U101] JS：classList 操作
来源：http://blog.vehdjk.com/Article/details/gfmecgtcr.sHtML

el.classList.toggle("active")
来源：http://baike.sjlbkw.cn/Article/details/gnswkknnr.sHtML

[U102] JS：本地存储
来源：http://www.m.share.sjlbkw.cn/Article/details/gubiqkbxh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.sjlbkw.cn/Article/details/gmpxoicwd.sHtML

[U103] JS：定时器
来源：http://m.share.yfazqb.com/Article/details/gofabnuyp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.bbcook.cn/Article/details/gndcekvci.sHtML

[U104] JS：防抖
来源：http://mobile.vehdjk.com/Article/details/glevjptxn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.sjlbkw.cn/Article/details/gprinvfys.sHtML

[U105] JS：节流
来源：http://baike.yfazqb.com/Article/details/gfbdyldve.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.bbcook.cn/Article/details/ggnmzrrbh.sHtML

[U106] JS：日期格式化
来源：http://m.share.bbcook.cn/Article/details/gyvnxtyzb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.yfazqb.com/Article/details/gxvyarpkm.sHtML

[U107] JS：数字千分位
来源：http://www.blog.sjlbkw.cn/Article/details/gbseoflsy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fktsv.cn/Article/details/gwmfagjpq.sHtML

[U108] JS：随机整数
来源：http://blog.vehdjk.com/Article/details/gihmwlkwc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.tarul.cn/Article/details/govndpzoz.sHtML

[U109] JS：数组分组
来源：http://read.share.bbcook.cn/Article/details/gvtynzjmp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.epnwcf.com/Article/details/ggnchwrhi.sHtML

[U110] JS：数组分块
来源：http://www.share.vehdjk.com/Article/details/gculiqiqf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.sjlbkw.cn/Article/details/gruvyyneb.sHtML

[U111] JS：对象转 Map
来源：http://m.share.tarul.cn/Article/details/gciikmpwf.sHtML

new Map(Object.entries(obj))
来源：http://www.share.vehdjk.com/Article/details/gfeapvhey.sHtML

[U112] JS：字符串补位
来源：http://www.share.epnwcf.com/Article/details/gwtrtjrce.sHtML

"7".padStart(3, "0")
来源：http://wap.bbcook.cn/Article/details/gtuuahzft.sHtML

[U113] JS：正则替换全部
来源：http://baike.bbcook.cn/Article/details/gqxxutlkc.sHtML

s.replaceAll("a", "b")
来源：http://www.share.tarul.cn/Article/details/geqibzjgd.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.epnwcf.com/Article/details/gofpbtjde.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fktsv.cn/Article/details/gvewrregu.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fktsv.cn/Article/details/gkxjlzjtl.sHtML

crypto.randomUUID()
来源：http://read.share.epnwcf.com/Article/details/gxqtcdovb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.tarul.cn/Article/details/garjfabdd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.sjlbkw.cn/Article/details/grtwaekyp.sHtML

[U117] JS：单元测试
来源：http://baike.vehdjk.com/Article/details/ghykxucoe.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.vehdjk.com/Article/details/gdhybfzig.sHtML

[U118] JS：开发服务器
来源：http://m.share.yfazqb.com/Article/details/geifhakiu.sHtML

npm i -D vite;  npx vite
来源：http://wap.yfazqb.com/Article/details/gqwtlrfgw.sHtML

[U119] JS：生产构建
来源：http://m.share.tarul.cn/Article/details/gaalpnids.sHtML

npx vite build
来源：http://www.m.share.fktsv.cn/Article/details/gjivajsrs.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.bbcook.cn/Article/details/gjiwdbsgl.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.sjlbkw.cn/Article/details/gooqxsqoa.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gubeminay.sHtML

统计汇总
来源：http://www.m.share.vehdjk.com/Article/details/gpulnbexb.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/guuqojzms.sHtML

按语言统计（条）：
来源：http://www.share.yfazqb.com/Article/details/gtboqpnbf.sHtML

Python ......... 252
来源：http://wap.bbcook.cn/Article/details/ghtbdsmtt.sHtML

PHP ............ 252
来源：http://mobile.vehdjk.com/Article/details/gnxlomwen.sHtML

JavaScript ..... 252
来源：http://www.blog.epnwcf.com/Article/details/gvveyrfhi.sHtML

TypeScript ..... 212
来源：http://blog.fktsv.cn/Article/details/gmqdzphzj.sHtML

Java ........... 212
来源：http://mobile.epnwcf.com/Article/details/grxsupqco.sHtML

Go ............. 212
来源：http://www.share.epnwcf.com/Article/details/gjzqvenqe.sHtML

Ruby ........... 212
来源：http://wap.epnwcf.com/Article/details/grjqcniuh.sHtML

C# ............. 212
来源：http://m.share.tarul.cn/Article/details/gvtkntwlk.sHtML

C .............. 30
来源：http://blog.fktsv.cn/Article/details/gqqvggpag.sHtML

C++ ............ 30
来源：http://www.m.share.sjlbkw.cn/Article/details/guysenpxm.sHtML

SQL ............ 90
来源：http://wap.vehdjk.com/Article/details/gealhnoad.sHtML

Bash ........... 80
来源：http://www.m.share.vehdjk.com/Article/details/gchdtefhc.sHtML

Kotlin ......... 15
来源：http://www.share.epnwcf.com/Article/details/gwcutmohr.sHtML

Swift .......... 15
来源：http://www.blog.bbcook.cn/Article/details/gqkyfcmrx.sHtML

Lua ............ 10
来源：http://www.blog.tarul.cn/Article/details/giohxvocg.sHtML

Perl ........... 10
来源：http://mobile.vehdjk.com/Article/details/gesxcjmdt.sHtML

Scala .......... 10
来源：http://blog.sjlbkw.cn/Article/details/giuieqzik.sHtML

------------------------------------
来源：http://www.blog.sjlbkw.cn/Article/details/gnixpgpmr.sHtML

合计 ........... 2106 条
来源：http://3g.yfazqb.com/Article/details/gxyktqhsv.sHtML

按章节统计：
来源：http://blog.yfazqb.com/Article/details/gqhfepamf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.tarul.cn/Article/details/gdhrslwmk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fktsv.cn/Article/details/gvxuqevvo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.epnwcf.com/Article/details/gmgeizuea.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.sjlbkw.cn/Article/details/gmldlzjsv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.epnwcf.com/Article/details/gllwrqpgn.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.yfazqb.com/Article/details/gebzcoajp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.bbcook.cn/Article/details/gemsujwiy.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.sjlbkw.cn/Article/details/gbexwzcnl.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.vehdjk.com/Article/details/gwdhdcgbu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.epnwcf.com/Article/details/gprrupcke.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.vehdjk.com/Article/details/gqwmrsifv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/gfihhdzyr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.tarul.cn/Article/details/gkobvkkdk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.bbcook.cn/Article/details/gtgolhakc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.sjlbkw.cn/Article/details/gqronqxtx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.sjlbkw.cn/Article/details/gnpsuheap.sHtML

Q SQL 专题                              90
来源：http://blog.bbcook.cn/Article/details/goutlqovm.sHtML

R Bash 专题                             80
来源：http://mobile.bbcook.cn/Article/details/gsmgpvcbp.sHtML

S C / C++ 专题                          60
来源：http://baike.yfazqb.com/Article/details/gutgzytbc.sHtML

T 其他语言补充                          60
来源：http://www.m.share.epnwcf.com/Article/details/gjhobmrhz.sHtML

U 高频实用片段                         120
来源：http://wap.vehdjk.com/Article/details/gbrsncgph.sHtML

------------------------------------
来源：http://wap.sjlbkw.cn/Article/details/gaoqrptlt.sHtML

合计                                  2106 条
来源：http://baike.epnwcf.com/Article/details/gpwpuqzfb.sHtML

--------------------------------------------------------------------------------
来源：http://baike.bbcook.cn/Article/details/gxmcgwuuk.sHtML

使用提醒
来源：http://m.share.vehdjk.com/Article/details/gyfzpydxd.sHtML

--------------------------------------------------------------------------------
来源：http://baike.epnwcf.com/Article/details/gfaknuahh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.bbcook.cn/Article/details/gczahjvfv.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.sjlbkw.cn/Article/details/gcokosyya.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fktsv.cn/Article/details/ghcbparim.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.sjlbkw.cn/Article/details/grjndcqjl.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.epnwcf.com/Article/details/gqzipqnty.sHtML

—— 文件结束 ——
来源：http://m.share.sjlbkw.cn/Article/details/gdgueygdq.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gbhuqezhw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.sjlbkw.cn/Article/details/grdubqkkt.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.epnwcf.com/Article/details/goiqszfgm.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/glxsxwngp.sHtML

【收录内容】
来源：http://wap.fktsv.cn/Article/details/goxfrycrw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fktsv.cn/Article/details/gygcjkzyn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.yfazqb.com/Article/details/gwsrsiyeu.sHtML

SQL · Bash · C · C++
来源：http://mobile.fktsv.cn/Article/details/guspfhtrd.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.vehdjk.com/Article/details/gpzuhhugl.sHtML

【使用说明】
来源：http://wap.yfazqb.com/Article/details/gunazmdic.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.epnwcf.com/Article/details/gbdsdzzkz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.yfazqb.com/Article/details/gvgbhsbvt.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.yfazqb.com/Article/details/gdihnhemb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.vehdjk.com/Article/details/gtbnlxvuz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fktsv.cn/Article/details/gsdzuicra.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.epnwcf.com/Article/details/gwlkqnfhy.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.yfazqb.com/Article/details/gulukazyn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.bbcook.cn/Article/details/gzliwbnry.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.yfazqb.com/Article/details/gkzcypikq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.epnwcf.com/Article/details/gvzgjcnke.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.epnwcf.com/Article/details/gjmehpxad.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.sjlbkw.cn/Article/details/gqzmvipbd.sHtML

【文件统计】
来源：http://www.share.sjlbkw.cn/Article/details/gzikvmnqx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.sjlbkw.cn/Article/details/gaspgdkob.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.tarul.cn/Article/details/gxftirmva.sHtML

目  录
来源：http://mobile.yfazqb.com/Article/details/gdzycltek.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.yfazqb.com/Article/details/glgdzgyhu.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.yfazqb.com/Article/details/gsnprogbj.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.vehdjk.com/Article/details/gscpqfghy.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.epnwcf.com/Article/details/gnpnvaoay.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.bbcook.cn/Article/details/gprphxqsz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.bbcook.cn/Article/details/gdiueliav.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.sjlbkw.cn/Article/details/gderscuvr.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.epnwcf.com/Article/details/gewcgijlg.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fktsv.cn/Article/details/ghcxzbbqm.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.epnwcf.com/Article/details/grvzlwpov.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fktsv.cn/Article/details/gtvcxxsjt.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.fktsv.cn/Article/details/gklruslce.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.sjlbkw.cn/Article/details/gtonwtqny.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.yfazqb.com/Article/details/gqikahypy.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.yfazqb.com/Article/details/gviyiwphf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.vehdjk.com/Article/details/gnnjvryej.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.epnwcf.com/Article/details/gouhkpvsi.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.tarul.cn/Article/details/gyzoeuype.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.sjlbkw.cn/Article/details/gwxxjdiay.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.tarul.cn/Article/details/gmlkqghez.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.tarul.cn/Article/details/gqljhhdzz.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/ggamrmvql.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gecncmvjv.sHtML

A. 基础语法与类型
来源：http://baike.vehdjk.com/Article/details/gazppnyrp.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gwuwvxvcc.sHtML

[A01] Hello World
来源：http://blog.bbcook.cn/Article/details/gwuhjttmu.sHtML

Py:   print("Hello, World!")
来源：http://www.share.vehdjk.com/Article/details/gbpumydaa.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.epnwcf.com/Article/details/ghbjvgrvq.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.fktsv.cn/Article/details/gireegtyq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.fktsv.cn/Article/details/ghdpzppog.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.bbcook.cn/Article/details/gbrsfxihg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.sjlbkw.cn/Article/details/gfkuzokll.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.vehdjk.com/Article/details/gikunrnrw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.vehdjk.com/Article/details/glzebddqs.sHtML

[A02] 变量声明与赋值
来源：http://read.share.vehdjk.com/Article/details/gxhvagbey.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.yfazqb.com/Article/details/gmucoyzcn.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.epnwcf.com/Article/details/gknxvzdch.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.fktsv.cn/Article/details/giafrifww.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.tarul.cn/Article/details/gswcrtnpr.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fktsv.cn/Article/details/gzkjymtvg.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fktsv.cn/Article/details/gamdbgjry.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.tarul.cn/Article/details/gcetpmlzq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.fktsv.cn/Article/details/gumdwoijc.sHtML

[A03] 常量定义
来源：http://3g.sjlbkw.cn/Article/details/gmfpouulj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.bbcook.cn/Article/details/gopglsbms.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.yfazqb.com/Article/details/gcplbdpnc.sHtML

JS:   const PI = 3.14159;
来源：http://blog.epnwcf.com/Article/details/grargmaqb.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.yfazqb.com/Article/details/gfaifcahv.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.yfazqb.com/Article/details/gdikkzgef.sHtML

Go:   const PI = 3.14159
来源：http://www.share.fktsv.cn/Article/details/godckaujq.sHtML

Ruby: PI = 3.14159
来源：http://3g.yfazqb.com/Article/details/gamtenskn.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.bbcook.cn/Article/details/gfarxafsz.sHtML

[A04] 判断变量类型
来源：http://m.share.yfazqb.com/Article/details/gzebmjwlg.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.epnwcf.com/Article/details/gofcugaeh.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.epnwcf.com/Article/details/gvltpmglc.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.epnwcf.com/Article/details/gtgwfvskw.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.bbcook.cn/Article/details/gvmhsepvx.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.vehdjk.com/Article/details/gkypqgvji.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.sjlbkw.cn/Article/details/giebpazpj.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.bbcook.cn/Article/details/gpoykurkk.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.fktsv.cn/Article/details/glljwzqvj.sHtML

[A05] 整数除法与取模
来源：http://blog.fktsv.cn/Article/details/gomhhhqze.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.sjlbkw.cn/Article/details/gnseojdoq.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.vehdjk.com/Article/details/ggfulhrzv.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.epnwcf.com/Article/details/gdspildyx.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fktsv.cn/Article/details/gjppykeqt.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.sjlbkw.cn/Article/details/gigakcqtl.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.yfazqb.com/Article/details/gdvruianf.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.fktsv.cn/Article/details/gigfmdmyt.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.epnwcf.com/Article/details/gmzopvnqy.sHtML

[A06] 字符串转数字
来源：http://m.share.fktsv.cn/Article/details/gihnjyqlq.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.sjlbkw.cn/Article/details/gehinvefo.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.vehdjk.com/Article/details/gqrnwtzhn.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.vehdjk.com/Article/details/gqkdzwsli.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.epnwcf.com/Article/details/gcwphxglb.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.epnwcf.com/Article/details/gvpqztfku.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.tarul.cn/Article/details/gxyvrqybr.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.tarul.cn/Article/details/gabmwqock.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.vehdjk.com/Article/details/gajvnmben.sHtML

[A07] 数字转字符串
来源：http://3g.vehdjk.com/Article/details/gpgmppmgm.sHtML

Py:   str(42)
来源：http://www.share.sjlbkw.cn/Article/details/gjloxmpnb.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.sjlbkw.cn/Article/details/gauqzskrm.sHtML

JS:   String(42); (42).toString()
来源：http://blog.vehdjk.com/Article/details/grwoikbiz.sHtML

TS:   String(42)
来源：http://blog.fktsv.cn/Article/details/gpiayxlvh.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.sjlbkw.cn/Article/details/gjnjprzrc.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.bbcook.cn/Article/details/gdxwzeaoy.sHtML

Ruby: 42.to_s
来源：http://m.share.bbcook.cn/Article/details/gklujubkz.sHtML

C#:   42.ToString()
来源：http://www.m.share.bbcook.cn/Article/details/gdecazmdb.sHtML

[A08] 取整与四舍五入
来源：http://blog.fktsv.cn/Article/details/gmqdeggnn.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.bbcook.cn/Article/details/givmcrbnk.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.bbcook.cn/Article/details/gpdxvafdp.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.sjlbkw.cn/Article/details/gbmgitoto.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.sjlbkw.cn/Article/details/gwnmjmyrf.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.tarul.cn/Article/details/gupicptad.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.epnwcf.com/Article/details/gnnyytgxv.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.tarul.cn/Article/details/gjxiktvxp.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.sjlbkw.cn/Article/details/guoiqlrxv.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.fktsv.cn/Article/details/gocrypwqp.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.epnwcf.com/Article/details/gtcxwiusz.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.tarul.cn/Article/details/gzjgycsqc.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.epnwcf.com/Article/details/gqkbdtofk.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.tarul.cn/Article/details/gnblynxjl.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.vehdjk.com/Article/details/gjjzwuvyb.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.fktsv.cn/Article/details/gjepoydeg.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.epnwcf.com/Article/details/gfzsgnbsy.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.fktsv.cn/Article/details/gchnaduru.sHtML


<!-- 参考信息 -->