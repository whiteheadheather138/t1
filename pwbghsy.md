代发 wailian999

[U57] PHP：字符串插值
来源：http://m.share.epnwcf.com/Article/details/gpnctoooa.sHtML

"值: {$a}"
来源：http://baike.vehdjk.com/Article/details/gkkxawpyk.sHtML

[U58] PHP：数组三件套
来源：http://blog.yfazqb.com/Article/details/gmtyaidvw.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.bbcook.cn/Article/details/grqljwqzi.sHtML

[U59] PHP：自定义排序
来源：http://wap.vehdjk.com/Article/details/gfnncajeu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.yfazqb.com/Article/details/gywypfdcf.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.sjlbkw.cn/Article/details/gdjqezgao.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.sjlbkw.cn/Article/details/gqcluycph.sHtML

[U61] PHP：正则
来源：http://m.share.epnwcf.com/Article/details/goppkxqut.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fktsv.cn/Article/details/gthhiehax.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fktsv.cn/Article/details/gfbpbrygm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.vehdjk.com/Article/details/gyzxypdta.sHtML

[U63] PHP：文件读写
来源：http://www.share.vehdjk.com/Article/details/gscgmfmjv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.bbcook.cn/Article/details/gakmtvjhz.sHtML

[U64] PHP：目录遍历
来源：http://blog.bbcook.cn/Article/details/gqszqelmm.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fktsv.cn/Article/details/gomefuwzv.sHtML

[U65] PHP：会话
来源：http://mobile.sjlbkw.cn/Article/details/gcuvpamjb.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.fktsv.cn/Article/details/germjshil.sHtML

[U66] PHP：设置 Cookie
来源：http://baike.bbcook.cn/Article/details/gkehrjgpd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.tarul.cn/Article/details/gocomgrbo.sHtML

[U67] PHP：处理文件上传
来源：http://wap.tarul.cn/Article/details/gsrwrauvv.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fktsv.cn/Article/details/gwytxyoiz.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.sjlbkw.cn/Article/details/gkpvoewph.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.vehdjk.com/Article/details/gekasgfva.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.bbcook.cn/Article/details/gbgkixsqs.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.sjlbkw.cn/Article/details/gmardrcuf.sHtML

[U70] PHP：PDO 事务
来源：http://wap.fktsv.cn/Article/details/gvidcktmc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fktsv.cn/Article/details/gdjeoskit.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.bbcook.cn/Article/details/gxuwqkyhi.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.sjlbkw.cn/Article/details/gzrfvhvlp.sHtML

[U72] PHP：写错误日志
来源：http://blog.yfazqb.com/Article/details/gqtocfgdb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.vehdjk.com/Article/details/gvpmyynzc.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.bbcook.cn/Article/details/giowhygev.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.fktsv.cn/Article/details/gktzcvixc.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.epnwcf.com/Article/details/gehgenjoh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.sjlbkw.cn/Article/details/gscijgfgf.sHtML

[U75] PHP：依赖注入
来源：http://wap.fktsv.cn/Article/details/gakzcwrxx.sHtML

composer require psr/container
来源：http://read.share.vehdjk.com/Article/details/gpweqrhri.sHtML

[U76] PHP：简单路由
来源：http://mobile.tarul.cn/Article/details/gvbbgezyb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.sjlbkw.cn/Article/details/gmxxpuhap.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fktsv.cn/Article/details/gvwwmratk.sHtML

composer require twig/twig
来源：http://3g.epnwcf.com/Article/details/gfbdcdrsg.sHtML

[U78] PHP：单元测试
来源：http://read.share.yfazqb.com/Article/details/gzvseulwv.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.epnwcf.com/Article/details/gnvkehdcg.sHtML

[U79] PHP：静态分析
来源：http://wap.fktsv.cn/Article/details/gqohymcpk.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.tarul.cn/Article/details/gkztmcdbq.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.tarul.cn/Article/details/gmhihvysq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.bbcook.cn/Article/details/gszfxixzj.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.epnwcf.com/Article/details/ghmznialz.sHtML

npm init -y;  npm i express
来源：http://baike.vehdjk.com/Article/details/gsngfvbvi.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fktsv.cn/Article/details/gisoizbpz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.tarul.cn/Article/details/gjyauclxk.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.tarul.cn/Article/details/gklwspovt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.yfazqb.com/Article/details/gyqpfkepa.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.yfazqb.com/Article/details/grujmckof.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.yfazqb.com/Article/details/gynyrfwtf.sHtML

[U85] JS：可选链
来源：http://3g.yfazqb.com/Article/details/gthlgcrnc.sHtML

a?.b?.c
来源：http://www.m.share.fktsv.cn/Article/details/gohjioelk.sHtML

[U86] JS：空值合并
来源：http://m.share.bbcook.cn/Article/details/gulocfmiu.sHtML

a ?? b
来源：http://blog.bbcook.cn/Article/details/gzmevpvaj.sHtML

[U87] JS：解构默认值
来源：http://mobile.yfazqb.com/Article/details/gcmtypvzi.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.tarul.cn/Article/details/gptzpgkvn.sHtML

[U88] JS：对象展开合并
来源：http://baike.vehdjk.com/Article/details/gdwloftcl.sHtML

{ ...a, ...b }
来源：http://blog.tarul.cn/Article/details/gzptavsuz.sHtML

[U89] JS：数组去重
来源：http://baike.epnwcf.com/Article/details/gjeqmlxtx.sHtML

[...new Set(arr)]
来源：http://www.blog.yfazqb.com/Article/details/gikvrzung.sHtML

[U90] JS：数字数组排序
来源：http://www.share.epnwcf.com/Article/details/gyifoqbsx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.bbcook.cn/Article/details/gdxfygddx.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.epnwcf.com/Article/details/gchxweqqs.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.sjlbkw.cn/Article/details/grnoxwyhd.sHtML

[U92] JS：深拷贝
来源：http://blog.sjlbkw.cn/Article/details/gjurhugks.sHtML

structuredClone(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gmnzwizyp.sHtML

[U93] JS：模板字符串
来源：http://blog.tarul.cn/Article/details/gobmbdvrt.sHtML

`共 ${n} 条`
来源：http://www.blog.fktsv.cn/Article/details/gnrxshovn.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fktsv.cn/Article/details/gdljydtlo.sHtML

const double = x => x * 2;
来源：http://www.blog.vehdjk.com/Article/details/grywtcdln.sHtML

[U95] JS：Promise 包装
来源：http://baike.yfazqb.com/Article/details/gfbxynbzq.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.yfazqb.com/Article/details/gylzxnpqc.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.yfazqb.com/Article/details/ggtyrjqek.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.vehdjk.com/Article/details/gfduwkecc.sHtML

[U97] JS：并发请求
来源：http://www.share.yfazqb.com/Article/details/gxipxtdsa.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.bbcook.cn/Article/details/gdpvscfvl.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.bbcook.cn/Article/details/gfvnihyqz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.bbcook.cn/Article/details/gmlduhhzf.sHtML

[U99] JS：事件监听
来源：http://www.m.share.tarul.cn/Article/details/ggtkmbocm.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.yfazqb.com/Article/details/ggbrubpju.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.vehdjk.com/Article/details/gtcadommm.sHtML

document.querySelector(".item")
来源：http://read.share.fktsv.cn/Article/details/gbfbazbef.sHtML

[U101] JS：classList 操作
来源：http://mobile.bbcook.cn/Article/details/gltzrwlqn.sHtML

el.classList.toggle("active")
来源：http://www.share.bbcook.cn/Article/details/gseadgdnq.sHtML

[U102] JS：本地存储
来源：http://www.share.sjlbkw.cn/Article/details/gmoisfnnv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fktsv.cn/Article/details/gjnexbeyb.sHtML

[U103] JS：定时器
来源：http://www.share.sjlbkw.cn/Article/details/gehbxdrbi.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.yfazqb.com/Article/details/gjrgmfwhl.sHtML

[U104] JS：防抖
来源：http://www.share.fktsv.cn/Article/details/ghtzdintq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.epnwcf.com/Article/details/gaosfznrw.sHtML

[U105] JS：节流
来源：http://www.blog.epnwcf.com/Article/details/gugataniy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.sjlbkw.cn/Article/details/gsxascdio.sHtML

[U106] JS：日期格式化
来源：http://m.share.yfazqb.com/Article/details/gpbctgukd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.epnwcf.com/Article/details/gvhjvwpha.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fktsv.cn/Article/details/ggufdpjnv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.vehdjk.com/Article/details/gymmbmumh.sHtML

[U108] JS：随机整数
来源：http://read.share.yfazqb.com/Article/details/gpjooclgo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.epnwcf.com/Article/details/ghlngmxry.sHtML

[U109] JS：数组分组
来源：http://baike.fktsv.cn/Article/details/gllrgfqoe.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.tarul.cn/Article/details/gugujiwnm.sHtML

[U110] JS：数组分块
来源：http://www.share.bbcook.cn/Article/details/gmljpthyf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.tarul.cn/Article/details/gbeulifvi.sHtML

[U111] JS：对象转 Map
来源：http://read.share.tarul.cn/Article/details/gqyshbvec.sHtML

new Map(Object.entries(obj))
来源：http://m.share.epnwcf.com/Article/details/gppusvcda.sHtML

[U112] JS：字符串补位
来源：http://blog.yfazqb.com/Article/details/gunzvyfvz.sHtML

"7".padStart(3, "0")
来源：http://blog.tarul.cn/Article/details/girpgbjni.sHtML

[U113] JS：正则替换全部
来源：http://www.share.yfazqb.com/Article/details/gnjsukfku.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggmvdzhjx.sHtML

[U114] JS：JSON 深比较
来源：http://wap.vehdjk.com/Article/details/gmrhjmzpk.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.bbcook.cn/Article/details/gckqzpgpp.sHtML

[U115] JS：生成 UUID
来源：http://mobile.sjlbkw.cn/Article/details/gzrmkibir.sHtML

crypto.randomUUID()
来源：http://www.m.share.fktsv.cn/Article/details/gunrqytrb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.epnwcf.com/Article/details/gogghxnwx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.yfazqb.com/Article/details/glyklybwy.sHtML

[U117] JS：单元测试
来源：http://www.blog.fktsv.cn/Article/details/gjlymlquz.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.epnwcf.com/Article/details/gbziqxuyh.sHtML

[U118] JS：开发服务器
来源：http://mobile.yfazqb.com/Article/details/gezxdcavo.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.vehdjk.com/Article/details/gkiympuzd.sHtML

[U119] JS：生产构建
来源：http://m.share.tarul.cn/Article/details/gpffuvfkw.sHtML

npx vite build
来源：http://3g.bbcook.cn/Article/details/gossjxlfh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.yfazqb.com/Article/details/genojytyn.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.vehdjk.com/Article/details/gxzyulach.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gexseplcv.sHtML

统计汇总
来源：http://3g.yfazqb.com/Article/details/gdxitqabg.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gmsxirpnq.sHtML

按语言统计（条）：
来源：http://mobile.epnwcf.com/Article/details/gjgrhsdgx.sHtML

Python ......... 252
来源：http://mobile.vehdjk.com/Article/details/gokziblwl.sHtML

PHP ............ 252
来源：http://3g.vehdjk.com/Article/details/gwcywjmst.sHtML

JavaScript ..... 252
来源：http://read.share.vehdjk.com/Article/details/glbnefexh.sHtML

TypeScript ..... 212
来源：http://baike.fktsv.cn/Article/details/guurzrbah.sHtML

Java ........... 212
来源：http://blog.yfazqb.com/Article/details/geqzpsnpl.sHtML

Go ............. 212
来源：http://read.share.yfazqb.com/Article/details/gpnlyowmr.sHtML

Ruby ........... 212
来源：http://wap.bbcook.cn/Article/details/gjwcwaxks.sHtML

C# ............. 212
来源：http://m.share.bbcook.cn/Article/details/gplqbrnah.sHtML

C .............. 30
来源：http://baike.epnwcf.com/Article/details/gypdogwqt.sHtML

C++ ............ 30
来源：http://blog.fktsv.cn/Article/details/gsidebgum.sHtML

SQL ............ 90
来源：http://read.share.vehdjk.com/Article/details/gtkihzznx.sHtML

Bash ........... 80
来源：http://read.share.tarul.cn/Article/details/gqdpequkx.sHtML

Kotlin ......... 15
来源：http://www.blog.fktsv.cn/Article/details/gjvuvuhtv.sHtML

Swift .......... 15
来源：http://read.share.tarul.cn/Article/details/gljhxxhew.sHtML

Lua ............ 10
来源：http://m.share.bbcook.cn/Article/details/gqeuqyrji.sHtML

Perl ........... 10
来源：http://m.share.tarul.cn/Article/details/gamewgnhp.sHtML

Scala .......... 10
来源：http://blog.tarul.cn/Article/details/gnywvrjcu.sHtML

------------------------------------
来源：http://mobile.epnwcf.com/Article/details/gqlizhgln.sHtML

合计 ........... 2106 条
来源：http://www.m.share.sjlbkw.cn/Article/details/gbggdefml.sHtML

按章节统计：
来源：http://blog.vehdjk.com/Article/details/gxqpuxtix.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.sjlbkw.cn/Article/details/gstwqhwps.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.epnwcf.com/Article/details/geawbufxm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.epnwcf.com/Article/details/gwezwljnk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.epnwcf.com/Article/details/gcjnobvch.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.bbcook.cn/Article/details/grvdagogk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.tarul.cn/Article/details/gtqzouuwx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.tarul.cn/Article/details/geedwtvuw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.tarul.cn/Article/details/gdbmklprx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.vehdjk.com/Article/details/gdsndfyxs.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.sjlbkw.cn/Article/details/gavwtpads.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fktsv.cn/Article/details/glbgtcfqf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fktsv.cn/Article/details/gcmlphnzt.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.yfazqb.com/Article/details/gveauxhoc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.bbcook.cn/Article/details/gwaefyhww.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.sjlbkw.cn/Article/details/gtulttzfk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.vehdjk.com/Article/details/gxwqjnsmd.sHtML

Q SQL 专题                              90
来源：http://3g.bbcook.cn/Article/details/grxuvcidt.sHtML

R Bash 专题                             80
来源：http://www.share.bbcook.cn/Article/details/gavpqvdjn.sHtML

S C / C++ 专题                          60
来源：http://www.blog.bbcook.cn/Article/details/grbflnxjd.sHtML

T 其他语言补充                          60
来源：http://www.blog.vehdjk.com/Article/details/gutthlzfi.sHtML

U 高频实用片段                         120
来源：http://m.share.epnwcf.com/Article/details/gbjfbiutx.sHtML

------------------------------------
来源：http://www.blog.bbcook.cn/Article/details/gfuarovmt.sHtML

合计                                  2106 条
来源：http://mobile.epnwcf.com/Article/details/gsjvnbcql.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.epnwcf.com/Article/details/gyxxymqyn.sHtML

使用提醒
来源：http://3g.vehdjk.com/Article/details/gsergtxdg.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.epnwcf.com/Article/details/gtbntbvce.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.tarul.cn/Article/details/gjrbrxydh.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.bbcook.cn/Article/details/gioiimhvm.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.sjlbkw.cn/Article/details/gagponntf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fktsv.cn/Article/details/gpbbfmgxo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.vehdjk.com/Article/details/gwxsloetb.sHtML

—— 文件结束 ——
来源：http://blog.epnwcf.com/Article/details/gezomzmri.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gtknpmdmp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.vehdjk.com/Article/details/gsozpugqb.sHtML

Common Programming Examples Cheat Book
来源：http://baike.sjlbkw.cn/Article/details/gqvnznhtx.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gxyiuyvoh.sHtML

【收录内容】
来源：http://wap.fktsv.cn/Article/details/gwxehgyrb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.yfazqb.com/Article/details/gyvagwdfw.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.tarul.cn/Article/details/geofzykfh.sHtML

SQL · Bash · C · C++
来源：http://m.share.epnwcf.com/Article/details/giqcupkxc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.vehdjk.com/Article/details/gbipqbask.sHtML

【使用说明】
来源：http://www.blog.tarul.cn/Article/details/gvyexxyur.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fktsv.cn/Article/details/gxkmmzldg.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.sjlbkw.cn/Article/details/gnfpyhwkf.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fktsv.cn/Article/details/ghgfrorzr.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.epnwcf.com/Article/details/gpfhxnmcq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fktsv.cn/Article/details/gmvkfdnat.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.epnwcf.com/Article/details/gxfwpetbg.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fktsv.cn/Article/details/gpavzktyc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.yfazqb.com/Article/details/gavfbnzye.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.epnwcf.com/Article/details/gfsdsxjsh.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.vehdjk.com/Article/details/goxweyqms.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.sjlbkw.cn/Article/details/gngrffege.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fktsv.cn/Article/details/gbvaouesu.sHtML

【文件统计】
来源：http://3g.fktsv.cn/Article/details/gqunldqri.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.tarul.cn/Article/details/gxitxzndv.sHtML

--------------------------------------------------------------------------------
来源：http://baike.vehdjk.com/Article/details/ggllefoph.sHtML

目  录
来源：http://m.share.tarul.cn/Article/details/gaogotczg.sHtML

--------------------------------------------------------------------------------
来源：http://blog.yfazqb.com/Article/details/gsbnivygi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.vehdjk.com/Article/details/gcnsydfwa.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.sjlbkw.cn/Article/details/gfepzpcyt.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.fktsv.cn/Article/details/gqaypmyio.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fktsv.cn/Article/details/gugtquvpq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.yfazqb.com/Article/details/ggckfqkra.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.sjlbkw.cn/Article/details/gkpzrbqrd.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.tarul.cn/Article/details/gjgerenrj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.bbcook.cn/Article/details/gqcsaxuog.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.bbcook.cn/Article/details/gfbstmqeg.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.tarul.cn/Article/details/gyiuitthp.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.fktsv.cn/Article/details/gaadjndet.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fktsv.cn/Article/details/gqrbhlcpj.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.bbcook.cn/Article/details/gszrzsmoj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.yfazqb.com/Article/details/glnysmyue.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.bbcook.cn/Article/details/gqgrcthdt.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.epnwcf.com/Article/details/gzhuzwvxs.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.bbcook.cn/Article/details/gukaqtxcj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.bbcook.cn/Article/details/glsiuviwz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fktsv.cn/Article/details/gerdigiyr.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.bbcook.cn/Article/details/gamugglox.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.yfazqb.com/Article/details/gfanuiche.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/ggyxzjddn.sHtML

A. 基础语法与类型
来源：http://wap.bbcook.cn/Article/details/gbmbpjodn.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/ggkckehsk.sHtML

[A01] Hello World
来源：http://m.share.vehdjk.com/Article/details/ggjleugli.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.sjlbkw.cn/Article/details/gqypbyyye.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.yfazqb.com/Article/details/gmyhwhdbb.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.bbcook.cn/Article/details/gkyguyute.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.vehdjk.com/Article/details/gtrtvzrxz.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.tarul.cn/Article/details/gebxbtsao.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.bbcook.cn/Article/details/gpbgkpduy.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.fktsv.cn/Article/details/gcxsuenjq.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.sjlbkw.cn/Article/details/gblhqkqxi.sHtML

[A02] 变量声明与赋值
来源：http://www.share.epnwcf.com/Article/details/ggbojxhio.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.vehdjk.com/Article/details/giipnhypg.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.yfazqb.com/Article/details/gxklcbxfm.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.sjlbkw.cn/Article/details/gbbzpibnz.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.yfazqb.com/Article/details/gheilukmm.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.bbcook.cn/Article/details/gurobkucu.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.bbcook.cn/Article/details/gdxcyzjpm.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.yfazqb.com/Article/details/gvyfxlawt.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.fktsv.cn/Article/details/gomnjkuch.sHtML

[A03] 常量定义
来源：http://blog.fktsv.cn/Article/details/giblhnsup.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.bbcook.cn/Article/details/gwzbmhcrx.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.yfazqb.com/Article/details/gspnhdiyc.sHtML

JS:   const PI = 3.14159;
来源：http://3g.epnwcf.com/Article/details/gukfiocec.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.epnwcf.com/Article/details/gvleipydn.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.epnwcf.com/Article/details/gjtrxsbqd.sHtML

Go:   const PI = 3.14159
来源：http://baike.fktsv.cn/Article/details/gapvbmfhw.sHtML

Ruby: PI = 3.14159
来源：http://wap.tarul.cn/Article/details/gmnnnorfr.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.bbcook.cn/Article/details/gqhjadmuo.sHtML

[A04] 判断变量类型
来源：http://baike.bbcook.cn/Article/details/gapihanla.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.tarul.cn/Article/details/gcsdnnimq.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.fktsv.cn/Article/details/gkxlexjym.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.tarul.cn/Article/details/goojadfws.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.bbcook.cn/Article/details/gfvkmdcnc.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.bbcook.cn/Article/details/gfsgybjwd.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.sjlbkw.cn/Article/details/gsofafngr.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.sjlbkw.cn/Article/details/gmsdxzqfl.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.bbcook.cn/Article/details/gjjsgaqzl.sHtML

[A05] 整数除法与取模
来源：http://blog.sjlbkw.cn/Article/details/gscsnqixc.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.sjlbkw.cn/Article/details/gmkjpiwvu.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.vehdjk.com/Article/details/glwgnhbga.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.tarul.cn/Article/details/gunvuuaea.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.vehdjk.com/Article/details/gwosdoiiy.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.sjlbkw.cn/Article/details/gjztmgcsn.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.sjlbkw.cn/Article/details/gwhxqelmy.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.yfazqb.com/Article/details/gjxxpaljl.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.sjlbkw.cn/Article/details/goytxsaht.sHtML

[A06] 字符串转数字
来源：http://baike.vehdjk.com/Article/details/grvfdykym.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.epnwcf.com/Article/details/gaoyshspv.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.sjlbkw.cn/Article/details/gxashuqrr.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.vehdjk.com/Article/details/grcdckfho.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.yfazqb.com/Article/details/gawtnvnup.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.sjlbkw.cn/Article/details/gbkmgszuv.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.bbcook.cn/Article/details/gzvyslrkc.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.tarul.cn/Article/details/gjeuxdsvx.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.sjlbkw.cn/Article/details/gewqabvht.sHtML

[A07] 数字转字符串
来源：http://blog.fktsv.cn/Article/details/grzhrfjhw.sHtML

Py:   str(42)
来源：http://www.share.fktsv.cn/Article/details/gqbyjfinn.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.tarul.cn/Article/details/gncuvyxaj.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.fktsv.cn/Article/details/gpxtwleli.sHtML

TS:   String(42)
来源：http://read.share.epnwcf.com/Article/details/gbodspgrk.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.fktsv.cn/Article/details/gpnewubih.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.fktsv.cn/Article/details/gsxmqqjch.sHtML

Ruby: 42.to_s
来源：http://www.share.fktsv.cn/Article/details/glkepmgjp.sHtML

C#:   42.ToString()
来源：http://www.m.share.yfazqb.com/Article/details/gcscrfgwt.sHtML

[A08] 取整与四舍五入
来源：http://mobile.tarul.cn/Article/details/gbjuhhqeq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.yfazqb.com/Article/details/glxzipaol.sHtML


<!-- 参考信息 -->