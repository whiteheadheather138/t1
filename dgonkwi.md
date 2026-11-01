代发 wailian999

[U61] PHP：正则
来源：http://www.m.share.sjlbkw.cn/Article/details/gcgwbxwax.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.yfazqb.com/Article/details/ggzxbpsto.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.bbcook.cn/Article/details/ghxcvimro.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.sjlbkw.cn/Article/details/ginnxbxxe.sHtML

[U63] PHP：文件读写
来源：http://wap.sjlbkw.cn/Article/details/ggmgenwup.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.vehdjk.com/Article/details/gtgraebgy.sHtML

[U64] PHP：目录遍历
来源：http://wap.vehdjk.com/Article/details/gybypqsbd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fktsv.cn/Article/details/gtygedlxb.sHtML

[U65] PHP：会话
来源：http://mobile.fktsv.cn/Article/details/gzoajvzee.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.yfazqb.com/Article/details/gvsxksncr.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.epnwcf.com/Article/details/gridzgjgi.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.bbcook.cn/Article/details/gozzuroyb.sHtML

[U67] PHP：处理文件上传
来源：http://blog.fktsv.cn/Article/details/gujpudlpt.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.tarul.cn/Article/details/gpwygwcwd.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.sjlbkw.cn/Article/details/gfztojldj.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://baike.epnwcf.com/Article/details/gskceqiop.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.yfazqb.com/Article/details/gnxwrrtgq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.bbcook.cn/Article/details/gtuemxsoo.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.epnwcf.com/Article/details/gbbxfxewl.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.sjlbkw.cn/Article/details/gqwxhuxjx.sHtML

[U71] PHP：抛出异常
来源：http://baike.epnwcf.com/Article/details/gdedpebct.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.bbcook.cn/Article/details/gddujnlal.sHtML

[U72] PHP：写错误日志
来源：http://blog.sjlbkw.cn/Article/details/gvqzmgkma.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.bbcook.cn/Article/details/gwscjsxld.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.tarul.cn/Article/details/gyprsaafl.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.vehdjk.com/Article/details/gbeixobvu.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.sjlbkw.cn/Article/details/gpgebymjc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.tarul.cn/Article/details/gdijneebx.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.sjlbkw.cn/Article/details/gpgsymrbk.sHtML

composer require psr/container
来源：http://blog.yfazqb.com/Article/details/gayimhxtu.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.bbcook.cn/Article/details/gebwrakss.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.vehdjk.com/Article/details/gdzwahsyq.sHtML

[U77] PHP：模板渲染
来源：http://wap.sjlbkw.cn/Article/details/gyimblqya.sHtML

composer require twig/twig
来源：http://3g.bbcook.cn/Article/details/glfmwupqe.sHtML

[U78] PHP：单元测试
来源：http://m.share.bbcook.cn/Article/details/gzpqyufav.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.fktsv.cn/Article/details/glwgyovqh.sHtML

[U79] PHP：静态分析
来源：http://3g.sjlbkw.cn/Article/details/grhwhhajx.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.yfazqb.com/Article/details/gzgfjocgi.sHtML

[U80] PHP：代码规范修复
来源：http://blog.bbcook.cn/Article/details/gmvmlidku.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.vehdjk.com/Article/details/gkuxfutpp.sHtML

[U81] JS：初始化项目
来源：http://m.share.fktsv.cn/Article/details/gkkselgrn.sHtML

npm init -y;  npm i express
来源：http://www.blog.tarul.cn/Article/details/gokmehokf.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.bbcook.cn/Article/details/gipsrdrrf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.bbcook.cn/Article/details/ggparymqg.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fktsv.cn/Article/details/gbsctlbkr.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.bbcook.cn/Article/details/gjgnjecbf.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.yfazqb.com/Article/details/gmcgweubu.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.vehdjk.com/Article/details/gxevbvjjm.sHtML

[U85] JS：可选链
来源：http://blog.yfazqb.com/Article/details/gygpzifsy.sHtML

a?.b?.c
来源：http://www.share.fktsv.cn/Article/details/gsnturxmq.sHtML

[U86] JS：空值合并
来源：http://3g.tarul.cn/Article/details/gtjhowhvb.sHtML

a ?? b
来源：http://www.share.vehdjk.com/Article/details/gwyusmlii.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.yfazqb.com/Article/details/ghbgeqvxk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.yfazqb.com/Article/details/gtzpuwgbw.sHtML

[U88] JS：对象展开合并
来源：http://wap.sjlbkw.cn/Article/details/gfvtdebmn.sHtML

{ ...a, ...b }
来源：http://read.share.yfazqb.com/Article/details/gofwcnbrn.sHtML

[U89] JS：数组去重
来源：http://www.share.vehdjk.com/Article/details/gomdihjwd.sHtML

[...new Set(arr)]
来源：http://m.share.tarul.cn/Article/details/gzajvvbwi.sHtML

[U90] JS：数字数组排序
来源：http://m.share.epnwcf.com/Article/details/gyfnoyodo.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.sjlbkw.cn/Article/details/gtcucjkmw.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.tarul.cn/Article/details/gnavdblok.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.vehdjk.com/Article/details/gjenxchph.sHtML

[U92] JS：深拷贝
来源：http://wap.bbcook.cn/Article/details/gmappimbf.sHtML

structuredClone(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gdxmortle.sHtML

[U93] JS：模板字符串
来源：http://read.share.fktsv.cn/Article/details/gjmerqngm.sHtML

`共 ${n} 条`
来源：http://m.share.sjlbkw.cn/Article/details/gcyhvpoae.sHtML

[U94] JS：箭头函数
来源：http://www.blog.epnwcf.com/Article/details/gimzzplan.sHtML

const double = x => x * 2;
来源：http://m.share.tarul.cn/Article/details/geoobnxub.sHtML

[U95] JS：Promise 包装
来源：http://m.share.epnwcf.com/Article/details/ghuxzcjph.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.yfazqb.com/Article/details/gmfsglpxh.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.bbcook.cn/Article/details/gldpgkhxg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fktsv.cn/Article/details/gorltrspu.sHtML

[U97] JS：并发请求
来源：http://3g.sjlbkw.cn/Article/details/gibqpjmcb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.vehdjk.com/Article/details/gwpzzdmwo.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.yfazqb.com/Article/details/gjyawjtie.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.tarul.cn/Article/details/ggvffxmgh.sHtML

[U99] JS：事件监听
来源：http://blog.sjlbkw.cn/Article/details/gaztognoo.sHtML

el.addEventListener("click", e => {})
来源：http://baike.yfazqb.com/Article/details/gmvavrzcx.sHtML

[U100] JS：DOM 查询
来源：http://mobile.vehdjk.com/Article/details/glewpfatl.sHtML

document.querySelector(".item")
来源：http://mobile.tarul.cn/Article/details/gtxmemmec.sHtML

[U101] JS：classList 操作
来源：http://m.share.tarul.cn/Article/details/grdcmttnu.sHtML

el.classList.toggle("active")
来源：http://wap.fktsv.cn/Article/details/gmhdfogld.sHtML

[U102] JS：本地存储
来源：http://www.m.share.bbcook.cn/Article/details/gduvwevzh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fktsv.cn/Article/details/gbngxplib.sHtML

[U103] JS：定时器
来源：http://mobile.bbcook.cn/Article/details/goombauoh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fktsv.cn/Article/details/gleaqbzvd.sHtML

[U104] JS：防抖
来源：http://wap.tarul.cn/Article/details/ghmexchzm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.epnwcf.com/Article/details/gzveqzblc.sHtML

[U105] JS：节流
来源：http://baike.epnwcf.com/Article/details/gteeuafro.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.vehdjk.com/Article/details/gowhhddcz.sHtML

[U106] JS：日期格式化
来源：http://3g.yfazqb.com/Article/details/gmbbokuuy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fktsv.cn/Article/details/gofukdisi.sHtML

[U107] JS：数字千分位
来源：http://wap.epnwcf.com/Article/details/ggajrxgku.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.vehdjk.com/Article/details/gmcmygmgy.sHtML

[U108] JS：随机整数
来源：http://www.blog.yfazqb.com/Article/details/gbpvkhskl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.vehdjk.com/Article/details/gymjhcsqd.sHtML

[U109] JS：数组分组
来源：http://blog.tarul.cn/Article/details/gawxwbnnn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.yfazqb.com/Article/details/gejwxerml.sHtML

[U110] JS：数组分块
来源：http://www.m.share.tarul.cn/Article/details/gusyulawq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fktsv.cn/Article/details/gligsboob.sHtML

[U111] JS：对象转 Map
来源：http://blog.yfazqb.com/Article/details/gtzxrsdab.sHtML

new Map(Object.entries(obj))
来源：http://3g.yfazqb.com/Article/details/gyftauusr.sHtML

[U112] JS：字符串补位
来源：http://blog.fktsv.cn/Article/details/gcnfkoxdr.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.tarul.cn/Article/details/gxpsijpso.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fktsv.cn/Article/details/gtpriarrn.sHtML

s.replaceAll("a", "b")
来源：http://baike.epnwcf.com/Article/details/gtwalmkog.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.vehdjk.com/Article/details/ggtgrgnes.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fktsv.cn/Article/details/gjddgfahh.sHtML

[U115] JS：生成 UUID
来源：http://baike.vehdjk.com/Article/details/ghkxvbwnp.sHtML

crypto.randomUUID()
来源：http://www.share.yfazqb.com/Article/details/gkwvalvwn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.sjlbkw.cn/Article/details/gmqczfciz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.yfazqb.com/Article/details/gxefwvvuy.sHtML

[U117] JS：单元测试
来源：http://blog.yfazqb.com/Article/details/guoeofddb.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fktsv.cn/Article/details/gvqrufmkr.sHtML

[U118] JS：开发服务器
来源：http://baike.tarul.cn/Article/details/gvczcjuvg.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.bbcook.cn/Article/details/guuwyqips.sHtML

[U119] JS：生产构建
来源：http://mobile.yfazqb.com/Article/details/gswwvbtue.sHtML

npx vite build
来源：http://baike.bbcook.cn/Article/details/glkfjqcym.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.sjlbkw.cn/Article/details/gelwmated.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.yfazqb.com/Article/details/gqltwreqi.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gvfrdmfdq.sHtML

统计汇总
来源：http://www.share.sjlbkw.cn/Article/details/gjjxjyhyu.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gqkzymvhj.sHtML

按语言统计（条）：
来源：http://m.share.vehdjk.com/Article/details/gibkdcrqf.sHtML

Python ......... 252
来源：http://mobile.yfazqb.com/Article/details/gmndiweou.sHtML

PHP ............ 252
来源：http://www.blog.tarul.cn/Article/details/gejeiichy.sHtML

JavaScript ..... 252
来源：http://read.share.sjlbkw.cn/Article/details/gijbdgruy.sHtML

TypeScript ..... 212
来源：http://www.blog.yfazqb.com/Article/details/gwqwdjtth.sHtML

Java ........... 212
来源：http://www.share.vehdjk.com/Article/details/gynxagncm.sHtML

Go ............. 212
来源：http://www.share.yfazqb.com/Article/details/gdogeibof.sHtML

Ruby ........... 212
来源：http://www.m.share.sjlbkw.cn/Article/details/gtojddvaa.sHtML

C# ............. 212
来源：http://m.share.epnwcf.com/Article/details/gahdfgtfl.sHtML

C .............. 30
来源：http://www.blog.tarul.cn/Article/details/gxobkdgud.sHtML

C++ ............ 30
来源：http://read.share.sjlbkw.cn/Article/details/gkgfvmwef.sHtML

SQL ............ 90
来源：http://www.m.share.yfazqb.com/Article/details/gbzjfesxn.sHtML

Bash ........... 80
来源：http://www.m.share.fktsv.cn/Article/details/gqfzukqnf.sHtML

Kotlin ......... 15
来源：http://mobile.vehdjk.com/Article/details/gpijxqoba.sHtML

Swift .......... 15
来源：http://blog.yfazqb.com/Article/details/guwzysezt.sHtML

Lua ............ 10
来源：http://m.share.sjlbkw.cn/Article/details/gcdtvjyyq.sHtML

Perl ........... 10
来源：http://read.share.fktsv.cn/Article/details/gjficmpwl.sHtML

Scala .......... 10
来源：http://baike.yfazqb.com/Article/details/gxriukrti.sHtML

------------------------------------
来源：http://3g.tarul.cn/Article/details/geelhmioy.sHtML

合计 ........... 2106 条
来源：http://3g.fktsv.cn/Article/details/gwgctulrn.sHtML

按章节统计：
来源：http://m.share.sjlbkw.cn/Article/details/guxrxzovw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.epnwcf.com/Article/details/gipknlctm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.epnwcf.com/Article/details/gdessosoq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.vehdjk.com/Article/details/gbrhtitli.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.vehdjk.com/Article/details/gacapyqsm.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.epnwcf.com/Article/details/glawlfugz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fktsv.cn/Article/details/gzszpbrlp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.yfazqb.com/Article/details/gxyzwwiii.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.epnwcf.com/Article/details/ggjalcdpx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.epnwcf.com/Article/details/gdivzlqtn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.vehdjk.com/Article/details/givzywgph.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.tarul.cn/Article/details/gjgolzdcb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.bbcook.cn/Article/details/gzfdgkfbd.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.epnwcf.com/Article/details/gtbrllgpq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.epnwcf.com/Article/details/gbcenmjwe.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.vehdjk.com/Article/details/gsanesmnb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.sjlbkw.cn/Article/details/glyczgpxm.sHtML

Q SQL 专题                              90
来源：http://www.blog.fktsv.cn/Article/details/gvlxpdmki.sHtML

R Bash 专题                             80
来源：http://baike.fktsv.cn/Article/details/gwassjhuk.sHtML

S C / C++ 专题                          60
来源：http://www.blog.vehdjk.com/Article/details/ghwnpwstl.sHtML

T 其他语言补充                          60
来源：http://blog.bbcook.cn/Article/details/gkymqptkc.sHtML

U 高频实用片段                         120
来源：http://baike.bbcook.cn/Article/details/grkbwqokh.sHtML

------------------------------------
来源：http://3g.bbcook.cn/Article/details/glkiazaij.sHtML

合计                                  2106 条
来源：http://baike.tarul.cn/Article/details/grjkbwkhx.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.tarul.cn/Article/details/guiouqglf.sHtML

使用提醒
来源：http://www.m.share.sjlbkw.cn/Article/details/gvklnufzg.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.sjlbkw.cn/Article/details/gklefycyy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.vehdjk.com/Article/details/gfjusdabx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.tarul.cn/Article/details/gkpooyitn.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.tarul.cn/Article/details/gibexxuxp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.sjlbkw.cn/Article/details/gxyzvvytm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.sjlbkw.cn/Article/details/gfomttsjy.sHtML

—— 文件结束 ——
来源：http://3g.vehdjk.com/Article/details/gnjlgnhwx.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gndusulzw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.yfazqb.com/Article/details/gsquawqyy.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.yfazqb.com/Article/details/gqgmrdkto.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gdaotirlu.sHtML

【收录内容】
来源：http://wap.fktsv.cn/Article/details/gikijbhfh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fktsv.cn/Article/details/gdjjufrbj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fktsv.cn/Article/details/gvmwtbpll.sHtML

SQL · Bash · C · C++
来源：http://www.share.fktsv.cn/Article/details/gnwvxbngy.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.bbcook.cn/Article/details/gltkiciap.sHtML

【使用说明】
来源：http://3g.sjlbkw.cn/Article/details/gjqohkeqm.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.sjlbkw.cn/Article/details/gnflpfekx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.tarul.cn/Article/details/gghruebtd.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.yfazqb.com/Article/details/gcdgkssgu.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.yfazqb.com/Article/details/glttiqlrg.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.tarul.cn/Article/details/gfiiqacjr.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fktsv.cn/Article/details/gzyqcaxyr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.bbcook.cn/Article/details/gzeobfhwo.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.vehdjk.com/Article/details/gqgbvbllj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.bbcook.cn/Article/details/gauidrsob.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.sjlbkw.cn/Article/details/gepcqqdkb.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fktsv.cn/Article/details/gqypnqcqi.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.vehdjk.com/Article/details/gnqafzyqb.sHtML

【文件统计】
来源：http://m.share.fktsv.cn/Article/details/gpckipbgw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.epnwcf.com/Article/details/gvawohxcu.sHtML

--------------------------------------------------------------------------------
来源：http://wap.vehdjk.com/Article/details/gcwnynzpa.sHtML

目  录
来源：http://blog.yfazqb.com/Article/details/glcvlchrv.sHtML

--------------------------------------------------------------------------------
来源：http://baike.epnwcf.com/Article/details/gcdkcqrpz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fktsv.cn/Article/details/gifznrrva.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.sjlbkw.cn/Article/details/gonmfudfs.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.vehdjk.com/Article/details/gsroaruyi.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.vehdjk.com/Article/details/grvemcwdr.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.yfazqb.com/Article/details/gjglgvkda.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.yfazqb.com/Article/details/gafabxeuk.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.yfazqb.com/Article/details/grtwbxrzo.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.epnwcf.com/Article/details/gcptxigaq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.epnwcf.com/Article/details/gigqilcla.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.bbcook.cn/Article/details/gwpksqfsz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.tarul.cn/Article/details/gfbdyqvmo.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.vehdjk.com/Article/details/glvboqwuk.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.vehdjk.com/Article/details/gmdcpcxfk.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.tarul.cn/Article/details/gzexkaztc.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.tarul.cn/Article/details/gpzoromin.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.bbcook.cn/Article/details/gdmumtymn.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.fktsv.cn/Article/details/gkelhndhm.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.sjlbkw.cn/Article/details/guqhwgrtw.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fktsv.cn/Article/details/gtkqflixo.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.yfazqb.com/Article/details/ggwjuaavs.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.yfazqb.com/Article/details/gfpdoqcsq.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/githujuxx.sHtML

A. 基础语法与类型
来源：http://mobile.tarul.cn/Article/details/gnlxdxsnr.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gvzaomnwa.sHtML

[A01] Hello World
来源：http://www.blog.vehdjk.com/Article/details/gqnnzlzte.sHtML

Py:   print("Hello, World!")
来源：http://read.share.yfazqb.com/Article/details/gwtuuguth.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.fktsv.cn/Article/details/gxvgfpzjq.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.tarul.cn/Article/details/gjlxvezvn.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.epnwcf.com/Article/details/gcryqkuda.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.sjlbkw.cn/Article/details/gbiuddtup.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.vehdjk.com/Article/details/giaelmnsc.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.tarul.cn/Article/details/gwfyygadi.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.yfazqb.com/Article/details/gfldnrmsv.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.epnwcf.com/Article/details/gshhbrzki.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.epnwcf.com/Article/details/gurqjolsr.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.tarul.cn/Article/details/gleanavtm.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fktsv.cn/Article/details/ggkgtqceh.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.tarul.cn/Article/details/gvmafnely.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.fktsv.cn/Article/details/gbokdezyo.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.tarul.cn/Article/details/gdkpybumw.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.sjlbkw.cn/Article/details/gsxijbbyz.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.yfazqb.com/Article/details/gwjixzqjt.sHtML

[A03] 常量定义
来源：http://read.share.epnwcf.com/Article/details/ggmseouff.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.tarul.cn/Article/details/gtozaflnn.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.vehdjk.com/Article/details/gnabankuk.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.epnwcf.com/Article/details/gmwjrpfqp.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.fktsv.cn/Article/details/glyqocooa.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.yfazqb.com/Article/details/geomrfuqe.sHtML

Go:   const PI = 3.14159
来源：http://www.share.yfazqb.com/Article/details/gpwhlxiel.sHtML

Ruby: PI = 3.14159
来源：http://m.share.yfazqb.com/Article/details/gbhnsxnjq.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.tarul.cn/Article/details/gljhafovu.sHtML

[A04] 判断变量类型
来源：http://read.share.sjlbkw.cn/Article/details/geqlbfzbv.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.fktsv.cn/Article/details/gnhnirtym.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.tarul.cn/Article/details/gixtewgpn.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.fktsv.cn/Article/details/giizakvmm.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.yfazqb.com/Article/details/gbravmbmt.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.bbcook.cn/Article/details/ginmssnqa.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.fktsv.cn/Article/details/gmwykeknw.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.fktsv.cn/Article/details/gupqksdij.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.sjlbkw.cn/Article/details/gycqmcvbf.sHtML

[A05] 整数除法与取模
来源：http://baike.fktsv.cn/Article/details/gqectmrad.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.yfazqb.com/Article/details/giuryoqrf.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.tarul.cn/Article/details/gxpphakod.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.sjlbkw.cn/Article/details/gfchskddg.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.tarul.cn/Article/details/gxpwxkqls.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.fktsv.cn/Article/details/gnxcawtnl.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.bbcook.cn/Article/details/gxxirewla.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.vehdjk.com/Article/details/ggzubnfjl.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.tarul.cn/Article/details/gqdirjkeh.sHtML

[A06] 字符串转数字
来源：http://3g.fktsv.cn/Article/details/gxuyxbmak.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.bbcook.cn/Article/details/gryahjblq.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.bbcook.cn/Article/details/glcltqatc.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.fktsv.cn/Article/details/gwarwkdxe.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.epnwcf.com/Article/details/gayehihjl.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.bbcook.cn/Article/details/gtxgjtovb.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.epnwcf.com/Article/details/gjulvfbog.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.tarul.cn/Article/details/gljmcahdx.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.fktsv.cn/Article/details/gisdrjbtz.sHtML

[A07] 数字转字符串
来源：http://www.blog.bbcook.cn/Article/details/gnriibpuz.sHtML

Py:   str(42)
来源：http://3g.bbcook.cn/Article/details/gwpjfwsti.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.fktsv.cn/Article/details/gmibljfbv.sHtML

JS:   String(42); (42).toString()
来源：http://wap.vehdjk.com/Article/details/gmcyzalto.sHtML

TS:   String(42)
来源：http://blog.fktsv.cn/Article/details/gqlfzgmql.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.vehdjk.com/Article/details/gtnmzbhdl.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.bbcook.cn/Article/details/gmifpajkx.sHtML

Ruby: 42.to_s
来源：http://mobile.sjlbkw.cn/Article/details/gnyeeyovm.sHtML

C#:   42.ToString()
来源：http://m.share.tarul.cn/Article/details/gjnkvrfla.sHtML

[A08] 取整与四舍五入
来源：http://baike.vehdjk.com/Article/details/gwqucmbau.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.bbcook.cn/Article/details/gqadhgpxb.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.sjlbkw.cn/Article/details/gnqjpiflz.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.tarul.cn/Article/details/gcymdotby.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.bbcook.cn/Article/details/gmtaqqndm.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.bbcook.cn/Article/details/gvsylntrm.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.yfazqb.com/Article/details/gmcyhaihz.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.tarul.cn/Article/details/guvuuxeos.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.epnwcf.com/Article/details/gbdahugal.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.sjlbkw.cn/Article/details/gszzrcwxv.sHtML


<!-- 参考信息 -->