代发 wailian999

[U61] PHP：正则
来源：http://baike.yfazqb.com/Article/details/gkltybbse.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.bbcook.cn/Article/details/givqzwxfg.sHtML

[U62] PHP：日期对象
来源：http://baike.tarul.cn/Article/details/ghvlzltjm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.sjlbkw.cn/Article/details/gfpxteitw.sHtML

[U63] PHP：文件读写
来源：http://mobile.bbcook.cn/Article/details/gxpvroriy.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.yfazqb.com/Article/details/gkcqmlaxc.sHtML

[U64] PHP：目录遍历
来源：http://www.share.bbcook.cn/Article/details/gljwfduzt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.tarul.cn/Article/details/gnsrdlbgs.sHtML

[U65] PHP：会话
来源：http://3g.vehdjk.com/Article/details/gmyefisge.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.vehdjk.com/Article/details/gcnreddvw.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.bbcook.cn/Article/details/gdegybpsc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.epnwcf.com/Article/details/gfosjhbsc.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.yfazqb.com/Article/details/gilzoezje.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.bbcook.cn/Article/details/gbvglmfvw.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.tarul.cn/Article/details/gdikrecto.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.vehdjk.com/Article/details/gfkiqipuf.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.bbcook.cn/Article/details/gxkvpjkdp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fktsv.cn/Article/details/gemkxoaxp.sHtML

[U70] PHP：PDO 事务
来源：http://3g.epnwcf.com/Article/details/gcwzwxwqz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.vehdjk.com/Article/details/gsdjfetru.sHtML

[U71] PHP：抛出异常
来源：http://3g.vehdjk.com/Article/details/gfdudvdbd.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.bbcook.cn/Article/details/gwjflwcyw.sHtML

[U72] PHP：写错误日志
来源：http://wap.tarul.cn/Article/details/ggfusdkiy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.bbcook.cn/Article/details/gylakhgun.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.sjlbkw.cn/Article/details/gomhjfzfs.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.fktsv.cn/Article/details/ggxodcile.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.epnwcf.com/Article/details/grmtsqszb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.bbcook.cn/Article/details/gdxeiypdr.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.tarul.cn/Article/details/gmsitgvwe.sHtML

composer require psr/container
来源：http://wap.bbcook.cn/Article/details/glmdtkexn.sHtML

[U76] PHP：简单路由
来源：http://3g.epnwcf.com/Article/details/gxrivmzgw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.yfazqb.com/Article/details/gpjdbqako.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.epnwcf.com/Article/details/grxwwsmck.sHtML

composer require twig/twig
来源：http://baike.sjlbkw.cn/Article/details/giagvaqgs.sHtML

[U78] PHP：单元测试
来源：http://www.blog.bbcook.cn/Article/details/gtjbsjqjy.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.yfazqb.com/Article/details/gpriccwzf.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.epnwcf.com/Article/details/gaqflmpgm.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.yfazqb.com/Article/details/guwxfvosg.sHtML

[U80] PHP：代码规范修复
来源：http://baike.fktsv.cn/Article/details/gcywtphau.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.vehdjk.com/Article/details/gooekodcq.sHtML

[U81] JS：初始化项目
来源：http://read.share.sjlbkw.cn/Article/details/grkclfvgx.sHtML

npm init -y;  npm i express
来源：http://read.share.epnwcf.com/Article/details/ghztxrmbi.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.sjlbkw.cn/Article/details/gdmcbhjdt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.tarul.cn/Article/details/gekhmxtjr.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.tarul.cn/Article/details/gkalhlpzi.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.yfazqb.com/Article/details/gjqthfdyr.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.tarul.cn/Article/details/gevwziwfl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.tarul.cn/Article/details/guvqdjvpe.sHtML

[U85] JS：可选链
来源：http://blog.bbcook.cn/Article/details/gudclrskt.sHtML

a?.b?.c
来源：http://mobile.sjlbkw.cn/Article/details/gmimlqtnt.sHtML

[U86] JS：空值合并
来源：http://www.blog.fktsv.cn/Article/details/gffnbwhfy.sHtML

a ?? b
来源：http://www.m.share.yfazqb.com/Article/details/gszenvhfp.sHtML

[U87] JS：解构默认值
来源：http://www.blog.bbcook.cn/Article/details/grdhzsmvi.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.epnwcf.com/Article/details/ggfubdrrn.sHtML

[U88] JS：对象展开合并
来源：http://mobile.yfazqb.com/Article/details/gtsmmfboe.sHtML

{ ...a, ...b }
来源：http://baike.fktsv.cn/Article/details/gbtkbrsxk.sHtML

[U89] JS：数组去重
来源：http://3g.epnwcf.com/Article/details/gctupnujg.sHtML

[...new Set(arr)]
来源：http://www.share.yfazqb.com/Article/details/gdyvqjedy.sHtML

[U90] JS：数字数组排序
来源：http://read.share.tarul.cn/Article/details/gcykusyyy.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.tarul.cn/Article/details/gmoiakvnt.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.bbcook.cn/Article/details/gjaebgqsg.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.yfazqb.com/Article/details/gcvfwmsph.sHtML

[U92] JS：深拷贝
来源：http://m.share.fktsv.cn/Article/details/ghqidjcvu.sHtML

structuredClone(obj)
来源：http://baike.yfazqb.com/Article/details/ggndzopvj.sHtML

[U93] JS：模板字符串
来源：http://m.share.sjlbkw.cn/Article/details/gcwxvvaze.sHtML

`共 ${n} 条`
来源：http://www.m.share.tarul.cn/Article/details/gpswqlkvh.sHtML

[U94] JS：箭头函数
来源：http://baike.bbcook.cn/Article/details/glgtzdpul.sHtML

const double = x => x * 2;
来源：http://3g.yfazqb.com/Article/details/gvlkputwg.sHtML

[U95] JS：Promise 包装
来源：http://mobile.tarul.cn/Article/details/gpprnmlkw.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.tarul.cn/Article/details/gjyymrbyl.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.tarul.cn/Article/details/gvaeoiavi.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.yfazqb.com/Article/details/gswlszfsc.sHtML

[U97] JS：并发请求
来源：http://read.share.tarul.cn/Article/details/gzegiihtx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.yfazqb.com/Article/details/gezpevzaq.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.bbcook.cn/Article/details/gsexpolga.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.tarul.cn/Article/details/gkdfhvdna.sHtML

[U99] JS：事件监听
来源：http://www.blog.epnwcf.com/Article/details/glrzrnftn.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.yfazqb.com/Article/details/goxdtkhws.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fktsv.cn/Article/details/gjgaldvwb.sHtML

document.querySelector(".item")
来源：http://baike.epnwcf.com/Article/details/gpxphizyg.sHtML

[U101] JS：classList 操作
来源：http://mobile.tarul.cn/Article/details/gwxcqatvt.sHtML

el.classList.toggle("active")
来源：http://baike.tarul.cn/Article/details/gqiwvmegg.sHtML

[U102] JS：本地存储
来源：http://www.share.bbcook.cn/Article/details/gqhqeofvs.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.yfazqb.com/Article/details/goeeozstg.sHtML

[U103] JS：定时器
来源：http://blog.bbcook.cn/Article/details/gugsudpdk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.tarul.cn/Article/details/gjwizmfwj.sHtML

[U104] JS：防抖
来源：http://baike.bbcook.cn/Article/details/gygleppld.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.bbcook.cn/Article/details/gsridzhwp.sHtML

[U105] JS：节流
来源：http://www.blog.vehdjk.com/Article/details/gklttopxr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.epnwcf.com/Article/details/gqmlsqitd.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.vehdjk.com/Article/details/guznnujkt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.vehdjk.com/Article/details/gqxhzzosj.sHtML

[U107] JS：数字千分位
来源：http://mobile.bbcook.cn/Article/details/ggocdzobm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.sjlbkw.cn/Article/details/gyjxwgcbq.sHtML

[U108] JS：随机整数
来源：http://wap.vehdjk.com/Article/details/gmgpgyqcx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.tarul.cn/Article/details/gatsacdkd.sHtML

[U109] JS：数组分组
来源：http://3g.yfazqb.com/Article/details/gpncvxnts.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.yfazqb.com/Article/details/gsnmorthq.sHtML

[U110] JS：数组分块
来源：http://www.m.share.tarul.cn/Article/details/gtapwmuxv.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.yfazqb.com/Article/details/gqtlanmce.sHtML

[U111] JS：对象转 Map
来源：http://m.share.yfazqb.com/Article/details/gbxxpxfsx.sHtML

new Map(Object.entries(obj))
来源：http://m.share.tarul.cn/Article/details/gjzrtedif.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.tarul.cn/Article/details/gpjpdvfbx.sHtML

"7".padStart(3, "0")
来源：http://m.share.tarul.cn/Article/details/guwicwzlv.sHtML

[U113] JS：正则替换全部
来源：http://blog.tarul.cn/Article/details/ggpcsprso.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.epnwcf.com/Article/details/gkfaztbsw.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fktsv.cn/Article/details/gfdrzhaic.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.bbcook.cn/Article/details/giznmooly.sHtML

[U115] JS：生成 UUID
来源：http://m.share.vehdjk.com/Article/details/gumqlqsqt.sHtML

crypto.randomUUID()
来源：http://www.share.fktsv.cn/Article/details/gwxvuzpnj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.epnwcf.com/Article/details/gwrljaymg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.epnwcf.com/Article/details/gjfkxpjdq.sHtML

[U117] JS：单元测试
来源：http://mobile.fktsv.cn/Article/details/gfavxmsbb.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.epnwcf.com/Article/details/gdvusfkly.sHtML

[U118] JS：开发服务器
来源：http://www.blog.bbcook.cn/Article/details/gjwoyxtzu.sHtML

npm i -D vite;  npx vite
来源：http://mobile.yfazqb.com/Article/details/gqitglzro.sHtML

[U119] JS：生产构建
来源：http://www.m.share.epnwcf.com/Article/details/gxcoawkao.sHtML

npx vite build
来源：http://read.share.sjlbkw.cn/Article/details/gjuarnhgv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.epnwcf.com/Article/details/gfbmkvmne.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.vehdjk.com/Article/details/gtlhefcag.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gtdztapci.sHtML

统计汇总
来源：http://wap.epnwcf.com/Article/details/gphyceyzo.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gyktrfbsh.sHtML

按语言统计（条）：
来源：http://3g.sjlbkw.cn/Article/details/goqypimly.sHtML

Python ......... 252
来源：http://3g.sjlbkw.cn/Article/details/gixmpowxn.sHtML

PHP ............ 252
来源：http://www.blog.yfazqb.com/Article/details/gnaxywktn.sHtML

JavaScript ..... 252
来源：http://3g.tarul.cn/Article/details/gtsuufcja.sHtML

TypeScript ..... 212
来源：http://www.m.share.fktsv.cn/Article/details/gyxkhquek.sHtML

Java ........... 212
来源：http://www.share.yfazqb.com/Article/details/gsawcygsp.sHtML

Go ............. 212
来源：http://blog.yfazqb.com/Article/details/gwcpiudde.sHtML

Ruby ........... 212
来源：http://read.share.epnwcf.com/Article/details/gxykpdazs.sHtML

C# ............. 212
来源：http://blog.epnwcf.com/Article/details/grisgbzwq.sHtML

C .............. 30
来源：http://baike.vehdjk.com/Article/details/ghokkfppz.sHtML

C++ ............ 30
来源：http://mobile.fktsv.cn/Article/details/gnqueuyua.sHtML

SQL ............ 90
来源：http://www.m.share.epnwcf.com/Article/details/glmlvwmda.sHtML

Bash ........... 80
来源：http://3g.bbcook.cn/Article/details/gprgqaipm.sHtML

Kotlin ......... 15
来源：http://wap.fktsv.cn/Article/details/ghwebuomt.sHtML

Swift .......... 15
来源：http://wap.bbcook.cn/Article/details/gcsabmpes.sHtML

Lua ............ 10
来源：http://wap.sjlbkw.cn/Article/details/gdqjjgrfy.sHtML

Perl ........... 10
来源：http://m.share.epnwcf.com/Article/details/grxyfieaj.sHtML

Scala .......... 10
来源：http://wap.fktsv.cn/Article/details/gqqwhpkxf.sHtML

------------------------------------
来源：http://read.share.epnwcf.com/Article/details/gojhgcywi.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fktsv.cn/Article/details/ggjwygmoe.sHtML

按章节统计：
来源：http://3g.bbcook.cn/Article/details/gladwcitf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.epnwcf.com/Article/details/gkvdheupr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.yfazqb.com/Article/details/gtvbcmrsj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.epnwcf.com/Article/details/gatvqgdgg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.tarul.cn/Article/details/gxnitcaci.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.epnwcf.com/Article/details/gjuwdpopp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.bbcook.cn/Article/details/gxahdfxzj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.vehdjk.com/Article/details/gcovkceag.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.sjlbkw.cn/Article/details/gzozzxvhy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.sjlbkw.cn/Article/details/gftrwsqhk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fktsv.cn/Article/details/gpivmvldd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.yfazqb.com/Article/details/goajcpceo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.tarul.cn/Article/details/gckfsfodw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.tarul.cn/Article/details/ghgopldkz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.epnwcf.com/Article/details/gpfcipdee.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.sjlbkw.cn/Article/details/gnxyklgwz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.tarul.cn/Article/details/gwuqaqgcg.sHtML

Q SQL 专题                              90
来源：http://www.share.bbcook.cn/Article/details/gahrtwaql.sHtML

R Bash 专题                             80
来源：http://mobile.yfazqb.com/Article/details/gtwmrwahp.sHtML

S C / C++ 专题                          60
来源：http://read.share.fktsv.cn/Article/details/gvhpwhxps.sHtML

T 其他语言补充                          60
来源：http://www.m.share.vehdjk.com/Article/details/ghykdyrzo.sHtML

U 高频实用片段                         120
来源：http://www.m.share.yfazqb.com/Article/details/gmyzfnxcm.sHtML

------------------------------------
来源：http://www.m.share.epnwcf.com/Article/details/gesqolgcr.sHtML

合计                                  2106 条
来源：http://baike.tarul.cn/Article/details/guidokcpm.sHtML

--------------------------------------------------------------------------------
来源：http://baike.bbcook.cn/Article/details/gtguexzyt.sHtML

使用提醒
来源：http://baike.fktsv.cn/Article/details/gbxfowgwl.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fktsv.cn/Article/details/gxfevbrhk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.epnwcf.com/Article/details/gklasfeyc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.sjlbkw.cn/Article/details/grhuvgkrm.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.bbcook.cn/Article/details/gimjseefn.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.tarul.cn/Article/details/geyscbjvp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.vehdjk.com/Article/details/gfflmwepg.sHtML

—— 文件结束 ——
来源：http://www.m.share.sjlbkw.cn/Article/details/gwpampmbz.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gnfewegnp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.sjlbkw.cn/Article/details/giqxijlfz.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fktsv.cn/Article/details/gjhjstbeh.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/grzfetzoo.sHtML

【收录内容】
来源：http://read.share.bbcook.cn/Article/details/gjpxufuhf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.tarul.cn/Article/details/gemyrdewc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.sjlbkw.cn/Article/details/gktriffrd.sHtML

SQL · Bash · C · C++
来源：http://wap.epnwcf.com/Article/details/gdqbaqdzd.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.sjlbkw.cn/Article/details/gurqvkdid.sHtML

【使用说明】
来源：http://wap.epnwcf.com/Article/details/grdxueswm.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.epnwcf.com/Article/details/gtjjrlnoc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fktsv.cn/Article/details/gzitdchkn.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.tarul.cn/Article/details/gucmvitke.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.tarul.cn/Article/details/ghggzgzee.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.tarul.cn/Article/details/goiixdxcc.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.bbcook.cn/Article/details/gorxeywsb.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.bbcook.cn/Article/details/ghhkxrhzg.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.epnwcf.com/Article/details/gkzmrnnxd.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.yfazqb.com/Article/details/gjhgucopn.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fktsv.cn/Article/details/gpoxwnxbu.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.tarul.cn/Article/details/gzqbxzrjb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.bbcook.cn/Article/details/gyjtyxxve.sHtML

【文件统计】
来源：http://read.share.bbcook.cn/Article/details/gqmrbavfm.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.vehdjk.com/Article/details/gnljdrxou.sHtML

--------------------------------------------------------------------------------
来源：http://wap.bbcook.cn/Article/details/gwkqokntg.sHtML

目  录
来源：http://www.share.tarul.cn/Article/details/ggltjohet.sHtML

--------------------------------------------------------------------------------
来源：http://wap.bbcook.cn/Article/details/gcdgqxsvk.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.bbcook.cn/Article/details/ggjepwktg.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fktsv.cn/Article/details/gzkyrvbol.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.epnwcf.com/Article/details/ggqmmbjwn.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.vehdjk.com/Article/details/gkgrczyrh.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.bbcook.cn/Article/details/gmjvxykcw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.tarul.cn/Article/details/gpbxnyeav.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.sjlbkw.cn/Article/details/gqvomtmas.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.sjlbkw.cn/Article/details/getfsjszy.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.bbcook.cn/Article/details/gwhheyppy.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.tarul.cn/Article/details/gdpjqbwtj.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.vehdjk.com/Article/details/gucnrcooa.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.vehdjk.com/Article/details/gglenwojw.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.sjlbkw.cn/Article/details/goubjafbn.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.epnwcf.com/Article/details/gvnlnaxlh.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/grfjcnuwr.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.epnwcf.com/Article/details/gugdzdyqc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.bbcook.cn/Article/details/gfytkgabb.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.bbcook.cn/Article/details/gxpniyfky.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.vehdjk.com/Article/details/ggwkoctfo.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.yfazqb.com/Article/details/gebzgdslo.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.vehdjk.com/Article/details/gqumldevc.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gwnyknnqj.sHtML

A. 基础语法与类型
来源：http://baike.yfazqb.com/Article/details/gzcxmllwa.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gdppkppbr.sHtML

[A01] Hello World
来源：http://wap.vehdjk.com/Article/details/ggpoczbuy.sHtML

Py:   print("Hello, World!")
来源：http://3g.bbcook.cn/Article/details/gnorcgkmv.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.yfazqb.com/Article/details/gfhkvntia.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.bbcook.cn/Article/details/gxjrxzpwr.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.epnwcf.com/Article/details/gtfkhmioa.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.yfazqb.com/Article/details/gvvyqqsqx.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.tarul.cn/Article/details/gnqecbdsb.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.tarul.cn/Article/details/gqiwrtbow.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fktsv.cn/Article/details/glqzyufqo.sHtML

[A02] 变量声明与赋值
来源：http://baike.fktsv.cn/Article/details/gblhdxbml.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.epnwcf.com/Article/details/gmjjokoth.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.epnwcf.com/Article/details/gwwaaexqw.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.vehdjk.com/Article/details/gjqbaaaph.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.sjlbkw.cn/Article/details/gvetmhoxu.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.bbcook.cn/Article/details/gnzybkdjz.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.yfazqb.com/Article/details/gxaygtaad.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.vehdjk.com/Article/details/ggsucewub.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.bbcook.cn/Article/details/gjfdkyaob.sHtML

[A03] 常量定义
来源：http://3g.vehdjk.com/Article/details/gyheflods.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.tarul.cn/Article/details/gdswwyaho.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.tarul.cn/Article/details/gfynfhjrk.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fktsv.cn/Article/details/gvarbafwf.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.tarul.cn/Article/details/gbicdssrf.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.yfazqb.com/Article/details/gkqvrnhsf.sHtML

Go:   const PI = 3.14159
来源：http://3g.fktsv.cn/Article/details/ggivitehj.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.tarul.cn/Article/details/gqikfkyih.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.sjlbkw.cn/Article/details/gjbrjwjtg.sHtML

[A04] 判断变量类型
来源：http://m.share.sjlbkw.cn/Article/details/ggoqglqxj.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.vehdjk.com/Article/details/ghjaoevkk.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.vehdjk.com/Article/details/goqhjcrsu.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.epnwcf.com/Article/details/ghgmmfgal.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.yfazqb.com/Article/details/ghvefqcbh.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.yfazqb.com/Article/details/gxydacykh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.yfazqb.com/Article/details/gbekmatoh.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.yfazqb.com/Article/details/gzthicwlj.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.tarul.cn/Article/details/gfqedssve.sHtML

[A05] 整数除法与取模
来源：http://blog.epnwcf.com/Article/details/gnlpizmki.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.tarul.cn/Article/details/gnoippsjr.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.vehdjk.com/Article/details/getekzhvy.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.vehdjk.com/Article/details/ggecivvor.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.bbcook.cn/Article/details/geurtcyqv.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.tarul.cn/Article/details/gsrcfexxe.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.fktsv.cn/Article/details/ggyezpept.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.tarul.cn/Article/details/gqvvrbbta.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.epnwcf.com/Article/details/gykfpxbld.sHtML

[A06] 字符串转数字
来源：http://baike.yfazqb.com/Article/details/grbkkynev.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.sjlbkw.cn/Article/details/gjandkivl.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.bbcook.cn/Article/details/gihmpxfif.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.yfazqb.com/Article/details/gpnhgpztp.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.tarul.cn/Article/details/gskonmqas.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.bbcook.cn/Article/details/gpqzobrvk.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.sjlbkw.cn/Article/details/gkxbavmid.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.yfazqb.com/Article/details/gtiiouvxu.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.tarul.cn/Article/details/gmuvsdmbu.sHtML

[A07] 数字转字符串
来源：http://baike.tarul.cn/Article/details/gxtnwkbdf.sHtML

Py:   str(42)
来源：http://3g.yfazqb.com/Article/details/gixeuyxve.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.tarul.cn/Article/details/gtpaiqvfl.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.bbcook.cn/Article/details/gdiywglmf.sHtML

TS:   String(42)
来源：http://blog.bbcook.cn/Article/details/gsilttftp.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.bbcook.cn/Article/details/gnxguljqk.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.tarul.cn/Article/details/gnxltitpm.sHtML

Ruby: 42.to_s
来源：http://wap.sjlbkw.cn/Article/details/giyojvfik.sHtML

C#:   42.ToString()
来源：http://www.share.fktsv.cn/Article/details/ggwwkqvlk.sHtML

[A08] 取整与四舍五入
来源：http://baike.epnwcf.com/Article/details/gxgyrmbib.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.bbcook.cn/Article/details/gdipineov.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.fktsv.cn/Article/details/gzzodjhxm.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.tarul.cn/Article/details/glhjuthex.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.fktsv.cn/Article/details/ggdyxucpq.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.yfazqb.com/Article/details/gmtcthzpy.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.bbcook.cn/Article/details/gmkzplbdk.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.tarul.cn/Article/details/gqwuowbez.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.yfazqb.com/Article/details/grjcryotk.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.vehdjk.com/Article/details/gesgxgnig.sHtML


<!-- 参考信息 -->