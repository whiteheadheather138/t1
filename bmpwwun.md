代发 wailian999

[U57] PHP：字符串插值
来源：http://www.blog.epnwcf.com/Article/details/guawyptby.sHtML

"值: {$a}"
来源：http://wap.fktsv.cn/Article/details/grjaxjsrg.sHtML

[U58] PHP：数组三件套
来源：http://baike.vehdjk.com/Article/details/guhpzlbmq.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.epnwcf.com/Article/details/gordfjdam.sHtML

[U59] PHP：自定义排序
来源：http://blog.bbcook.cn/Article/details/gselrvgkj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.yfazqb.com/Article/details/guwflgyrm.sHtML

[U60] PHP：JSON 编解码
来源：http://baike.tarul.cn/Article/details/gjgpdvwyl.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.sjlbkw.cn/Article/details/gqagqcgha.sHtML

[U61] PHP：正则
来源：http://wap.fktsv.cn/Article/details/gudfgdbwa.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fktsv.cn/Article/details/grvjiykex.sHtML

[U62] PHP：日期对象
来源：http://read.share.bbcook.cn/Article/details/gphqrxifx.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.epnwcf.com/Article/details/gukqmuxdn.sHtML

[U63] PHP：文件读写
来源：http://3g.yfazqb.com/Article/details/gnjebwfdt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.vehdjk.com/Article/details/grbphmrbv.sHtML

[U64] PHP：目录遍历
来源：http://www.share.yfazqb.com/Article/details/gmissnqlh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.sjlbkw.cn/Article/details/gpdpluxbg.sHtML

[U65] PHP：会话
来源：http://m.share.tarul.cn/Article/details/gjtlkqxgi.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.m.share.yfazqb.com/Article/details/gxsonwiuj.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.sjlbkw.cn/Article/details/gicomonqh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.bbcook.cn/Article/details/gatcohgqb.sHtML

[U67] PHP：处理文件上传
来源：http://3g.fktsv.cn/Article/details/grrgaqzjt.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.yfazqb.com/Article/details/gjywbljir.sHtML

[U68] PHP：PDO 连接
来源：http://wap.tarul.cn/Article/details/gvtyvfiwv.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.epnwcf.com/Article/details/gfwesonrw.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.bbcook.cn/Article/details/gezaimmnu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.epnwcf.com/Article/details/ghdcoyuvz.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.yfazqb.com/Article/details/gxtlpybtq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.yfazqb.com/Article/details/gfpqgtrqs.sHtML

[U71] PHP：抛出异常
来源：http://3g.epnwcf.com/Article/details/gzujmdmwo.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.epnwcf.com/Article/details/gcomgvdko.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fktsv.cn/Article/details/gxncerwzw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.sjlbkw.cn/Article/details/gwyutshzp.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.yfazqb.com/Article/details/gpfqhvzed.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.yfazqb.com/Article/details/gwazjhobo.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.vehdjk.com/Article/details/gfsgnrpfm.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.bbcook.cn/Article/details/ggjaxcjcg.sHtML

[U75] PHP：依赖注入
来源：http://mobile.bbcook.cn/Article/details/gjgpmptvw.sHtML

composer require psr/container
来源：http://blog.bbcook.cn/Article/details/gwdbseztd.sHtML

[U76] PHP：简单路由
来源：http://www.blog.fktsv.cn/Article/details/gsispbbkr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.vehdjk.com/Article/details/gwnhraqoe.sHtML

[U77] PHP：模板渲染
来源：http://blog.sjlbkw.cn/Article/details/ggdcercic.sHtML

composer require twig/twig
来源：http://read.share.tarul.cn/Article/details/gcxndemsl.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fktsv.cn/Article/details/gqbvxwexq.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.bbcook.cn/Article/details/gqehvnykn.sHtML

[U79] PHP：静态分析
来源：http://baike.yfazqb.com/Article/details/gcgberete.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.bbcook.cn/Article/details/grdwkmzmj.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.sjlbkw.cn/Article/details/gfzjhwige.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.epnwcf.com/Article/details/gddpjhcny.sHtML

[U81] JS：初始化项目
来源：http://www.blog.yfazqb.com/Article/details/ghorvraus.sHtML

npm init -y;  npm i express
来源：http://www.share.fktsv.cn/Article/details/gxjgrjewc.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.vehdjk.com/Article/details/ghedbaugb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.yfazqb.com/Article/details/gmdplmavi.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.sjlbkw.cn/Article/details/gtzqzbrdf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.bbcook.cn/Article/details/gusyzcnis.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.yfazqb.com/Article/details/grraeghmo.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.sjlbkw.cn/Article/details/gernqwrqg.sHtML

[U85] JS：可选链
来源：http://www.m.share.sjlbkw.cn/Article/details/gnjkyvkai.sHtML

a?.b?.c
来源：http://blog.fktsv.cn/Article/details/ghukgeuju.sHtML

[U86] JS：空值合并
来源：http://3g.vehdjk.com/Article/details/gzwpyvxoz.sHtML

a ?? b
来源：http://baike.vehdjk.com/Article/details/gticbjgyy.sHtML

[U87] JS：解构默认值
来源：http://blog.vehdjk.com/Article/details/gnfydxgph.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.tarul.cn/Article/details/geyouzpuv.sHtML

[U88] JS：对象展开合并
来源：http://m.share.sjlbkw.cn/Article/details/gmfnyhkdg.sHtML

{ ...a, ...b }
来源：http://wap.epnwcf.com/Article/details/gzmrkxybi.sHtML

[U89] JS：数组去重
来源：http://baike.bbcook.cn/Article/details/gkatakabv.sHtML

[...new Set(arr)]
来源：http://wap.tarul.cn/Article/details/gftotvmos.sHtML

[U90] JS：数字数组排序
来源：http://m.share.sjlbkw.cn/Article/details/grgifxigi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.epnwcf.com/Article/details/gcipcyrwr.sHtML

[U91] JS：对象键值遍历
来源：http://blog.tarul.cn/Article/details/gltkaguqi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.yfazqb.com/Article/details/gkuyycitz.sHtML

[U92] JS：深拷贝
来源：http://m.share.epnwcf.com/Article/details/gyzkvyvht.sHtML

structuredClone(obj)
来源：http://3g.yfazqb.com/Article/details/gfszpieks.sHtML

[U93] JS：模板字符串
来源：http://wap.epnwcf.com/Article/details/gfsqxrmnf.sHtML

`共 ${n} 条`
来源：http://mobile.epnwcf.com/Article/details/gdedfyrbo.sHtML

[U94] JS：箭头函数
来源：http://3g.sjlbkw.cn/Article/details/gbwkaqcvd.sHtML

const double = x => x * 2;
来源：http://m.share.sjlbkw.cn/Article/details/gskowhxeg.sHtML

[U95] JS：Promise 包装
来源：http://3g.bbcook.cn/Article/details/gkyflajns.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.vehdjk.com/Article/details/gfdcvdcev.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.epnwcf.com/Article/details/gchbywdce.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.bbcook.cn/Article/details/gdxnhfqjv.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fktsv.cn/Article/details/gzwcpimoc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.sjlbkw.cn/Article/details/gfsfvznkc.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fktsv.cn/Article/details/gpiwioxuc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.epnwcf.com/Article/details/ghiydgkiq.sHtML

[U99] JS：事件监听
来源：http://read.share.epnwcf.com/Article/details/glelsunnx.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fktsv.cn/Article/details/gsfttxcdq.sHtML

[U100] JS：DOM 查询
来源：http://wap.yfazqb.com/Article/details/gbepymssy.sHtML

document.querySelector(".item")
来源：http://baike.fktsv.cn/Article/details/gkiqdexzj.sHtML

[U101] JS：classList 操作
来源：http://m.share.vehdjk.com/Article/details/gkkqbfheg.sHtML

el.classList.toggle("active")
来源：http://m.share.sjlbkw.cn/Article/details/gkhcxsntk.sHtML

[U102] JS：本地存储
来源：http://www.m.share.tarul.cn/Article/details/gymjknhya.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fktsv.cn/Article/details/gkqzcsgvp.sHtML

[U103] JS：定时器
来源：http://baike.tarul.cn/Article/details/gyeqkplxz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.epnwcf.com/Article/details/guxrxeedj.sHtML

[U104] JS：防抖
来源：http://m.share.vehdjk.com/Article/details/glxwsyaad.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.epnwcf.com/Article/details/gipwahnex.sHtML

[U105] JS：节流
来源：http://www.m.share.tarul.cn/Article/details/gvmxjdtch.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.sjlbkw.cn/Article/details/gusebuxup.sHtML

[U106] JS：日期格式化
来源：http://m.share.bbcook.cn/Article/details/gvgylhgdz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fktsv.cn/Article/details/gvchpnnju.sHtML

[U107] JS：数字千分位
来源：http://mobile.epnwcf.com/Article/details/gxvubzbgo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.yfazqb.com/Article/details/ggwbdxqmv.sHtML

[U108] JS：随机整数
来源：http://www.blog.yfazqb.com/Article/details/gxvpxljsq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fktsv.cn/Article/details/gssgoqgle.sHtML

[U109] JS：数组分组
来源：http://www.blog.sjlbkw.cn/Article/details/grdpzmazv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.tarul.cn/Article/details/gajlsujfn.sHtML

[U110] JS：数组分块
来源：http://m.share.epnwcf.com/Article/details/gjqfpqmem.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.sjlbkw.cn/Article/details/gcktpyiln.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.epnwcf.com/Article/details/gjsjluhaz.sHtML

new Map(Object.entries(obj))
来源：http://wap.vehdjk.com/Article/details/gwkhvprau.sHtML

[U112] JS：字符串补位
来源：http://m.share.yfazqb.com/Article/details/ggohklduy.sHtML

"7".padStart(3, "0")
来源：http://3g.sjlbkw.cn/Article/details/gakgpkosj.sHtML

[U113] JS：正则替换全部
来源：http://3g.tarul.cn/Article/details/gsjvupcvw.sHtML

s.replaceAll("a", "b")
来源：http://www.share.sjlbkw.cn/Article/details/gerlgqayc.sHtML

[U114] JS：JSON 深比较
来源：http://3g.epnwcf.com/Article/details/gogetosjx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.tarul.cn/Article/details/gdinbiymp.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.tarul.cn/Article/details/gfffqydmh.sHtML

crypto.randomUUID()
来源：http://m.share.epnwcf.com/Article/details/gwuihppsp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.vehdjk.com/Article/details/gethclrng.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.tarul.cn/Article/details/gpvtldbez.sHtML

[U117] JS：单元测试
来源：http://wap.vehdjk.com/Article/details/gxgccxidv.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.epnwcf.com/Article/details/gvengdosh.sHtML

[U118] JS：开发服务器
来源：http://blog.bbcook.cn/Article/details/gthqlgmzw.sHtML

npm i -D vite;  npx vite
来源：http://www.share.tarul.cn/Article/details/grdmphwly.sHtML

[U119] JS：生产构建
来源：http://blog.tarul.cn/Article/details/gfxmnolhe.sHtML

npx vite build
来源：http://www.share.fktsv.cn/Article/details/gxxqiedss.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fktsv.cn/Article/details/genpxbuma.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.vehdjk.com/Article/details/ggjcfofnu.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gloqrrxym.sHtML

统计汇总
来源：http://m.share.fktsv.cn/Article/details/gnkfwjarz.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/ghbqefyee.sHtML

按语言统计（条）：
来源：http://baike.vehdjk.com/Article/details/gwokqevoz.sHtML

Python ......... 252
来源：http://3g.fktsv.cn/Article/details/guwnkbgmv.sHtML

PHP ............ 252
来源：http://m.share.tarul.cn/Article/details/gelwyyvmw.sHtML

JavaScript ..... 252
来源：http://m.share.yfazqb.com/Article/details/gdahheznh.sHtML

TypeScript ..... 212
来源：http://3g.bbcook.cn/Article/details/gvslaujpf.sHtML

Java ........... 212
来源：http://www.share.bbcook.cn/Article/details/glxitpbuy.sHtML

Go ............. 212
来源：http://www.blog.tarul.cn/Article/details/gpcqpnlce.sHtML

Ruby ........... 212
来源：http://baike.yfazqb.com/Article/details/ghoemhgvz.sHtML

C# ............. 212
来源：http://read.share.tarul.cn/Article/details/gqksqsoae.sHtML

C .............. 30
来源：http://read.share.yfazqb.com/Article/details/gmawtudcs.sHtML

C++ ............ 30
来源：http://www.m.share.tarul.cn/Article/details/gplildkbk.sHtML

SQL ............ 90
来源：http://www.share.bbcook.cn/Article/details/gqapljugk.sHtML

Bash ........... 80
来源：http://read.share.bbcook.cn/Article/details/gigjcscqi.sHtML

Kotlin ......... 15
来源：http://blog.tarul.cn/Article/details/gwzhgcvpr.sHtML

Swift .......... 15
来源：http://3g.vehdjk.com/Article/details/guiqmizof.sHtML

Lua ............ 10
来源：http://www.m.share.bbcook.cn/Article/details/gknqumecf.sHtML

Perl ........... 10
来源：http://3g.bbcook.cn/Article/details/gfomjzyno.sHtML

Scala .......... 10
来源：http://m.share.sjlbkw.cn/Article/details/gsqltquuy.sHtML

------------------------------------
来源：http://blog.tarul.cn/Article/details/grbnkubid.sHtML

合计 ........... 2106 条
来源：http://blog.vehdjk.com/Article/details/gkoundrbm.sHtML

按章节统计：
来源：http://3g.yfazqb.com/Article/details/gpwxcoeyw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.epnwcf.com/Article/details/gixrnfmxd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.sjlbkw.cn/Article/details/ggiclpewk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.epnwcf.com/Article/details/gjhbxsnse.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.bbcook.cn/Article/details/grjdoqmjo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.yfazqb.com/Article/details/gyjmkopsg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.epnwcf.com/Article/details/gryvsocrj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.vehdjk.com/Article/details/giqsgutdy.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.bbcook.cn/Article/details/gyylsmbkr.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.sjlbkw.cn/Article/details/gpnucnfft.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.tarul.cn/Article/details/gdyfnxrpy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fktsv.cn/Article/details/gegdzpzrh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fktsv.cn/Article/details/ghznaqocb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.sjlbkw.cn/Article/details/gtmdhvmid.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fktsv.cn/Article/details/gjdumlrlm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.tarul.cn/Article/details/gujdqjgig.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.tarul.cn/Article/details/gxvdmbaqs.sHtML

Q SQL 专题                              90
来源：http://wap.bbcook.cn/Article/details/gyrfzdvak.sHtML

R Bash 专题                             80
来源：http://blog.sjlbkw.cn/Article/details/gnbuvbtil.sHtML

S C / C++ 专题                          60
来源：http://read.share.fktsv.cn/Article/details/gukhzfdvw.sHtML

T 其他语言补充                          60
来源：http://www.m.share.yfazqb.com/Article/details/gavjstyll.sHtML

U 高频实用片段                         120
来源：http://baike.epnwcf.com/Article/details/gpmwgxjnx.sHtML

------------------------------------
来源：http://3g.vehdjk.com/Article/details/guuukvyyi.sHtML

合计                                  2106 条
来源：http://wap.fktsv.cn/Article/details/gqdunaxsa.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.epnwcf.com/Article/details/gwjucezjx.sHtML

使用提醒
来源：http://www.m.share.vehdjk.com/Article/details/gwhtjwpfe.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.tarul.cn/Article/details/grisrrlfl.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.sjlbkw.cn/Article/details/gyikfsgvg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.tarul.cn/Article/details/gxvklqqjs.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.sjlbkw.cn/Article/details/gpdupojiu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.tarul.cn/Article/details/giuxhdnel.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.sjlbkw.cn/Article/details/gardinekv.sHtML

—— 文件结束 ——
来源：http://m.share.fktsv.cn/Article/details/ggidebkeu.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/glhfcdaab.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.epnwcf.com/Article/details/gzpsucjot.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.sjlbkw.cn/Article/details/ghbzcuemb.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gosibszwa.sHtML

【收录内容】
来源：http://wap.vehdjk.com/Article/details/gxyzbmzaw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fktsv.cn/Article/details/gemnxqzkd.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.epnwcf.com/Article/details/gedbcauos.sHtML

SQL · Bash · C · C++
来源：http://wap.yfazqb.com/Article/details/gfysoypkh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.epnwcf.com/Article/details/grulhsaue.sHtML

【使用说明】
来源：http://mobile.fktsv.cn/Article/details/grdebaqli.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.tarul.cn/Article/details/gcktlpqcg.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.tarul.cn/Article/details/gsetnpjsu.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.vehdjk.com/Article/details/gncwpkljw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.sjlbkw.cn/Article/details/gckppteim.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.bbcook.cn/Article/details/gbhdgnjdv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.epnwcf.com/Article/details/gjjrvdsjt.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.epnwcf.com/Article/details/gejunwfje.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.epnwcf.com/Article/details/gbieupglc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.bbcook.cn/Article/details/gkiagrzim.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.vehdjk.com/Article/details/gyyixlbfu.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.tarul.cn/Article/details/gphasgvar.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.bbcook.cn/Article/details/gwzxbxqun.sHtML

【文件统计】
来源：http://3g.fktsv.cn/Article/details/gcerkjbng.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fktsv.cn/Article/details/gmqiixwjq.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.yfazqb.com/Article/details/gleqtjlgi.sHtML

目  录
来源：http://www.share.bbcook.cn/Article/details/gjktsqolr.sHtML

--------------------------------------------------------------------------------
来源：http://3g.vehdjk.com/Article/details/gmtlcatdm.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.bbcook.cn/Article/details/gxbzsifkn.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.epnwcf.com/Article/details/gtoydraos.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.yfazqb.com/Article/details/gxiirncxi.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.vehdjk.com/Article/details/guxammmfk.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fktsv.cn/Article/details/gqtavgskh.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.epnwcf.com/Article/details/gzakttrgg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.sjlbkw.cn/Article/details/gkksndqmm.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.bbcook.cn/Article/details/gadpjilwk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.vehdjk.com/Article/details/ggxoudhsw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.epnwcf.com/Article/details/gvphbwxbx.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.sjlbkw.cn/Article/details/gzdynrvth.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.epnwcf.com/Article/details/gjsivkkfl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.yfazqb.com/Article/details/gyindwxtv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.yfazqb.com/Article/details/ggefoejtx.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.epnwcf.com/Article/details/grhjoyijq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.bbcook.cn/Article/details/gqcloeayj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.tarul.cn/Article/details/gepjbmibf.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.epnwcf.com/Article/details/gtgaqqwkz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.epnwcf.com/Article/details/gimadolsc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.yfazqb.com/Article/details/gdurfwjgg.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.vehdjk.com/Article/details/gxuxwuvpg.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gwcfxlpnq.sHtML

A. 基础语法与类型
来源：http://m.share.tarul.cn/Article/details/gzmqyjabv.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gyxdghuor.sHtML

[A01] Hello World
来源：http://wap.vehdjk.com/Article/details/gmbbwjodp.sHtML

Py:   print("Hello, World!")
来源：http://blog.yfazqb.com/Article/details/glmtfodce.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.tarul.cn/Article/details/gcotvajag.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.fktsv.cn/Article/details/gilgmaddn.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.tarul.cn/Article/details/gzvwkblue.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.vehdjk.com/Article/details/gwknbavue.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.bbcook.cn/Article/details/ggdhxxcoo.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fktsv.cn/Article/details/gcopdpkub.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.yfazqb.com/Article/details/guspjnoah.sHtML

[A02] 变量声明与赋值
来源：http://m.share.yfazqb.com/Article/details/gcwlprzmc.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.vehdjk.com/Article/details/gdegqkzpz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.epnwcf.com/Article/details/gqdahmrfi.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.vehdjk.com/Article/details/gvtceloyf.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.tarul.cn/Article/details/gwwomzgyu.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.yfazqb.com/Article/details/gicyyhdlg.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.sjlbkw.cn/Article/details/ghvnqwnal.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.vehdjk.com/Article/details/ggcnlxovk.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.tarul.cn/Article/details/gzudnunff.sHtML

[A03] 常量定义
来源：http://baike.vehdjk.com/Article/details/ggscdfaqu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.vehdjk.com/Article/details/gpcjfhgcl.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.tarul.cn/Article/details/gkkwlktgz.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.sjlbkw.cn/Article/details/gpqqjtgkk.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.tarul.cn/Article/details/gsciakznm.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.sjlbkw.cn/Article/details/gvwmmirdb.sHtML

Go:   const PI = 3.14159
来源：http://m.share.yfazqb.com/Article/details/gbyefqopf.sHtML

Ruby: PI = 3.14159
来源：http://blog.tarul.cn/Article/details/gedkmpwyt.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.tarul.cn/Article/details/gpfmvxnrr.sHtML

[A04] 判断变量类型
来源：http://wap.vehdjk.com/Article/details/gakubogzf.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.yfazqb.com/Article/details/gfrxijqdq.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.fktsv.cn/Article/details/gklxnapjt.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.sjlbkw.cn/Article/details/gjnjsmnxf.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.fktsv.cn/Article/details/gcvduymon.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.vehdjk.com/Article/details/gjzthkpjj.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.tarul.cn/Article/details/gjgktkuvq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.vehdjk.com/Article/details/gjfvzwxtr.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.fktsv.cn/Article/details/grvpbnuyv.sHtML

[A05] 整数除法与取模
来源：http://m.share.vehdjk.com/Article/details/gzvckcxnf.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.vehdjk.com/Article/details/gxuqftaem.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.tarul.cn/Article/details/gknhabtmd.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fktsv.cn/Article/details/ggbddpajn.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fktsv.cn/Article/details/gzjqxarbi.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.yfazqb.com/Article/details/gfuwaevrv.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.tarul.cn/Article/details/gkguhjafh.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.yfazqb.com/Article/details/grjkgcjtd.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.tarul.cn/Article/details/gzddxzxoo.sHtML

[A06] 字符串转数字
来源：http://baike.sjlbkw.cn/Article/details/gukuymczk.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.yfazqb.com/Article/details/gfzrftyct.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.vehdjk.com/Article/details/goxuclfud.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.sjlbkw.cn/Article/details/gsrvuwozg.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.fktsv.cn/Article/details/gebpnlkpm.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.fktsv.cn/Article/details/gsmymfcmu.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.fktsv.cn/Article/details/gdljgyigx.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.sjlbkw.cn/Article/details/guzvdijpw.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.fktsv.cn/Article/details/gsdczvwwz.sHtML

[A07] 数字转字符串
来源：http://blog.vehdjk.com/Article/details/gksgasoaa.sHtML

Py:   str(42)
来源：http://blog.fktsv.cn/Article/details/gnfczhjaz.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.bbcook.cn/Article/details/ghywkjeqd.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.tarul.cn/Article/details/gvmrdcben.sHtML

TS:   String(42)
来源：http://3g.tarul.cn/Article/details/grnihssic.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.fktsv.cn/Article/details/gxsidcrdf.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.epnwcf.com/Article/details/glibbkpzy.sHtML

Ruby: 42.to_s
来源：http://wap.tarul.cn/Article/details/gfcgjxpeb.sHtML

C#:   42.ToString()
来源：http://wap.bbcook.cn/Article/details/gtlnsktvh.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.tarul.cn/Article/details/gzkevonrz.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.sjlbkw.cn/Article/details/gjwobyvij.sHtML


<!-- 参考信息 -->