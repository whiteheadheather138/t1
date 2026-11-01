代发 wailian999

[U59] PHP：自定义排序
来源：http://read.share.sjlbkw.cn/Article/details/grdbcdcos.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.tarul.cn/Article/details/gmondjxwo.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.yfazqb.com/Article/details/gdkycewii.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.sjlbkw.cn/Article/details/gtezvgitu.sHtML

[U61] PHP：正则
来源：http://3g.bbcook.cn/Article/details/gjrmjdlzw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.yfazqb.com/Article/details/gycuutnwe.sHtML

[U62] PHP：日期对象
来源：http://baike.epnwcf.com/Article/details/gjsxqcrsw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.bbcook.cn/Article/details/gcujclqxb.sHtML

[U63] PHP：文件读写
来源：http://blog.epnwcf.com/Article/details/grulwpzcl.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.tarul.cn/Article/details/ghlkkymxl.sHtML

[U64] PHP：目录遍历
来源：http://3g.yfazqb.com/Article/details/gyovjbmfv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.epnwcf.com/Article/details/ghjfmebgo.sHtML

[U65] PHP：会话
来源：http://mobile.yfazqb.com/Article/details/gutxyoosv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fktsv.cn/Article/details/gdgaoubqv.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.epnwcf.com/Article/details/gzoapdbbd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.tarul.cn/Article/details/gwuhnqoeu.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.bbcook.cn/Article/details/gsypwzysi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.sjlbkw.cn/Article/details/glswbtbrw.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.bbcook.cn/Article/details/gswojdlww.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.epnwcf.com/Article/details/gfswlcfmv.sHtML

[U69] PHP：PDO 预处理
来源：http://www.blog.bbcook.cn/Article/details/gegzvkxmx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.epnwcf.com/Article/details/gextyrizj.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.bbcook.cn/Article/details/gouttzhse.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.yfazqb.com/Article/details/glwmftkcv.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.yfazqb.com/Article/details/glqscvhln.sHtML

throw new RuntimeException("失败", 500);
来源：http://baike.vehdjk.com/Article/details/gihbxvxom.sHtML

[U72] PHP：写错误日志
来源：http://www.share.epnwcf.com/Article/details/gudxddjxr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.epnwcf.com/Article/details/gdhkjnwlu.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.sjlbkw.cn/Article/details/gnioakcvd.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.epnwcf.com/Article/details/gpdgnholb.sHtML

[U74] PHP：读取环境变量
来源：http://baike.sjlbkw.cn/Article/details/gdlvlxfxw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.bbcook.cn/Article/details/gexxnfhdo.sHtML

[U75] PHP：依赖注入
来源：http://www.share.epnwcf.com/Article/details/guzpefpiz.sHtML

composer require psr/container
来源：http://blog.fktsv.cn/Article/details/gnxrkvprc.sHtML

[U76] PHP：简单路由
来源：http://blog.epnwcf.com/Article/details/gvmdxyqsa.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.bbcook.cn/Article/details/gaoqbcydz.sHtML

[U77] PHP：模板渲染
来源：http://blog.tarul.cn/Article/details/gouzgycvc.sHtML

composer require twig/twig
来源：http://wap.tarul.cn/Article/details/gqcvutirl.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.yfazqb.com/Article/details/giaarqhjl.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.tarul.cn/Article/details/grymvgjxb.sHtML

[U79] PHP：静态分析
来源：http://blog.tarul.cn/Article/details/gwyfmmakn.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.tarul.cn/Article/details/gmorjvdbc.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fktsv.cn/Article/details/gybtxmdtq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fktsv.cn/Article/details/ggfbwvilg.sHtML

[U81] JS：初始化项目
来源：http://3g.sjlbkw.cn/Article/details/gqvqkelxd.sHtML

npm init -y;  npm i express
来源：http://3g.sjlbkw.cn/Article/details/gokwbsyeu.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.bbcook.cn/Article/details/gkwegnjtb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.sjlbkw.cn/Article/details/ghmrixwsm.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.vehdjk.com/Article/details/grgqpauqw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.yfazqb.com/Article/details/gumobtopd.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.epnwcf.com/Article/details/gvbiqwurn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.vehdjk.com/Article/details/gdjfuixpl.sHtML

[U85] JS：可选链
来源：http://www.m.share.vehdjk.com/Article/details/glhtrsrvn.sHtML

a?.b?.c
来源：http://www.blog.yfazqb.com/Article/details/gcqmkxlgb.sHtML

[U86] JS：空值合并
来源：http://mobile.sjlbkw.cn/Article/details/gwefmuizh.sHtML

a ?? b
来源：http://www.m.share.fktsv.cn/Article/details/gjwxfczsw.sHtML

[U87] JS：解构默认值
来源：http://baike.sjlbkw.cn/Article/details/gjormqeby.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.sjlbkw.cn/Article/details/gutlxaxpk.sHtML

[U88] JS：对象展开合并
来源：http://read.share.vehdjk.com/Article/details/gychxydno.sHtML

{ ...a, ...b }
来源：http://3g.epnwcf.com/Article/details/ghkaopamw.sHtML

[U89] JS：数组去重
来源：http://read.share.fktsv.cn/Article/details/gjxtafjwy.sHtML

[...new Set(arr)]
来源：http://read.share.vehdjk.com/Article/details/gdndrhvej.sHtML

[U90] JS：数字数组排序
来源：http://m.share.tarul.cn/Article/details/gxonymlnv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.vehdjk.com/Article/details/gaqtphtbf.sHtML

[U91] JS：对象键值遍历
来源：http://blog.vehdjk.com/Article/details/grjlvpunj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.sjlbkw.cn/Article/details/gajlkmgmc.sHtML

[U92] JS：深拷贝
来源：http://m.share.tarul.cn/Article/details/geeoqdcyr.sHtML

structuredClone(obj)
来源：http://www.share.vehdjk.com/Article/details/gayrdpdpu.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.vehdjk.com/Article/details/gxdkrkwfn.sHtML

`共 ${n} 条`
来源：http://wap.bbcook.cn/Article/details/gsdfigrms.sHtML

[U94] JS：箭头函数
来源：http://baike.vehdjk.com/Article/details/gfqijyfoc.sHtML

const double = x => x * 2;
来源：http://wap.yfazqb.com/Article/details/gbpgzpxqd.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.bbcook.cn/Article/details/gcfnhvrtn.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fktsv.cn/Article/details/gumltcwcw.sHtML

[U96] JS：async/await 与异常
来源：http://blog.bbcook.cn/Article/details/gdoddwqxq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.yfazqb.com/Article/details/gvwwldoef.sHtML

[U97] JS：并发请求
来源：http://read.share.yfazqb.com/Article/details/gsxmzmlbd.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fktsv.cn/Article/details/gtkrkakmz.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fktsv.cn/Article/details/gnkncwltp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.vehdjk.com/Article/details/gkhxtigzn.sHtML

[U99] JS：事件监听
来源：http://www.share.tarul.cn/Article/details/gtbgaezrb.sHtML

el.addEventListener("click", e => {})
来源：http://3g.epnwcf.com/Article/details/geobbzafb.sHtML

[U100] JS：DOM 查询
来源：http://m.share.vehdjk.com/Article/details/gexwfbdhl.sHtML

document.querySelector(".item")
来源：http://www.blog.fktsv.cn/Article/details/grwhuxwhe.sHtML

[U101] JS：classList 操作
来源：http://3g.fktsv.cn/Article/details/guzjmtugu.sHtML

el.classList.toggle("active")
来源：http://blog.sjlbkw.cn/Article/details/ghdxxvqyl.sHtML

[U102] JS：本地存储
来源：http://baike.tarul.cn/Article/details/gdedafmiq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.sjlbkw.cn/Article/details/gxsirbxpb.sHtML

[U103] JS：定时器
来源：http://www.blog.yfazqb.com/Article/details/gagccudhr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.bbcook.cn/Article/details/gmxdmmkns.sHtML

[U104] JS：防抖
来源：http://www.m.share.yfazqb.com/Article/details/gmenqknok.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fktsv.cn/Article/details/gldansyat.sHtML

[U105] JS：节流
来源：http://blog.tarul.cn/Article/details/gspwanceh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.yfazqb.com/Article/details/gvgahsxht.sHtML

[U106] JS：日期格式化
来源：http://3g.tarul.cn/Article/details/ghblymdsa.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.tarul.cn/Article/details/ghstrlxkf.sHtML

[U107] JS：数字千分位
来源：http://3g.fktsv.cn/Article/details/gznnlmvqq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.epnwcf.com/Article/details/gxlltpigs.sHtML

[U108] JS：随机整数
来源：http://www.blog.sjlbkw.cn/Article/details/gssarjqre.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.yfazqb.com/Article/details/gmamjdwhf.sHtML

[U109] JS：数组分组
来源：http://baike.tarul.cn/Article/details/gprosjlpc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fktsv.cn/Article/details/gdfyovwvj.sHtML

[U110] JS：数组分块
来源：http://3g.sjlbkw.cn/Article/details/gbprreoxi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.tarul.cn/Article/details/gqamfnfvk.sHtML

[U111] JS：对象转 Map
来源：http://m.share.bbcook.cn/Article/details/gkqnrzaxl.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fktsv.cn/Article/details/gxgskohck.sHtML

[U112] JS：字符串补位
来源：http://www.blog.vehdjk.com/Article/details/gryqemmtp.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.yfazqb.com/Article/details/gsutkbotz.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fktsv.cn/Article/details/ggugseigy.sHtML

s.replaceAll("a", "b")
来源：http://baike.vehdjk.com/Article/details/grrsnbdjo.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.bbcook.cn/Article/details/ggwouxnhh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.bbcook.cn/Article/details/ggxtghjaz.sHtML

[U115] JS：生成 UUID
来源：http://3g.vehdjk.com/Article/details/gkkpuluvv.sHtML

crypto.randomUUID()
来源：http://read.share.epnwcf.com/Article/details/grvxzjlst.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fktsv.cn/Article/details/gowlrrier.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fktsv.cn/Article/details/gcffyrsry.sHtML

[U117] JS：单元测试
来源：http://blog.yfazqb.com/Article/details/gnslniflz.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.vehdjk.com/Article/details/gqvedzmpy.sHtML

[U118] JS：开发服务器
来源：http://blog.fktsv.cn/Article/details/gozwpdlfd.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.yfazqb.com/Article/details/gqzxdxmrq.sHtML

[U119] JS：生产构建
来源：http://wap.tarul.cn/Article/details/ggdhmtqol.sHtML

npx vite build
来源：http://www.m.share.tarul.cn/Article/details/gijmmaswb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.vehdjk.com/Article/details/geezddmwd.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.epnwcf.com/Article/details/gexgkhlnh.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gabmvzpkh.sHtML

统计汇总
来源：http://read.share.epnwcf.com/Article/details/giulrinpb.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gikxhiqqt.sHtML

按语言统计（条）：
来源：http://baike.tarul.cn/Article/details/gbwpuxikq.sHtML

Python ......... 252
来源：http://m.share.vehdjk.com/Article/details/ghrklouxe.sHtML

PHP ............ 252
来源：http://www.m.share.tarul.cn/Article/details/gpcrylyvy.sHtML

JavaScript ..... 252
来源：http://mobile.bbcook.cn/Article/details/gepprvqji.sHtML

TypeScript ..... 212
来源：http://www.m.share.yfazqb.com/Article/details/gulprvzes.sHtML

Java ........... 212
来源：http://3g.tarul.cn/Article/details/gqpcsmiti.sHtML

Go ............. 212
来源：http://baike.sjlbkw.cn/Article/details/gztqjgrxp.sHtML

Ruby ........... 212
来源：http://www.blog.vehdjk.com/Article/details/gnjsbztsw.sHtML

C# ............. 212
来源：http://read.share.vehdjk.com/Article/details/gznlognvn.sHtML

C .............. 30
来源：http://m.share.yfazqb.com/Article/details/goximbybd.sHtML

C++ ............ 30
来源：http://wap.sjlbkw.cn/Article/details/gjoanxhfq.sHtML

SQL ............ 90
来源：http://www.blog.sjlbkw.cn/Article/details/gzuundjkl.sHtML

Bash ........... 80
来源：http://mobile.sjlbkw.cn/Article/details/gkgnopwxd.sHtML

Kotlin ......... 15
来源：http://blog.vehdjk.com/Article/details/gesfxzbjq.sHtML

Swift .......... 15
来源：http://www.share.bbcook.cn/Article/details/gvpepwwwc.sHtML

Lua ............ 10
来源：http://www.blog.tarul.cn/Article/details/gidrxfgjl.sHtML

Perl ........... 10
来源：http://www.blog.fktsv.cn/Article/details/gocbeczrz.sHtML

Scala .......... 10
来源：http://www.share.tarul.cn/Article/details/gbgopvwcn.sHtML

------------------------------------
来源：http://3g.bbcook.cn/Article/details/gndtoaenr.sHtML

合计 ........... 2106 条
来源：http://3g.tarul.cn/Article/details/gidyglnzw.sHtML

按章节统计：
来源：http://baike.epnwcf.com/Article/details/gcglnamtf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.sjlbkw.cn/Article/details/gqyjapupx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.yfazqb.com/Article/details/gaalshyif.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.bbcook.cn/Article/details/gspirvjpg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fktsv.cn/Article/details/gfjpxeznn.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.sjlbkw.cn/Article/details/gtodenfvc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fktsv.cn/Article/details/gmfwhpucg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fktsv.cn/Article/details/guowxbhup.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fktsv.cn/Article/details/gyvazvhcn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.sjlbkw.cn/Article/details/gstaoueaq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.yfazqb.com/Article/details/gzbwtinnt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.bbcook.cn/Article/details/gqlmswtqg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.yfazqb.com/Article/details/goltepzft.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.epnwcf.com/Article/details/gowamljcy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fktsv.cn/Article/details/gqfqgnzjm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fktsv.cn/Article/details/gxstxsggt.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.sjlbkw.cn/Article/details/gvlukrxod.sHtML

Q SQL 专题                              90
来源：http://3g.bbcook.cn/Article/details/gzcxgngqq.sHtML

R Bash 专题                             80
来源：http://baike.epnwcf.com/Article/details/gktnwmeha.sHtML

S C / C++ 专题                          60
来源：http://blog.sjlbkw.cn/Article/details/gkmahdjyz.sHtML

T 其他语言补充                          60
来源：http://wap.bbcook.cn/Article/details/gsrlsgqie.sHtML

U 高频实用片段                         120
来源：http://www.blog.yfazqb.com/Article/details/gqpjvpevz.sHtML

------------------------------------
来源：http://www.share.tarul.cn/Article/details/gvvstdgzl.sHtML

合计                                  2106 条
来源：http://www.m.share.epnwcf.com/Article/details/ghaxkungu.sHtML

--------------------------------------------------------------------------------
来源：http://blog.yfazqb.com/Article/details/gbpchedgl.sHtML

使用提醒
来源：http://www.m.share.yfazqb.com/Article/details/gpxhyxmjy.sHtML

--------------------------------------------------------------------------------
来源：http://3g.sjlbkw.cn/Article/details/gpcumhsvc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.vehdjk.com/Article/details/ghwrsanro.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.yfazqb.com/Article/details/gherhjrfe.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.yfazqb.com/Article/details/gadorqoob.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.yfazqb.com/Article/details/gbybimbma.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.yfazqb.com/Article/details/gnmuvkiex.sHtML

—— 文件结束 ——
来源：http://www.blog.bbcook.cn/Article/details/gbnumpgew.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gezkiczpd.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.bbcook.cn/Article/details/gqfibmxrp.sHtML

Common Programming Examples Cheat Book
来源：http://wap.tarul.cn/Article/details/gihruejjw.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gklcmxrus.sHtML

【收录内容】
来源：http://mobile.yfazqb.com/Article/details/gxkljvcbf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fktsv.cn/Article/details/giemrnhpx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.tarul.cn/Article/details/glclzwilz.sHtML

SQL · Bash · C · C++
来源：http://read.share.sjlbkw.cn/Article/details/gkagariof.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.vehdjk.com/Article/details/gkjocfbvv.sHtML

【使用说明】
来源：http://blog.epnwcf.com/Article/details/grrgjgjux.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.vehdjk.com/Article/details/gydqhvelm.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.sjlbkw.cn/Article/details/gmwnpexkp.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.yfazqb.com/Article/details/gcdcrcypr.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.epnwcf.com/Article/details/ghqyxuxnl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.vehdjk.com/Article/details/gzgxapcgv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.epnwcf.com/Article/details/gktbonimq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fktsv.cn/Article/details/ghijcbiem.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.tarul.cn/Article/details/ghrngyemu.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.sjlbkw.cn/Article/details/gabktkcej.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.sjlbkw.cn/Article/details/gxexusgsh.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.epnwcf.com/Article/details/gvqswaazw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.sjlbkw.cn/Article/details/gjplvvaqk.sHtML

【文件统计】
来源：http://www.blog.yfazqb.com/Article/details/geabcitrd.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.vehdjk.com/Article/details/gkjsmxioy.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fktsv.cn/Article/details/gxdzyxclv.sHtML

目  录
来源：http://blog.sjlbkw.cn/Article/details/gnqpmlbxu.sHtML

--------------------------------------------------------------------------------
来源：http://3g.sjlbkw.cn/Article/details/gycvdxfgd.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.bbcook.cn/Article/details/grufhorvy.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.vehdjk.com/Article/details/gsgsynslh.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.vehdjk.com/Article/details/grmedvwgt.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.yfazqb.com/Article/details/gjtkkrsag.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.sjlbkw.cn/Article/details/gtnngfklt.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.yfazqb.com/Article/details/gggglodhh.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.vehdjk.com/Article/details/gelcwtnlf.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.tarul.cn/Article/details/gpkauokgp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.bbcook.cn/Article/details/gawobhmvn.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.yfazqb.com/Article/details/gguvisare.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.tarul.cn/Article/details/gdqyxpenb.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.sjlbkw.cn/Article/details/gvuxwhqdc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fktsv.cn/Article/details/gycjhtpnb.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.sjlbkw.cn/Article/details/gtypzkfrf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.tarul.cn/Article/details/gtrfifkxy.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.epnwcf.com/Article/details/gkgmyqvla.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.yfazqb.com/Article/details/grgatyemc.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.tarul.cn/Article/details/gadhyspcf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.bbcook.cn/Article/details/gycdekkmw.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.bbcook.cn/Article/details/ggbadlcqa.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.bbcook.cn/Article/details/ggfghzkci.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/ggqnnobhx.sHtML

A. 基础语法与类型
来源：http://baike.tarul.cn/Article/details/gswhfeqla.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gizevjzyd.sHtML

[A01] Hello World
来源：http://3g.bbcook.cn/Article/details/ghglnupki.sHtML

Py:   print("Hello, World!")
来源：http://read.share.bbcook.cn/Article/details/gmdbqdutd.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.tarul.cn/Article/details/googhsfqr.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.tarul.cn/Article/details/glarysfxv.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.tarul.cn/Article/details/gpvirrisa.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.yfazqb.com/Article/details/gnuqgpvep.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.tarul.cn/Article/details/gshshtrjc.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.bbcook.cn/Article/details/gbnbfglja.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.yfazqb.com/Article/details/geqrkqmzv.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.tarul.cn/Article/details/gtkvhwgbc.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.vehdjk.com/Article/details/gsgwywdmf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.yfazqb.com/Article/details/gyoxumvvz.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.bbcook.cn/Article/details/gqtgsfwbd.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.tarul.cn/Article/details/gkmigkdya.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.sjlbkw.cn/Article/details/gswhsdazs.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.fktsv.cn/Article/details/gtxwzujhq.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fktsv.cn/Article/details/guyvqwide.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.yfazqb.com/Article/details/gztsgmywu.sHtML

[A03] 常量定义
来源：http://www.share.epnwcf.com/Article/details/ghhlphhoq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.bbcook.cn/Article/details/gxnkbqvtl.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.sjlbkw.cn/Article/details/gqxqyhjat.sHtML

JS:   const PI = 3.14159;
来源：http://blog.tarul.cn/Article/details/gnllwxfsn.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.yfazqb.com/Article/details/gykrcvozt.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.sjlbkw.cn/Article/details/gesfndapi.sHtML

Go:   const PI = 3.14159
来源：http://baike.epnwcf.com/Article/details/gsbeyxauu.sHtML

Ruby: PI = 3.14159
来源：http://baike.vehdjk.com/Article/details/gfaqgkjxw.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.bbcook.cn/Article/details/georrjwjb.sHtML

[A04] 判断变量类型
来源：http://m.share.tarul.cn/Article/details/gatssmjpg.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.epnwcf.com/Article/details/ggkjharlz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.bbcook.cn/Article/details/gduouehfh.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.epnwcf.com/Article/details/gepdouzpw.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.bbcook.cn/Article/details/gxgmtwvtb.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.vehdjk.com/Article/details/gshkzlrvg.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.epnwcf.com/Article/details/gbhzlypxx.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.vehdjk.com/Article/details/gtwunbkql.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.vehdjk.com/Article/details/gfkidayvb.sHtML

[A05] 整数除法与取模
来源：http://read.share.sjlbkw.cn/Article/details/gsvtsjyra.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.bbcook.cn/Article/details/gxmuricul.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.tarul.cn/Article/details/glrogxirx.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fktsv.cn/Article/details/grauotwqf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.tarul.cn/Article/details/gapxycbed.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.bbcook.cn/Article/details/gwnuhmwgp.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.vehdjk.com/Article/details/gahkooxtx.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.fktsv.cn/Article/details/gqnifyhuz.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.sjlbkw.cn/Article/details/gsojfnqbp.sHtML

[A06] 字符串转数字
来源：http://m.share.tarul.cn/Article/details/gqnefmaqw.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.tarul.cn/Article/details/gjrkijntv.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.vehdjk.com/Article/details/goypqmqky.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.yfazqb.com/Article/details/gbkocbrmo.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.sjlbkw.cn/Article/details/gceipzbdf.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.tarul.cn/Article/details/gtmojtucl.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.sjlbkw.cn/Article/details/giuvwelpq.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.bbcook.cn/Article/details/grlyigpvn.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.tarul.cn/Article/details/gpggpcgbh.sHtML

[A07] 数字转字符串
来源：http://www.blog.tarul.cn/Article/details/gogozivhk.sHtML

Py:   str(42)
来源：http://read.share.yfazqb.com/Article/details/glsreteuf.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.fktsv.cn/Article/details/gtxjgxywr.sHtML

JS:   String(42); (42).toString()
来源：http://3g.fktsv.cn/Article/details/goqaovsxb.sHtML

TS:   String(42)
来源：http://mobile.yfazqb.com/Article/details/ggbzsidvw.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.yfazqb.com/Article/details/glyjndvds.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.fktsv.cn/Article/details/gdrswkgzr.sHtML

Ruby: 42.to_s
来源：http://baike.bbcook.cn/Article/details/grdqcgyxy.sHtML

C#:   42.ToString()
来源：http://mobile.bbcook.cn/Article/details/geatkxrmo.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.bbcook.cn/Article/details/gnlhrrvmr.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.fktsv.cn/Article/details/gbvzqyidj.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.bbcook.cn/Article/details/gngmguwvp.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.epnwcf.com/Article/details/gtwqpuogj.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.sjlbkw.cn/Article/details/gxoinxisq.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.tarul.cn/Article/details/ggvqkukei.sHtML


<!-- 参考信息 -->