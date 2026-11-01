代发 wailian999

[U59] PHP：自定义排序
来源：http://read.share.bbcook.cn/Article/details/gnwdpcshw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.bbcook.cn/Article/details/gsmsetwpk.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.sjlbkw.cn/Article/details/gidddyagp.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.sjlbkw.cn/Article/details/gjzcpcgaw.sHtML

[U61] PHP：正则
来源：http://wap.tarul.cn/Article/details/gderpszld.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.bbcook.cn/Article/details/ghoettylo.sHtML

[U62] PHP：日期对象
来源：http://m.share.sjlbkw.cn/Article/details/gcljyeiym.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fktsv.cn/Article/details/ggjvuddjm.sHtML

[U63] PHP：文件读写
来源：http://3g.vehdjk.com/Article/details/gocpfntqi.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.bbcook.cn/Article/details/ghdihhczy.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.vehdjk.com/Article/details/gvvuqmybd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fktsv.cn/Article/details/gdykuwjis.sHtML

[U65] PHP：会话
来源：http://www.share.yfazqb.com/Article/details/gzftnetsk.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.bbcook.cn/Article/details/gcwappulx.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.vehdjk.com/Article/details/ghcdmzplt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.yfazqb.com/Article/details/grymsdiez.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fktsv.cn/Article/details/gxgnlpahp.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.yfazqb.com/Article/details/gczojzcpi.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fktsv.cn/Article/details/gznfxmlde.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.tarul.cn/Article/details/gmglwqaop.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.epnwcf.com/Article/details/gffelfqcn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.sjlbkw.cn/Article/details/guuylxeos.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.bbcook.cn/Article/details/ghiukggxn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.yfazqb.com/Article/details/gyftxglnj.sHtML

[U71] PHP：抛出异常
来源：http://baike.bbcook.cn/Article/details/glrpjtagi.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fktsv.cn/Article/details/guiptsczs.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.bbcook.cn/Article/details/gzpglegsv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.yfazqb.com/Article/details/gtfwqzutr.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.tarul.cn/Article/details/gdihqlbar.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.tarul.cn/Article/details/gsazdvvok.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.fktsv.cn/Article/details/gzgoloxqb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fktsv.cn/Article/details/gumeoxjia.sHtML

[U75] PHP：依赖注入
来源：http://read.share.fktsv.cn/Article/details/glzrcdjwx.sHtML

composer require psr/container
来源：http://www.blog.tarul.cn/Article/details/gscrnaarq.sHtML

[U76] PHP：简单路由
来源：http://3g.vehdjk.com/Article/details/gsgxhwkfu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.yfazqb.com/Article/details/ghzwidngm.sHtML

[U77] PHP：模板渲染
来源：http://blog.sjlbkw.cn/Article/details/gcqgjbroy.sHtML

composer require twig/twig
来源：http://3g.sjlbkw.cn/Article/details/gugekfibn.sHtML

[U78] PHP：单元测试
来源：http://blog.tarul.cn/Article/details/gvwklasll.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.sjlbkw.cn/Article/details/giajlbzxb.sHtML

[U79] PHP：静态分析
来源：http://m.share.yfazqb.com/Article/details/gewtmltsa.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.sjlbkw.cn/Article/details/gmczbiiiw.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.fktsv.cn/Article/details/gsfmpfpmb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.yfazqb.com/Article/details/gsyjbjmhy.sHtML

[U81] JS：初始化项目
来源：http://www.share.epnwcf.com/Article/details/gjolpaxan.sHtML

npm init -y;  npm i express
来源：http://www.share.tarul.cn/Article/details/gbfgvwqqt.sHtML

[U82] JS：package.json 脚本
来源：http://wap.bbcook.cn/Article/details/gdzqxijll.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fktsv.cn/Article/details/gjamvrcsg.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.sjlbkw.cn/Article/details/gvovgipyv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.bbcook.cn/Article/details/glteiesno.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.yfazqb.com/Article/details/gkcppptjt.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.yfazqb.com/Article/details/gfayblzkm.sHtML

[U85] JS：可选链
来源：http://www.share.sjlbkw.cn/Article/details/gxhoqahjb.sHtML

a?.b?.c
来源：http://3g.yfazqb.com/Article/details/gmqnsvtye.sHtML

[U86] JS：空值合并
来源：http://blog.epnwcf.com/Article/details/gdsocdwcn.sHtML

a ?? b
来源：http://3g.tarul.cn/Article/details/gutvswvcc.sHtML

[U87] JS：解构默认值
来源：http://m.share.bbcook.cn/Article/details/gkrfbhbvq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.yfazqb.com/Article/details/gjchxbvgc.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.fktsv.cn/Article/details/glekntkes.sHtML

{ ...a, ...b }
来源：http://www.share.fktsv.cn/Article/details/gjbiigptn.sHtML

[U89] JS：数组去重
来源：http://wap.tarul.cn/Article/details/gcnenfyse.sHtML

[...new Set(arr)]
来源：http://www.m.share.tarul.cn/Article/details/girezzjoz.sHtML

[U90] JS：数字数组排序
来源：http://3g.tarul.cn/Article/details/guwcuiwex.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.yfazqb.com/Article/details/gxmoefgti.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.epnwcf.com/Article/details/gumjtxbbu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.bbcook.cn/Article/details/gvlookmxj.sHtML

[U92] JS：深拷贝
来源：http://3g.tarul.cn/Article/details/gziyncluq.sHtML

structuredClone(obj)
来源：http://baike.fktsv.cn/Article/details/gsgciloph.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fktsv.cn/Article/details/gveifybsn.sHtML

`共 ${n} 条`
来源：http://3g.fktsv.cn/Article/details/gmrkqnexq.sHtML

[U94] JS：箭头函数
来源：http://www.blog.vehdjk.com/Article/details/gxdwgwdnu.sHtML

const double = x => x * 2;
来源：http://www.m.share.yfazqb.com/Article/details/gicpjcfaw.sHtML

[U95] JS：Promise 包装
来源：http://www.share.bbcook.cn/Article/details/gvixduuyr.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.sjlbkw.cn/Article/details/gldxgples.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.bbcook.cn/Article/details/gxzvhhqxc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.epnwcf.com/Article/details/gxcjyblzm.sHtML

[U97] JS：并发请求
来源：http://mobile.vehdjk.com/Article/details/gmcmuolbu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.tarul.cn/Article/details/gguzlzzql.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.tarul.cn/Article/details/ghrfilvnz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.tarul.cn/Article/details/gykuqiapl.sHtML

[U99] JS：事件监听
来源：http://www.share.epnwcf.com/Article/details/grdmduyyt.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.tarul.cn/Article/details/ghtmiqupd.sHtML

[U100] JS：DOM 查询
来源：http://mobile.sjlbkw.cn/Article/details/guckmjksf.sHtML

document.querySelector(".item")
来源：http://3g.epnwcf.com/Article/details/gkqmesuxy.sHtML

[U101] JS：classList 操作
来源：http://3g.sjlbkw.cn/Article/details/gxcmjvsfw.sHtML

el.classList.toggle("active")
来源：http://wap.bbcook.cn/Article/details/gntaymfsn.sHtML

[U102] JS：本地存储
来源：http://wap.epnwcf.com/Article/details/gjzaamjei.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fktsv.cn/Article/details/gbcxemwvy.sHtML

[U103] JS：定时器
来源：http://www.m.share.sjlbkw.cn/Article/details/gjgjdziri.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.epnwcf.com/Article/details/ggvbyvots.sHtML

[U104] JS：防抖
来源：http://mobile.fktsv.cn/Article/details/gelhzpxwk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.bbcook.cn/Article/details/gdxxcasav.sHtML

[U105] JS：节流
来源：http://blog.fktsv.cn/Article/details/gyvajiktq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fktsv.cn/Article/details/grlstldvr.sHtML

[U106] JS：日期格式化
来源：http://read.share.tarul.cn/Article/details/grxolnjsn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.tarul.cn/Article/details/gyluoljcf.sHtML

[U107] JS：数字千分位
来源：http://read.share.tarul.cn/Article/details/gonourcno.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.yfazqb.com/Article/details/gkmocsqyu.sHtML

[U108] JS：随机整数
来源：http://m.share.tarul.cn/Article/details/gvucdjuby.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.yfazqb.com/Article/details/gjmlorjdr.sHtML

[U109] JS：数组分组
来源：http://www.share.bbcook.cn/Article/details/gpbrkizfe.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.vehdjk.com/Article/details/gbwdzrjbo.sHtML

[U110] JS：数组分块
来源：http://mobile.yfazqb.com/Article/details/gxisdzxjl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.vehdjk.com/Article/details/gcgeuouft.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fktsv.cn/Article/details/griysnqzw.sHtML

new Map(Object.entries(obj))
来源：http://blog.vehdjk.com/Article/details/ghhptauvi.sHtML

[U112] JS：字符串补位
来源：http://read.share.sjlbkw.cn/Article/details/geplqamup.sHtML

"7".padStart(3, "0")
来源：http://wap.sjlbkw.cn/Article/details/gbtvqibwk.sHtML

[U113] JS：正则替换全部
来源：http://blog.yfazqb.com/Article/details/gqnvooaap.sHtML

s.replaceAll("a", "b")
来源：http://read.share.yfazqb.com/Article/details/ggurapemp.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.vehdjk.com/Article/details/gneqlujet.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.sjlbkw.cn/Article/details/ghwoksxbt.sHtML

[U115] JS：生成 UUID
来源：http://wap.epnwcf.com/Article/details/gcaesjpfj.sHtML

crypto.randomUUID()
来源：http://blog.bbcook.cn/Article/details/gckpxophr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.tarul.cn/Article/details/gwqdsbktq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.bbcook.cn/Article/details/gyipouspi.sHtML

[U117] JS：单元测试
来源：http://baike.tarul.cn/Article/details/ghpxgyugw.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fktsv.cn/Article/details/glxgatipg.sHtML

[U118] JS：开发服务器
来源：http://3g.fktsv.cn/Article/details/gssdvbnhv.sHtML

npm i -D vite;  npx vite
来源：http://read.share.vehdjk.com/Article/details/glzjunuoz.sHtML

[U119] JS：生产构建
来源：http://www.blog.yfazqb.com/Article/details/gwouysvtm.sHtML

npx vite build
来源：http://www.m.share.bbcook.cn/Article/details/gdtjjlkxq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.vehdjk.com/Article/details/gchbaxesb.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.epnwcf.com/Article/details/gcmcgjpph.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gelwnotnq.sHtML

统计汇总
来源：http://baike.vehdjk.com/Article/details/gsgyetatp.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gtvajsmwn.sHtML

按语言统计（条）：
来源：http://www.m.share.yfazqb.com/Article/details/gbemttdqv.sHtML

Python ......... 252
来源：http://wap.bbcook.cn/Article/details/gploqmbjk.sHtML

PHP ............ 252
来源：http://www.share.tarul.cn/Article/details/gmbadaodm.sHtML

JavaScript ..... 252
来源：http://www.blog.sjlbkw.cn/Article/details/grppiugoz.sHtML

TypeScript ..... 212
来源：http://mobile.fktsv.cn/Article/details/gphnhuqcr.sHtML

Java ........... 212
来源：http://3g.epnwcf.com/Article/details/gdeetzchq.sHtML

Go ............. 212
来源：http://m.share.yfazqb.com/Article/details/gpzwhglkd.sHtML

Ruby ........... 212
来源：http://wap.bbcook.cn/Article/details/gqdyxvuwt.sHtML

C# ............. 212
来源：http://www.share.fktsv.cn/Article/details/gsqjeyyqk.sHtML

C .............. 30
来源：http://mobile.epnwcf.com/Article/details/gbiyaqwjy.sHtML

C++ ............ 30
来源：http://wap.tarul.cn/Article/details/gjnmytxeg.sHtML

SQL ............ 90
来源：http://read.share.bbcook.cn/Article/details/gbbaridoh.sHtML

Bash ........... 80
来源：http://3g.bbcook.cn/Article/details/gzjhldyim.sHtML

Kotlin ......... 15
来源：http://m.share.fktsv.cn/Article/details/gwdkauxos.sHtML

Swift .......... 15
来源：http://www.share.bbcook.cn/Article/details/gtkakmzjp.sHtML

Lua ............ 10
来源：http://3g.bbcook.cn/Article/details/gcuojqvvi.sHtML

Perl ........... 10
来源：http://read.share.yfazqb.com/Article/details/grjfopnyi.sHtML

Scala .......... 10
来源：http://www.m.share.bbcook.cn/Article/details/gdojptlug.sHtML

------------------------------------
来源：http://m.share.epnwcf.com/Article/details/gsoopxjbz.sHtML

合计 ........... 2106 条
来源：http://mobile.vehdjk.com/Article/details/gciuhhvdb.sHtML

按章节统计：
来源：http://blog.sjlbkw.cn/Article/details/ggicoesyg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.yfazqb.com/Article/details/gkserhyrz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fktsv.cn/Article/details/gxmmlcczc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fktsv.cn/Article/details/grlthjrrt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.epnwcf.com/Article/details/gvsvfcilo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.bbcook.cn/Article/details/gbllykzoe.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.bbcook.cn/Article/details/gxbabncdv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.epnwcf.com/Article/details/gkncphulo.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.epnwcf.com/Article/details/gyydmqkvj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.yfazqb.com/Article/details/glikszbai.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.vehdjk.com/Article/details/gnyfxzjqb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.yfazqb.com/Article/details/gsvljsuol.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.vehdjk.com/Article/details/gfsngpwtf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fktsv.cn/Article/details/gsjdrjyou.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.epnwcf.com/Article/details/gvjgizcfm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.yfazqb.com/Article/details/gtrmobrsc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.epnwcf.com/Article/details/gloikkmcf.sHtML

Q SQL 专题                              90
来源：http://mobile.tarul.cn/Article/details/guvrcwaiw.sHtML

R Bash 专题                             80
来源：http://3g.fktsv.cn/Article/details/gimdvhcqx.sHtML

S C / C++ 专题                          60
来源：http://blog.tarul.cn/Article/details/gnxiqzaxc.sHtML

T 其他语言补充                          60
来源：http://blog.epnwcf.com/Article/details/gnihafrjf.sHtML

U 高频实用片段                         120
来源：http://3g.vehdjk.com/Article/details/gikdwtedf.sHtML

------------------------------------
来源：http://wap.sjlbkw.cn/Article/details/gjybruxxz.sHtML

合计                                  2106 条
来源：http://baike.tarul.cn/Article/details/gziozaegj.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fktsv.cn/Article/details/gfbesxjjv.sHtML

使用提醒
来源：http://www.blog.tarul.cn/Article/details/geztzgdsx.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.vehdjk.com/Article/details/ghwpdexlc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.bbcook.cn/Article/details/gkuwabfft.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.vehdjk.com/Article/details/gjwxdioez.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fktsv.cn/Article/details/gxmgdopby.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.tarul.cn/Article/details/gpdbrxnjh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fktsv.cn/Article/details/grrfqfxca.sHtML

—— 文件结束 ——
来源：http://www.blog.fktsv.cn/Article/details/gnuklvwnc.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gxnarndhg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.yfazqb.com/Article/details/gzovmpcpd.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.bbcook.cn/Article/details/gminyqdhf.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gbfmlkbpq.sHtML

【收录内容】
来源：http://3g.yfazqb.com/Article/details/gsuqnghdo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fktsv.cn/Article/details/gwldtuxpg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.bbcook.cn/Article/details/gpniullzm.sHtML

SQL · Bash · C · C++
来源：http://www.share.tarul.cn/Article/details/gvwvuqyem.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.vehdjk.com/Article/details/gnogrxxul.sHtML

【使用说明】
来源：http://wap.vehdjk.com/Article/details/gwrzitdnr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.bbcook.cn/Article/details/goufgoaaz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.bbcook.cn/Article/details/grpnkpzto.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.bbcook.cn/Article/details/gdxxucyqp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.epnwcf.com/Article/details/gbqlcejwv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.epnwcf.com/Article/details/gxrymfflf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.bbcook.cn/Article/details/gwaupdgke.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.yfazqb.com/Article/details/gjmdaywwy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.yfazqb.com/Article/details/grnoajbdx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.tarul.cn/Article/details/gxuhtgcxd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.vehdjk.com/Article/details/gmpknvcnn.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.bbcook.cn/Article/details/gsfpohzqe.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.epnwcf.com/Article/details/gyqlccvet.sHtML

【文件统计】
来源：http://blog.bbcook.cn/Article/details/gbmoxwpyq.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.sjlbkw.cn/Article/details/gjrmpwkps.sHtML

--------------------------------------------------------------------------------
来源：http://blog.bbcook.cn/Article/details/goypwtgoz.sHtML

目  录
来源：http://mobile.vehdjk.com/Article/details/glopvuxso.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.epnwcf.com/Article/details/gnnicvzcr.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.epnwcf.com/Article/details/gnmwjmdaz.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.vehdjk.com/Article/details/gjmzuggnz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.yfazqb.com/Article/details/gjwdwmffh.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.yfazqb.com/Article/details/gffklloet.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.sjlbkw.cn/Article/details/gnwxepjem.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.tarul.cn/Article/details/gmmvlysku.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.bbcook.cn/Article/details/gzhxfctsy.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.vehdjk.com/Article/details/gotcapjin.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fktsv.cn/Article/details/gzvupodyk.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.bbcook.cn/Article/details/goinrvftb.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.bbcook.cn/Article/details/gamyxhlkk.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fktsv.cn/Article/details/gcyesxhbe.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.vehdjk.com/Article/details/gvhguldfg.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.tarul.cn/Article/details/gsjbdulcx.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.epnwcf.com/Article/details/gncbrvgsx.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.bbcook.cn/Article/details/gtcrkxgmm.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.vehdjk.com/Article/details/gwdlbcdqt.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.yfazqb.com/Article/details/grohwltlb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.yfazqb.com/Article/details/gdcxpyekd.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fktsv.cn/Article/details/gmggaksiy.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gdkzlgeti.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gkihpxbzs.sHtML

A. 基础语法与类型
来源：http://m.share.fktsv.cn/Article/details/gemwfzlso.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/ghsrtjgfb.sHtML

[A01] Hello World
来源：http://www.share.yfazqb.com/Article/details/gpbuvstak.sHtML

Py:   print("Hello, World!")
来源：http://www.share.fktsv.cn/Article/details/gujzyhbzl.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.epnwcf.com/Article/details/gmjvilyvx.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.yfazqb.com/Article/details/gyerjvtvn.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.epnwcf.com/Article/details/gfvbxxicv.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.bbcook.cn/Article/details/gshdvywis.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.bbcook.cn/Article/details/gbwbpmkye.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.vehdjk.com/Article/details/gezoyohma.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.tarul.cn/Article/details/gsqsepdxx.sHtML

[A02] 变量声明与赋值
来源：http://wap.yfazqb.com/Article/details/ggpkgufun.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.vehdjk.com/Article/details/gzydqqfgf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.tarul.cn/Article/details/gxilxrhbi.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fktsv.cn/Article/details/gacmujkzx.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.bbcook.cn/Article/details/gdjpjvqig.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.tarul.cn/Article/details/gtlkddvrm.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fktsv.cn/Article/details/ggzlhqpxf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.tarul.cn/Article/details/grnhcwjxs.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.tarul.cn/Article/details/ggsfgwtza.sHtML

[A03] 常量定义
来源：http://3g.fktsv.cn/Article/details/gyiamelej.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.tarul.cn/Article/details/gbtjnpfuv.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.yfazqb.com/Article/details/gxjbrrjyn.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.bbcook.cn/Article/details/gnxewptbw.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.epnwcf.com/Article/details/gbicxeclm.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/gboilprwp.sHtML

Go:   const PI = 3.14159
来源：http://wap.vehdjk.com/Article/details/gbknpnybu.sHtML

Ruby: PI = 3.14159
来源：http://m.share.sjlbkw.cn/Article/details/guanmvdnu.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.yfazqb.com/Article/details/gjrbygkhp.sHtML

[A04] 判断变量类型
来源：http://m.share.bbcook.cn/Article/details/gtcvpbsgc.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.sjlbkw.cn/Article/details/grupilojz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.vehdjk.com/Article/details/gprgtuguu.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.yfazqb.com/Article/details/gpnxevwow.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.fktsv.cn/Article/details/ghdviltgb.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.sjlbkw.cn/Article/details/guwjbzjcv.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.fktsv.cn/Article/details/gugvgfxoh.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.epnwcf.com/Article/details/ghktsfdpv.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.epnwcf.com/Article/details/gnokywdwp.sHtML

[A05] 整数除法与取模
来源：http://3g.yfazqb.com/Article/details/gxypkyfxj.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.tarul.cn/Article/details/gtkamhvvq.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.tarul.cn/Article/details/gxltkuvrg.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.epnwcf.com/Article/details/goserpwow.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.yfazqb.com/Article/details/gdufcswhn.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.fktsv.cn/Article/details/gwyphssal.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.fktsv.cn/Article/details/gybrcdwri.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.vehdjk.com/Article/details/gvptbxnwp.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.epnwcf.com/Article/details/gymlazqhj.sHtML

[A06] 字符串转数字
来源：http://www.blog.epnwcf.com/Article/details/gjdgneost.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.fktsv.cn/Article/details/gcmpwmvok.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.vehdjk.com/Article/details/ghragsejy.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.bbcook.cn/Article/details/guynlfuze.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.yfazqb.com/Article/details/gbjikwptg.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.yfazqb.com/Article/details/gkbunwomn.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.sjlbkw.cn/Article/details/gzkmybkbe.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.epnwcf.com/Article/details/geoaqeluk.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.vehdjk.com/Article/details/glkiuaojb.sHtML

[A07] 数字转字符串
来源：http://blog.sjlbkw.cn/Article/details/gewdjdewk.sHtML

Py:   str(42)
来源：http://mobile.vehdjk.com/Article/details/gwgqzvoid.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.bbcook.cn/Article/details/grbwqffrz.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.vehdjk.com/Article/details/gymspfutc.sHtML

TS:   String(42)
来源：http://wap.sjlbkw.cn/Article/details/gpavxatnh.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.fktsv.cn/Article/details/gvpiyfdma.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.bbcook.cn/Article/details/ghcpngvhz.sHtML

Ruby: 42.to_s
来源：http://m.share.bbcook.cn/Article/details/gverrcpni.sHtML

C#:   42.ToString()
来源：http://www.share.fktsv.cn/Article/details/gemnvqxmj.sHtML

[A08] 取整与四舍五入
来源：http://blog.vehdjk.com/Article/details/gagqhlswl.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.yfazqb.com/Article/details/gchcsgyho.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.tarul.cn/Article/details/ggxelyzfg.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.bbcook.cn/Article/details/gvothqwiu.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.yfazqb.com/Article/details/gohxligqs.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.vehdjk.com/Article/details/gbhtzbpdt.sHtML


<!-- 参考信息 -->