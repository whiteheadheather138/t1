代发 wailian999

[U65] PHP：会话
来源：http://www.share.yfazqb.com/Article/details/gnvofviws.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fktsv.cn/Article/details/gicucpxee.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.vehdjk.com/Article/details/gkhqjgcgj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.tarul.cn/Article/details/goghxtput.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fktsv.cn/Article/details/getxecqnm.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfkbmrzwx.sHtML

[U68] PHP：PDO 连接
来源：http://mobile.yfazqb.com/Article/details/gijhzpcqw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.yfazqb.com/Article/details/gcqwslidd.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fktsv.cn/Article/details/gcumxhpcv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.bbcook.cn/Article/details/gslxjevdp.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.vehdjk.com/Article/details/ghsijbxyc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.tarul.cn/Article/details/gkcxvodei.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.vehdjk.com/Article/details/goblxkkuv.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.sjlbkw.cn/Article/details/gxjacepsg.sHtML

[U72] PHP：写错误日志
来源：http://wap.epnwcf.com/Article/details/gqcpjymhy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.sjlbkw.cn/Article/details/gphpipczi.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.bbcook.cn/Article/details/gjpzwswfp.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.vehdjk.com/Article/details/gcpwdkhhr.sHtML

[U74] PHP：读取环境变量
来源：http://wap.bbcook.cn/Article/details/gocdgfion.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fktsv.cn/Article/details/gpqvjgybt.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.tarul.cn/Article/details/gxvmnmdxi.sHtML

composer require psr/container
来源：http://m.share.sjlbkw.cn/Article/details/gaxpxcoec.sHtML

[U76] PHP：简单路由
来源：http://3g.epnwcf.com/Article/details/gwaodgugh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.sjlbkw.cn/Article/details/gorzfvfvk.sHtML

[U77] PHP：模板渲染
来源：http://mobile.bbcook.cn/Article/details/gyuskaauz.sHtML

composer require twig/twig
来源：http://www.share.epnwcf.com/Article/details/gxmgbcstt.sHtML

[U78] PHP：单元测试
来源：http://baike.sjlbkw.cn/Article/details/gdvvjtnlb.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.bbcook.cn/Article/details/gmkmidswh.sHtML

[U79] PHP：静态分析
来源：http://www.share.sjlbkw.cn/Article/details/gpvyexpjf.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.sjlbkw.cn/Article/details/gqoxjksoe.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fktsv.cn/Article/details/ghtzvrisn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.vehdjk.com/Article/details/gwgryuwnc.sHtML

[U81] JS：初始化项目
来源：http://mobile.fktsv.cn/Article/details/grkvotimo.sHtML

npm init -y;  npm i express
来源：http://baike.yfazqb.com/Article/details/gzrkkormy.sHtML

[U82] JS：package.json 脚本
来源：http://blog.sjlbkw.cn/Article/details/gtsesxfun.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.bbcook.cn/Article/details/gbydsibai.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.yfazqb.com/Article/details/gxykvwkzw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.tarul.cn/Article/details/gyovwdfcm.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.vehdjk.com/Article/details/gadfvgeqd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.sjlbkw.cn/Article/details/gbyalbjxi.sHtML

[U85] JS：可选链
来源：http://www.share.fktsv.cn/Article/details/gxdhvsocp.sHtML

a?.b?.c
来源：http://wap.epnwcf.com/Article/details/gvlhgkwhm.sHtML

[U86] JS：空值合并
来源：http://read.share.tarul.cn/Article/details/gcoxqenwp.sHtML

a ?? b
来源：http://3g.fktsv.cn/Article/details/gwkhcgcgv.sHtML

[U87] JS：解构默认值
来源：http://3g.fktsv.cn/Article/details/gdqaezxuu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.epnwcf.com/Article/details/gybloccmt.sHtML

[U88] JS：对象展开合并
来源：http://3g.yfazqb.com/Article/details/gtfphggok.sHtML

{ ...a, ...b }
来源：http://baike.sjlbkw.cn/Article/details/gbasuciew.sHtML

[U89] JS：数组去重
来源：http://m.share.epnwcf.com/Article/details/gwapmztwo.sHtML

[...new Set(arr)]
来源：http://www.m.share.tarul.cn/Article/details/gxgcuujtw.sHtML

[U90] JS：数字数组排序
来源：http://wap.sjlbkw.cn/Article/details/gjqwljgfm.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.bbcook.cn/Article/details/gkynxybif.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.sjlbkw.cn/Article/details/gepcpgmbi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.epnwcf.com/Article/details/gotlkruui.sHtML

[U92] JS：深拷贝
来源：http://mobile.sjlbkw.cn/Article/details/ghkcoaytn.sHtML

structuredClone(obj)
来源：http://blog.fktsv.cn/Article/details/gqtxzhkgt.sHtML

[U93] JS：模板字符串
来源：http://blog.sjlbkw.cn/Article/details/gxywtjhjh.sHtML

`共 ${n} 条`
来源：http://3g.yfazqb.com/Article/details/gwmljcqtg.sHtML

[U94] JS：箭头函数
来源：http://blog.fktsv.cn/Article/details/gnyllsdvv.sHtML

const double = x => x * 2;
来源：http://m.share.bbcook.cn/Article/details/grrscqkwv.sHtML

[U95] JS：Promise 包装
来源：http://baike.yfazqb.com/Article/details/gcdjirzwg.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.yfazqb.com/Article/details/gokjkjfmr.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fktsv.cn/Article/details/gbbtmszpz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.epnwcf.com/Article/details/geojmfkpe.sHtML

[U97] JS：并发请求
来源：http://mobile.vehdjk.com/Article/details/grieadyjj.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.bbcook.cn/Article/details/gnixgvzgs.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.yfazqb.com/Article/details/gpwebhcyr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.sjlbkw.cn/Article/details/gpanajynr.sHtML

[U99] JS：事件监听
来源：http://m.share.bbcook.cn/Article/details/gvqzzanio.sHtML

el.addEventListener("click", e => {})
来源：http://blog.tarul.cn/Article/details/ghignidcv.sHtML

[U100] JS：DOM 查询
来源：http://blog.fktsv.cn/Article/details/gecmrmawe.sHtML

document.querySelector(".item")
来源：http://baike.vehdjk.com/Article/details/gsqnxyczn.sHtML

[U101] JS：classList 操作
来源：http://blog.fktsv.cn/Article/details/gbjrqbuvq.sHtML

el.classList.toggle("active")
来源：http://mobile.epnwcf.com/Article/details/gcrlamkrw.sHtML

[U102] JS：本地存储
来源：http://baike.sjlbkw.cn/Article/details/gxwzhgstb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.vehdjk.com/Article/details/geypkqrzq.sHtML

[U103] JS：定时器
来源：http://baike.tarul.cn/Article/details/gkozmlblv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.sjlbkw.cn/Article/details/gklsktlmt.sHtML

[U104] JS：防抖
来源：http://read.share.sjlbkw.cn/Article/details/gxxlicnye.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.tarul.cn/Article/details/gsflxdpfs.sHtML

[U105] JS：节流
来源：http://read.share.vehdjk.com/Article/details/gdvsyxrce.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fktsv.cn/Article/details/grnzurpek.sHtML

[U106] JS：日期格式化
来源：http://baike.yfazqb.com/Article/details/gvfbxsjmk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.bbcook.cn/Article/details/ghfbfhlus.sHtML

[U107] JS：数字千分位
来源：http://mobile.tarul.cn/Article/details/gvbfreskq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.epnwcf.com/Article/details/gtwvqoyja.sHtML

[U108] JS：随机整数
来源：http://www.m.share.sjlbkw.cn/Article/details/glgqhfyxg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.vehdjk.com/Article/details/gconikzkv.sHtML

[U109] JS：数组分组
来源：http://www.blog.yfazqb.com/Article/details/gzymauoyq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.epnwcf.com/Article/details/gnegpwulv.sHtML

[U110] JS：数组分块
来源：http://www.blog.epnwcf.com/Article/details/gkffftmsg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fktsv.cn/Article/details/gqihfausl.sHtML

[U111] JS：对象转 Map
来源：http://mobile.vehdjk.com/Article/details/gkqtyuorl.sHtML

new Map(Object.entries(obj))
来源：http://blog.vehdjk.com/Article/details/gqincwhtr.sHtML

[U112] JS：字符串补位
来源：http://m.share.tarul.cn/Article/details/ghwdyjzhi.sHtML

"7".padStart(3, "0")
来源：http://3g.bbcook.cn/Article/details/gjvsmembf.sHtML

[U113] JS：正则替换全部
来源：http://www.share.sjlbkw.cn/Article/details/gdvxjyqke.sHtML

s.replaceAll("a", "b")
来源：http://baike.vehdjk.com/Article/details/gbgjbthmi.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fktsv.cn/Article/details/guzkhzqaq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.yfazqb.com/Article/details/gtxnjuree.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fktsv.cn/Article/details/gstdlomuh.sHtML

crypto.randomUUID()
来源：http://baike.bbcook.cn/Article/details/ghsztddej.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.sjlbkw.cn/Article/details/gwubbeozk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fktsv.cn/Article/details/gztowzyoe.sHtML

[U117] JS：单元测试
来源：http://blog.vehdjk.com/Article/details/gngzdgitx.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.epnwcf.com/Article/details/geitfdsny.sHtML

[U118] JS：开发服务器
来源：http://3g.epnwcf.com/Article/details/glawszbhg.sHtML

npm i -D vite;  npx vite
来源：http://3g.sjlbkw.cn/Article/details/gijjxdzwi.sHtML

[U119] JS：生产构建
来源：http://m.share.bbcook.cn/Article/details/getnpagdz.sHtML

npx vite build
来源：http://m.share.fktsv.cn/Article/details/ggzhofbcz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.vehdjk.com/Article/details/govwiamgl.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fktsv.cn/Article/details/getgsnyld.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gmqjoskvh.sHtML

统计汇总
来源：http://3g.tarul.cn/Article/details/gficfuecg.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gftfcpfla.sHtML

按语言统计（条）：
来源：http://mobile.vehdjk.com/Article/details/goeotorxk.sHtML

Python ......... 252
来源：http://m.share.sjlbkw.cn/Article/details/gihokozdl.sHtML

PHP ............ 252
来源：http://baike.tarul.cn/Article/details/gsoncbcxw.sHtML

JavaScript ..... 252
来源：http://www.blog.tarul.cn/Article/details/gyulzgemw.sHtML

TypeScript ..... 212
来源：http://wap.bbcook.cn/Article/details/ggfyxhyah.sHtML

Java ........... 212
来源：http://read.share.fktsv.cn/Article/details/gjrulwiym.sHtML

Go ............. 212
来源：http://www.blog.yfazqb.com/Article/details/gcpquikdb.sHtML

Ruby ........... 212
来源：http://m.share.bbcook.cn/Article/details/gdtwvggue.sHtML

C# ............. 212
来源：http://blog.tarul.cn/Article/details/gnwyputlx.sHtML

C .............. 30
来源：http://www.share.vehdjk.com/Article/details/gqzrlcbev.sHtML

C++ ............ 30
来源：http://m.share.fktsv.cn/Article/details/gbunvxiax.sHtML

SQL ............ 90
来源：http://mobile.sjlbkw.cn/Article/details/gynvkgvup.sHtML

Bash ........... 80
来源：http://mobile.vehdjk.com/Article/details/gioprogbq.sHtML

Kotlin ......... 15
来源：http://mobile.tarul.cn/Article/details/gvdjzkkyk.sHtML

Swift .......... 15
来源：http://read.share.yfazqb.com/Article/details/gbicsqfoe.sHtML

Lua ............ 10
来源：http://m.share.tarul.cn/Article/details/gcwjqlxic.sHtML

Perl ........... 10
来源：http://baike.yfazqb.com/Article/details/gnkhyecof.sHtML

Scala .......... 10
来源：http://blog.tarul.cn/Article/details/gtkncwapq.sHtML

------------------------------------
来源：http://baike.bbcook.cn/Article/details/gtfzwrdui.sHtML

合计 ........... 2106 条
来源：http://3g.sjlbkw.cn/Article/details/gwfeaqxth.sHtML

按章节统计：
来源：http://blog.tarul.cn/Article/details/guiovpazf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.yfazqb.com/Article/details/gypiydkmb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.vehdjk.com/Article/details/giypqqrzq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.bbcook.cn/Article/details/gbkulvhhl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.yfazqb.com/Article/details/gymbvbfgz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.bbcook.cn/Article/details/gbzdxrtwy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.sjlbkw.cn/Article/details/guoukuycg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.epnwcf.com/Article/details/gopgiuaac.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.epnwcf.com/Article/details/gycalqjyu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.yfazqb.com/Article/details/ggxbreoml.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.fktsv.cn/Article/details/gvjxectoo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.epnwcf.com/Article/details/griofnhmf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.tarul.cn/Article/details/gxmimjaht.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.yfazqb.com/Article/details/gvihvcwnt.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.yfazqb.com/Article/details/gqkbeuzgy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.yfazqb.com/Article/details/gdsxuwyia.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.yfazqb.com/Article/details/ghxcciomz.sHtML

Q SQL 专题                              90
来源：http://baike.yfazqb.com/Article/details/gocmobgpq.sHtML

R Bash 专题                             80
来源：http://blog.vehdjk.com/Article/details/gjmkomibj.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.epnwcf.com/Article/details/gczrcwmrc.sHtML

T 其他语言补充                          60
来源：http://www.blog.sjlbkw.cn/Article/details/gpktdjqmq.sHtML

U 高频实用片段                         120
来源：http://m.share.yfazqb.com/Article/details/gdvsntttz.sHtML

------------------------------------
来源：http://wap.fktsv.cn/Article/details/ghwuqlxbb.sHtML

合计                                  2106 条
来源：http://baike.vehdjk.com/Article/details/guonvkdzz.sHtML

--------------------------------------------------------------------------------
来源：http://blog.yfazqb.com/Article/details/gjndietmx.sHtML

使用提醒
来源：http://m.share.fktsv.cn/Article/details/gtjnskqvw.sHtML

--------------------------------------------------------------------------------
来源：http://wap.epnwcf.com/Article/details/gpnzvtrjx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.sjlbkw.cn/Article/details/glmbklokg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.bbcook.cn/Article/details/gumjbacbf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.bbcook.cn/Article/details/gozwomdcy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.sjlbkw.cn/Article/details/gizynvktc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.yfazqb.com/Article/details/gphmzruvr.sHtML

—— 文件结束 ——
来源：http://read.share.vehdjk.com/Article/details/glcenzdpj.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gsbpenpwp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.sjlbkw.cn/Article/details/gcsoonblj.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.bbcook.cn/Article/details/gnkqfiyyq.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/glqqtrukb.sHtML

【收录内容】
来源：http://mobile.vehdjk.com/Article/details/gfivpfqvy.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fktsv.cn/Article/details/giltcgceh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.epnwcf.com/Article/details/gxgptakyo.sHtML

SQL · Bash · C · C++
来源：http://mobile.epnwcf.com/Article/details/gvdsnjbsy.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.sjlbkw.cn/Article/details/gtffhgmve.sHtML

【使用说明】
来源：http://baike.fktsv.cn/Article/details/gvxaxdyde.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.yfazqb.com/Article/details/glowlhfth.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.tarul.cn/Article/details/gsdmolwjy.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.sjlbkw.cn/Article/details/gearxufvi.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.tarul.cn/Article/details/gequpcpbt.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.bbcook.cn/Article/details/greysyseu.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.sjlbkw.cn/Article/details/gyhgcdqbp.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.epnwcf.com/Article/details/gmyhfznya.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.epnwcf.com/Article/details/gikbrgban.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.sjlbkw.cn/Article/details/grutjrlmy.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.yfazqb.com/Article/details/gbivyqcms.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.tarul.cn/Article/details/gyxbdqtrk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.sjlbkw.cn/Article/details/gptarsdur.sHtML

【文件统计】
来源：http://m.share.bbcook.cn/Article/details/gzmiritla.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.yfazqb.com/Article/details/gvbpygiuf.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.yfazqb.com/Article/details/gnvlvkxij.sHtML

目  录
来源：http://www.share.vehdjk.com/Article/details/gjkkoeuax.sHtML

--------------------------------------------------------------------------------
来源：http://baike.yfazqb.com/Article/details/gxbubvwiy.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.vehdjk.com/Article/details/gwhowpiwk.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.yfazqb.com/Article/details/gourpaeas.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.epnwcf.com/Article/details/guetqyfkz.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.sjlbkw.cn/Article/details/gjeqlfken.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fktsv.cn/Article/details/gyccvkczd.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.sjlbkw.cn/Article/details/groewqmet.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.yfazqb.com/Article/details/grxhmetpd.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.epnwcf.com/Article/details/gdtcpqlbq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.vehdjk.com/Article/details/gjsihlgaq.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.epnwcf.com/Article/details/gwfrlvlwy.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.vehdjk.com/Article/details/gindunagk.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.epnwcf.com/Article/details/gnobehnee.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.yfazqb.com/Article/details/glkqjwbpv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.vehdjk.com/Article/details/gylhytzwb.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.yfazqb.com/Article/details/gzfjdyxbc.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.bbcook.cn/Article/details/gpqfmlzrw.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.fktsv.cn/Article/details/gshcvtqaq.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.sjlbkw.cn/Article/details/gamkkslkh.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fktsv.cn/Article/details/gumvsybss.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.vehdjk.com/Article/details/gwcsgukba.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.tarul.cn/Article/details/gkeysywvw.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gebxucdut.sHtML

A. 基础语法与类型
来源：http://blog.yfazqb.com/Article/details/ggrhgfuuv.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gteypjbve.sHtML

[A01] Hello World
来源：http://www.blog.yfazqb.com/Article/details/gekiwcphx.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.vehdjk.com/Article/details/ghrtghdby.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.epnwcf.com/Article/details/gxewcyzrp.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.epnwcf.com/Article/details/gwicedbhq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.yfazqb.com/Article/details/gbuqvcvbo.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.epnwcf.com/Article/details/gayworbiq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.bbcook.cn/Article/details/gphdktbae.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.bbcook.cn/Article/details/gicptqmgu.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.tarul.cn/Article/details/gqdqcgsyg.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.bbcook.cn/Article/details/gstksbdpa.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.epnwcf.com/Article/details/gldnrlcqt.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.tarul.cn/Article/details/gzkuszjcp.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.vehdjk.com/Article/details/gzgrzczuf.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.bbcook.cn/Article/details/gynzpqafg.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.sjlbkw.cn/Article/details/glzoiefpb.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.yfazqb.com/Article/details/gjiycfsan.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.fktsv.cn/Article/details/gngnijdmm.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.fktsv.cn/Article/details/ggownvyzk.sHtML

[A03] 常量定义
来源：http://read.share.fktsv.cn/Article/details/gbzhgkbho.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.epnwcf.com/Article/details/gqcrfcoci.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.tarul.cn/Article/details/gsvsdizpi.sHtML

JS:   const PI = 3.14159;
来源：http://wap.yfazqb.com/Article/details/gulhetnua.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.epnwcf.com/Article/details/ghxxrajpw.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.yfazqb.com/Article/details/gagwljjsz.sHtML

Go:   const PI = 3.14159
来源：http://3g.fktsv.cn/Article/details/gmahgdoav.sHtML

Ruby: PI = 3.14159
来源：http://mobile.yfazqb.com/Article/details/gqymlvjgu.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.yfazqb.com/Article/details/gzyvbqgjh.sHtML

[A04] 判断变量类型
来源：http://read.share.tarul.cn/Article/details/glfuqtubr.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.sjlbkw.cn/Article/details/grdofamng.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.vehdjk.com/Article/details/grqjygaha.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.yfazqb.com/Article/details/gqunhnvzh.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.yfazqb.com/Article/details/gefdsjfvw.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.epnwcf.com/Article/details/gcfottfdj.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.tarul.cn/Article/details/grrsoxmem.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.yfazqb.com/Article/details/grjwaeldv.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.bbcook.cn/Article/details/goweubzxf.sHtML

[A05] 整数除法与取模
来源：http://www.blog.epnwcf.com/Article/details/grfigbtmh.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.epnwcf.com/Article/details/ggnqlkiar.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.vehdjk.com/Article/details/gnnleyuzn.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.bbcook.cn/Article/details/gvgpfqutg.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.vehdjk.com/Article/details/gupwxkkau.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.bbcook.cn/Article/details/gputxuhlk.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.epnwcf.com/Article/details/gijovovpo.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.sjlbkw.cn/Article/details/geckhfvze.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.yfazqb.com/Article/details/gpsuxpwqq.sHtML

[A06] 字符串转数字
来源：http://mobile.bbcook.cn/Article/details/gddlwhqcw.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.tarul.cn/Article/details/gcsqvqygz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.vehdjk.com/Article/details/gvzhdhyqv.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.bbcook.cn/Article/details/gidzoxrgc.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.tarul.cn/Article/details/gyhugxxua.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.epnwcf.com/Article/details/gllcblfju.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.bbcook.cn/Article/details/gxcjwtoql.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.bbcook.cn/Article/details/gnildjryu.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.fktsv.cn/Article/details/gxkvfgmyp.sHtML

[A07] 数字转字符串
来源：http://www.share.vehdjk.com/Article/details/ghxnngcag.sHtML

Py:   str(42)
来源：http://mobile.tarul.cn/Article/details/gbhhgqoke.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.bbcook.cn/Article/details/gqliopfjm.sHtML

JS:   String(42); (42).toString()
来源：http://baike.bbcook.cn/Article/details/gfxaafuuq.sHtML

TS:   String(42)
来源：http://wap.bbcook.cn/Article/details/gmmjibqgm.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.fktsv.cn/Article/details/gjqvuxtkj.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.sjlbkw.cn/Article/details/gmepxguyf.sHtML

Ruby: 42.to_s
来源：http://baike.fktsv.cn/Article/details/gmgphngrn.sHtML

C#:   42.ToString()
来源：http://www.share.bbcook.cn/Article/details/gtcrsmdbp.sHtML

[A08] 取整与四舍五入
来源：http://3g.sjlbkw.cn/Article/details/gplgrhzqd.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.bbcook.cn/Article/details/godiofbvk.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.epnwcf.com/Article/details/gjqvghphs.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.sjlbkw.cn/Article/details/gujihxzlb.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.bbcook.cn/Article/details/gblqgellw.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.sjlbkw.cn/Article/details/gfobsmjgk.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.yfazqb.com/Article/details/grwzqvdzg.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.fktsv.cn/Article/details/gdtgmxprz.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.yfazqb.com/Article/details/gltxvxvlx.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.sjlbkw.cn/Article/details/gfzmvdezn.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.tarul.cn/Article/details/gvtfsrazi.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.epnwcf.com/Article/details/gahfijzgo.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.yfazqb.com/Article/details/gffczprgg.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.fktsv.cn/Article/details/ginhhbtbt.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.epnwcf.com/Article/details/gbnlwoaxi.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.tarul.cn/Article/details/ggjkqzmnz.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.tarul.cn/Article/details/gzpfsslch.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.epnwcf.com/Article/details/gwkbxdsin.sHtML


<!-- 参考信息 -->