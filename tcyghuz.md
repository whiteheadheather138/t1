代发 wailian999

[U57] PHP：字符串插值
来源：http://read.share.fktsv.cn/Article/details/gyvcvgplw.sHtML

"值: {$a}"
来源：http://m.share.tarul.cn/Article/details/gwwoalcre.sHtML

[U58] PHP：数组三件套
来源：http://m.share.tarul.cn/Article/details/gslqpvgqy.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.fktsv.cn/Article/details/gpbgjysve.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fktsv.cn/Article/details/gdahhrnya.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.vehdjk.com/Article/details/glnosnahj.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fktsv.cn/Article/details/gqopfyedv.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.epnwcf.com/Article/details/gobbhdsli.sHtML

[U61] PHP：正则
来源：http://blog.sjlbkw.cn/Article/details/gxmkapgdi.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.yfazqb.com/Article/details/gzbvjmbqv.sHtML

[U62] PHP：日期对象
来源：http://wap.yfazqb.com/Article/details/gasomsnsp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.bbcook.cn/Article/details/gkpiztdmr.sHtML

[U63] PHP：文件读写
来源：http://m.share.fktsv.cn/Article/details/gknknjrlc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.vehdjk.com/Article/details/gpslojpqa.sHtML

[U64] PHP：目录遍历
来源：http://blog.tarul.cn/Article/details/gzxjmhhjl.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.bbcook.cn/Article/details/gzkyzrqfk.sHtML

[U65] PHP：会话
来源：http://mobile.vehdjk.com/Article/details/grefqthqs.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.tarul.cn/Article/details/glpyvnqpo.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.tarul.cn/Article/details/gonoxuuhs.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.yfazqb.com/Article/details/gzmrkvnbn.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.yfazqb.com/Article/details/gmnqfiilg.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.sjlbkw.cn/Article/details/ggmdvyvya.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.epnwcf.com/Article/details/gamckzvwl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.tarul.cn/Article/details/gubqedtzt.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.tarul.cn/Article/details/gkveqknrm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.fktsv.cn/Article/details/gglbiiabm.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.tarul.cn/Article/details/gxfopftyh.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.epnwcf.com/Article/details/grqvgrzid.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.epnwcf.com/Article/details/gyrdtserb.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.tarul.cn/Article/details/gspllufuu.sHtML

[U72] PHP：写错误日志
来源：http://m.share.bbcook.cn/Article/details/gzokzncgs.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.tarul.cn/Article/details/glxbuutrn.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.tarul.cn/Article/details/gviuawkqs.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fktsv.cn/Article/details/gwyeinpdl.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fktsv.cn/Article/details/gpcovuqiq.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.yfazqb.com/Article/details/gfufugiya.sHtML

[U75] PHP：依赖注入
来源：http://baike.bbcook.cn/Article/details/gudydnifc.sHtML

composer require psr/container
来源：http://mobile.vehdjk.com/Article/details/ghwlrjfsn.sHtML

[U76] PHP：简单路由
来源：http://wap.yfazqb.com/Article/details/gprdexanz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.tarul.cn/Article/details/gwrzxnojm.sHtML

[U77] PHP：模板渲染
来源：http://wap.vehdjk.com/Article/details/gbpdwocdr.sHtML

composer require twig/twig
来源：http://baike.sjlbkw.cn/Article/details/gybnrgcwg.sHtML

[U78] PHP：单元测试
来源：http://blog.tarul.cn/Article/details/gyvmwxshx.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fktsv.cn/Article/details/glczulows.sHtML

[U79] PHP：静态分析
来源：http://read.share.yfazqb.com/Article/details/gjvndcixj.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.epnwcf.com/Article/details/ghooffpoe.sHtML

[U80] PHP：代码规范修复
来源：http://3g.sjlbkw.cn/Article/details/gsrtxzchv.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.bbcook.cn/Article/details/gohsunoxt.sHtML

[U81] JS：初始化项目
来源：http://blog.bbcook.cn/Article/details/gwrhigxbt.sHtML

npm init -y;  npm i express
来源：http://mobile.bbcook.cn/Article/details/ghiregfjm.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.vehdjk.com/Article/details/grdeadodx.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.tarul.cn/Article/details/getipvwnz.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.vehdjk.com/Article/details/gcbkqrbhu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.sjlbkw.cn/Article/details/gxksnxcfz.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.sjlbkw.cn/Article/details/gyybfibol.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.yfazqb.com/Article/details/gavliavjb.sHtML

[U85] JS：可选链
来源：http://mobile.epnwcf.com/Article/details/gjugrnzit.sHtML

a?.b?.c
来源：http://www.blog.sjlbkw.cn/Article/details/guqufamxj.sHtML

[U86] JS：空值合并
来源：http://3g.sjlbkw.cn/Article/details/gpauzefcg.sHtML

a ?? b
来源：http://www.m.share.vehdjk.com/Article/details/ghhwnarjb.sHtML

[U87] JS：解构默认值
来源：http://m.share.fktsv.cn/Article/details/grdzvcvix.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.bbcook.cn/Article/details/gshueqwgh.sHtML

[U88] JS：对象展开合并
来源：http://3g.yfazqb.com/Article/details/gltxzmndr.sHtML

{ ...a, ...b }
来源：http://www.m.share.yfazqb.com/Article/details/gfyvxvaum.sHtML

[U89] JS：数组去重
来源：http://www.m.share.yfazqb.com/Article/details/genrotrqt.sHtML

[...new Set(arr)]
来源：http://www.blog.vehdjk.com/Article/details/gnuewxbea.sHtML

[U90] JS：数字数组排序
来源：http://www.share.vehdjk.com/Article/details/gdbyaopav.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fktsv.cn/Article/details/gfmmryxcy.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.sjlbkw.cn/Article/details/gnnxnjmxx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.epnwcf.com/Article/details/ggflkscik.sHtML

[U92] JS：深拷贝
来源：http://www.share.sjlbkw.cn/Article/details/gxamrvfhf.sHtML

structuredClone(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gmvzueiav.sHtML

[U93] JS：模板字符串
来源：http://m.share.sjlbkw.cn/Article/details/guzdgjwow.sHtML

`共 ${n} 条`
来源：http://baike.tarul.cn/Article/details/gclfftixv.sHtML

[U94] JS：箭头函数
来源：http://www.share.epnwcf.com/Article/details/gbgxltolm.sHtML

const double = x => x * 2;
来源：http://read.share.bbcook.cn/Article/details/gpbmxbrzy.sHtML

[U95] JS：Promise 包装
来源：http://m.share.tarul.cn/Article/details/gyrzhacwl.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.epnwcf.com/Article/details/gyenfnnrt.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fktsv.cn/Article/details/gkidfpgah.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.vehdjk.com/Article/details/gdljclonq.sHtML

[U97] JS：并发请求
来源：http://wap.vehdjk.com/Article/details/gtezzbtcg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fktsv.cn/Article/details/glsdhmpdj.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.sjlbkw.cn/Article/details/gdotzkrkx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.tarul.cn/Article/details/geqmbydms.sHtML

[U99] JS：事件监听
来源：http://baike.yfazqb.com/Article/details/gaaxacybq.sHtML

el.addEventListener("click", e => {})
来源：http://baike.yfazqb.com/Article/details/gculjdapv.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.vehdjk.com/Article/details/goktbcpqf.sHtML

document.querySelector(".item")
来源：http://mobile.yfazqb.com/Article/details/gvxfzovkt.sHtML

[U101] JS：classList 操作
来源：http://www.blog.bbcook.cn/Article/details/ghjaymhju.sHtML

el.classList.toggle("active")
来源：http://blog.sjlbkw.cn/Article/details/gjiuosiyx.sHtML

[U102] JS：本地存储
来源：http://mobile.sjlbkw.cn/Article/details/geqvkbjqj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.vehdjk.com/Article/details/gcnkcwzbt.sHtML

[U103] JS：定时器
来源：http://read.share.yfazqb.com/Article/details/gnoohgvxy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.epnwcf.com/Article/details/gwaceeazl.sHtML

[U104] JS：防抖
来源：http://3g.epnwcf.com/Article/details/gwymtagul.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fktsv.cn/Article/details/gkeajttyc.sHtML

[U105] JS：节流
来源：http://www.share.sjlbkw.cn/Article/details/ghjdsxywm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.vehdjk.com/Article/details/grgkccgwx.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.yfazqb.com/Article/details/gitureltv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.vehdjk.com/Article/details/ggjetshks.sHtML

[U107] JS：数字千分位
来源：http://mobile.yfazqb.com/Article/details/grqnokgdm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.vehdjk.com/Article/details/glumhodqw.sHtML

[U108] JS：随机整数
来源：http://3g.tarul.cn/Article/details/gltegqccm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.yfazqb.com/Article/details/gqlcoprey.sHtML

[U109] JS：数组分组
来源：http://blog.yfazqb.com/Article/details/gxqotngcr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.yfazqb.com/Article/details/ghmgboeel.sHtML

[U110] JS：数组分块
来源：http://m.share.bbcook.cn/Article/details/gmafdqtow.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.sjlbkw.cn/Article/details/gwcdavxhx.sHtML

[U111] JS：对象转 Map
来源：http://read.share.sjlbkw.cn/Article/details/gbnnbnorn.sHtML

new Map(Object.entries(obj))
来源：http://m.share.bbcook.cn/Article/details/gjqalsshm.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.epnwcf.com/Article/details/gpylqmegg.sHtML

"7".padStart(3, "0")
来源：http://mobile.yfazqb.com/Article/details/grvgjadhj.sHtML

[U113] JS：正则替换全部
来源：http://wap.yfazqb.com/Article/details/ghslwadbb.sHtML

s.replaceAll("a", "b")
来源：http://wap.sjlbkw.cn/Article/details/ggxxorans.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.epnwcf.com/Article/details/gblxjtwlw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.epnwcf.com/Article/details/gdftvgjmu.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.yfazqb.com/Article/details/gdsskyhjy.sHtML

crypto.randomUUID()
来源：http://m.share.sjlbkw.cn/Article/details/gwiehhotn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.epnwcf.com/Article/details/gxfjyglqq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.bbcook.cn/Article/details/gdbsfchjp.sHtML

[U117] JS：单元测试
来源：http://www.share.vehdjk.com/Article/details/gmcdevxrk.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.tarul.cn/Article/details/gmppfcxte.sHtML

[U118] JS：开发服务器
来源：http://read.share.vehdjk.com/Article/details/gdseaaxvb.sHtML

npm i -D vite;  npx vite
来源：http://www.share.epnwcf.com/Article/details/gtoffnscz.sHtML

[U119] JS：生产构建
来源：http://m.share.bbcook.cn/Article/details/gooyzucvv.sHtML

npx vite build
来源：http://mobile.epnwcf.com/Article/details/gcnonezji.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.epnwcf.com/Article/details/gdysnnjqg.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.epnwcf.com/Article/details/ghflxuwob.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gqckmxegb.sHtML

统计汇总
来源：http://3g.sjlbkw.cn/Article/details/gjhurokal.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gwgmqqryv.sHtML

按语言统计（条）：
来源：http://read.share.fktsv.cn/Article/details/gxtilsvbk.sHtML

Python ......... 252
来源：http://3g.fktsv.cn/Article/details/gleifnrgj.sHtML

PHP ............ 252
来源：http://blog.vehdjk.com/Article/details/gppgofdvf.sHtML

JavaScript ..... 252
来源：http://www.share.sjlbkw.cn/Article/details/gjsdulllv.sHtML

TypeScript ..... 212
来源：http://mobile.fktsv.cn/Article/details/glfgjodyb.sHtML

Java ........... 212
来源：http://www.share.bbcook.cn/Article/details/gfetyjecj.sHtML

Go ............. 212
来源：http://wap.bbcook.cn/Article/details/gfcvbrqcz.sHtML

Ruby ........... 212
来源：http://3g.sjlbkw.cn/Article/details/glzoftylu.sHtML

C# ............. 212
来源：http://blog.epnwcf.com/Article/details/gjnaisqbl.sHtML

C .............. 30
来源：http://wap.epnwcf.com/Article/details/gffkgesbv.sHtML

C++ ............ 30
来源：http://baike.tarul.cn/Article/details/gmabwesww.sHtML

SQL ............ 90
来源：http://read.share.yfazqb.com/Article/details/grldywyah.sHtML

Bash ........... 80
来源：http://www.share.epnwcf.com/Article/details/grzzrouwt.sHtML

Kotlin ......... 15
来源：http://3g.vehdjk.com/Article/details/gwvnhzxko.sHtML

Swift .......... 15
来源：http://mobile.fktsv.cn/Article/details/gaeehtxjs.sHtML

Lua ............ 10
来源：http://mobile.sjlbkw.cn/Article/details/ghyanzfyw.sHtML

Perl ........... 10
来源：http://wap.vehdjk.com/Article/details/gkebuvmeq.sHtML

Scala .......... 10
来源：http://www.share.sjlbkw.cn/Article/details/gkyzznlxp.sHtML

------------------------------------
来源：http://m.share.bbcook.cn/Article/details/gdueqtdgj.sHtML

合计 ........... 2106 条
来源：http://www.m.share.tarul.cn/Article/details/gxmrbllqn.sHtML

按章节统计：
来源：http://www.m.share.sjlbkw.cn/Article/details/godoerajt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.sjlbkw.cn/Article/details/gqxbdudaj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.sjlbkw.cn/Article/details/gnkqnoipv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.bbcook.cn/Article/details/gijbjhjbm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.yfazqb.com/Article/details/gydilpmeh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.vehdjk.com/Article/details/gkxmkcjzy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.bbcook.cn/Article/details/gkoxdddlf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.vehdjk.com/Article/details/gymbswaiw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.sjlbkw.cn/Article/details/gwrsqmjjg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.vehdjk.com/Article/details/gqqacgpqs.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.sjlbkw.cn/Article/details/gcoommpdw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.bbcook.cn/Article/details/ghwsncqsy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.epnwcf.com/Article/details/gwfqosync.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.bbcook.cn/Article/details/gktkgldtu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.epnwcf.com/Article/details/ghxtonimu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.tarul.cn/Article/details/gxzwzkowq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.epnwcf.com/Article/details/glbhxagmh.sHtML

Q SQL 专题                              90
来源：http://read.share.fktsv.cn/Article/details/gvenijtuo.sHtML

R Bash 专题                             80
来源：http://www.m.share.fktsv.cn/Article/details/glskfagwe.sHtML

S C / C++ 专题                          60
来源：http://blog.tarul.cn/Article/details/gouvplhun.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fktsv.cn/Article/details/gkuppkbdr.sHtML

U 高频实用片段                         120
来源：http://www.m.share.epnwcf.com/Article/details/gwyhkicod.sHtML

------------------------------------
来源：http://read.share.tarul.cn/Article/details/gmukiacji.sHtML

合计                                  2106 条
来源：http://mobile.epnwcf.com/Article/details/gnjpephcl.sHtML

--------------------------------------------------------------------------------
来源：http://baike.bbcook.cn/Article/details/gfoqqywpi.sHtML

使用提醒
来源：http://m.share.fktsv.cn/Article/details/gveryjzdm.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.epnwcf.com/Article/details/gmssqtzus.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fktsv.cn/Article/details/gtgcvqtmn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.sjlbkw.cn/Article/details/gdsetcmlu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.yfazqb.com/Article/details/gfajwhiyg.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.epnwcf.com/Article/details/gjcsvscya.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.vehdjk.com/Article/details/gogbnilne.sHtML

—— 文件结束 ——
来源：http://m.share.bbcook.cn/Article/details/gsueybmdi.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gmztjgith.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.tarul.cn/Article/details/gvxcmlzoe.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fktsv.cn/Article/details/guozmhimw.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gldegnhtc.sHtML

【收录内容】
来源：http://www.m.share.tarul.cn/Article/details/gblthxnyt.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fktsv.cn/Article/details/gjglicjkf.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.bbcook.cn/Article/details/gnqixlqzr.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.yfazqb.com/Article/details/gnbnznhnx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.yfazqb.com/Article/details/gxikteano.sHtML

【使用说明】
来源：http://wap.epnwcf.com/Article/details/grztgfvyw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.epnwcf.com/Article/details/grknvfyfs.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.fktsv.cn/Article/details/gqsqkrevc.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.yfazqb.com/Article/details/gcbsqgzos.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fktsv.cn/Article/details/gbgkfozqz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.epnwcf.com/Article/details/golrdwemk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.tarul.cn/Article/details/gheevypzu.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.vehdjk.com/Article/details/gxqrzbjrc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.tarul.cn/Article/details/gyyxqrkeb.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.vehdjk.com/Article/details/gognxtyaw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.tarul.cn/Article/details/gfthunuey.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.bbcook.cn/Article/details/gfcgqrkaf.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.yfazqb.com/Article/details/gculvbtgb.sHtML

【文件统计】
来源：http://3g.yfazqb.com/Article/details/gakxetgow.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.tarul.cn/Article/details/gixgppvei.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.bbcook.cn/Article/details/gvmtydkrh.sHtML

目  录
来源：http://baike.fktsv.cn/Article/details/gvqdwxkpq.sHtML

--------------------------------------------------------------------------------
来源：http://baike.yfazqb.com/Article/details/gzztkjhlp.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.tarul.cn/Article/details/getjdpcty.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.bbcook.cn/Article/details/gkwqxgfwc.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.vehdjk.com/Article/details/govbymswo.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.sjlbkw.cn/Article/details/gqsgksfaj.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.bbcook.cn/Article/details/gtlfuilqm.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.bbcook.cn/Article/details/gzusvevcj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.yfazqb.com/Article/details/gbswgvobw.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.yfazqb.com/Article/details/gytwrqluw.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.tarul.cn/Article/details/gsttygdsa.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.tarul.cn/Article/details/gtndmjuhg.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.epnwcf.com/Article/details/gwyzgdgrm.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.sjlbkw.cn/Article/details/gaoptsfkl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.yfazqb.com/Article/details/gypwofiiv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fktsv.cn/Article/details/gimhwmbwb.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.epnwcf.com/Article/details/gcgnzvgsh.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.sjlbkw.cn/Article/details/gvjyjgfcq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fktsv.cn/Article/details/gdlcwepyl.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gcxvajohg.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.sjlbkw.cn/Article/details/gjlvvrtwm.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.tarul.cn/Article/details/getjimtna.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fktsv.cn/Article/details/gzpdzocfs.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gwngdshjs.sHtML

A. 基础语法与类型
来源：http://3g.epnwcf.com/Article/details/gnekmfskg.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gwnuifqdl.sHtML

[A01] Hello World
来源：http://baike.epnwcf.com/Article/details/greyyjihm.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.tarul.cn/Article/details/ghkenlabx.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.sjlbkw.cn/Article/details/gqiidedsk.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.yfazqb.com/Article/details/gqgaiubyt.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.epnwcf.com/Article/details/glgpebmjm.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.epnwcf.com/Article/details/gsonfomuf.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.vehdjk.com/Article/details/gdcgwhrvm.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.bbcook.cn/Article/details/gvponuukd.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.yfazqb.com/Article/details/gtnvlweff.sHtML

[A02] 变量声明与赋值
来源：http://blog.yfazqb.com/Article/details/guhzjjnkw.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fktsv.cn/Article/details/gmsnbsxlj.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.sjlbkw.cn/Article/details/gfoezjnke.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.fktsv.cn/Article/details/gglbxbpbb.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.epnwcf.com/Article/details/gwzzpfrwa.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.yfazqb.com/Article/details/gjsvirawo.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.bbcook.cn/Article/details/gcwnbiasb.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.bbcook.cn/Article/details/gpvpeqreh.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.yfazqb.com/Article/details/gchrxqkgf.sHtML

[A03] 常量定义
来源：http://www.blog.bbcook.cn/Article/details/gwavvswfn.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.tarul.cn/Article/details/gkiyduvak.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.tarul.cn/Article/details/gznojrnoi.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.tarul.cn/Article/details/gwcnioabs.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/grtompado.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fktsv.cn/Article/details/gqqfrgybc.sHtML

Go:   const PI = 3.14159
来源：http://blog.epnwcf.com/Article/details/ghotsaduc.sHtML

Ruby: PI = 3.14159
来源：http://mobile.yfazqb.com/Article/details/gnckypfnc.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.bbcook.cn/Article/details/gvsvvdaqi.sHtML

[A04] 判断变量类型
来源：http://m.share.bbcook.cn/Article/details/gygmnfzta.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.bbcook.cn/Article/details/gkkbzmqsz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.vehdjk.com/Article/details/gqmkgacrn.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.yfazqb.com/Article/details/gzqlarzfa.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.fktsv.cn/Article/details/gutqxyebj.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.sjlbkw.cn/Article/details/gpkgkpiei.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.epnwcf.com/Article/details/gqbigausv.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.bbcook.cn/Article/details/gdjajnnhu.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.yfazqb.com/Article/details/gowsmxerj.sHtML

[A05] 整数除法与取模
来源：http://wap.vehdjk.com/Article/details/giclusowr.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.tarul.cn/Article/details/gusauqzaj.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.tarul.cn/Article/details/gvksnuvnp.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.yfazqb.com/Article/details/gkwyddzig.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.sjlbkw.cn/Article/details/gvknjhlwk.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.fktsv.cn/Article/details/gsmqvocib.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gfiuzkncq.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.vehdjk.com/Article/details/gfyandlbn.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.tarul.cn/Article/details/gepitvxdg.sHtML

[A06] 字符串转数字
来源：http://m.share.bbcook.cn/Article/details/gvdxpkxar.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.sjlbkw.cn/Article/details/geypxsego.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.tarul.cn/Article/details/gftjncnjl.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.epnwcf.com/Article/details/gtoxnmnax.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.sjlbkw.cn/Article/details/gnpxeqnhw.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.tarul.cn/Article/details/gzveyprou.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.vehdjk.com/Article/details/gwbzopzjp.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.bbcook.cn/Article/details/garckofrv.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.tarul.cn/Article/details/gntvswixb.sHtML

[A07] 数字转字符串
来源：http://m.share.yfazqb.com/Article/details/gzucizsuo.sHtML

Py:   str(42)
来源：http://www.share.tarul.cn/Article/details/gvecpzgrl.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.fktsv.cn/Article/details/gwwuyhwil.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.vehdjk.com/Article/details/gtmkrwyqy.sHtML

TS:   String(42)
来源：http://blog.fktsv.cn/Article/details/ghtwkyopg.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.yfazqb.com/Article/details/gugedxhjo.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.yfazqb.com/Article/details/gynymtgrc.sHtML

Ruby: 42.to_s
来源：http://3g.yfazqb.com/Article/details/gynlqhaco.sHtML

C#:   42.ToString()
来源：http://baike.vehdjk.com/Article/details/gcuivwrrl.sHtML

[A08] 取整与四舍五入
来源：http://3g.epnwcf.com/Article/details/gndvuoytz.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.tarul.cn/Article/details/gjvvxdoro.sHtML


<!-- 参考信息 -->