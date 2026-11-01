代发 wailian999

[U57] PHP：字符串插值
来源：http://m.share.yfazqb.com/Article/details/gxofkgiha.sHtML

"值: {$a}"
来源：http://www.m.share.vehdjk.com/Article/details/gzehbjzzn.sHtML

[U58] PHP：数组三件套
来源：http://blog.sjlbkw.cn/Article/details/grcxzgdmm.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.sjlbkw.cn/Article/details/gqfongykg.sHtML

[U59] PHP：自定义排序
来源：http://read.share.yfazqb.com/Article/details/guvkqkqnf.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.tarul.cn/Article/details/gqpoiohij.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.bbcook.cn/Article/details/gezrleplo.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fktsv.cn/Article/details/gfiinkjja.sHtML

[U61] PHP：正则
来源：http://www.share.epnwcf.com/Article/details/grjyvpfay.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.bbcook.cn/Article/details/gsjkaixrj.sHtML

[U62] PHP：日期对象
来源：http://baike.sjlbkw.cn/Article/details/glqgwsnlp.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.tarul.cn/Article/details/gslxfctgx.sHtML

[U63] PHP：文件读写
来源：http://mobile.fktsv.cn/Article/details/grmsozwsc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.epnwcf.com/Article/details/gqknbmrlm.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fktsv.cn/Article/details/gzrisndhi.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://3g.sjlbkw.cn/Article/details/gaaukenjh.sHtML

[U65] PHP：会话
来源：http://mobile.sjlbkw.cn/Article/details/gnnoechck.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.sjlbkw.cn/Article/details/gapqbkpyy.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.vehdjk.com/Article/details/gigiluqxv.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.vehdjk.com/Article/details/gqkqfrleu.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.fktsv.cn/Article/details/gljpmtozb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.vehdjk.com/Article/details/gwjdwhjdc.sHtML

[U68] PHP：PDO 连接
来源：http://baike.epnwcf.com/Article/details/gnqtxqhhu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.epnwcf.com/Article/details/gkvlthxdg.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.yfazqb.com/Article/details/gspewdlfc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.epnwcf.com/Article/details/gbzspynlx.sHtML

[U70] PHP：PDO 事务
来源：http://3g.sjlbkw.cn/Article/details/gbjycntjp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.epnwcf.com/Article/details/gspowcsoa.sHtML

[U71] PHP：抛出异常
来源：http://3g.vehdjk.com/Article/details/gszslgfpb.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.sjlbkw.cn/Article/details/gwwayzrzn.sHtML

[U72] PHP：写错误日志
来源：http://mobile.bbcook.cn/Article/details/gixgomtql.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.epnwcf.com/Article/details/gjtvkytdf.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.m.share.vehdjk.com/Article/details/gvsjltdir.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.epnwcf.com/Article/details/gyqlpmekt.sHtML

[U74] PHP：读取环境变量
来源：http://wap.yfazqb.com/Article/details/gsliscmli.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.vehdjk.com/Article/details/gzkajlxvl.sHtML

[U75] PHP：依赖注入
来源：http://read.share.sjlbkw.cn/Article/details/grdomfpoj.sHtML

composer require psr/container
来源：http://mobile.bbcook.cn/Article/details/gukouazrf.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fktsv.cn/Article/details/grcryijlp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.bbcook.cn/Article/details/gjebrbvrl.sHtML

[U77] PHP：模板渲染
来源：http://wap.bbcook.cn/Article/details/gttwvqcxp.sHtML

composer require twig/twig
来源：http://m.share.yfazqb.com/Article/details/gcpknoium.sHtML

[U78] PHP：单元测试
来源：http://www.blog.vehdjk.com/Article/details/gzxdkvohk.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.tarul.cn/Article/details/gljiftfmm.sHtML

[U79] PHP：静态分析
来源：http://wap.epnwcf.com/Article/details/gbyfkhymt.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.yfazqb.com/Article/details/gqrjfjpzm.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.yfazqb.com/Article/details/guqnzgiok.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.vehdjk.com/Article/details/gsqibivxv.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.bbcook.cn/Article/details/goqelvwju.sHtML

npm init -y;  npm i express
来源：http://www.blog.fktsv.cn/Article/details/gzsgiufmv.sHtML

[U82] JS：package.json 脚本
来源：http://wap.tarul.cn/Article/details/gcoiknrog.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.sjlbkw.cn/Article/details/gytqzxrdw.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.fktsv.cn/Article/details/grrpvokgd.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.bbcook.cn/Article/details/ggjmjnjae.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.sjlbkw.cn/Article/details/gppnsgkmq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.fktsv.cn/Article/details/gyznvcgud.sHtML

[U85] JS：可选链
来源：http://www.blog.bbcook.cn/Article/details/gvmadutta.sHtML

a?.b?.c
来源：http://read.share.tarul.cn/Article/details/gbxyedehl.sHtML

[U86] JS：空值合并
来源：http://read.share.fktsv.cn/Article/details/gijfxlygm.sHtML

a ?? b
来源：http://www.share.vehdjk.com/Article/details/gcecbpygn.sHtML

[U87] JS：解构默认值
来源：http://wap.epnwcf.com/Article/details/grizxqmfs.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.vehdjk.com/Article/details/gjzabckdj.sHtML

[U88] JS：对象展开合并
来源：http://mobile.bbcook.cn/Article/details/ggmhzwnul.sHtML

{ ...a, ...b }
来源：http://m.share.epnwcf.com/Article/details/gxvhhwkxz.sHtML

[U89] JS：数组去重
来源：http://www.m.share.sjlbkw.cn/Article/details/gljivuttt.sHtML

[...new Set(arr)]
来源：http://www.blog.tarul.cn/Article/details/gdxrfmzll.sHtML

[U90] JS：数字数组排序
来源：http://3g.yfazqb.com/Article/details/gghvrmsad.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.bbcook.cn/Article/details/gvizkyeiu.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fktsv.cn/Article/details/gjlmcnneo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.vehdjk.com/Article/details/gubqqirfo.sHtML

[U92] JS：深拷贝
来源：http://m.share.yfazqb.com/Article/details/gzmwpjqhk.sHtML

structuredClone(obj)
来源：http://m.share.epnwcf.com/Article/details/gdprdgxpo.sHtML

[U93] JS：模板字符串
来源：http://mobile.yfazqb.com/Article/details/glmojksza.sHtML

`共 ${n} 条`
来源：http://blog.yfazqb.com/Article/details/gtehxsrgb.sHtML

[U94] JS：箭头函数
来源：http://read.share.sjlbkw.cn/Article/details/gvxfdqwuq.sHtML

const double = x => x * 2;
来源：http://blog.tarul.cn/Article/details/gteomlvnl.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fktsv.cn/Article/details/gqzotaelm.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fktsv.cn/Article/details/gmvwaokez.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.sjlbkw.cn/Article/details/galkvsgnw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.yfazqb.com/Article/details/ggoqevvxq.sHtML

[U97] JS：并发请求
来源：http://3g.fktsv.cn/Article/details/gzvdmgjjs.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.tarul.cn/Article/details/gifwxvqdy.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.sjlbkw.cn/Article/details/gcnehhzsu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.yfazqb.com/Article/details/gxtypkktt.sHtML

[U99] JS：事件监听
来源：http://wap.fktsv.cn/Article/details/gnlxdkfdo.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.bbcook.cn/Article/details/glffyqrnd.sHtML

[U100] JS：DOM 查询
来源：http://3g.tarul.cn/Article/details/gnpnwpqfq.sHtML

document.querySelector(".item")
来源：http://3g.sjlbkw.cn/Article/details/ggtlxenyl.sHtML

[U101] JS：classList 操作
来源：http://wap.fktsv.cn/Article/details/gzyevblgq.sHtML

el.classList.toggle("active")
来源：http://3g.fktsv.cn/Article/details/gjvvuxqir.sHtML

[U102] JS：本地存储
来源：http://m.share.fktsv.cn/Article/details/gcmwncstd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.epnwcf.com/Article/details/gxklhcqoy.sHtML

[U103] JS：定时器
来源：http://m.share.tarul.cn/Article/details/gydlimhmt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.bbcook.cn/Article/details/gfwlahbfr.sHtML

[U104] JS：防抖
来源：http://3g.bbcook.cn/Article/details/ggmounrco.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.bbcook.cn/Article/details/gjszlwybo.sHtML

[U105] JS：节流
来源：http://3g.yfazqb.com/Article/details/gbsyyqctv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.yfazqb.com/Article/details/gzgltpxux.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.bbcook.cn/Article/details/gpgpknmso.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.yfazqb.com/Article/details/gltqvuhow.sHtML

[U107] JS：数字千分位
来源：http://mobile.fktsv.cn/Article/details/gjfppklbi.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.epnwcf.com/Article/details/gjybkznac.sHtML

[U108] JS：随机整数
来源：http://www.m.share.yfazqb.com/Article/details/gwagoanhy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.vehdjk.com/Article/details/gvplojopo.sHtML

[U109] JS：数组分组
来源：http://baike.vehdjk.com/Article/details/gcrljudoe.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.sjlbkw.cn/Article/details/gflrwwvpj.sHtML

[U110] JS：数组分块
来源：http://www.m.share.yfazqb.com/Article/details/gsnncnrme.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.bbcook.cn/Article/details/gyyhtduzm.sHtML

[U111] JS：对象转 Map
来源：http://baike.sjlbkw.cn/Article/details/gxxpyirqb.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.tarul.cn/Article/details/gqhhbobdf.sHtML

[U112] JS：字符串补位
来源：http://wap.sjlbkw.cn/Article/details/gktyedqfg.sHtML

"7".padStart(3, "0")
来源：http://www.blog.tarul.cn/Article/details/gwlvsjtdh.sHtML

[U113] JS：正则替换全部
来源：http://www.share.tarul.cn/Article/details/gxcbjgioz.sHtML

s.replaceAll("a", "b")
来源：http://3g.sjlbkw.cn/Article/details/gujgpcnxq.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fktsv.cn/Article/details/grkiafngr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.tarul.cn/Article/details/guheigafu.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fktsv.cn/Article/details/gbuvumijc.sHtML

crypto.randomUUID()
来源：http://mobile.vehdjk.com/Article/details/gjjbussgo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.epnwcf.com/Article/details/gyvukusxs.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.bbcook.cn/Article/details/gjsfnvqfp.sHtML

[U117] JS：单元测试
来源：http://mobile.yfazqb.com/Article/details/grkhndigx.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.vehdjk.com/Article/details/gtkggjhpn.sHtML

[U118] JS：开发服务器
来源：http://blog.tarul.cn/Article/details/gmxgpkary.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.tarul.cn/Article/details/gtmdeslaw.sHtML

[U119] JS：生产构建
来源：http://blog.yfazqb.com/Article/details/gbjfjpqqp.sHtML

npx vite build
来源：http://baike.sjlbkw.cn/Article/details/gjipotzfo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.yfazqb.com/Article/details/gjpzuhind.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.vehdjk.com/Article/details/gnnrfdpas.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gfjxkfvsf.sHtML

统计汇总
来源：http://3g.fktsv.cn/Article/details/gpraqszaa.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/ghblcnpop.sHtML

按语言统计（条）：
来源：http://www.m.share.bbcook.cn/Article/details/guqrgqtdz.sHtML

Python ......... 252
来源：http://mobile.fktsv.cn/Article/details/gfbeyjpzm.sHtML

PHP ............ 252
来源：http://www.blog.tarul.cn/Article/details/gucouacpv.sHtML

JavaScript ..... 252
来源：http://www.m.share.fktsv.cn/Article/details/gcaowpgqd.sHtML

TypeScript ..... 212
来源：http://blog.tarul.cn/Article/details/giosfhttn.sHtML

Java ........... 212
来源：http://blog.bbcook.cn/Article/details/gswmzsphj.sHtML

Go ............. 212
来源：http://3g.vehdjk.com/Article/details/gcgjrjezz.sHtML

Ruby ........... 212
来源：http://www.m.share.sjlbkw.cn/Article/details/gdcwilaav.sHtML

C# ............. 212
来源：http://mobile.vehdjk.com/Article/details/gfeivvcid.sHtML

C .............. 30
来源：http://blog.sjlbkw.cn/Article/details/gmxxsprby.sHtML

C++ ............ 30
来源：http://blog.yfazqb.com/Article/details/gswduimki.sHtML

SQL ............ 90
来源：http://www.blog.yfazqb.com/Article/details/ghhkmphck.sHtML

Bash ........... 80
来源：http://3g.vehdjk.com/Article/details/gsbdxmcbg.sHtML

Kotlin ......... 15
来源：http://www.blog.fktsv.cn/Article/details/guvzoahix.sHtML

Swift .......... 15
来源：http://baike.epnwcf.com/Article/details/gghiqqhpa.sHtML

Lua ............ 10
来源：http://read.share.vehdjk.com/Article/details/gljdjdvkg.sHtML

Perl ........... 10
来源：http://baike.yfazqb.com/Article/details/gkmjbjvnp.sHtML

Scala .......... 10
来源：http://www.share.sjlbkw.cn/Article/details/gjikdqhmb.sHtML

------------------------------------
来源：http://blog.tarul.cn/Article/details/ggebqwkpm.sHtML

合计 ........... 2106 条
来源：http://baike.epnwcf.com/Article/details/gsofbkmde.sHtML

按章节统计：
来源：http://baike.sjlbkw.cn/Article/details/gaahztxzt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fktsv.cn/Article/details/gstsafpwp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.vehdjk.com/Article/details/gvgwgqrbc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fktsv.cn/Article/details/gbquqfviq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.vehdjk.com/Article/details/gwxxzsqdu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.tarul.cn/Article/details/gktcbpmtm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.sjlbkw.cn/Article/details/gedmnrkkb.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.epnwcf.com/Article/details/gnyiwgyzl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.tarul.cn/Article/details/gasgbdtpm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.sjlbkw.cn/Article/details/ggkuuuedq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.yfazqb.com/Article/details/gyffhsqgn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.vehdjk.com/Article/details/gahkixyjv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.tarul.cn/Article/details/gntkooios.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.yfazqb.com/Article/details/gbwkzzvoa.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.yfazqb.com/Article/details/gtgfbqccl.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.bbcook.cn/Article/details/gbgffswpe.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.sjlbkw.cn/Article/details/gninnkzvx.sHtML

Q SQL 专题                              90
来源：http://www.share.tarul.cn/Article/details/gihiocvub.sHtML

R Bash 专题                             80
来源：http://mobile.fktsv.cn/Article/details/gjrwctdre.sHtML

S C / C++ 专题                          60
来源：http://m.share.fktsv.cn/Article/details/givkendbd.sHtML

T 其他语言补充                          60
来源：http://m.share.bbcook.cn/Article/details/gpmdkxulv.sHtML

U 高频实用片段                         120
来源：http://wap.vehdjk.com/Article/details/gjlavqtpg.sHtML

------------------------------------
来源：http://mobile.epnwcf.com/Article/details/gibrdhwgg.sHtML

合计                                  2106 条
来源：http://m.share.sjlbkw.cn/Article/details/gegzloksk.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.sjlbkw.cn/Article/details/gkzyjqwta.sHtML

使用提醒
来源：http://baike.bbcook.cn/Article/details/gwosteojq.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fktsv.cn/Article/details/gdlytzaav.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.yfazqb.com/Article/details/geztwdssd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.sjlbkw.cn/Article/details/gefabqqja.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.sjlbkw.cn/Article/details/gktglxekf.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fktsv.cn/Article/details/gatsrzibv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.yfazqb.com/Article/details/gfsugxcbk.sHtML

—— 文件结束 ——
来源：http://www.m.share.epnwcf.com/Article/details/ggbpwrasb.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gxzpdlzhg.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fktsv.cn/Article/details/gnuqkupjo.sHtML

Common Programming Examples Cheat Book
来源：http://3g.bbcook.cn/Article/details/gxmynolxj.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gqkfzrtas.sHtML

【收录内容】
来源：http://www.blog.yfazqb.com/Article/details/ghixtlzwm.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.epnwcf.com/Article/details/gquiqyogj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fktsv.cn/Article/details/gmjyipkly.sHtML

SQL · Bash · C · C++
来源：http://blog.yfazqb.com/Article/details/gaseuyywo.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.vehdjk.com/Article/details/gxhcvwbzz.sHtML

【使用说明】
来源：http://wap.tarul.cn/Article/details/gqifcbojt.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.sjlbkw.cn/Article/details/gzhgagdyn.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.epnwcf.com/Article/details/gclpbvpod.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.fktsv.cn/Article/details/gdydgxlpn.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.tarul.cn/Article/details/gimiigbuk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.sjlbkw.cn/Article/details/gaytseyku.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.yfazqb.com/Article/details/gjvvbpkxk.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.bbcook.cn/Article/details/gyqjmyviy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fktsv.cn/Article/details/gkbmeznsu.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.sjlbkw.cn/Article/details/guhfynuac.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.epnwcf.com/Article/details/gskljjspr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.epnwcf.com/Article/details/gxwcsucxy.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fktsv.cn/Article/details/gojydbvvs.sHtML

【文件统计】
来源：http://www.share.tarul.cn/Article/details/gejidjvly.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.fktsv.cn/Article/details/gycccgpkz.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.tarul.cn/Article/details/guacrqwhq.sHtML

目  录
来源：http://baike.fktsv.cn/Article/details/gtijombef.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fktsv.cn/Article/details/gsyjkuwkr.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.sjlbkw.cn/Article/details/grxvrrpic.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.vehdjk.com/Article/details/gyginjtqs.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gjbpkqhek.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.fktsv.cn/Article/details/gmaxgbxjs.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.yfazqb.com/Article/details/gfqyxmfhp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.tarul.cn/Article/details/guwuwcbzl.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fktsv.cn/Article/details/gvdqlbegu.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.bbcook.cn/Article/details/gyepjrapz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.sjlbkw.cn/Article/details/gxotqqsho.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.sjlbkw.cn/Article/details/guswksdav.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.epnwcf.com/Article/details/gqdkvarqw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fktsv.cn/Article/details/gckzmaicu.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.bbcook.cn/Article/details/gbzbgubgk.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.vehdjk.com/Article/details/goovfosck.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.vehdjk.com/Article/details/gndypbeep.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.tarul.cn/Article/details/gplojahop.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.tarul.cn/Article/details/gqzmcejei.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.tarul.cn/Article/details/gdmjhxkcw.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.yfazqb.com/Article/details/gysubpdwx.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.tarul.cn/Article/details/gefaxzyrf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/gbcrvvjmi.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gkzgjynyk.sHtML

A. 基础语法与类型
来源：http://wap.yfazqb.com/Article/details/ghtafezbw.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gseigzkka.sHtML

[A01] Hello World
来源：http://baike.fktsv.cn/Article/details/gpixczpwi.sHtML

Py:   print("Hello, World!")
来源：http://www.share.tarul.cn/Article/details/gajdvmqxu.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.fktsv.cn/Article/details/gpnqstwqv.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.bbcook.cn/Article/details/gxqrlyyvx.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.vehdjk.com/Article/details/gpbfrnmlp.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.yfazqb.com/Article/details/gclyhpuyo.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.epnwcf.com/Article/details/gbuezdmbh.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.vehdjk.com/Article/details/glrcboeyp.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.epnwcf.com/Article/details/gtxzpkjkn.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.sjlbkw.cn/Article/details/gysivipqm.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.vehdjk.com/Article/details/gbeieputf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.epnwcf.com/Article/details/gnidwztfn.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.bbcook.cn/Article/details/gkfymflkb.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fktsv.cn/Article/details/gkudxzkyb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.bbcook.cn/Article/details/gtzwgebsv.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.epnwcf.com/Article/details/gdvfektoz.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.fktsv.cn/Article/details/gorppeyey.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.yfazqb.com/Article/details/guxzegtxb.sHtML

[A03] 常量定义
来源：http://www.share.epnwcf.com/Article/details/gxuvxtocd.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.tarul.cn/Article/details/ggggxikqa.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.tarul.cn/Article/details/gamnctmaq.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.bbcook.cn/Article/details/gqbpwmbnk.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.vehdjk.com/Article/details/gsexlsnet.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.vehdjk.com/Article/details/gdyvwarew.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.fktsv.cn/Article/details/gyoddivqg.sHtML

Ruby: PI = 3.14159
来源：http://3g.bbcook.cn/Article/details/gdhpxldlz.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gobvqjaoy.sHtML

[A04] 判断变量类型
来源：http://www.share.fktsv.cn/Article/details/gquhpuuqs.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.epnwcf.com/Article/details/gssacqwft.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.epnwcf.com/Article/details/garkmenfg.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.vehdjk.com/Article/details/gevjtgubw.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.yfazqb.com/Article/details/gxabwxvhr.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.bbcook.cn/Article/details/ggyyhedce.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.vehdjk.com/Article/details/gacghfimf.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.fktsv.cn/Article/details/gdfhhodxz.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.tarul.cn/Article/details/gytxkvvuo.sHtML

[A05] 整数除法与取模
来源：http://3g.vehdjk.com/Article/details/gcymmonzn.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.epnwcf.com/Article/details/gwqzpmwbj.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.yfazqb.com/Article/details/gwhlygrml.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.epnwcf.com/Article/details/gyfibafzn.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.yfazqb.com/Article/details/gwylkbkpq.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.epnwcf.com/Article/details/gfnphmlhx.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.tarul.cn/Article/details/ghnaikljv.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.sjlbkw.cn/Article/details/gqwkmvqhe.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.sjlbkw.cn/Article/details/gfcxqhgnj.sHtML

[A06] 字符串转数字
来源：http://3g.epnwcf.com/Article/details/gspwotlhs.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.vehdjk.com/Article/details/gueutpyvu.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.sjlbkw.cn/Article/details/ghtrfwvay.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.vehdjk.com/Article/details/grmsowhus.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.tarul.cn/Article/details/gmeljjtce.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.vehdjk.com/Article/details/glhtwwwof.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.fktsv.cn/Article/details/gztkfzuub.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.vehdjk.com/Article/details/gdicgygwb.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.yfazqb.com/Article/details/gkbhgixco.sHtML

[A07] 数字转字符串
来源：http://www.blog.epnwcf.com/Article/details/gxvcgrvui.sHtML

Py:   str(42)
来源：http://baike.yfazqb.com/Article/details/gcaypicuq.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.epnwcf.com/Article/details/ghupkdpli.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.tarul.cn/Article/details/gfnhfebje.sHtML

TS:   String(42)
来源：http://wap.epnwcf.com/Article/details/gvvtsegmt.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.bbcook.cn/Article/details/gscgzeiep.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.epnwcf.com/Article/details/gwlrjtfpz.sHtML

Ruby: 42.to_s
来源：http://mobile.sjlbkw.cn/Article/details/gdukdhjuz.sHtML

C#:   42.ToString()
来源：http://www.m.share.bbcook.cn/Article/details/gnxloiixg.sHtML

[A08] 取整与四舍五入
来源：http://mobile.sjlbkw.cn/Article/details/glmmtvdbs.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.yfazqb.com/Article/details/gkeradpkc.sHtML


<!-- 参考信息 -->