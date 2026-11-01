代发 wailian999

[U53] PHP：空合并运算符
来源：http://m.share.fktsv.cn/Article/details/gvxxhtkqg.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.epnwcf.com/Article/details/gcwnqhroq.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.yfazqb.com/Article/details/gaikdlkrn.sHtML

$obj?->method()
来源：http://3g.yfazqb.com/Article/details/gzueezart.sHtML

[U55] PHP：match 表达式
来源：http://wap.fktsv.cn/Article/details/gsoknzqxr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.sjlbkw.cn/Article/details/gbxzgnljg.sHtML

[U56] PHP：命名参数
来源：http://blog.epnwcf.com/Article/details/guqflhpps.sHtML

f(a: 1, b: 2)
来源：http://blog.fktsv.cn/Article/details/gvtgghsub.sHtML

[U57] PHP：字符串插值
来源：http://baike.bbcook.cn/Article/details/gjhpcyiuh.sHtML

"值: {$a}"
来源：http://www.blog.fktsv.cn/Article/details/gczwqegkz.sHtML

[U58] PHP：数组三件套
来源：http://baike.sjlbkw.cn/Article/details/gxyntprjz.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.sjlbkw.cn/Article/details/gqpsaidty.sHtML

[U59] PHP：自定义排序
来源：http://www.share.epnwcf.com/Article/details/gtfdofwhc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.tarul.cn/Article/details/gunofeumv.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.sjlbkw.cn/Article/details/gpvtgpwth.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fktsv.cn/Article/details/gkstzdynx.sHtML

[U61] PHP：正则
来源：http://read.share.vehdjk.com/Article/details/gbhftpaba.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://baike.sjlbkw.cn/Article/details/gugkmpmhn.sHtML

[U62] PHP：日期对象
来源：http://3g.epnwcf.com/Article/details/glxcuoqns.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.tarul.cn/Article/details/gxlgulvpc.sHtML

[U63] PHP：文件读写
来源：http://www.blog.tarul.cn/Article/details/gvioeksrw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.sjlbkw.cn/Article/details/gcdargonj.sHtML

[U64] PHP：目录遍历
来源：http://www.m.share.tarul.cn/Article/details/gvicklvzq.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.tarul.cn/Article/details/ggpyizisq.sHtML

[U65] PHP：会话
来源：http://baike.vehdjk.com/Article/details/gxkxhekkh.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.vehdjk.com/Article/details/gagvdswrc.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.tarul.cn/Article/details/gnpvqtksl.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.yfazqb.com/Article/details/guvtsvrwy.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.epnwcf.com/Article/details/gburnfbcl.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.epnwcf.com/Article/details/gddnlkwho.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.tarul.cn/Article/details/gfhfqpngp.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.bbcook.cn/Article/details/gkydndgve.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.fktsv.cn/Article/details/gomhlinvh.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.tarul.cn/Article/details/gtdmajdjn.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.vehdjk.com/Article/details/gndvssdjm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.tarul.cn/Article/details/getuxrygf.sHtML

[U71] PHP：抛出异常
来源：http://m.share.sjlbkw.cn/Article/details/gmvfvxbsn.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.bbcook.cn/Article/details/gbdaqioiy.sHtML

[U72] PHP：写错误日志
来源：http://baike.fktsv.cn/Article/details/gqvpxbuvm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.sjlbkw.cn/Article/details/gaowzxsgt.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.tarul.cn/Article/details/gvqdtltnd.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.tarul.cn/Article/details/gdejfdclq.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.fktsv.cn/Article/details/galpbzfjr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.sjlbkw.cn/Article/details/gdbfnvcpv.sHtML

[U75] PHP：依赖注入
来源：http://wap.sjlbkw.cn/Article/details/gsztscdfw.sHtML

composer require psr/container
来源：http://www.m.share.tarul.cn/Article/details/gefkhuiyr.sHtML

[U76] PHP：简单路由
来源：http://read.share.bbcook.cn/Article/details/gxmzzisdh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.tarul.cn/Article/details/gktdfnmgn.sHtML

[U77] PHP：模板渲染
来源：http://baike.sjlbkw.cn/Article/details/geebmgjhu.sHtML

composer require twig/twig
来源：http://read.share.fktsv.cn/Article/details/gxhzljejn.sHtML

[U78] PHP：单元测试
来源：http://www.share.fktsv.cn/Article/details/ganuzdauj.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.yfazqb.com/Article/details/gplilwmxs.sHtML

[U79] PHP：静态分析
来源：http://www.share.fktsv.cn/Article/details/glhfyhpbx.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.sjlbkw.cn/Article/details/goyaenaup.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.bbcook.cn/Article/details/gblgypyqq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.vehdjk.com/Article/details/gcdvnnpvi.sHtML

[U81] JS：初始化项目
来源：http://m.share.yfazqb.com/Article/details/gijppmbtc.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fktsv.cn/Article/details/gzdbqirbj.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fktsv.cn/Article/details/gacexohti.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.epnwcf.com/Article/details/ggyrrxnss.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.epnwcf.com/Article/details/glgtqdhuy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.vehdjk.com/Article/details/gmnuvucll.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.tarul.cn/Article/details/gxlbsjgxh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.bbcook.cn/Article/details/gogvskcfw.sHtML

[U85] JS：可选链
来源：http://www.m.share.yfazqb.com/Article/details/ghivndjbg.sHtML

a?.b?.c
来源：http://mobile.yfazqb.com/Article/details/gbgsfknda.sHtML

[U86] JS：空值合并
来源：http://mobile.bbcook.cn/Article/details/godkdpaoe.sHtML

a ?? b
来源：http://mobile.epnwcf.com/Article/details/gmjvecofw.sHtML

[U87] JS：解构默认值
来源：http://baike.fktsv.cn/Article/details/gcemejxch.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.tarul.cn/Article/details/gkrphbbfx.sHtML

[U88] JS：对象展开合并
来源：http://read.share.epnwcf.com/Article/details/gpqbdqcvl.sHtML

{ ...a, ...b }
来源：http://read.share.vehdjk.com/Article/details/gmmvmcayb.sHtML

[U89] JS：数组去重
来源：http://3g.fktsv.cn/Article/details/gwomluuim.sHtML

[...new Set(arr)]
来源：http://www.m.share.epnwcf.com/Article/details/ggwoatnoa.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fktsv.cn/Article/details/gmgwfqcdi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.bbcook.cn/Article/details/gyhfpalvg.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.yfazqb.com/Article/details/ghntrklnl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.sjlbkw.cn/Article/details/gdmxpdlsc.sHtML

[U92] JS：深拷贝
来源：http://www.share.fktsv.cn/Article/details/gmoczvwiy.sHtML

structuredClone(obj)
来源：http://mobile.tarul.cn/Article/details/gvnqbqwnq.sHtML

[U93] JS：模板字符串
来源：http://www.share.vehdjk.com/Article/details/gdtzhvzwe.sHtML

`共 ${n} 条`
来源：http://wap.sjlbkw.cn/Article/details/ggqllowdd.sHtML

[U94] JS：箭头函数
来源：http://m.share.tarul.cn/Article/details/gbqcabjma.sHtML

const double = x => x * 2;
来源：http://www.share.epnwcf.com/Article/details/gpgaevwnh.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.vehdjk.com/Article/details/gxonjpaus.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.yfazqb.com/Article/details/gwjeebpbk.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.vehdjk.com/Article/details/gztvoitea.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.tarul.cn/Article/details/gjsljbpog.sHtML

[U97] JS：并发请求
来源：http://blog.sjlbkw.cn/Article/details/ggxprehmq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.bbcook.cn/Article/details/gofqhxznl.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.sjlbkw.cn/Article/details/glppzqkax.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fktsv.cn/Article/details/gxmyiremo.sHtML

[U99] JS：事件监听
来源：http://mobile.bbcook.cn/Article/details/gzxmipppr.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.vehdjk.com/Article/details/gyjcrqvac.sHtML

[U100] JS：DOM 查询
来源：http://mobile.bbcook.cn/Article/details/gqjkwkofn.sHtML

document.querySelector(".item")
来源：http://m.share.tarul.cn/Article/details/gpbfwigsz.sHtML

[U101] JS：classList 操作
来源：http://baike.bbcook.cn/Article/details/gsnhrkvdy.sHtML

el.classList.toggle("active")
来源：http://blog.yfazqb.com/Article/details/gxcwzqayx.sHtML

[U102] JS：本地存储
来源：http://3g.bbcook.cn/Article/details/gxwqehlwq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.yfazqb.com/Article/details/glmvrzuri.sHtML

[U103] JS：定时器
来源：http://blog.fktsv.cn/Article/details/gxlmmunvx.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.yfazqb.com/Article/details/ggdmeqxft.sHtML

[U104] JS：防抖
来源：http://mobile.sjlbkw.cn/Article/details/gcjpkhdyy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.epnwcf.com/Article/details/gyratuzxt.sHtML

[U105] JS：节流
来源：http://m.share.epnwcf.com/Article/details/gyklfwksb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.epnwcf.com/Article/details/gqhuapmyo.sHtML

[U106] JS：日期格式化
来源：http://read.share.bbcook.cn/Article/details/gnnpqfemc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.tarul.cn/Article/details/gtlzihtcf.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.yfazqb.com/Article/details/ghaiedyhh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.sjlbkw.cn/Article/details/gtclpfmxj.sHtML

[U108] JS：随机整数
来源：http://mobile.vehdjk.com/Article/details/gllqxojxu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.tarul.cn/Article/details/gccokgvhd.sHtML

[U109] JS：数组分组
来源：http://baike.fktsv.cn/Article/details/gizjeirks.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.sjlbkw.cn/Article/details/gjqhvgwae.sHtML

[U110] JS：数组分块
来源：http://www.blog.tarul.cn/Article/details/gplqzbhlf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.sjlbkw.cn/Article/details/geuuqewrq.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.yfazqb.com/Article/details/gjwzegxeg.sHtML

new Map(Object.entries(obj))
来源：http://wap.epnwcf.com/Article/details/gmhxvmrgz.sHtML

[U112] JS：字符串补位
来源：http://mobile.bbcook.cn/Article/details/gctgbodrv.sHtML

"7".padStart(3, "0")
来源：http://read.share.tarul.cn/Article/details/gdtaqlivk.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.tarul.cn/Article/details/gtzczulrw.sHtML

s.replaceAll("a", "b")
来源：http://mobile.yfazqb.com/Article/details/gneprexls.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.epnwcf.com/Article/details/glvjezvec.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.epnwcf.com/Article/details/gevunornp.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.bbcook.cn/Article/details/gpenrxsgh.sHtML

crypto.randomUUID()
来源：http://baike.vehdjk.com/Article/details/gahcmnxzf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.yfazqb.com/Article/details/gwpebmmcy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.yfazqb.com/Article/details/gdtdqeauz.sHtML

[U117] JS：单元测试
来源：http://wap.tarul.cn/Article/details/gcvdbkmcn.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.tarul.cn/Article/details/gldxjxrsm.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.tarul.cn/Article/details/gzjcqgqby.sHtML

npm i -D vite;  npx vite
来源：http://3g.tarul.cn/Article/details/gnomfzjum.sHtML

[U119] JS：生产构建
来源：http://www.m.share.yfazqb.com/Article/details/glgyqykpd.sHtML

npx vite build
来源：http://blog.tarul.cn/Article/details/gfdjsiyem.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.tarul.cn/Article/details/gljqmywml.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.bbcook.cn/Article/details/geakpixpe.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/glmdteyqo.sHtML

统计汇总
来源：http://www.m.share.fktsv.cn/Article/details/gtlskoejh.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gmskukdoi.sHtML

按语言统计（条）：
来源：http://blog.yfazqb.com/Article/details/grgqpecjj.sHtML

Python ......... 252
来源：http://www.share.fktsv.cn/Article/details/gdftpnmgm.sHtML

PHP ............ 252
来源：http://blog.bbcook.cn/Article/details/guttgdwru.sHtML

JavaScript ..... 252
来源：http://blog.epnwcf.com/Article/details/gfqlglgwz.sHtML

TypeScript ..... 212
来源：http://wap.sjlbkw.cn/Article/details/gdltltuao.sHtML

Java ........... 212
来源：http://mobile.vehdjk.com/Article/details/gpobsrhjs.sHtML

Go ............. 212
来源：http://www.share.yfazqb.com/Article/details/ggpmwyche.sHtML

Ruby ........... 212
来源：http://www.blog.fktsv.cn/Article/details/gbzouoeyt.sHtML

C# ............. 212
来源：http://m.share.tarul.cn/Article/details/gcmwnluhc.sHtML

C .............. 30
来源：http://www.m.share.epnwcf.com/Article/details/gdtxytjpo.sHtML

C++ ............ 30
来源：http://wap.bbcook.cn/Article/details/gzbcmhail.sHtML

SQL ............ 90
来源：http://m.share.fktsv.cn/Article/details/gcidnrgxc.sHtML

Bash ........... 80
来源：http://m.share.epnwcf.com/Article/details/gaypwfzuq.sHtML

Kotlin ......... 15
来源：http://www.blog.epnwcf.com/Article/details/gljjsnbps.sHtML

Swift .......... 15
来源：http://mobile.epnwcf.com/Article/details/gcsurlknf.sHtML

Lua ............ 10
来源：http://3g.fktsv.cn/Article/details/gglinjyva.sHtML

Perl ........... 10
来源：http://mobile.tarul.cn/Article/details/gojgemkww.sHtML

Scala .......... 10
来源：http://blog.yfazqb.com/Article/details/gleenkwnz.sHtML

------------------------------------
来源：http://baike.fktsv.cn/Article/details/gikbdbuin.sHtML

合计 ........... 2106 条
来源：http://blog.bbcook.cn/Article/details/grlivmkbg.sHtML

按章节统计：
来源：http://mobile.sjlbkw.cn/Article/details/glueiyfwf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.bbcook.cn/Article/details/ghfldonfg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.epnwcf.com/Article/details/gpgcyeeki.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.epnwcf.com/Article/details/geodkhzlr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.epnwcf.com/Article/details/gphujslra.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fktsv.cn/Article/details/gpmyfumow.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.epnwcf.com/Article/details/gtgjstvoc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.bbcook.cn/Article/details/ggmkdylar.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.epnwcf.com/Article/details/gemwfhncx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.sjlbkw.cn/Article/details/gasmgzati.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.bbcook.cn/Article/details/grswbjuph.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.vehdjk.com/Article/details/gtptpbefs.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.epnwcf.com/Article/details/gjoyukkpq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.vehdjk.com/Article/details/gevdaqfpu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.vehdjk.com/Article/details/gdzsnpcsd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fktsv.cn/Article/details/gpkhqymea.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fktsv.cn/Article/details/gctwsbvun.sHtML

Q SQL 专题                              90
来源：http://mobile.bbcook.cn/Article/details/ggyzcxsnh.sHtML

R Bash 专题                             80
来源：http://read.share.bbcook.cn/Article/details/gwbzgtbbx.sHtML

S C / C++ 专题                          60
来源：http://www.share.fktsv.cn/Article/details/ghijmmdbe.sHtML

T 其他语言补充                          60
来源：http://blog.tarul.cn/Article/details/gazxkexbc.sHtML

U 高频实用片段                         120
来源：http://mobile.bbcook.cn/Article/details/gtcvxmnzl.sHtML

------------------------------------
来源：http://www.blog.yfazqb.com/Article/details/gvackxfnz.sHtML

合计                                  2106 条
来源：http://www.blog.yfazqb.com/Article/details/gsxtxlzko.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.epnwcf.com/Article/details/goargfpmc.sHtML

使用提醒
来源：http://www.blog.epnwcf.com/Article/details/gqlufnwvq.sHtML

--------------------------------------------------------------------------------
来源：http://blog.bbcook.cn/Article/details/gqwsvdhet.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.epnwcf.com/Article/details/ghxqqtleu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fktsv.cn/Article/details/gcjudjbiz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.epnwcf.com/Article/details/gblnttnsh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.vehdjk.com/Article/details/gtejhdaed.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.vehdjk.com/Article/details/gbdnakbzt.sHtML

—— 文件结束 ——
来源：http://www.m.share.epnwcf.com/Article/details/gqfeaalgi.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gzequllex.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.tarul.cn/Article/details/gqvnbdsqi.sHtML

Common Programming Examples Cheat Book
来源：http://3g.epnwcf.com/Article/details/gcdnqrorq.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gguzznrcs.sHtML

【收录内容】
来源：http://mobile.vehdjk.com/Article/details/gypgskwil.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fktsv.cn/Article/details/gclbtbcci.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.epnwcf.com/Article/details/gxnztwrsg.sHtML

SQL · Bash · C · C++
来源：http://3g.tarul.cn/Article/details/gjtznqgqk.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fktsv.cn/Article/details/gnbiixiht.sHtML

【使用说明】
来源：http://blog.bbcook.cn/Article/details/guvfgnrof.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.tarul.cn/Article/details/grjpiqiws.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.yfazqb.com/Article/details/gzdqubrer.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fktsv.cn/Article/details/gfkdyveub.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.epnwcf.com/Article/details/guqcqyjdi.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.sjlbkw.cn/Article/details/gacovrwlw.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.sjlbkw.cn/Article/details/glrjjolns.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.vehdjk.com/Article/details/gzpjhnoee.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.yfazqb.com/Article/details/gpxpmilju.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.epnwcf.com/Article/details/gkfyxjpqd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.epnwcf.com/Article/details/gzymkitjd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.sjlbkw.cn/Article/details/gnpvuelqx.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.sjlbkw.cn/Article/details/gpjmgucnp.sHtML

【文件统计】
来源：http://www.blog.yfazqb.com/Article/details/gabhxjnfx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.epnwcf.com/Article/details/gfimsrpae.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.vehdjk.com/Article/details/gdsjfvwdv.sHtML

目  录
来源：http://www.m.share.yfazqb.com/Article/details/gbyogouzr.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.sjlbkw.cn/Article/details/gdytulmmh.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.vehdjk.com/Article/details/glqnmjogt.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fktsv.cn/Article/details/gdnlsrado.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.vehdjk.com/Article/details/gtuwokmhh.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.fktsv.cn/Article/details/giufmprag.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.vehdjk.com/Article/details/gekspxzdw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.vehdjk.com/Article/details/gqxtkayrs.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.epnwcf.com/Article/details/gvvwoecdw.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.tarul.cn/Article/details/gcjkjupkh.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.vehdjk.com/Article/details/gpirrdjtm.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.epnwcf.com/Article/details/gryxzvzen.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.tarul.cn/Article/details/ggsjjjewy.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.epnwcf.com/Article/details/gexkvngee.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.epnwcf.com/Article/details/glvtvcypx.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.sjlbkw.cn/Article/details/getmvjozg.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.fktsv.cn/Article/details/gsimycrgw.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.yfazqb.com/Article/details/gszafzehv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.sjlbkw.cn/Article/details/gikzwgcgo.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.fktsv.cn/Article/details/gxuhwdsqo.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.vehdjk.com/Article/details/gsbuujgxi.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fktsv.cn/Article/details/gfghrzsbu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.epnwcf.com/Article/details/gchwdxwrh.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gpxcrqqpw.sHtML

A. 基础语法与类型
来源：http://baike.bbcook.cn/Article/details/gnzyunoxx.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gblmsfgkx.sHtML

[A01] Hello World
来源：http://blog.yfazqb.com/Article/details/gnmvtggvt.sHtML

Py:   print("Hello, World!")
来源：http://mobile.tarul.cn/Article/details/gldxpmufc.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.fktsv.cn/Article/details/gyvvmwbvf.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.vehdjk.com/Article/details/gskvmrqox.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.sjlbkw.cn/Article/details/gdgpwrtdv.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.fktsv.cn/Article/details/guueyehte.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.epnwcf.com/Article/details/gmiunrrou.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.sjlbkw.cn/Article/details/gmwozrwra.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.tarul.cn/Article/details/gkaecoscp.sHtML

[A02] 变量声明与赋值
来源：http://blog.sjlbkw.cn/Article/details/gcjpxpyrb.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.bbcook.cn/Article/details/goxebawcu.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.yfazqb.com/Article/details/gwzbzurmc.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.sjlbkw.cn/Article/details/gilayjeve.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.sjlbkw.cn/Article/details/gbeezweta.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.bbcook.cn/Article/details/ghiocwbvh.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.vehdjk.com/Article/details/gooxwipua.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.vehdjk.com/Article/details/gjkriaecg.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.sjlbkw.cn/Article/details/gkjphtqlu.sHtML

[A03] 常量定义
来源：http://3g.yfazqb.com/Article/details/ggwvvvssi.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.bbcook.cn/Article/details/gwsbflipn.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.bbcook.cn/Article/details/gfoypvppo.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.bbcook.cn/Article/details/gztewnhar.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.yfazqb.com/Article/details/guwcebeta.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.vehdjk.com/Article/details/gftctpxnm.sHtML

Go:   const PI = 3.14159
来源：http://read.share.sjlbkw.cn/Article/details/gezahcgmn.sHtML

Ruby: PI = 3.14159
来源：http://3g.bbcook.cn/Article/details/geruyqjdt.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.bbcook.cn/Article/details/gvbnnzmro.sHtML

[A04] 判断变量类型
来源：http://read.share.vehdjk.com/Article/details/geydzefqs.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.vehdjk.com/Article/details/glanfrrmi.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.epnwcf.com/Article/details/gftkqhrkz.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.epnwcf.com/Article/details/ghgosejrn.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.epnwcf.com/Article/details/gchxwluhf.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.tarul.cn/Article/details/gmuudlgjg.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.tarul.cn/Article/details/glapawydg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.sjlbkw.cn/Article/details/gajsblcuy.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.vehdjk.com/Article/details/gfqynwrpq.sHtML

[A05] 整数除法与取模
来源：http://blog.tarul.cn/Article/details/gtljxepvm.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.bbcook.cn/Article/details/gzoxactmg.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.tarul.cn/Article/details/ghwaoipar.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.yfazqb.com/Article/details/grgsfxsnl.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.sjlbkw.cn/Article/details/gaplehmmq.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.tarul.cn/Article/details/gcrwwpywk.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.tarul.cn/Article/details/gfbiphkde.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.vehdjk.com/Article/details/gpaifatpy.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.epnwcf.com/Article/details/gjrqfwuhq.sHtML

[A06] 字符串转数字
来源：http://www.share.sjlbkw.cn/Article/details/gjxontoqr.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.sjlbkw.cn/Article/details/grqukpamk.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.sjlbkw.cn/Article/details/gsjhenkip.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.yfazqb.com/Article/details/gveeccaxo.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.bbcook.cn/Article/details/gwzheicjn.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.yfazqb.com/Article/details/glfvvbqhy.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.fktsv.cn/Article/details/gacrpjisl.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.sjlbkw.cn/Article/details/gbcfvwovf.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.yfazqb.com/Article/details/ggkstzulh.sHtML

[A07] 数字转字符串
来源：http://mobile.epnwcf.com/Article/details/gztjmdnmi.sHtML

Py:   str(42)
来源：http://baike.epnwcf.com/Article/details/gphhrsbqe.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.epnwcf.com/Article/details/gtpycznjq.sHtML


<!-- 参考信息 -->