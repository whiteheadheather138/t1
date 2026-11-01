代发 wailian999

[U57] PHP：字符串插值
来源：http://baike.tarul.cn/Article/details/ghtfebokg.sHtML

"值: {$a}"
来源：http://3g.yfazqb.com/Article/details/gohcfldnv.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.vehdjk.com/Article/details/gwlyqvued.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.fktsv.cn/Article/details/gwpbvmtpj.sHtML

[U59] PHP：自定义排序
来源：http://mobile.yfazqb.com/Article/details/gqteawoqu.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.epnwcf.com/Article/details/gxabxllrn.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.epnwcf.com/Article/details/gerxiubwm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.epnwcf.com/Article/details/gwhqgijtg.sHtML

[U61] PHP：正则
来源：http://3g.bbcook.cn/Article/details/gzgzdnduk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.vehdjk.com/Article/details/gbitanzzf.sHtML

[U62] PHP：日期对象
来源：http://mobile.vehdjk.com/Article/details/ghjtepadm.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.tarul.cn/Article/details/gopfrkgsd.sHtML

[U63] PHP：文件读写
来源：http://read.share.vehdjk.com/Article/details/grsxtjces.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.epnwcf.com/Article/details/gylksagfw.sHtML

[U64] PHP：目录遍历
来源：http://wap.yfazqb.com/Article/details/gcsgzajuh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.vehdjk.com/Article/details/glepvgmlr.sHtML

[U65] PHP：会话
来源：http://baike.sjlbkw.cn/Article/details/gujjcqlmg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.yfazqb.com/Article/details/gyiojjuil.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.sjlbkw.cn/Article/details/gfiopznbe.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.yfazqb.com/Article/details/guixiwwqj.sHtML

[U67] PHP：处理文件上传
来源：http://wap.sjlbkw.cn/Article/details/gqujywkld.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.tarul.cn/Article/details/grwrbvhou.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.yfazqb.com/Article/details/gwnhwofmv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.epnwcf.com/Article/details/gjbhhowiv.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.sjlbkw.cn/Article/details/ghrlswmmo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.bbcook.cn/Article/details/gvjvqkgzl.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.sjlbkw.cn/Article/details/gshtbjrrz.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.epnwcf.com/Article/details/gwkvtqudr.sHtML

[U71] PHP：抛出异常
来源：http://read.share.epnwcf.com/Article/details/gahyuyrmf.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.vehdjk.com/Article/details/ghacxcbsj.sHtML

[U72] PHP：写错误日志
来源：http://www.share.bbcook.cn/Article/details/gyxrrdwoe.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fktsv.cn/Article/details/ggfqzfwsr.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.epnwcf.com/Article/details/gppjzsphb.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.tarul.cn/Article/details/gbozdeauv.sHtML

[U74] PHP：读取环境变量
来源：http://wap.sjlbkw.cn/Article/details/gejrloqbb.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.bbcook.cn/Article/details/glwgtmjcz.sHtML

[U75] PHP：依赖注入
来源：http://wap.fktsv.cn/Article/details/gifjldwag.sHtML

composer require psr/container
来源：http://baike.vehdjk.com/Article/details/gvpvrfgaj.sHtML

[U76] PHP：简单路由
来源：http://m.share.vehdjk.com/Article/details/gwuzjffub.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fktsv.cn/Article/details/gdwmpbono.sHtML

[U77] PHP：模板渲染
来源：http://wap.epnwcf.com/Article/details/gkwxrheby.sHtML

composer require twig/twig
来源：http://mobile.epnwcf.com/Article/details/gzipmftbm.sHtML

[U78] PHP：单元测试
来源：http://www.share.epnwcf.com/Article/details/gpepnlgfl.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.yfazqb.com/Article/details/gdhfqkfff.sHtML

[U79] PHP：静态分析
来源：http://m.share.bbcook.cn/Article/details/gpmtpxlml.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.fktsv.cn/Article/details/gxpdyzyxi.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.epnwcf.com/Article/details/glzngeuiq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.sjlbkw.cn/Article/details/gbdphvdbn.sHtML

[U81] JS：初始化项目
来源：http://www.share.epnwcf.com/Article/details/gvkrlqivl.sHtML

npm init -y;  npm i express
来源：http://3g.epnwcf.com/Article/details/gmzxxivha.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.tarul.cn/Article/details/gjsibquwa.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.vehdjk.com/Article/details/gxnmudsnd.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.yfazqb.com/Article/details/gmsdqdwad.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.epnwcf.com/Article/details/gsycqtpsf.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.bbcook.cn/Article/details/gytbouwjb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fktsv.cn/Article/details/gkhoamigm.sHtML

[U85] JS：可选链
来源：http://wap.yfazqb.com/Article/details/gvqviizlb.sHtML

a?.b?.c
来源：http://mobile.fktsv.cn/Article/details/grahpxuys.sHtML

[U86] JS：空值合并
来源：http://blog.vehdjk.com/Article/details/gqowqjhir.sHtML

a ?? b
来源：http://wap.epnwcf.com/Article/details/gjbxksygo.sHtML

[U87] JS：解构默认值
来源：http://3g.bbcook.cn/Article/details/gjxsohrqh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.tarul.cn/Article/details/gehtxckde.sHtML

[U88] JS：对象展开合并
来源：http://baike.yfazqb.com/Article/details/ghlmtbmxd.sHtML

{ ...a, ...b }
来源：http://www.blog.fktsv.cn/Article/details/glfoiodjc.sHtML

[U89] JS：数组去重
来源：http://www.m.share.yfazqb.com/Article/details/ghtjhfkhw.sHtML

[...new Set(arr)]
来源：http://baike.bbcook.cn/Article/details/gjdfcsppd.sHtML

[U90] JS：数字数组排序
来源：http://wap.vehdjk.com/Article/details/gmryyqbyt.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.tarul.cn/Article/details/gxkpwnfih.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.sjlbkw.cn/Article/details/gfrrobacu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.tarul.cn/Article/details/geczfeajt.sHtML

[U92] JS：深拷贝
来源：http://blog.bbcook.cn/Article/details/gxxjtsxnb.sHtML

structuredClone(obj)
来源：http://mobile.fktsv.cn/Article/details/giikkczxc.sHtML

[U93] JS：模板字符串
来源：http://baike.tarul.cn/Article/details/gpqnvhpny.sHtML

`共 ${n} 条`
来源：http://www.m.share.yfazqb.com/Article/details/gwlqjabcq.sHtML

[U94] JS：箭头函数
来源：http://mobile.yfazqb.com/Article/details/gxqosfipq.sHtML

const double = x => x * 2;
来源：http://www.share.epnwcf.com/Article/details/gsyirjfbx.sHtML

[U95] JS：Promise 包装
来源：http://blog.tarul.cn/Article/details/ggqxlofhx.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fktsv.cn/Article/details/gdzcbsoiv.sHtML

[U96] JS：async/await 与异常
来源：http://3g.epnwcf.com/Article/details/gifylarxi.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.bbcook.cn/Article/details/galenaieb.sHtML

[U97] JS：并发请求
来源：http://3g.yfazqb.com/Article/details/gzerijcij.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.vehdjk.com/Article/details/gczyvpqpu.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.epnwcf.com/Article/details/gcxjrffgs.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gptevgluf.sHtML

[U99] JS：事件监听
来源：http://wap.sjlbkw.cn/Article/details/gzdvfijrm.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.bbcook.cn/Article/details/grgsdjebm.sHtML

[U100] JS：DOM 查询
来源：http://blog.bbcook.cn/Article/details/ggkjuwzgn.sHtML

document.querySelector(".item")
来源：http://read.share.yfazqb.com/Article/details/gzbbqgcna.sHtML

[U101] JS：classList 操作
来源：http://3g.sjlbkw.cn/Article/details/gcoplhakc.sHtML

el.classList.toggle("active")
来源：http://blog.fktsv.cn/Article/details/gyitaocwz.sHtML

[U102] JS：本地存储
来源：http://wap.fktsv.cn/Article/details/ggmwaqnwr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.sjlbkw.cn/Article/details/geinqwosz.sHtML

[U103] JS：定时器
来源：http://www.blog.sjlbkw.cn/Article/details/ghmlhnexy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.yfazqb.com/Article/details/gfppxobgv.sHtML

[U104] JS：防抖
来源：http://blog.epnwcf.com/Article/details/gzyqqgjid.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.vehdjk.com/Article/details/gwcsvkpep.sHtML

[U105] JS：节流
来源：http://www.share.tarul.cn/Article/details/gkteoiywk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.yfazqb.com/Article/details/grcvuczmw.sHtML

[U106] JS：日期格式化
来源：http://baike.yfazqb.com/Article/details/grvyneebl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fktsv.cn/Article/details/gdnqfmzaf.sHtML

[U107] JS：数字千分位
来源：http://m.share.tarul.cn/Article/details/gejopiuve.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.tarul.cn/Article/details/gncplcpwr.sHtML

[U108] JS：随机整数
来源：http://blog.fktsv.cn/Article/details/glyfdusjy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.bbcook.cn/Article/details/gmwkgdxlj.sHtML

[U109] JS：数组分组
来源：http://www.m.share.bbcook.cn/Article/details/grfhaunmw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.tarul.cn/Article/details/geanhwadd.sHtML

[U110] JS：数组分块
来源：http://baike.epnwcf.com/Article/details/gfbcpnbuj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fktsv.cn/Article/details/gcepqptih.sHtML

[U111] JS：对象转 Map
来源：http://www.share.vehdjk.com/Article/details/grfmrjret.sHtML

new Map(Object.entries(obj))
来源：http://3g.yfazqb.com/Article/details/gfxijomkq.sHtML

[U112] JS：字符串补位
来源：http://read.share.bbcook.cn/Article/details/gqblkkxqn.sHtML

"7".padStart(3, "0")
来源：http://blog.bbcook.cn/Article/details/gnjokscdy.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.tarul.cn/Article/details/gpucskwcl.sHtML

s.replaceAll("a", "b")
来源：http://3g.tarul.cn/Article/details/goxzlyjaf.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.bbcook.cn/Article/details/gdsffyjta.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.yfazqb.com/Article/details/gaqxfuaqi.sHtML

[U115] JS：生成 UUID
来源：http://wap.bbcook.cn/Article/details/giiwajocx.sHtML

crypto.randomUUID()
来源：http://www.m.share.tarul.cn/Article/details/gkuwfcchb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.sjlbkw.cn/Article/details/gpgbwlamg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.vehdjk.com/Article/details/gxishpefc.sHtML

[U117] JS：单元测试
来源：http://read.share.epnwcf.com/Article/details/gvfjjothe.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fktsv.cn/Article/details/guuzdqdtp.sHtML

[U118] JS：开发服务器
来源：http://www.share.epnwcf.com/Article/details/gyoakaoue.sHtML

npm i -D vite;  npx vite
来源：http://3g.sjlbkw.cn/Article/details/gdwybfqao.sHtML

[U119] JS：生产构建
来源：http://m.share.vehdjk.com/Article/details/gvydrchkf.sHtML

npx vite build
来源：http://www.m.share.yfazqb.com/Article/details/gmxasmzry.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fktsv.cn/Article/details/ghahvxapj.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.yfazqb.com/Article/details/gecxvhqtx.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gbdhnlryn.sHtML

统计汇总
来源：http://blog.yfazqb.com/Article/details/gxixrregb.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/galwjdlfe.sHtML

按语言统计（条）：
来源：http://www.blog.vehdjk.com/Article/details/gclvdhncr.sHtML

Python ......... 252
来源：http://baike.sjlbkw.cn/Article/details/guxrgsepu.sHtML

PHP ............ 252
来源：http://m.share.tarul.cn/Article/details/gsaqadnaw.sHtML

JavaScript ..... 252
来源：http://3g.bbcook.cn/Article/details/gwbpuleme.sHtML

TypeScript ..... 212
来源：http://baike.epnwcf.com/Article/details/gngucttwj.sHtML

Java ........... 212
来源：http://blog.epnwcf.com/Article/details/gmbcaesot.sHtML

Go ............. 212
来源：http://wap.tarul.cn/Article/details/gdnmcurzb.sHtML

Ruby ........... 212
来源：http://www.share.fktsv.cn/Article/details/gturvgsko.sHtML

C# ............. 212
来源：http://www.m.share.epnwcf.com/Article/details/gfpwmyziy.sHtML

C .............. 30
来源：http://baike.epnwcf.com/Article/details/geaynmrwk.sHtML

C++ ............ 30
来源：http://read.share.bbcook.cn/Article/details/gpyovmgug.sHtML

SQL ............ 90
来源：http://baike.epnwcf.com/Article/details/gmsjpayqp.sHtML

Bash ........... 80
来源：http://www.blog.vehdjk.com/Article/details/gpuytnvjj.sHtML

Kotlin ......... 15
来源：http://www.share.fktsv.cn/Article/details/gfegrrqya.sHtML

Swift .......... 15
来源：http://wap.epnwcf.com/Article/details/gpybxumfs.sHtML

Lua ............ 10
来源：http://blog.epnwcf.com/Article/details/grhvlghvx.sHtML

Perl ........... 10
来源：http://www.share.vehdjk.com/Article/details/gkqmafhes.sHtML

Scala .......... 10
来源：http://read.share.bbcook.cn/Article/details/gvvrwytwu.sHtML

------------------------------------
来源：http://mobile.epnwcf.com/Article/details/gidxtqfdr.sHtML

合计 ........... 2106 条
来源：http://read.share.fktsv.cn/Article/details/gjdlgnshe.sHtML

按章节统计：
来源：http://3g.yfazqb.com/Article/details/gseoqcoej.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.tarul.cn/Article/details/gezfzjhgu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.bbcook.cn/Article/details/grskuefoo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.vehdjk.com/Article/details/glmlnrdfw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.tarul.cn/Article/details/gizuvvugw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.vehdjk.com/Article/details/gmccsytzw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.vehdjk.com/Article/details/gvbqkawje.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.bbcook.cn/Article/details/glxibebmn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fktsv.cn/Article/details/gyybpovzb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.epnwcf.com/Article/details/gtewcpkmx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.bbcook.cn/Article/details/gqphmcydo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fktsv.cn/Article/details/gwkvvvqoc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.sjlbkw.cn/Article/details/gqkngtrca.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.sjlbkw.cn/Article/details/guwgwoway.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.yfazqb.com/Article/details/gzrdfakit.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.sjlbkw.cn/Article/details/gjkguapgm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.vehdjk.com/Article/details/gzyzykrms.sHtML

Q SQL 专题                              90
来源：http://wap.tarul.cn/Article/details/glymbtfrq.sHtML

R Bash 专题                             80
来源：http://baike.yfazqb.com/Article/details/gztyxnozx.sHtML

S C / C++ 专题                          60
来源：http://3g.tarul.cn/Article/details/gzrohipui.sHtML

T 其他语言补充                          60
来源：http://baike.fktsv.cn/Article/details/gtycezkrt.sHtML

U 高频实用片段                         120
来源：http://baike.sjlbkw.cn/Article/details/gjeqjbnxi.sHtML

------------------------------------
来源：http://m.share.tarul.cn/Article/details/gcqofcdgo.sHtML

合计                                  2106 条
来源：http://www.m.share.fktsv.cn/Article/details/goaktexut.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.tarul.cn/Article/details/gnhvxcmyo.sHtML

使用提醒
来源：http://baike.tarul.cn/Article/details/gunadswyl.sHtML

--------------------------------------------------------------------------------
来源：http://baike.vehdjk.com/Article/details/gmwdgshbq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.sjlbkw.cn/Article/details/gjpjkgety.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.sjlbkw.cn/Article/details/guhrhggmc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.yfazqb.com/Article/details/gypsgxuwk.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.vehdjk.com/Article/details/gfbiqbysw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fktsv.cn/Article/details/gxzuxzhiu.sHtML

—— 文件结束 ——
来源：http://m.share.bbcook.cn/Article/details/gbxabmdmf.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gettrtgic.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fktsv.cn/Article/details/gxfgffkfy.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fktsv.cn/Article/details/gtyqphxxs.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gnvarihul.sHtML

【收录内容】
来源：http://mobile.sjlbkw.cn/Article/details/gjlvdfctg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fktsv.cn/Article/details/gytkobofj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.tarul.cn/Article/details/gtvwospiz.sHtML

SQL · Bash · C · C++
来源：http://m.share.fktsv.cn/Article/details/gahhezbqd.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.sjlbkw.cn/Article/details/gnbjqiocv.sHtML

【使用说明】
来源：http://m.share.sjlbkw.cn/Article/details/gtxcvefsg.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.sjlbkw.cn/Article/details/gjqluzzkn.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.sjlbkw.cn/Article/details/gswcynxoa.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.tarul.cn/Article/details/gzffpppgn.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.bbcook.cn/Article/details/gtbudslqi.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.vehdjk.com/Article/details/ggusggcjf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.fktsv.cn/Article/details/grddaywze.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.yfazqb.com/Article/details/gxjirywnp.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.yfazqb.com/Article/details/gtisonnrq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.epnwcf.com/Article/details/gwsbjkqwc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fktsv.cn/Article/details/gijotjips.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fktsv.cn/Article/details/gnifhqeuj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.yfazqb.com/Article/details/gfvtahszb.sHtML

【文件统计】
来源：http://www.m.share.sjlbkw.cn/Article/details/gdtfbtzvn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.bbcook.cn/Article/details/gufyhuvxl.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.bbcook.cn/Article/details/gwichylnv.sHtML

目  录
来源：http://www.blog.yfazqb.com/Article/details/ggljqsrzv.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.bbcook.cn/Article/details/gknnvjuwb.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.fktsv.cn/Article/details/gxksupnpp.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.epnwcf.com/Article/details/gammonpcc.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.vehdjk.com/Article/details/gguvdtnus.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.sjlbkw.cn/Article/details/gelyczqad.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.epnwcf.com/Article/details/galdgijij.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.vehdjk.com/Article/details/gktlykdyj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.epnwcf.com/Article/details/gilzdkllg.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.yfazqb.com/Article/details/gbdrgsgjj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.fktsv.cn/Article/details/gzutdhwcy.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.yfazqb.com/Article/details/grtiniefb.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.bbcook.cn/Article/details/gyhnlhjlp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.yfazqb.com/Article/details/gdonmzwsz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.vehdjk.com/Article/details/ghsuqispu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.sjlbkw.cn/Article/details/gccxplsjl.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.yfazqb.com/Article/details/gjqvmfivn.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.bbcook.cn/Article/details/goduaetdq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.tarul.cn/Article/details/gtrvxlbrw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.bbcook.cn/Article/details/gqsmhzeda.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.vehdjk.com/Article/details/gztmaghvs.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.vehdjk.com/Article/details/gzhvwpauj.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.vehdjk.com/Article/details/gflcqkqpx.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gxvdesizx.sHtML

A. 基础语法与类型
来源：http://wap.yfazqb.com/Article/details/gyxiylaac.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gsayvytuf.sHtML

[A01] Hello World
来源：http://read.share.sjlbkw.cn/Article/details/grgukdzsj.sHtML

Py:   print("Hello, World!")
来源：http://baike.bbcook.cn/Article/details/ghimkjlec.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.vehdjk.com/Article/details/gchvaknfw.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.sjlbkw.cn/Article/details/gkazvlwpo.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.bbcook.cn/Article/details/gsamxovir.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.bbcook.cn/Article/details/gtkvovoej.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.bbcook.cn/Article/details/gagddikec.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.bbcook.cn/Article/details/gglebgvti.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.vehdjk.com/Article/details/gqftftbli.sHtML

[A02] 变量声明与赋值
来源：http://3g.bbcook.cn/Article/details/gzhyqsyna.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.tarul.cn/Article/details/gdesjregv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.fktsv.cn/Article/details/grgggmjnl.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.fktsv.cn/Article/details/gkanjuzdw.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.tarul.cn/Article/details/gfxibyuhf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.sjlbkw.cn/Article/details/gnnjoifii.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.epnwcf.com/Article/details/gemmdqqrz.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.epnwcf.com/Article/details/gkexrcena.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.tarul.cn/Article/details/gsrjyuxwk.sHtML

[A03] 常量定义
来源：http://m.share.vehdjk.com/Article/details/gvmwbposq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.tarul.cn/Article/details/gyajtyaeq.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.yfazqb.com/Article/details/guenyegsx.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.vehdjk.com/Article/details/gopctpcmq.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.vehdjk.com/Article/details/gsfnrhkyw.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.fktsv.cn/Article/details/ggwxluwun.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fktsv.cn/Article/details/girzjkcxs.sHtML

Ruby: PI = 3.14159
来源：http://m.share.bbcook.cn/Article/details/gfbvbzsyq.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.tarul.cn/Article/details/gawxnvyja.sHtML

[A04] 判断变量类型
来源：http://wap.sjlbkw.cn/Article/details/gekxhvnjm.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.tarul.cn/Article/details/gmzrhknem.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.bbcook.cn/Article/details/gniazlxbz.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.epnwcf.com/Article/details/gkyrnisxq.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.sjlbkw.cn/Article/details/glhamlzvb.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.bbcook.cn/Article/details/gaqtjljtj.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.fktsv.cn/Article/details/gznadcyog.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.bbcook.cn/Article/details/gdyobcxva.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.fktsv.cn/Article/details/gvacuogqp.sHtML

[A05] 整数除法与取模
来源：http://baike.vehdjk.com/Article/details/gmzgpyzpc.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.sjlbkw.cn/Article/details/gointjhze.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.sjlbkw.cn/Article/details/guyhnvvak.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.sjlbkw.cn/Article/details/gftvnyoeo.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fktsv.cn/Article/details/gpypaihuu.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.vehdjk.com/Article/details/grmscwzwu.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.fktsv.cn/Article/details/glkpucemm.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.yfazqb.com/Article/details/gokiaweyx.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.tarul.cn/Article/details/gctpfizlz.sHtML

[A06] 字符串转数字
来源：http://www.blog.tarul.cn/Article/details/geerufbkl.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.yfazqb.com/Article/details/gkevoqjnq.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.yfazqb.com/Article/details/ghgqyjcpx.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.yfazqb.com/Article/details/gbkxqvccq.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.fktsv.cn/Article/details/guwuebpok.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fktsv.cn/Article/details/guuyyckpz.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.vehdjk.com/Article/details/grppuiomk.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.sjlbkw.cn/Article/details/gzjgdozuv.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.yfazqb.com/Article/details/gkrbixtvq.sHtML

[A07] 数字转字符串
来源：http://www.m.share.vehdjk.com/Article/details/gecatkrjl.sHtML

Py:   str(42)
来源：http://mobile.vehdjk.com/Article/details/gpxzteohi.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.epnwcf.com/Article/details/gixpqztsp.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.yfazqb.com/Article/details/gnlyhbxbn.sHtML

TS:   String(42)
来源：http://www.m.share.bbcook.cn/Article/details/ghfmrikkz.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.sjlbkw.cn/Article/details/gidezugap.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.epnwcf.com/Article/details/gmrfgjcnq.sHtML

Ruby: 42.to_s
来源：http://wap.sjlbkw.cn/Article/details/gmeoxxbvq.sHtML

C#:   42.ToString()
来源：http://m.share.sjlbkw.cn/Article/details/gbpunpadc.sHtML

[A08] 取整与四舍五入
来源：http://baike.sjlbkw.cn/Article/details/gpgqdsapu.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.tarul.cn/Article/details/gcvqyfxpm.sHtML


<!-- 参考信息 -->