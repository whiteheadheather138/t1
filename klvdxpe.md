代发 wailian999

[U59] PHP：自定义排序
来源：http://www.share.tarul.cn/Article/details/gzggmnsdb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.epnwcf.com/Article/details/gdiuwqcsc.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.vehdjk.com/Article/details/gwemdurmz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.bbcook.cn/Article/details/gpcepqkfv.sHtML

[U61] PHP：正则
来源：http://mobile.yfazqb.com/Article/details/ghwrkkhjr.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.epnwcf.com/Article/details/gbhqzdqst.sHtML

[U62] PHP：日期对象
来源：http://baike.epnwcf.com/Article/details/gueuxqfyz.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.bbcook.cn/Article/details/gygvmiyhf.sHtML

[U63] PHP：文件读写
来源：http://mobile.vehdjk.com/Article/details/gvgtfvkrp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.vehdjk.com/Article/details/gktcsnthk.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.tarul.cn/Article/details/gtlorvain.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.yfazqb.com/Article/details/gowoztbne.sHtML

[U65] PHP：会话
来源：http://mobile.yfazqb.com/Article/details/gndxycjef.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.vehdjk.com/Article/details/gotaacrvu.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.bbcook.cn/Article/details/ghahxvmvy.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.vehdjk.com/Article/details/gjanfsdjm.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.tarul.cn/Article/details/gbwiwspky.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fktsv.cn/Article/details/gebymkenj.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.tarul.cn/Article/details/gzhmvcfvf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.sjlbkw.cn/Article/details/gtnocaaxj.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.bbcook.cn/Article/details/gibivfdma.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fktsv.cn/Article/details/gbhsuhern.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fktsv.cn/Article/details/gmeozvefk.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.bbcook.cn/Article/details/gccgdjywz.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.vehdjk.com/Article/details/gvdirhsoc.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.yfazqb.com/Article/details/gvsbnekio.sHtML

[U72] PHP：写错误日志
来源：http://m.share.yfazqb.com/Article/details/gryxpoqzu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.sjlbkw.cn/Article/details/gvskkksvk.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.sjlbkw.cn/Article/details/gyptsqdwf.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.sjlbkw.cn/Article/details/gztipkjno.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.epnwcf.com/Article/details/gjcdnspjc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.vehdjk.com/Article/details/gpwkfxrln.sHtML

[U75] PHP：依赖注入
来源：http://wap.bbcook.cn/Article/details/ggygnwewz.sHtML

composer require psr/container
来源：http://wap.yfazqb.com/Article/details/gxypfwarl.sHtML

[U76] PHP：简单路由
来源：http://www.blog.sjlbkw.cn/Article/details/gjnnxkvsw.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.sjlbkw.cn/Article/details/gbmceycxl.sHtML

[U77] PHP：模板渲染
来源：http://wap.yfazqb.com/Article/details/gdyhllnpp.sHtML

composer require twig/twig
来源：http://www.share.bbcook.cn/Article/details/gtuiobhyf.sHtML

[U78] PHP：单元测试
来源：http://blog.tarul.cn/Article/details/gvfzvvuap.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.yfazqb.com/Article/details/gfulhxbhw.sHtML

[U79] PHP：静态分析
来源：http://www.blog.tarul.cn/Article/details/gmoqtqdur.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.tarul.cn/Article/details/gpnuhubqf.sHtML

[U80] PHP：代码规范修复
来源：http://blog.yfazqb.com/Article/details/gdzpopkfq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.tarul.cn/Article/details/guvhlaoyj.sHtML

[U81] JS：初始化项目
来源：http://mobile.sjlbkw.cn/Article/details/gnxwodkzb.sHtML

npm init -y;  npm i express
来源：http://www.share.bbcook.cn/Article/details/gbpyknoih.sHtML

[U82] JS：package.json 脚本
来源：http://blog.yfazqb.com/Article/details/gxnrfjlpr.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.yfazqb.com/Article/details/gualpoanq.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.tarul.cn/Article/details/ghchxjply.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.tarul.cn/Article/details/gegdnnkgm.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.fktsv.cn/Article/details/gdltsubzg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.epnwcf.com/Article/details/gdgtdpktm.sHtML

[U85] JS：可选链
来源：http://3g.fktsv.cn/Article/details/glswdolau.sHtML

a?.b?.c
来源：http://read.share.bbcook.cn/Article/details/gfkqawptg.sHtML

[U86] JS：空值合并
来源：http://baike.sjlbkw.cn/Article/details/gaqjzppie.sHtML

a ?? b
来源：http://blog.yfazqb.com/Article/details/gyivgpklt.sHtML

[U87] JS：解构默认值
来源：http://baike.sjlbkw.cn/Article/details/gdjbdyied.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.vehdjk.com/Article/details/gyqfjuvte.sHtML

[U88] JS：对象展开合并
来源：http://baike.tarul.cn/Article/details/gjjplsgta.sHtML

{ ...a, ...b }
来源：http://blog.sjlbkw.cn/Article/details/gojqvovqh.sHtML

[U89] JS：数组去重
来源：http://www.blog.yfazqb.com/Article/details/gmqcobdbo.sHtML

[...new Set(arr)]
来源：http://mobile.fktsv.cn/Article/details/gmgimgczr.sHtML

[U90] JS：数字数组排序
来源：http://3g.sjlbkw.cn/Article/details/gksaipgrk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.tarul.cn/Article/details/gpglilayq.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fktsv.cn/Article/details/gtrqjzsmj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.yfazqb.com/Article/details/gniutkkmj.sHtML

[U92] JS：深拷贝
来源：http://baike.epnwcf.com/Article/details/gduytnscq.sHtML

structuredClone(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gqooerlvi.sHtML

[U93] JS：模板字符串
来源：http://blog.epnwcf.com/Article/details/gtipzpcjl.sHtML

`共 ${n} 条`
来源：http://blog.yfazqb.com/Article/details/gmgmuywlf.sHtML

[U94] JS：箭头函数
来源：http://3g.yfazqb.com/Article/details/gjwmfbqof.sHtML

const double = x => x * 2;
来源：http://www.m.share.tarul.cn/Article/details/gzbjddxkm.sHtML

[U95] JS：Promise 包装
来源：http://blog.epnwcf.com/Article/details/ganwubnsg.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.tarul.cn/Article/details/gvfnnphit.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.epnwcf.com/Article/details/ghgikzxzy.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.tarul.cn/Article/details/gywvhyfje.sHtML

[U97] JS：并发请求
来源：http://m.share.yfazqb.com/Article/details/gvhfqsyjf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.epnwcf.com/Article/details/gaakaweue.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fktsv.cn/Article/details/gggzoslhi.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.yfazqb.com/Article/details/gfkfpeqdd.sHtML

[U99] JS：事件监听
来源：http://blog.bbcook.cn/Article/details/gvquvaaxd.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fktsv.cn/Article/details/gzzoxcluq.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.epnwcf.com/Article/details/giolckdmn.sHtML

document.querySelector(".item")
来源：http://m.share.epnwcf.com/Article/details/gyhwhujop.sHtML

[U101] JS：classList 操作
来源：http://m.share.tarul.cn/Article/details/gltcplbam.sHtML

el.classList.toggle("active")
来源：http://www.blog.epnwcf.com/Article/details/gjuyxpinn.sHtML

[U102] JS：本地存储
来源：http://read.share.vehdjk.com/Article/details/gfoxlpqcq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.epnwcf.com/Article/details/gmamilsis.sHtML

[U103] JS：定时器
来源：http://wap.epnwcf.com/Article/details/ghfwpdutk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.yfazqb.com/Article/details/gyewiroeg.sHtML

[U104] JS：防抖
来源：http://mobile.bbcook.cn/Article/details/gxpmkkedg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fktsv.cn/Article/details/gkyjmznmg.sHtML

[U105] JS：节流
来源：http://3g.epnwcf.com/Article/details/gmyoynugj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.bbcook.cn/Article/details/gjnodbxpi.sHtML

[U106] JS：日期格式化
来源：http://read.share.bbcook.cn/Article/details/gkkvckcez.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fktsv.cn/Article/details/glcnrwnpt.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqxfyggt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.bbcook.cn/Article/details/gwwwossjy.sHtML

[U108] JS：随机整数
来源：http://mobile.tarul.cn/Article/details/guzvmpfic.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fktsv.cn/Article/details/gepixwpjw.sHtML

[U109] JS：数组分组
来源：http://wap.bbcook.cn/Article/details/gqtdrynxt.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.sjlbkw.cn/Article/details/gdhreuagq.sHtML

[U110] JS：数组分块
来源：http://baike.tarul.cn/Article/details/gcvkqcluw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.tarul.cn/Article/details/gypwqmkxi.sHtML

[U111] JS：对象转 Map
来源：http://read.share.sjlbkw.cn/Article/details/gjccoecfc.sHtML

new Map(Object.entries(obj))
来源：http://wap.bbcook.cn/Article/details/gdmacpawh.sHtML

[U112] JS：字符串补位
来源：http://baike.bbcook.cn/Article/details/gjjidcxlf.sHtML

"7".padStart(3, "0")
来源：http://m.share.yfazqb.com/Article/details/gqdokpimx.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fktsv.cn/Article/details/gkpjjgqqs.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.tarul.cn/Article/details/gpqbvxfff.sHtML

[U114] JS：JSON 深比较
来源：http://blog.tarul.cn/Article/details/gtyqtomct.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.epnwcf.com/Article/details/grldafdqa.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.yfazqb.com/Article/details/gycjcahma.sHtML

crypto.randomUUID()
来源：http://www.m.share.fktsv.cn/Article/details/giuiaoqbs.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.bbcook.cn/Article/details/guwxbbhyy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.epnwcf.com/Article/details/gysynxjsw.sHtML

[U117] JS：单元测试
来源：http://baike.sjlbkw.cn/Article/details/gvjwtxtnz.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.tarul.cn/Article/details/gnefljhrk.sHtML

[U118] JS：开发服务器
来源：http://wap.tarul.cn/Article/details/gfureeapo.sHtML

npm i -D vite;  npx vite
来源：http://baike.fktsv.cn/Article/details/gbjxynwfs.sHtML

[U119] JS：生产构建
来源：http://www.share.tarul.cn/Article/details/gzbxupsps.sHtML

npx vite build
来源：http://blog.sjlbkw.cn/Article/details/gjmrvjeub.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.vehdjk.com/Article/details/ggimibzxp.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.tarul.cn/Article/details/gfjqtgwhg.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gaepptnwa.sHtML

统计汇总
来源：http://m.share.tarul.cn/Article/details/gmssqnxlq.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/guykfluyo.sHtML

按语言统计（条）：
来源：http://www.m.share.bbcook.cn/Article/details/glpdetgpb.sHtML

Python ......... 252
来源：http://m.share.epnwcf.com/Article/details/gzaaudgwp.sHtML

PHP ............ 252
来源：http://mobile.vehdjk.com/Article/details/gercspuxd.sHtML

JavaScript ..... 252
来源：http://wap.fktsv.cn/Article/details/gdtoknqvj.sHtML

TypeScript ..... 212
来源：http://read.share.yfazqb.com/Article/details/gwyhtifss.sHtML

Java ........... 212
来源：http://read.share.yfazqb.com/Article/details/gueoddrzq.sHtML

Go ............. 212
来源：http://wap.sjlbkw.cn/Article/details/gkiwzlrdp.sHtML

Ruby ........... 212
来源：http://www.blog.vehdjk.com/Article/details/gpqwlflcv.sHtML

C# ............. 212
来源：http://read.share.fktsv.cn/Article/details/gokznyfdd.sHtML

C .............. 30
来源：http://blog.epnwcf.com/Article/details/gjaycbbbz.sHtML

C++ ............ 30
来源：http://baike.yfazqb.com/Article/details/gxhnhrfyb.sHtML

SQL ............ 90
来源：http://baike.tarul.cn/Article/details/gufxfyejq.sHtML

Bash ........... 80
来源：http://m.share.fktsv.cn/Article/details/gptaigxzg.sHtML

Kotlin ......... 15
来源：http://read.share.bbcook.cn/Article/details/getbqxvup.sHtML

Swift .......... 15
来源：http://read.share.bbcook.cn/Article/details/glwoctuzu.sHtML

Lua ............ 10
来源：http://mobile.bbcook.cn/Article/details/gzwuzhkmg.sHtML

Perl ........... 10
来源：http://read.share.sjlbkw.cn/Article/details/gjpbhydki.sHtML

Scala .......... 10
来源：http://wap.bbcook.cn/Article/details/gwbqvxjyu.sHtML

------------------------------------
来源：http://m.share.fktsv.cn/Article/details/gbbujnvdj.sHtML

合计 ........... 2106 条
来源：http://3g.bbcook.cn/Article/details/gwfbacyvo.sHtML

按章节统计：
来源：http://3g.epnwcf.com/Article/details/gxivzfqwf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.bbcook.cn/Article/details/gkbaxnjqy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.sjlbkw.cn/Article/details/gytufwywq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.bbcook.cn/Article/details/gqnhbcglq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.bbcook.cn/Article/details/gjkczieeb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.epnwcf.com/Article/details/ghqhyzajo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.yfazqb.com/Article/details/gvycmgfat.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fktsv.cn/Article/details/gmfvqklno.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.yfazqb.com/Article/details/gixaztzhz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.epnwcf.com/Article/details/gungwqeun.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.bbcook.cn/Article/details/gsxgwrsvc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.bbcook.cn/Article/details/gdksmdbzi.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.sjlbkw.cn/Article/details/gmduwjikv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fktsv.cn/Article/details/gdzovdsjq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.sjlbkw.cn/Article/details/goggvwgwm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.tarul.cn/Article/details/gmyjkceqc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.epnwcf.com/Article/details/gieqslshx.sHtML

Q SQL 专题                              90
来源：http://blog.bbcook.cn/Article/details/gqopqkffn.sHtML

R Bash 专题                             80
来源：http://www.blog.vehdjk.com/Article/details/gczmzhasz.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.epnwcf.com/Article/details/gsveefcqe.sHtML

T 其他语言补充                          60
来源：http://baike.vehdjk.com/Article/details/gedwhvbkf.sHtML

U 高频实用片段                         120
来源：http://wap.yfazqb.com/Article/details/gbjkzlztr.sHtML

------------------------------------
来源：http://baike.tarul.cn/Article/details/gwdxfgilq.sHtML

合计                                  2106 条
来源：http://www.blog.bbcook.cn/Article/details/gshrwoqyv.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.sjlbkw.cn/Article/details/guqablscr.sHtML

使用提醒
来源：http://3g.sjlbkw.cn/Article/details/gxlnjghod.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fktsv.cn/Article/details/gqbjchkvr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fktsv.cn/Article/details/gnxlwatyu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.tarul.cn/Article/details/glxruuzlu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.vehdjk.com/Article/details/gesbjhgbt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.bbcook.cn/Article/details/gfouhosvc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fktsv.cn/Article/details/gqewxggcx.sHtML

—— 文件结束 ——
来源：http://m.share.bbcook.cn/Article/details/gjojovnxd.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/glqztyder.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.bbcook.cn/Article/details/gswtkzaum.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fktsv.cn/Article/details/gkkafirrf.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gmuhlmpzz.sHtML

【收录内容】
来源：http://www.blog.epnwcf.com/Article/details/gywvwuhwn.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.sjlbkw.cn/Article/details/gnlbjtojx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.sjlbkw.cn/Article/details/gmnxeafax.sHtML

SQL · Bash · C · C++
来源：http://3g.yfazqb.com/Article/details/gnpnyqmdo.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.sjlbkw.cn/Article/details/gjxhcqfis.sHtML

【使用说明】
来源：http://wap.yfazqb.com/Article/details/gzmtprjpk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fktsv.cn/Article/details/gwfevjkpc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.vehdjk.com/Article/details/gsvgvayqy.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.vehdjk.com/Article/details/glnvvadto.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.vehdjk.com/Article/details/gujvkqwnl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.epnwcf.com/Article/details/gxfgilybq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.vehdjk.com/Article/details/gfcbaxfbw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.bbcook.cn/Article/details/gnhznrcsr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.epnwcf.com/Article/details/gtaubhbbs.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.yfazqb.com/Article/details/gtrhmlvgp.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.tarul.cn/Article/details/gkqtehqrx.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.bbcook.cn/Article/details/gfbjrgybm.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fktsv.cn/Article/details/gjfgmtcco.sHtML

【文件统计】
来源：http://m.share.bbcook.cn/Article/details/gofrrsucw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.bbcook.cn/Article/details/gborwykfz.sHtML

--------------------------------------------------------------------------------
来源：http://blog.sjlbkw.cn/Article/details/gahsrsold.sHtML

目  录
来源：http://baike.epnwcf.com/Article/details/grzhiwmyl.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.yfazqb.com/Article/details/gngtbvcqe.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.tarul.cn/Article/details/gnqwpqwle.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.vehdjk.com/Article/details/gjlyqwyjy.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.epnwcf.com/Article/details/gprhcvgmj.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.tarul.cn/Article/details/gkrkzuqay.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.tarul.cn/Article/details/gtajvmron.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.tarul.cn/Article/details/gneoynilj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.sjlbkw.cn/Article/details/ghcutxafi.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.tarul.cn/Article/details/gjxyzrzrx.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.sjlbkw.cn/Article/details/gkywrvsoi.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.bbcook.cn/Article/details/gjaynkbqn.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fktsv.cn/Article/details/gkbvyiybe.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.sjlbkw.cn/Article/details/gatiprlbq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.yfazqb.com/Article/details/gzsmynzew.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.epnwcf.com/Article/details/gegdrrgpl.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.tarul.cn/Article/details/gowpnhneh.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.epnwcf.com/Article/details/gtdhmwfae.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.sjlbkw.cn/Article/details/glmdlalls.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.epnwcf.com/Article/details/gnyaxffmz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.epnwcf.com/Article/details/gbftgpbaq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.epnwcf.com/Article/details/gahgkrrzo.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.vehdjk.com/Article/details/gcvclmsrs.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gkxmfayre.sHtML

A. 基础语法与类型
来源：http://baike.yfazqb.com/Article/details/gwdooltjr.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gdlzhbwbp.sHtML

[A01] Hello World
来源：http://blog.sjlbkw.cn/Article/details/ggezozhpd.sHtML

Py:   print("Hello, World!")
来源：http://www.share.vehdjk.com/Article/details/gckrwkxyn.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.bbcook.cn/Article/details/gjhraioaz.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.bbcook.cn/Article/details/gfqtanzso.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.vehdjk.com/Article/details/gnpzqqgps.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.tarul.cn/Article/details/gxxkyumat.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.sjlbkw.cn/Article/details/gmadtnyex.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.tarul.cn/Article/details/gibvvkivc.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.tarul.cn/Article/details/grpxffenl.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.epnwcf.com/Article/details/gopwxvysi.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.sjlbkw.cn/Article/details/gcjvplasd.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.bbcook.cn/Article/details/gbgugqbyy.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fktsv.cn/Article/details/gonhtzmln.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fktsv.cn/Article/details/gsejqfnqt.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fktsv.cn/Article/details/guqvvyjlg.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.epnwcf.com/Article/details/gtuemohbg.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.fktsv.cn/Article/details/ghaidtoqp.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.sjlbkw.cn/Article/details/gfkvllouj.sHtML

[A03] 常量定义
来源：http://www.share.vehdjk.com/Article/details/gxsoknajo.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.fktsv.cn/Article/details/gxbcnjhgc.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.epnwcf.com/Article/details/gqhcjjrzr.sHtML

JS:   const PI = 3.14159;
来源：http://blog.vehdjk.com/Article/details/gqhcawypc.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.tarul.cn/Article/details/gazqdedyd.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.tarul.cn/Article/details/gncagfrcu.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.fktsv.cn/Article/details/gekithoxf.sHtML

Ruby: PI = 3.14159
来源：http://baike.tarul.cn/Article/details/gcdrimrys.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.bbcook.cn/Article/details/gyxkaacbg.sHtML

[A04] 判断变量类型
来源：http://blog.tarul.cn/Article/details/gzzcdbjgw.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.sjlbkw.cn/Article/details/ggttwkths.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.bbcook.cn/Article/details/gcvxiikvm.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.vehdjk.com/Article/details/gormefakx.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.fktsv.cn/Article/details/gceagfipt.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.vehdjk.com/Article/details/gisxhkwvr.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.bbcook.cn/Article/details/gwuopjciy.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.fktsv.cn/Article/details/gqarsnyel.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.sjlbkw.cn/Article/details/geimxcmud.sHtML

[A05] 整数除法与取模
来源：http://www.blog.vehdjk.com/Article/details/gquzjdypg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.vehdjk.com/Article/details/gelgxbqkj.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.bbcook.cn/Article/details/gratqvgmh.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.bbcook.cn/Article/details/gtntxctny.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.sjlbkw.cn/Article/details/gbawbtjsn.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.fktsv.cn/Article/details/gfbyscitg.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.yfazqb.com/Article/details/gxeflemki.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.vehdjk.com/Article/details/gyqrnatph.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.epnwcf.com/Article/details/gxejxxcmk.sHtML

[A06] 字符串转数字
来源：http://wap.tarul.cn/Article/details/gxjvvrtkk.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.vehdjk.com/Article/details/gyltciucp.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.fktsv.cn/Article/details/gkjvpybhl.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.yfazqb.com/Article/details/gwetvmqqa.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.fktsv.cn/Article/details/gbfucmvbo.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.bbcook.cn/Article/details/guebgfugh.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.fktsv.cn/Article/details/gmzifucbx.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.vehdjk.com/Article/details/gzjoejdpb.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.fktsv.cn/Article/details/giapynuwg.sHtML

[A07] 数字转字符串
来源：http://wap.sjlbkw.cn/Article/details/goopymrvu.sHtML

Py:   str(42)
来源：http://wap.bbcook.cn/Article/details/gntiqzocs.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.yfazqb.com/Article/details/gzpxxobui.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.sjlbkw.cn/Article/details/gsebfohev.sHtML

TS:   String(42)
来源：http://mobile.epnwcf.com/Article/details/gdpbvcfye.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.yfazqb.com/Article/details/gmpjvdpti.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.fktsv.cn/Article/details/gqrldkbrv.sHtML

Ruby: 42.to_s
来源：http://www.blog.bbcook.cn/Article/details/gmcxjieza.sHtML

C#:   42.ToString()
来源：http://baike.epnwcf.com/Article/details/gpkequkqu.sHtML

[A08] 取整与四舍五入
来源：http://wap.sjlbkw.cn/Article/details/goumscvhk.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.tarul.cn/Article/details/gfomamxgk.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.yfazqb.com/Article/details/gmcpyaned.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.fktsv.cn/Article/details/gxgveanbc.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.yfazqb.com/Article/details/geoqubdiw.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.epnwcf.com/Article/details/gxjcziiil.sHtML


<!-- 参考信息 -->