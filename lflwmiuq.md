代发 wailian999

[U55] PHP：match 表达式
来源：http://saz.zycfv.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sra.daxiang520.top

[U56] PHP：命名参数
来源：http://ejc.yj20258.top

f(a: 1, b: 2)
来源：http://drx.zhijiandao.cn

[U57] PHP：字符串插值
来源：http://hvm.zhixingplan.top

"值: {$a}"
来源：http://cdh.feifeiyinyue.top

[U58] PHP：数组三件套
来源：http://rki.hfpthk.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://hxg.mhx1999.top

[U59] PHP：自定义排序
来源：http://gkd.zhaomingkeji.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pzg.zhixingplan.top

[U60] PHP：JSON 编解码
来源：http://aip.jinqigfzy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nst.sjlbkw.cn

[U61] PHP：正则
来源：http://orp.uphjek.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ylw.bbcook.cn

[U62] PHP：日期对象
来源：http://sno.yvedp.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uid.iojbl.cn

[U63] PHP：文件读写
来源：http://ldp.svipenyu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wum.aizwys.cn

[U64] PHP：目录遍历
来源：http://bqg.ywan-chungtsiang.top

glob("dir/*.php");  scandir("dir");
来源：http://zbm.nanxinkj.top

[U65] PHP：会话
来源：http://vko.fktsv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://hpv.xinyue.icu

[U66] PHP：设置 Cookie
来源：http://bqo.epnwcf.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://srl.hongshengwenyu.top

[U67] PHP：处理文件上传
来源：http://okg.jinqigufen.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://idm.daxiang520.top

[U68] PHP：PDO 连接
来源：http://egb.yj20258888.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nlk.sweek.top

[U69] PHP：PDO 预处理
来源：http://slb.chenjidiqi.icu

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://whg.zhixingplan.top

[U70] PHP：PDO 事务
来源：http://kgx.haohaochexian.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://weh.yuanzhike.top

[U71] PHP：抛出异常
来源：http://bvk.ydzc1.top

throw new RuntimeException("失败", 500);
来源：http://cde.ehwqpu.com

[U72] PHP：写错误日志
来源：http://lbk.zhixingplan.top

error_log("失败: " . $e->getMessage());
来源：http://eft.tanke756.top

[U73] PHP：读取 ini 配置
来源：http://hpc.shanyushiyangkeji.top

parse_ini_file("config.ini", true)
来源：http://zga.9152youxi.cn

[U74] PHP：读取环境变量
来源：http://nsy.hammf.cn

getenv("APP_ENV") ?: "production"
来源：http://nej.zhijiandao.cn

[U75] PHP：依赖注入
来源：http://cyf.aizwys.cn

composer require psr/container
来源：http://lvs.iojbl.cn

[U76] PHP：简单路由
来源：http://kzj.hnxiangtu.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vob.yuanzhike.top

[U77] PHP：模板渲染
来源：http://cnw.jyoumei.cn

composer require twig/twig
来源：http://qqx.jyoumei.cn

[U78] PHP：单元测试
来源：http://vcq.hywenlv.cn

composer require --dev phpunit/phpunit
来源：http://hxi.epnwcf.com

[U79] PHP：静态分析
来源：http://adu.uphjek.com

composer require --dev phpstan/phpstan
来源：http://civ.dashuyun.cn

[U80] PHP：代码规范修复
来源：http://sck.iojbl.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://sge.gzhubu.top

[U81] JS：初始化项目
来源：http://rcx.smart0.xyz

npm init -y;  npm i express
来源：http://uuq.epnwcf.com

[U82] JS：package.json 脚本
来源：http://gtk.sxryk.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://krb.jinghuilouyu.cn

[U83] JS：ES Module 导入导出
来源：http://gdu.nanxinkj.top

export const a = 1;  import { a } from "./m.js";
来源：http://udf.xuanzx.com

[U84] JS：CommonJS 写法
来源：http://npy.ivvv.top

module.exports = { a };  const { a } = require("./m");
来源：http://tla.xuetiantiany.cn

[U85] JS：可选链
来源：http://orw.yonumen.top

a?.b?.c
来源：http://qya.shuidangran.top

[U86] JS：空值合并
来源：http://bbh.fanxiaobao.xyz

a ?? b
来源：http://auy.havefunace.top

[U87] JS：解构默认值
来源：http://odl.sufxvd.cn

const { a = 1, b = 2 } = obj;
来源：http://rzh.ehwqpu.com

[U88] JS：对象展开合并
来源：http://vim.ppjwa.cn

{ ...a, ...b }
来源：http://vve.sufxvd.cn

[U89] JS：数组去重
来源：http://eru.hysaishi.cn

[...new Set(arr)]
来源：http://adm.jinqigufen.top

[U90] JS：数字数组排序
来源：http://cuj.xylfe.cn

[...arr].sort((a, b) => a - b)
来源：http://fpb.dianchejie.cn

[U91] JS：对象键值遍历
来源：http://eky.bbcook.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://hbf.xingfuxueyuan.xyz

[U92] JS：深拷贝
来源：http://zyc.tanke756.top

structuredClone(obj)
来源：http://etb.sysykeji.top

[U93] JS：模板字符串
来源：http://fxl.mhx1999.top

`共 ${n} 条`
来源：http://fbm.fengsongda.top

[U94] JS：箭头函数
来源：http://joh.yueranfly.top

const double = x => x * 2;
来源：http://vsw.zhoulong.xyz

[U95] JS：Promise 包装
来源：http://vgm.hnqzz.top

new Promise((resolve, reject) => {})
来源：http://dbi.hysaishi.cn

[U96] JS：async/await 与异常
来源：http://cfg.daria6918.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qvl.jlsjyb.cn

[U97] JS：并发请求
来源：http://ksa.smart0.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://nab.9152youxi.cn

[U98] JS：fetch 带 JSON
来源：http://hdw.iojbl.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://roo.cucudq.cn

[U99] JS：事件监听
来源：http://ynb.epnwcf.com

el.addEventListener("click", e => {})
来源：http://kqr.zdqjudy.top

[U100] JS：DOM 查询
来源：http://fbh.snrcjt.cn

document.querySelector(".item")
来源：http://lsw.haohaochexian.top

[U101] JS：classList 操作
来源：http://qdv.svipenyu.cn

el.classList.toggle("active")
来源：http://mgg.fehbvm.com

[U102] JS：本地存储
来源：http://hfd.hysaishi.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://lbl.ivvv.top

[U103] JS：定时器
来源：http://ypu.cheryme.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://pto.hcnkem.com

[U104] JS：防抖
来源：http://isf.birdmap.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://znx.ppjwa.cn

[U105] JS：节流
来源：http://pul.guowangkeji.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://idh.daria6918.cn

[U106] JS：日期格式化
来源：http://esh.fanxiaobao.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://oyj.ivvv.top

[U107] JS：数字千分位
来源：http://gsi.aibaodan.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://pjj.cashguo.top

[U108] JS：随机整数
来源：http://ziq.bbcook.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://fjq.jlsjyb.cn

[U109] JS：数组分组
来源：http://khw.smart0.xyz

Object.groupBy(arr, x => x.type)
来源：http://ewf.316326.xyz

[U110] JS：数组分块
来源：http://uvq.yangfankeji.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://bwf.ehwqpu.com

[U111] JS：对象转 Map
来源：http://dli.jinqigfzy.top

new Map(Object.entries(obj))
来源：http://sxd.yj20258.top

[U112] JS：字符串补位
来源：http://vdm.sysykeji.top

"7".padStart(3, "0")
来源：http://fcb.sweek.top

[U113] JS：正则替换全部
来源：http://rci.hnxiangtu.top

s.replaceAll("a", "b")
来源：http://jtl.fanxiaobao.xyz

[U114] JS：JSON 深比较
来源：http://umk.ydjk.org.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://dqa.cashguo.top

[U115] JS：生成 UUID
来源：http://gwd.yuxming.cn

crypto.randomUUID()
来源：http://byn.bjfxy.top

[U116] JS：类型检查（JSDoc）
来源：http://oiw.sufxvd.cn

/** @param {string} name */ function f(name) {}
来源：http://jgk.ppjwa.cn

[U117] JS：单元测试
来源：http://zxx.xingfuxueyuan.xyz

npm i -D vitest;  npx vitest
来源：http://fio.jlsjyb.cn

[U118] JS：开发服务器
来源：http://ojq.0kj1m.cn

npm i -D vite;  npx vite
来源：http://ppg.jiagoushi.top

[U119] JS：生产构建
来源：http://gpl.wangdashe.top

npx vite build
来源：http://xqh.uphjek.com

[U120] JS：读取环境变量（Vite）
来源：http://vua.ybcxt.top

import.meta.env.VITE_API_URL
来源：http://hxl.ydzc1.top

================================================================================
来源：http://feg.fehbvm.com

统计汇总
来源：http://rdj.hesvh.cn

================================================================================
来源：http://bwo.yfazqb.com

按语言统计（条）：
来源：http://eew.shanyushiyangkeji.top

Python ......... 252
来源：http://mlx.yuanzhike.top

PHP ............ 252
来源：http://qek.ehwqpu.com

JavaScript ..... 252
来源：http://bdc.shanyushiyangtech.top

TypeScript ..... 212
来源：http://ust.hywenlv.cn

Java ........... 212
来源：http://ftr.hfpthk.cn

Go ............. 212
来源：http://liz.yongpay.top

Ruby ........... 212
来源：http://xos.xziqi.cn

C# ............. 212
来源：http://kiw.shanyushiyangtech.top

C .............. 30
来源：http://wuk.yongpay.top

C++ ............ 30
来源：http://qve.zhijiandao.cn

SQL ............ 90
来源：http://shx.tianlin.xyz

Bash ........... 80
来源：http://seu.yj20258.top

Kotlin ......... 15
来源：http://iih.xylfe.cn

Swift .......... 15
来源：http://bln.0kj1m.cn

Lua ............ 10
来源：http://ccb.chenzaomai.com

Perl ........... 10
来源：http://kta.guowangkeji.top

Scala .......... 10
来源：http://wru.fzhhl.top

------------------------------------
来源：http://ran.yanxiufei.cn

合计 ........... 2106 条
来源：http://zou.meibo888.top

按章节统计：
来源：http://evq.jlsjyb.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://bqe.gotoacloud.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tki.iojbl.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://oea.zdqjudy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://usl.zhijiandao.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ahy.fehbvm.com

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://eoz.fanxiaobao.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://irz.jiagoushi.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://abf.feifeiyinyue.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://igr.gaohongyu789.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://lfv.yfazqb.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://tdc.yueranfly.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://iwt.bjfxy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zqf.mhx1999.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://phl.xziqi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://szw.ehwqpu.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://aul.tarul.cn

Q SQL 专题                              90
来源：http://gjn.xuetiantiany.cn

R Bash 专题                             80
来源：http://mqj.hfpthk.cn

S C / C++ 专题                          60
来源：http://pdm.zhoulong.xyz

T 其他语言补充                          60
来源：http://kbo.daria6918.cn

U 高频实用片段                         120
来源：http://oei.ydjk.org.cn

------------------------------------
来源：http://wdz.zhixingplan.top

合计                                  2106 条
来源：http://yhr.0kj1m.cn

--------------------------------------------------------------------------------
来源：http://ukk.sjlbkw.cn

使用提醒
来源：http://eil.gaohongyu789.top

--------------------------------------------------------------------------------
来源：http://gcr.yj20258888.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://shj.tanke756.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ixu.tianlin.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://orz.uphjek.com

在旧版本上使用前请先确认语法支持情况。
来源：http://zyi.jiagoushi.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lbe.tanke756.top

—— 文件结束 ——
来源：http://civ.havefunace.top

================================================================================
来源：http://agv.snrcjt.cn

程序语言常见例子速查手册（2024 版）
来源：http://mca.tianlin.xyz

Common Programming Examples Cheat Book
来源：http://kfm.gogol.net.cn

================================================================================
来源：http://krt.zhiwuduotai.top

【收录内容】
来源：http://etn.tarul.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://xvl.xuanzx.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ovi.xuanzx.com

SQL · Bash · C · C++
来源：http://jcx.yuxming.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://nuu.gaohongyu789.top

【使用说明】
来源：http://ksv.quarkkingdee.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lxt.zhiwuduotai.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qrx.ivvv.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://upf.vehdjk.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rcd.epnwcf.com

Bash:  Shell         C:     C             C++:   C++
来源：http://vti.yongpay.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xff.yonumen.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://llu.cheryme.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://ehx.ctjpmb.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ozf.daxiang520.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nxv.quarkkingdee.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mfk.52xcode.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://upi.ydzc1.top

【文件统计】
来源：http://sis.sjlbkw.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tox.ctjpmb.com

--------------------------------------------------------------------------------
来源：http://qfq.svipenyu.cn

目  录
来源：http://kon.snrcjt.cn

--------------------------------------------------------------------------------
来源：http://puu.vehdjk.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ave.jianghu66.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://obh.zhixingplan.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://rzh.fehbvm.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nzg.gotoacloud.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hug.shuidangran.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wef.yj20258888.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ork.dianchejie.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://vwf.bjfxy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tmp.shanyushiyangkeji.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://czu.zhoulong.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://qsg.fanxiaobao.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://agt.meibo888.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://qll.feifeiyinyue.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://oqm.snrcjt.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://hyk.ehwqpu.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cay.ivvv.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ulh.nwbrower.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://azg.fktsv.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://aek.52xcode.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://shp.jqgfzy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://thh.c1oappe.top

================================================================================
来源：http://cvn.xziqi.cn

A. 基础语法与类型
来源：http://pht.jyoumei.cn

================================================================================
来源：http://kzr.tianlin.xyz

[A01] Hello World
来源：http://mmi.yvedp.cn

Py:   print("Hello, World!")
来源：http://uou.yj20258888.top

PHP:  echo "Hello, World!";
来源：http://efw.zhijiandao.cn

JS:   console.log("Hello, World!");
来源：http://vkr.zhijiandao.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://lsd.daria6918.cn

Java: System.out.println("Hello, World!");
来源：http://sqm.snrcjt.cn

Go:   fmt.Println("Hello, World!")
来源：http://rkq.vqdsnc.cn

Ruby: puts "Hello, World!"
来源：http://ydt.sysykeji.top

C#:   Console.WriteLine("Hello, World!");
来源：http://mui.jinyuanbaomall.cn

[A02] 变量声明与赋值
来源：http://uzg.gogol.net.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://uys.xingfuxueyuan.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://fmx.nanxuanxn.top

JS:   let name = "Alex"; const age = 20;
来源：http://eqz.shuidangran.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ued.iojbl.cn

Java: String name = "Alex"; int age = 20;
来源：http://uvc.yj20258888.top

Go:   name := "Alex"; age := 20
来源：http://fep.birdmap.top

Ruby: name = "Alex"; age = 20
来源：http://akv.hysaishi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://bgi.yj20258888.top

[A03] 常量定义
来源：http://smq.pycfn.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fxb.pengpengdd.cyou

PHP:  const PI = 3.14159;
来源：http://jzm.yanxiufei.cn

JS:   const PI = 3.14159;
来源：http://csh.hnxiangtu.top

TS:   const PI: number = 3.14159;
来源：http://tzs.cheryme.top

Java: static final double PI = 3.14159;
来源：http://lfo.ydzc1.top

Go:   const PI = 3.14159
来源：http://jxp.cucudq.cn

Ruby: PI = 3.14159
来源：http://apj.gaohongyu789.top

C#:   const double PI = 3.14159;
来源：http://fch.yj20258888.top

[A04] 判断变量类型
来源：http://rqs.jyoumei.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://qdm.sjlbkw.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://rem.shanyushiyangkeji.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://sop.xylfe.cn

TS:   typeof x; x instanceof Date
来源：http://pnz.redwolf501.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wzb.tian-w.cn

Go:   reflect.TypeOf(x).Name()
来源：http://iuf.meibo888.top

Ruby: x.class; x.is_a?(Integer)
来源：http://lom.uphjek.com

C#:   x.GetType().Name; x is int
来源：http://mnp.aizwys.cn

[A05] 整数除法与取模
来源：http://hfd.hammf.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xjr.ppjwa.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://gti.haohaochexian.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://oyx.vqdsnc.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://bss.xylfe.cn

Java: 7 / 2; 7 % 2
来源：http://ube.yanxiufei.cn

Go:   7 / 2; 7 % 2
来源：http://efd.snrcjt.cn

Ruby: 7 / 2; 7 % 2
来源：http://uij.daxiang520.top

C#:   7 / 2; 7 % 2
来源：http://vdx.jinqigfzy.top

[A06] 字符串转数字
来源：http://sml.c1oappe.top

Py:   int("42"); float("3.14")
来源：http://dtp.shangyingyoupin.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://aak.fengsongda.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pcm.haohaochexian.top

TS:   parseInt("42", 10); Number("42")
来源：http://naj.bjfxy.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://irz.gogol.net.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://jua.smart0.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://ykh.yj202588.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://adq.bbcook.cn

[A07] 数字转字符串
来源：http://ugw.wangshuangyany.cn

Py:   str(42)
来源：http://okq.dianchejie.cn

PHP:  (string) 42; strval(42)
来源：http://cwh.pycfn.com

JS:   String(42); (42).toString()
来源：http://npo.hammf.cn

TS:   String(42)
来源：http://mhv.yfazqb.com

Java: String.valueOf(42); Integer.toString(42)
来源：http://nek.ybcxt.top

Go:   strconv.Itoa(42)
来源：http://xdv.fanxiaobao.xyz


<!-- 参考信息 -->