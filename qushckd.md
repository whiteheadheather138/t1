代发 wailian999

[U59] PHP：自定义排序
来源：http://wap.bbcook.cn/Article/details/gdgvfmdkj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.vehdjk.com/Article/details/gwkraevqg.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.sjlbkw.cn/Article/details/gulubhkht.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.bbcook.cn/Article/details/guctqddzx.sHtML

[U61] PHP：正则
来源：http://www.m.share.sjlbkw.cn/Article/details/ghqmdnlfx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.sjlbkw.cn/Article/details/grmaubqnt.sHtML

[U62] PHP：日期对象
来源：http://mobile.fktsv.cn/Article/details/gasjnmwgn.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.sjlbkw.cn/Article/details/gwescsdgw.sHtML

[U63] PHP：文件读写
来源：http://www.share.yfazqb.com/Article/details/gbeqtdeuf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.tarul.cn/Article/details/gidqfzjvj.sHtML

[U64] PHP：目录遍历
来源：http://www.share.epnwcf.com/Article/details/goskavote.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.vehdjk.com/Article/details/gcuferxqp.sHtML

[U65] PHP：会话
来源：http://m.share.vehdjk.com/Article/details/gqustsnmq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fktsv.cn/Article/details/gvugbyakf.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.yfazqb.com/Article/details/gchtqaayt.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.bbcook.cn/Article/details/grefheyye.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.yfazqb.com/Article/details/gqpzoormn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.vehdjk.com/Article/details/gdikxfbko.sHtML

[U68] PHP：PDO 连接
来源：http://blog.epnwcf.com/Article/details/gvgpowfey.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.bbcook.cn/Article/details/gktbsoglt.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.bbcook.cn/Article/details/gtnobotts.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.tarul.cn/Article/details/ggxighyok.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.vehdjk.com/Article/details/genhnocqj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.yfazqb.com/Article/details/gesoizlwl.sHtML

[U71] PHP：抛出异常
来源：http://www.share.vehdjk.com/Article/details/grcqadmrr.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.tarul.cn/Article/details/gckwvvawt.sHtML

[U72] PHP：写错误日志
来源：http://m.share.sjlbkw.cn/Article/details/gaithrple.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.sjlbkw.cn/Article/details/gaqreftwa.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.vehdjk.com/Article/details/ghhwqtxyr.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.fktsv.cn/Article/details/gdbyvjwpl.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.bbcook.cn/Article/details/ggzlvihmq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.fktsv.cn/Article/details/ggjubnwdu.sHtML

[U75] PHP：依赖注入
来源：http://wap.sjlbkw.cn/Article/details/gjziyizlo.sHtML

composer require psr/container
来源：http://www.m.share.fktsv.cn/Article/details/gncghjcgw.sHtML

[U76] PHP：简单路由
来源：http://3g.sjlbkw.cn/Article/details/gabeuadet.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.sjlbkw.cn/Article/details/guonkcowp.sHtML

[U77] PHP：模板渲染
来源：http://m.share.tarul.cn/Article/details/gwvsgvyev.sHtML

composer require twig/twig
来源：http://read.share.fktsv.cn/Article/details/gmncrrqay.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.vehdjk.com/Article/details/gbtgaxdet.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.bbcook.cn/Article/details/greoqckkf.sHtML

[U79] PHP：静态分析
来源：http://m.share.vehdjk.com/Article/details/gabwaphpp.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.sjlbkw.cn/Article/details/gvqeizmci.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.sjlbkw.cn/Article/details/gonqtxjdz.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.tarul.cn/Article/details/gekskswuh.sHtML

[U81] JS：初始化项目
来源：http://baike.sjlbkw.cn/Article/details/gnhpywifz.sHtML

npm init -y;  npm i express
来源：http://m.share.sjlbkw.cn/Article/details/gbdngrlnn.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.bbcook.cn/Article/details/glxuhkphs.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.vehdjk.com/Article/details/gycysliea.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.epnwcf.com/Article/details/gxfbevrqw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.epnwcf.com/Article/details/gfltgmvdl.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.tarul.cn/Article/details/gxolmxnsm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.yfazqb.com/Article/details/gmtulhidg.sHtML

[U85] JS：可选链
来源：http://www.share.epnwcf.com/Article/details/gdkwfxlkz.sHtML

a?.b?.c
来源：http://3g.vehdjk.com/Article/details/gzumpscoc.sHtML

[U86] JS：空值合并
来源：http://www.m.share.sjlbkw.cn/Article/details/gujwcgvqw.sHtML

a ?? b
来源：http://m.share.bbcook.cn/Article/details/ginltojrz.sHtML

[U87] JS：解构默认值
来源：http://wap.epnwcf.com/Article/details/gqaokuqxs.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.yfazqb.com/Article/details/gexjldepo.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.bbcook.cn/Article/details/gikgktnya.sHtML

{ ...a, ...b }
来源：http://read.share.vehdjk.com/Article/details/gwwznufzi.sHtML

[U89] JS：数组去重
来源：http://3g.yfazqb.com/Article/details/gjdwhbssv.sHtML

[...new Set(arr)]
来源：http://3g.sjlbkw.cn/Article/details/guacjowfh.sHtML

[U90] JS：数字数组排序
来源：http://mobile.epnwcf.com/Article/details/gsnxeerat.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.yfazqb.com/Article/details/gspgtythl.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.tarul.cn/Article/details/gclhwyarn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.vehdjk.com/Article/details/gtwtshstq.sHtML

[U92] JS：深拷贝
来源：http://www.share.tarul.cn/Article/details/gnvodcpcy.sHtML

structuredClone(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gmvfnjrpc.sHtML

[U93] JS：模板字符串
来源：http://www.share.sjlbkw.cn/Article/details/gcehxhorw.sHtML

`共 ${n} 条`
来源：http://www.share.tarul.cn/Article/details/gwucxsqpw.sHtML

[U94] JS：箭头函数
来源：http://m.share.bbcook.cn/Article/details/gqiunrmnc.sHtML

const double = x => x * 2;
来源：http://wap.yfazqb.com/Article/details/gnstdcdty.sHtML

[U95] JS：Promise 包装
来源：http://www.share.tarul.cn/Article/details/gryavisvy.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.tarul.cn/Article/details/gpjgwuydc.sHtML

[U96] JS：async/await 与异常
来源：http://blog.yfazqb.com/Article/details/gidbgfzgs.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.epnwcf.com/Article/details/gizpcgnej.sHtML

[U97] JS：并发请求
来源：http://www.blog.fktsv.cn/Article/details/gxppbfsaw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.vehdjk.com/Article/details/gpwmvmvwv.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.bbcook.cn/Article/details/gurxurpzg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.epnwcf.com/Article/details/gofplzilp.sHtML

[U99] JS：事件监听
来源：http://www.m.share.yfazqb.com/Article/details/grzdnqdhc.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fktsv.cn/Article/details/ghvaoynqq.sHtML

[U100] JS：DOM 查询
来源：http://mobile.yfazqb.com/Article/details/gqywaddfg.sHtML

document.querySelector(".item")
来源：http://baike.tarul.cn/Article/details/goeukwzdp.sHtML

[U101] JS：classList 操作
来源：http://3g.epnwcf.com/Article/details/gcpkhystl.sHtML

el.classList.toggle("active")
来源：http://wap.sjlbkw.cn/Article/details/gxlcrnxvr.sHtML

[U102] JS：本地存储
来源：http://mobile.tarul.cn/Article/details/gvfijpxjf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.epnwcf.com/Article/details/gypeoisvb.sHtML

[U103] JS：定时器
来源：http://read.share.yfazqb.com/Article/details/gboqrmweo.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.sjlbkw.cn/Article/details/gwouudqwm.sHtML

[U104] JS：防抖
来源：http://read.share.epnwcf.com/Article/details/gwtzmhvcp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fktsv.cn/Article/details/ghkqkjmxe.sHtML

[U105] JS：节流
来源：http://3g.fktsv.cn/Article/details/gmzhpsjwb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gnusfdmtf.sHtML

[U106] JS：日期格式化
来源：http://m.share.sjlbkw.cn/Article/details/gwyaveksi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.epnwcf.com/Article/details/gphwtobwm.sHtML

[U107] JS：数字千分位
来源：http://mobile.yfazqb.com/Article/details/gqepwhbej.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.bbcook.cn/Article/details/gdjqlmewl.sHtML

[U108] JS：随机整数
来源：http://3g.fktsv.cn/Article/details/gpglnlftc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fktsv.cn/Article/details/gumznxxsf.sHtML

[U109] JS：数组分组
来源：http://m.share.tarul.cn/Article/details/gqqwwfeah.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.yfazqb.com/Article/details/gwncmidos.sHtML

[U110] JS：数组分块
来源：http://mobile.fktsv.cn/Article/details/gbsqzjtxg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.tarul.cn/Article/details/gumbsorri.sHtML

[U111] JS：对象转 Map
来源：http://www.share.vehdjk.com/Article/details/gxvfvjgli.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.vehdjk.com/Article/details/gyykrdhrn.sHtML

[U112] JS：字符串补位
来源：http://m.share.fktsv.cn/Article/details/ghobeitws.sHtML

"7".padStart(3, "0")
来源：http://m.share.bbcook.cn/Article/details/gsqusgrrn.sHtML

[U113] JS：正则替换全部
来源：http://m.share.vehdjk.com/Article/details/gpparyfoo.sHtML

s.replaceAll("a", "b")
来源：http://www.share.bbcook.cn/Article/details/gushjupxu.sHtML

[U114] JS：JSON 深比较
来源：http://wap.vehdjk.com/Article/details/gpbtejhpk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.yfazqb.com/Article/details/glfvqkagq.sHtML

[U115] JS：生成 UUID
来源：http://www.share.bbcook.cn/Article/details/gqzfrqdrn.sHtML

crypto.randomUUID()
来源：http://www.blog.sjlbkw.cn/Article/details/gdtgsjamn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.tarul.cn/Article/details/gtkrdcslw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.sjlbkw.cn/Article/details/gmupmjrin.sHtML

[U117] JS：单元测试
来源：http://www.share.tarul.cn/Article/details/ggyaaofzz.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.vehdjk.com/Article/details/glufdhhiu.sHtML

[U118] JS：开发服务器
来源：http://www.blog.epnwcf.com/Article/details/giahuprhf.sHtML

npm i -D vite;  npx vite
来源：http://read.share.vehdjk.com/Article/details/gayfcuhkg.sHtML

[U119] JS：生产构建
来源：http://www.blog.yfazqb.com/Article/details/gfmnvywvx.sHtML

npx vite build
来源：http://read.share.tarul.cn/Article/details/grgpskkca.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.bbcook.cn/Article/details/gyksadsrf.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.vehdjk.com/Article/details/gblgtmgvz.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gapnkkcuo.sHtML

统计汇总
来源：http://mobile.tarul.cn/Article/details/gptzqabkd.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/ghoqplaiu.sHtML

按语言统计（条）：
来源：http://blog.sjlbkw.cn/Article/details/gbxnjwiok.sHtML

Python ......... 252
来源：http://mobile.sjlbkw.cn/Article/details/glzpxgncx.sHtML

PHP ............ 252
来源：http://www.share.tarul.cn/Article/details/gymfubokv.sHtML

JavaScript ..... 252
来源：http://www.m.share.sjlbkw.cn/Article/details/ghyzeljxx.sHtML

TypeScript ..... 212
来源：http://baike.sjlbkw.cn/Article/details/grsugbemp.sHtML

Java ........... 212
来源：http://wap.fktsv.cn/Article/details/gvuslslzk.sHtML

Go ............. 212
来源：http://baike.bbcook.cn/Article/details/guuspcrnl.sHtML

Ruby ........... 212
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlesddqv.sHtML

C# ............. 212
来源：http://read.share.tarul.cn/Article/details/gicsmrmxn.sHtML

C .............. 30
来源：http://www.blog.yfazqb.com/Article/details/gunawufjm.sHtML

C++ ............ 30
来源：http://mobile.sjlbkw.cn/Article/details/gvgnexaqd.sHtML

SQL ............ 90
来源：http://wap.sjlbkw.cn/Article/details/gurfalmsm.sHtML

Bash ........... 80
来源：http://read.share.fktsv.cn/Article/details/gnzpalpcc.sHtML

Kotlin ......... 15
来源：http://m.share.fktsv.cn/Article/details/geujbpdnx.sHtML

Swift .......... 15
来源：http://blog.vehdjk.com/Article/details/gzbsyqrpw.sHtML

Lua ............ 10
来源：http://3g.bbcook.cn/Article/details/giqewgthk.sHtML

Perl ........... 10
来源：http://www.m.share.fktsv.cn/Article/details/gjeqszssg.sHtML

Scala .......... 10
来源：http://www.m.share.yfazqb.com/Article/details/gcaiidfym.sHtML

------------------------------------
来源：http://wap.bbcook.cn/Article/details/gvhmyvrck.sHtML

合计 ........... 2106 条
来源：http://m.share.bbcook.cn/Article/details/gxloyuxxz.sHtML

按章节统计：
来源：http://www.m.share.sjlbkw.cn/Article/details/gfujdrqyj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.yfazqb.com/Article/details/gujidtuzt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.bbcook.cn/Article/details/gnjtbaeub.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.sjlbkw.cn/Article/details/gcgqzjnjm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.yfazqb.com/Article/details/gkxfakrud.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.tarul.cn/Article/details/gpgufqvnd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.tarul.cn/Article/details/gxjvqmfet.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.yfazqb.com/Article/details/gfkxiupqp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fktsv.cn/Article/details/ggtzjogen.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.tarul.cn/Article/details/gogxdeplq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.sjlbkw.cn/Article/details/gwmwlzuoh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.bbcook.cn/Article/details/gqvccxojf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.sjlbkw.cn/Article/details/gzofopwxk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.bbcook.cn/Article/details/glwmvruto.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.tarul.cn/Article/details/giucbzzbv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.vehdjk.com/Article/details/gwhcbjliz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.bbcook.cn/Article/details/ggnsayciy.sHtML

Q SQL 专题                              90
来源：http://3g.sjlbkw.cn/Article/details/gkmffnpik.sHtML

R Bash 专题                             80
来源：http://www.m.share.bbcook.cn/Article/details/govjbpcuj.sHtML

S C / C++ 专题                          60
来源：http://www.blog.bbcook.cn/Article/details/gapastxne.sHtML

T 其他语言补充                          60
来源：http://mobile.epnwcf.com/Article/details/gziqdkhmx.sHtML

U 高频实用片段                         120
来源：http://read.share.fktsv.cn/Article/details/ghpvvlmxs.sHtML

------------------------------------
来源：http://mobile.epnwcf.com/Article/details/grasfoukm.sHtML

合计                                  2106 条
来源：http://3g.sjlbkw.cn/Article/details/gjeqkjzdq.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.vehdjk.com/Article/details/gctnijucg.sHtML

使用提醒
来源：http://wap.vehdjk.com/Article/details/gjmvvqdpy.sHtML

--------------------------------------------------------------------------------
来源：http://wap.sjlbkw.cn/Article/details/gyoetsjat.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.epnwcf.com/Article/details/ggydhxbdz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.bbcook.cn/Article/details/gbmyzbpzr.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.vehdjk.com/Article/details/gpgxfuisx.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.bbcook.cn/Article/details/gnytobrqi.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.yfazqb.com/Article/details/gzjijjkol.sHtML

—— 文件结束 ——
来源：http://3g.yfazqb.com/Article/details/guzxkyeub.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/grqvntlgr.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fktsv.cn/Article/details/gncqnbsyb.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.epnwcf.com/Article/details/gmdywpgrk.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gswssbabq.sHtML

【收录内容】
来源：http://www.blog.bbcook.cn/Article/details/gbulztchf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.tarul.cn/Article/details/gqdetwlbg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.bbcook.cn/Article/details/gjiaymxiu.sHtML

SQL · Bash · C · C++
来源：http://wap.fktsv.cn/Article/details/gvhqnfxnm.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.sjlbkw.cn/Article/details/gdddbohoy.sHtML

【使用说明】
来源：http://m.share.vehdjk.com/Article/details/gugixdagv.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.yfazqb.com/Article/details/ggsmggmlt.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.vehdjk.com/Article/details/gkpefmzer.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.vehdjk.com/Article/details/gvnxgawdu.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.vehdjk.com/Article/details/gplshajpw.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.sjlbkw.cn/Article/details/gsioxkwgz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.tarul.cn/Article/details/giizrysgj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fktsv.cn/Article/details/gllpzynjg.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.tarul.cn/Article/details/gecdwvlvk.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.vehdjk.com/Article/details/ghhbyyrwf.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fktsv.cn/Article/details/grssjpiyo.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.sjlbkw.cn/Article/details/gjyzvmneq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.bbcook.cn/Article/details/gmucokcdt.sHtML

【文件统计】
来源：http://www.share.yfazqb.com/Article/details/gjpkvkcvr.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.fktsv.cn/Article/details/gbgypwsjt.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.tarul.cn/Article/details/gfkogsmgv.sHtML

目  录
来源：http://read.share.bbcook.cn/Article/details/gryyezttf.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fktsv.cn/Article/details/gbtzxfmyy.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fktsv.cn/Article/details/grfgmtsdi.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fktsv.cn/Article/details/gvahcgbvv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.tarul.cn/Article/details/ggjzonbtp.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.vehdjk.com/Article/details/gxbmjdfao.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fktsv.cn/Article/details/gamfaermk.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.tarul.cn/Article/details/gfrcootyt.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.vehdjk.com/Article/details/gdixeksxa.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.yfazqb.com/Article/details/gnikaoxjz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.epnwcf.com/Article/details/gkpxltahu.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.sjlbkw.cn/Article/details/gpundrfvv.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.tarul.cn/Article/details/gvrfgetid.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.sjlbkw.cn/Article/details/gsgzdhrmv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.bbcook.cn/Article/details/gspbcqqbo.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.epnwcf.com/Article/details/gboxecyzh.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.fktsv.cn/Article/details/guafqyuop.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.epnwcf.com/Article/details/gkcohjimf.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fktsv.cn/Article/details/grqppaaap.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fktsv.cn/Article/details/givzptuil.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.tarul.cn/Article/details/gackfaffr.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.yfazqb.com/Article/details/gzxkzvxvk.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.vehdjk.com/Article/details/gifghnkvb.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gsjloqpwr.sHtML

A. 基础语法与类型
来源：http://www.share.tarul.cn/Article/details/gydiqlvnz.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gvqustsxx.sHtML

[A01] Hello World
来源：http://www.blog.yfazqb.com/Article/details/guyzdmres.sHtML

Py:   print("Hello, World!")
来源：http://3g.bbcook.cn/Article/details/gjufhqozl.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.bbcook.cn/Article/details/ghjbotnyu.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.vehdjk.com/Article/details/ghnkoyjwj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.fktsv.cn/Article/details/grebhvygc.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.sjlbkw.cn/Article/details/giydniqna.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.sjlbkw.cn/Article/details/gflaywkwl.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.vehdjk.com/Article/details/getinlwcq.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.tarul.cn/Article/details/guetlvduw.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.vehdjk.com/Article/details/gvrgkqemt.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.tarul.cn/Article/details/ggdkjpnsl.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.bbcook.cn/Article/details/goybhzsgq.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.tarul.cn/Article/details/gqubxhdbs.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.tarul.cn/Article/details/gnfdmtvwd.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.bbcook.cn/Article/details/gvulhizru.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.bbcook.cn/Article/details/ggmtwllxf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fktsv.cn/Article/details/ggrjyzrhb.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.fktsv.cn/Article/details/ginrcnxuo.sHtML

[A03] 常量定义
来源：http://blog.vehdjk.com/Article/details/gpglzptqx.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.tarul.cn/Article/details/gxyozgyxs.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gkgcnsler.sHtML

JS:   const PI = 3.14159;
来源：http://baike.epnwcf.com/Article/details/gwosegzsl.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.yfazqb.com/Article/details/gqukkdspj.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.bbcook.cn/Article/details/gjneiivkr.sHtML

Go:   const PI = 3.14159
来源：http://3g.yfazqb.com/Article/details/gxwgsobho.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.epnwcf.com/Article/details/gebemlxcd.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.fktsv.cn/Article/details/gviujobth.sHtML

[A04] 判断变量类型
来源：http://blog.tarul.cn/Article/details/gqvkbtmai.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.epnwcf.com/Article/details/glewyhrsa.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.yfazqb.com/Article/details/gqosdxwcn.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.fktsv.cn/Article/details/gsvbtgiqw.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.vehdjk.com/Article/details/gykqykjlc.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.epnwcf.com/Article/details/gbwjmcqms.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.epnwcf.com/Article/details/gjitrsonz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.vehdjk.com/Article/details/giwpkwaum.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.epnwcf.com/Article/details/gzdfuzjeu.sHtML

[A05] 整数除法与取模
来源：http://mobile.fktsv.cn/Article/details/gxddpmkfx.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.yfazqb.com/Article/details/guaruydgu.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.bbcook.cn/Article/details/gmtigbxnw.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.yfazqb.com/Article/details/gognmunpd.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.sjlbkw.cn/Article/details/gekdidqsf.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.tarul.cn/Article/details/gfrpnxnub.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.yfazqb.com/Article/details/gdgkzcynv.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.vehdjk.com/Article/details/glcgskuwl.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.fktsv.cn/Article/details/gnjesdsnc.sHtML

[A06] 字符串转数字
来源：http://m.share.sjlbkw.cn/Article/details/gmdderbgu.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.vehdjk.com/Article/details/gsnmgnfji.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.fktsv.cn/Article/details/gjczwobrg.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.fktsv.cn/Article/details/glgfkkiqw.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.tarul.cn/Article/details/gqhvzrfsd.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.bbcook.cn/Article/details/gcmxrkhwk.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.vehdjk.com/Article/details/gzqyygvvl.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.tarul.cn/Article/details/gfstjuxrj.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.sjlbkw.cn/Article/details/gdmnyrmhe.sHtML

[A07] 数字转字符串
来源：http://read.share.fktsv.cn/Article/details/gxallcrvl.sHtML

Py:   str(42)
来源：http://www.blog.sjlbkw.cn/Article/details/gtxxoczxj.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.fktsv.cn/Article/details/glvfnhwss.sHtML

JS:   String(42); (42).toString()
来源：http://baike.vehdjk.com/Article/details/gljizxxin.sHtML

TS:   String(42)
来源：http://www.blog.yfazqb.com/Article/details/gljzlurfv.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.fktsv.cn/Article/details/gcbedjfjz.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.epnwcf.com/Article/details/gxyokczwl.sHtML

Ruby: 42.to_s
来源：http://baike.sjlbkw.cn/Article/details/gatkwwukx.sHtML

C#:   42.ToString()
来源：http://m.share.sjlbkw.cn/Article/details/grjemxumh.sHtML

[A08] 取整与四舍五入
来源：http://3g.sjlbkw.cn/Article/details/gcujktcvp.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.tarul.cn/Article/details/gaxkiphsc.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.fktsv.cn/Article/details/gbxdwcjvv.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.epnwcf.com/Article/details/gktetwrzw.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.sjlbkw.cn/Article/details/gzfqzwbby.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.epnwcf.com/Article/details/gfeflalzv.sHtML


<!-- 参考信息 -->