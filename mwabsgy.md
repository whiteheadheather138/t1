代发 wailian999

[U61] PHP：正则
来源：http://www.blog.bbcook.cn/Article/details/gjswhgiug.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.sjlbkw.cn/Article/details/gmxwcursp.sHtML

[U62] PHP：日期对象
来源：http://read.share.bbcook.cn/Article/details/gtsqmfsgj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.bbcook.cn/Article/details/gyqbcvyvn.sHtML

[U63] PHP：文件读写
来源：http://blog.bbcook.cn/Article/details/geuibyheh.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fktsv.cn/Article/details/gtjrorjgj.sHtML

[U64] PHP：目录遍历
来源：http://baike.fktsv.cn/Article/details/grmotlxpv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.tarul.cn/Article/details/gezsjafud.sHtML

[U65] PHP：会话
来源：http://m.share.yfazqb.com/Article/details/gyiwjiomw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.tarul.cn/Article/details/gvabnljgz.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.yfazqb.com/Article/details/gfrsdjajv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.tarul.cn/Article/details/gtxuuinof.sHtML

[U67] PHP：处理文件上传
来源：http://wap.bbcook.cn/Article/details/gxeivpocf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.bbcook.cn/Article/details/gfygabahv.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.tarul.cn/Article/details/girmfiisr.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.vehdjk.com/Article/details/gograjvlc.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.yfazqb.com/Article/details/gfwykasnm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fktsv.cn/Article/details/grlzpvzln.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.epnwcf.com/Article/details/gxpmkpmur.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.tarul.cn/Article/details/ghablkczo.sHtML

[U71] PHP：抛出异常
来源：http://wap.tarul.cn/Article/details/gzmziiqdz.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.vehdjk.com/Article/details/gvbvaxtsk.sHtML

[U72] PHP：写错误日志
来源：http://baike.vehdjk.com/Article/details/gdisycexm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.sjlbkw.cn/Article/details/gokijzkzg.sHtML

[U73] PHP：读取 ini 配置
来源：http://m.share.sjlbkw.cn/Article/details/gjrlqehtn.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.bbcook.cn/Article/details/gfgofauzs.sHtML

[U74] PHP：读取环境变量
来源：http://3g.bbcook.cn/Article/details/grxnbucyu.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.tarul.cn/Article/details/geqbatdub.sHtML

[U75] PHP：依赖注入
来源：http://3g.fktsv.cn/Article/details/gpqnyfkgt.sHtML

composer require psr/container
来源：http://mobile.bbcook.cn/Article/details/gtfrxzubq.sHtML

[U76] PHP：简单路由
来源：http://m.share.yfazqb.com/Article/details/gkoruhghi.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.epnwcf.com/Article/details/gyyvedcma.sHtML

[U77] PHP：模板渲染
来源：http://read.share.sjlbkw.cn/Article/details/gsjrliacr.sHtML

composer require twig/twig
来源：http://baike.sjlbkw.cn/Article/details/gpuvisszj.sHtML

[U78] PHP：单元测试
来源：http://baike.tarul.cn/Article/details/gwaunrebh.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.yfazqb.com/Article/details/gqwfveazr.sHtML

[U79] PHP：静态分析
来源：http://m.share.bbcook.cn/Article/details/gxiiyyyze.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.epnwcf.com/Article/details/gewxdjyno.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.bbcook.cn/Article/details/gomchuxdt.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.vehdjk.com/Article/details/gpynantiz.sHtML

[U81] JS：初始化项目
来源：http://mobile.tarul.cn/Article/details/ghovbinqg.sHtML

npm init -y;  npm i express
来源：http://blog.bbcook.cn/Article/details/gvilxwifi.sHtML

[U82] JS：package.json 脚本
来源：http://blog.yfazqb.com/Article/details/grsgdtkfb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fktsv.cn/Article/details/golmmiigl.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.epnwcf.com/Article/details/gxvtevtih.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fktsv.cn/Article/details/gjocxaxvc.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.epnwcf.com/Article/details/gmzuktvrn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.epnwcf.com/Article/details/gmomcmdki.sHtML

[U85] JS：可选链
来源：http://www.m.share.vehdjk.com/Article/details/ghmgxcdae.sHtML

a?.b?.c
来源：http://mobile.epnwcf.com/Article/details/gyeapvdip.sHtML

[U86] JS：空值合并
来源：http://3g.fktsv.cn/Article/details/gyjkiwtzk.sHtML

a ?? b
来源：http://mobile.epnwcf.com/Article/details/gbcsqgdgb.sHtML

[U87] JS：解构默认值
来源：http://read.share.yfazqb.com/Article/details/gikzlmjxc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.bbcook.cn/Article/details/gavitlwgn.sHtML

[U88] JS：对象展开合并
来源：http://3g.bbcook.cn/Article/details/gspkptahz.sHtML

{ ...a, ...b }
来源：http://mobile.tarul.cn/Article/details/gpimcvhgj.sHtML

[U89] JS：数组去重
来源：http://www.m.share.epnwcf.com/Article/details/grfkbarjl.sHtML

[...new Set(arr)]
来源：http://m.share.vehdjk.com/Article/details/gxhbtpkpy.sHtML

[U90] JS：数字数组排序
来源：http://m.share.sjlbkw.cn/Article/details/gbknqfucv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.yfazqb.com/Article/details/grirgqlaz.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.sjlbkw.cn/Article/details/glpfydscj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.vehdjk.com/Article/details/gglywqwxf.sHtML

[U92] JS：深拷贝
来源：http://mobile.fktsv.cn/Article/details/gfogxzamd.sHtML

structuredClone(obj)
来源：http://www.blog.yfazqb.com/Article/details/gxveqiklf.sHtML

[U93] JS：模板字符串
来源：http://read.share.sjlbkw.cn/Article/details/gousvofku.sHtML

`共 ${n} 条`
来源：http://read.share.epnwcf.com/Article/details/gtmqnpqvt.sHtML

[U94] JS：箭头函数
来源：http://www.blog.vehdjk.com/Article/details/gmpyugoyq.sHtML

const double = x => x * 2;
来源：http://blog.sjlbkw.cn/Article/details/gwsyfikor.sHtML

[U95] JS：Promise 包装
来源：http://mobile.bbcook.cn/Article/details/gsuuaxmsj.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.vehdjk.com/Article/details/gwsetowzb.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.tarul.cn/Article/details/gqmrjzoqk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.bbcook.cn/Article/details/gxqcfyzki.sHtML

[U97] JS：并发请求
来源：http://blog.yfazqb.com/Article/details/gcilkkdmz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.yfazqb.com/Article/details/gqkqpnvuc.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.yfazqb.com/Article/details/gfumafypk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.epnwcf.com/Article/details/gxfrzydef.sHtML

[U99] JS：事件监听
来源：http://blog.yfazqb.com/Article/details/gmxzuoqwy.sHtML

el.addEventListener("click", e => {})
来源：http://3g.sjlbkw.cn/Article/details/glpykwshe.sHtML

[U100] JS：DOM 查询
来源：http://wap.yfazqb.com/Article/details/gnoajoicl.sHtML

document.querySelector(".item")
来源：http://www.m.share.yfazqb.com/Article/details/gjuiiqyav.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fktsv.cn/Article/details/gyuejzarv.sHtML

el.classList.toggle("active")
来源：http://read.share.tarul.cn/Article/details/gwwuuruwn.sHtML

[U102] JS：本地存储
来源：http://baike.epnwcf.com/Article/details/ggafevolx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.yfazqb.com/Article/details/gwlcdvkwo.sHtML

[U103] JS：定时器
来源：http://mobile.epnwcf.com/Article/details/grbchndnb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.sjlbkw.cn/Article/details/gippotidi.sHtML

[U104] JS：防抖
来源：http://mobile.fktsv.cn/Article/details/gupzykaol.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.tarul.cn/Article/details/gpnnlibmf.sHtML

[U105] JS：节流
来源：http://read.share.fktsv.cn/Article/details/grshcetal.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.vehdjk.com/Article/details/gjqcotodz.sHtML

[U106] JS：日期格式化
来源：http://baike.vehdjk.com/Article/details/gjunjpjhg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.bbcook.cn/Article/details/gooqtwqao.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.tarul.cn/Article/details/gwzjfskpn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.vehdjk.com/Article/details/gkwhwfecn.sHtML

[U108] JS：随机整数
来源：http://www.share.vehdjk.com/Article/details/gilgvpjca.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.epnwcf.com/Article/details/gmkvpwuof.sHtML

[U109] JS：数组分组
来源：http://read.share.vehdjk.com/Article/details/grfxpiszz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmdugaqb.sHtML

[U110] JS：数组分块
来源：http://mobile.bbcook.cn/Article/details/gaoqdxyrz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fktsv.cn/Article/details/gdzhibkqe.sHtML

[U111] JS：对象转 Map
来源：http://m.share.sjlbkw.cn/Article/details/gadztznlk.sHtML

new Map(Object.entries(obj))
来源：http://wap.tarul.cn/Article/details/gkopekufo.sHtML

[U112] JS：字符串补位
来源：http://www.share.epnwcf.com/Article/details/gsmjztanx.sHtML

"7".padStart(3, "0")
来源：http://www.blog.tarul.cn/Article/details/gshqiszuv.sHtML

[U113] JS：正则替换全部
来源：http://wap.tarul.cn/Article/details/gryrjgkhe.sHtML

s.replaceAll("a", "b")
来源：http://m.share.epnwcf.com/Article/details/glumvpwfg.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.vehdjk.com/Article/details/gzffwqarr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fktsv.cn/Article/details/gkikhpxlq.sHtML

[U115] JS：生成 UUID
来源：http://www.share.tarul.cn/Article/details/ggzybxvuw.sHtML

crypto.randomUUID()
来源：http://www.share.fktsv.cn/Article/details/giyxwmnyn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.vehdjk.com/Article/details/givrurvgt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.vehdjk.com/Article/details/gqufccuyz.sHtML

[U117] JS：单元测试
来源：http://wap.yfazqb.com/Article/details/grcyxokaw.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.vehdjk.com/Article/details/gndkqovza.sHtML

[U118] JS：开发服务器
来源：http://read.share.fktsv.cn/Article/details/gmtohmdfh.sHtML

npm i -D vite;  npx vite
来源：http://www.share.tarul.cn/Article/details/gjkhygedr.sHtML

[U119] JS：生产构建
来源：http://read.share.sjlbkw.cn/Article/details/ggdrcgaak.sHtML

npx vite build
来源：http://www.share.epnwcf.com/Article/details/ghfwkdmki.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fktsv.cn/Article/details/gpafbywbn.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.sjlbkw.cn/Article/details/gpzlstuzj.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gwcmurenk.sHtML

统计汇总
来源：http://www.blog.tarul.cn/Article/details/grsjexian.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gyqmhacvb.sHtML

按语言统计（条）：
来源：http://www.m.share.sjlbkw.cn/Article/details/gmwoxtwng.sHtML

Python ......... 252
来源：http://read.share.vehdjk.com/Article/details/glnssoulf.sHtML

PHP ............ 252
来源：http://m.share.vehdjk.com/Article/details/gupovpaao.sHtML

JavaScript ..... 252
来源：http://baike.vehdjk.com/Article/details/ghwgsrwby.sHtML

TypeScript ..... 212
来源：http://blog.epnwcf.com/Article/details/gqbkkwvzh.sHtML

Java ........... 212
来源：http://m.share.epnwcf.com/Article/details/ggbaqomdg.sHtML

Go ............. 212
来源：http://baike.sjlbkw.cn/Article/details/gktqqwyaf.sHtML

Ruby ........... 212
来源：http://3g.bbcook.cn/Article/details/gwlsodkxn.sHtML

C# ............. 212
来源：http://www.share.epnwcf.com/Article/details/gixhpfjui.sHtML

C .............. 30
来源：http://mobile.bbcook.cn/Article/details/gknhufczd.sHtML

C++ ............ 30
来源：http://www.blog.sjlbkw.cn/Article/details/gfjisedcn.sHtML

SQL ............ 90
来源：http://m.share.tarul.cn/Article/details/gyzutmoqo.sHtML

Bash ........... 80
来源：http://read.share.sjlbkw.cn/Article/details/grmzvzcpi.sHtML

Kotlin ......... 15
来源：http://www.m.share.sjlbkw.cn/Article/details/gikykuysz.sHtML

Swift .......... 15
来源：http://3g.fktsv.cn/Article/details/gbdabgwuc.sHtML

Lua ............ 10
来源：http://m.share.yfazqb.com/Article/details/gvzzgpvuc.sHtML

Perl ........... 10
来源：http://www.m.share.bbcook.cn/Article/details/gablzmumw.sHtML

Scala .......... 10
来源：http://www.m.share.yfazqb.com/Article/details/gwdwinezu.sHtML

------------------------------------
来源：http://read.share.vehdjk.com/Article/details/gwrghscig.sHtML

合计 ........... 2106 条
来源：http://blog.fktsv.cn/Article/details/gflsqgyot.sHtML

按章节统计：
来源：http://m.share.tarul.cn/Article/details/gghaiusfn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.yfazqb.com/Article/details/ghlbkutyv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.yfazqb.com/Article/details/gocztytvi.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.sjlbkw.cn/Article/details/gxtdmmwew.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.yfazqb.com/Article/details/gswfuskcm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fktsv.cn/Article/details/gazdnzaww.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.yfazqb.com/Article/details/gpoxirbuv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fktsv.cn/Article/details/gkdvqeuui.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fktsv.cn/Article/details/gvgjijdab.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.tarul.cn/Article/details/gyxcnixnu.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.sjlbkw.cn/Article/details/gloxakpkt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.bbcook.cn/Article/details/gtqhgwdbs.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.tarul.cn/Article/details/glrzzomhn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.epnwcf.com/Article/details/gsoisgugt.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.vehdjk.com/Article/details/gnoivptih.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.bbcook.cn/Article/details/grpwdwjhr.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.vehdjk.com/Article/details/ghltsehjd.sHtML

Q SQL 专题                              90
来源：http://3g.bbcook.cn/Article/details/gqsxjeoke.sHtML

R Bash 专题                             80
来源：http://www.blog.sjlbkw.cn/Article/details/gmktkchol.sHtML

S C / C++ 专题                          60
来源：http://wap.bbcook.cn/Article/details/gmyalmuhg.sHtML

T 其他语言补充                          60
来源：http://mobile.tarul.cn/Article/details/gbrnldcha.sHtML

U 高频实用片段                         120
来源：http://read.share.yfazqb.com/Article/details/gfdblicjc.sHtML

------------------------------------
来源：http://www.blog.yfazqb.com/Article/details/gpxedhpre.sHtML

合计                                  2106 条
来源：http://baike.yfazqb.com/Article/details/grpcpxevc.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.bbcook.cn/Article/details/gmrucpwvf.sHtML

使用提醒
来源：http://www.m.share.tarul.cn/Article/details/giukikivh.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fktsv.cn/Article/details/gymbtzkls.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.epnwcf.com/Article/details/gyrnpfhtw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.sjlbkw.cn/Article/details/gyqydtise.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.vehdjk.com/Article/details/gaozydcoy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.tarul.cn/Article/details/gryzujeiy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.sjlbkw.cn/Article/details/gjjrdnmjw.sHtML

—— 文件结束 ——
来源：http://www.m.share.sjlbkw.cn/Article/details/gvrimwjpw.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gmbtqfitp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.vehdjk.com/Article/details/gwivyhjwa.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.vehdjk.com/Article/details/gbzjcblqt.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/grocbrqxm.sHtML

【收录内容】
来源：http://www.blog.sjlbkw.cn/Article/details/gqdldsftg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.fktsv.cn/Article/details/gqmmdfvev.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.vehdjk.com/Article/details/gfwasldbj.sHtML

SQL · Bash · C · C++
来源：http://www.share.bbcook.cn/Article/details/gziololug.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.bbcook.cn/Article/details/gbffriqfd.sHtML

【使用说明】
来源：http://read.share.sjlbkw.cn/Article/details/glwinnbsz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.vehdjk.com/Article/details/gurhvkpma.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.fktsv.cn/Article/details/gvjcriknd.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.tarul.cn/Article/details/gelivlwdl.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fktsv.cn/Article/details/gxwvpznvu.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.sjlbkw.cn/Article/details/gxmszyvig.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.yfazqb.com/Article/details/gauigpbxj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.yfazqb.com/Article/details/gxrbmaabk.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.bbcook.cn/Article/details/ghawvgzob.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.tarul.cn/Article/details/gsdckdkeh.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.bbcook.cn/Article/details/gxtawtfuf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.vehdjk.com/Article/details/gowamtbkm.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.vehdjk.com/Article/details/gjsilqwva.sHtML

【文件统计】
来源：http://www.blog.yfazqb.com/Article/details/glcbauwxy.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.yfazqb.com/Article/details/gnfqbiccq.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.vehdjk.com/Article/details/gydqfdmrx.sHtML

目  录
来源：http://baike.yfazqb.com/Article/details/gxfupxuou.sHtML

--------------------------------------------------------------------------------
来源：http://3g.tarul.cn/Article/details/ggnbeyptq.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.bbcook.cn/Article/details/ggmiqgbzb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.vehdjk.com/Article/details/gdcrosjfu.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.tarul.cn/Article/details/gpxtgykaf.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.epnwcf.com/Article/details/gfydoyswg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.tarul.cn/Article/details/goehepmvg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.yfazqb.com/Article/details/gqtmnzocz.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.fktsv.cn/Article/details/gifxkdibn.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fktsv.cn/Article/details/goyehfpjt.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.tarul.cn/Article/details/gsoanqhhr.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.tarul.cn/Article/details/gapxrzuot.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.fktsv.cn/Article/details/gnavdotkw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.bbcook.cn/Article/details/gajdrnwih.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.sjlbkw.cn/Article/details/gaqdqpvcs.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.vehdjk.com/Article/details/gzggfpydn.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.yfazqb.com/Article/details/gcwdrdzgg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.fktsv.cn/Article/details/gwaaorbvy.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.fktsv.cn/Article/details/gdwhdqptt.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.yfazqb.com/Article/details/gehhurydd.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.epnwcf.com/Article/details/gsjhvhekg.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fktsv.cn/Article/details/gkpjtugag.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.yfazqb.com/Article/details/gejngcrjw.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/ghjtqjoww.sHtML

A. 基础语法与类型
来源：http://www.blog.epnwcf.com/Article/details/gczremowd.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gkbpcrogm.sHtML

[A01] Hello World
来源：http://mobile.sjlbkw.cn/Article/details/gruzfwmkx.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.sjlbkw.cn/Article/details/gdbkjccbg.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.fktsv.cn/Article/details/gdgavpzlk.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.vehdjk.com/Article/details/gswicgylg.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.bbcook.cn/Article/details/ggcawshti.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.sjlbkw.cn/Article/details/guksztjbf.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.epnwcf.com/Article/details/gyxprusbd.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fktsv.cn/Article/details/gwfljgyju.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.tarul.cn/Article/details/ggelqdhzq.sHtML

[A02] 变量声明与赋值
来源：http://mobile.yfazqb.com/Article/details/gcmggyeer.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.epnwcf.com/Article/details/gjdprvraz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.epnwcf.com/Article/details/gklemqcci.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.epnwcf.com/Article/details/ggnrmibbc.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.tarul.cn/Article/details/gyndtnabs.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.vehdjk.com/Article/details/gkweusdse.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.bbcook.cn/Article/details/ghxsfouln.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.fktsv.cn/Article/details/gxczkyifx.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.tarul.cn/Article/details/gxpwqrfgy.sHtML

[A03] 常量定义
来源：http://wap.sjlbkw.cn/Article/details/gkuoyycoq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.tarul.cn/Article/details/gzcfitxdn.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.sjlbkw.cn/Article/details/glcnlfnad.sHtML

JS:   const PI = 3.14159;
来源：http://wap.epnwcf.com/Article/details/gesgjlhjk.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.sjlbkw.cn/Article/details/gawwkxork.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.bbcook.cn/Article/details/gwhqrbkqg.sHtML

Go:   const PI = 3.14159
来源：http://3g.bbcook.cn/Article/details/gkssexspq.sHtML

Ruby: PI = 3.14159
来源：http://blog.tarul.cn/Article/details/gkpiqahxn.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.yfazqb.com/Article/details/gyxdcsrmu.sHtML

[A04] 判断变量类型
来源：http://mobile.tarul.cn/Article/details/gvdjblnfg.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.vehdjk.com/Article/details/gxurppduf.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.epnwcf.com/Article/details/gndycksyz.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.sjlbkw.cn/Article/details/gumilawqk.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.fktsv.cn/Article/details/gcaafluzr.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.fktsv.cn/Article/details/gndcgovxo.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.bbcook.cn/Article/details/gzoirvfwl.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.bbcook.cn/Article/details/givfzccpy.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.fktsv.cn/Article/details/gnsagsohu.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.tarul.cn/Article/details/gyefvdbia.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.sjlbkw.cn/Article/details/gukhgfcmy.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.sjlbkw.cn/Article/details/gpkihnlek.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.tarul.cn/Article/details/gryzgwvwp.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.tarul.cn/Article/details/gebjklsfi.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.sjlbkw.cn/Article/details/gqohhoasq.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.yfazqb.com/Article/details/gbrwtfimz.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.yfazqb.com/Article/details/geseqcuio.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.epnwcf.com/Article/details/gsillkuww.sHtML

[A06] 字符串转数字
来源：http://read.share.sjlbkw.cn/Article/details/gajqixlbo.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.vehdjk.com/Article/details/gpijnsafk.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.vehdjk.com/Article/details/gbbxkltjd.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.yfazqb.com/Article/details/gblzsggst.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.vehdjk.com/Article/details/guqevjgrx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.tarul.cn/Article/details/giiwajgrk.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.vehdjk.com/Article/details/gnxqfiwqo.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.tarul.cn/Article/details/gpxwkuepn.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.tarul.cn/Article/details/gzyxkgkfw.sHtML

[A07] 数字转字符串
来源：http://www.m.share.fktsv.cn/Article/details/gonbxtojh.sHtML

Py:   str(42)
来源：http://wap.tarul.cn/Article/details/gmalxnqek.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.tarul.cn/Article/details/gvkzyefxy.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.sjlbkw.cn/Article/details/gbclglacx.sHtML

TS:   String(42)
来源：http://baike.sjlbkw.cn/Article/details/gudtzbwti.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.fktsv.cn/Article/details/gmksyolqi.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.bbcook.cn/Article/details/gizxwicgk.sHtML

Ruby: 42.to_s
来源：http://www.blog.epnwcf.com/Article/details/gatvbetxq.sHtML

C#:   42.ToString()
来源：http://www.m.share.bbcook.cn/Article/details/gheyhrcqt.sHtML

[A08] 取整与四舍五入
来源：http://mobile.sjlbkw.cn/Article/details/gmehohoht.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.sjlbkw.cn/Article/details/gvslilibq.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.vehdjk.com/Article/details/gpupyqlze.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.epnwcf.com/Article/details/gmfnlgfnn.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.vehdjk.com/Article/details/gbvcbinzn.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.vehdjk.com/Article/details/gsmttsdqw.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.epnwcf.com/Article/details/gvzmxadqp.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.bbcook.cn/Article/details/gmpxeywct.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.bbcook.cn/Article/details/gpztdczkn.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.sjlbkw.cn/Article/details/guybvcgpf.sHtML


<!-- 参考信息 -->