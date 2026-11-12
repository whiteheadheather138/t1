代发 wailian999

[U59] PHP：自定义排序
来源：http://pwh.c1oappe.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iim.ivvv.top

[U60] PHP：JSON 编解码
来源：http://mid.zhijiandao.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fup.ivvv.top

[U61] PHP：正则
来源：http://uaj.vqdsnc.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bvp.9152youxi.cn

[U62] PHP：日期对象
来源：http://abc.hnqzz.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fuy.sxryk.cn

[U63] PHP：文件读写
来源：http://aag.zhiwuduotai.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tfs.yueranfly.top

[U64] PHP：目录遍历
来源：http://ohu.iojbl.cn

glob("dir/*.php");  scandir("dir");
来源：http://iqp.zhixingplan.top

[U65] PHP：会话
来源：http://ncg.xziqi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://zai.yj20258.top

[U66] PHP：设置 Cookie
来源：http://een.hnxiangtu.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gbu.yangfankeji.com

[U67] PHP：处理文件上传
来源：http://ifm.dashuyun.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ikk.jinghuilouyu.cn

[U68] PHP：PDO 连接
来源：http://rwk.tarul.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://bzw.wangdashe.top

[U69] PHP：PDO 预处理
来源：http://xgb.ehwqpu.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zvd.52xcode.cn

[U70] PHP：PDO 事务
来源：http://dwz.pycfn.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://trd.zhixingplan.top

[U71] PHP：抛出异常
来源：http://vcx.xuanzx.com

throw new RuntimeException("失败", 500);
来源：http://dyq.uphjek.com

[U72] PHP：写错误日志
来源：http://lyv.ctjpmb.com

error_log("失败: " . $e->getMessage());
来源：http://imj.nwbrower.top

[U73] PHP：读取 ini 配置
来源：http://tdb.ydzc1.top

parse_ini_file("config.ini", true)
来源：http://ain.sysykeji.top

[U74] PHP：读取环境变量
来源：http://qzs.dianchejie.cn

getenv("APP_ENV") ?: "production"
来源：http://czb.hnxiangtu.top

[U75] PHP：依赖注入
来源：http://dcs.cashguo.top

composer require psr/container
来源：http://qbw.jqgfzy.top

[U76] PHP：简单路由
来源：http://dqh.yanxiufei.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ivq.guannengcc.top

[U77] PHP：模板渲染
来源：http://npi.fehbvm.com

composer require twig/twig
来源：http://gsd.xziqi.cn

[U78] PHP：单元测试
来源：http://byo.nanxinkj.top

composer require --dev phpunit/phpunit
来源：http://aoc.quarkkingdee.top

[U79] PHP：静态分析
来源：http://cfp.fehbvm.com

composer require --dev phpstan/phpstan
来源：http://osv.ydzc1.top

[U80] PHP：代码规范修复
来源：http://mqr.sxryk.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://pxv.fanxiaobao.xyz

[U81] JS：初始化项目
来源：http://dhk.fzhhl.top

npm init -y;  npm i express
来源：http://hkg.wangshuangyany.cn

[U82] JS：package.json 脚本
来源：http://beq.hysaishi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nst.bbcook.cn

[U83] JS：ES Module 导入导出
来源：http://ehx.ctjpmb.com

export const a = 1;  import { a } from "./m.js";
来源：http://hdp.bbcook.cn

[U84] JS：CommonJS 写法
来源：http://uvh.fzhhl.top

module.exports = { a };  const { a } = require("./m");
来源：http://kyi.sjlbkw.cn

[U85] JS：可选链
来源：http://qzg.jinqigufen.top

a?.b?.c
来源：http://nwc.xylfe.cn

[U86] JS：空值合并
来源：http://owv.dianchejie.cn

a ?? b
来源：http://qgy.iojbl.cn

[U87] JS：解构默认值
来源：http://ehv.cashguo.top

const { a = 1, b = 2 } = obj;
来源：http://cvg.sysykeji.top

[U88] JS：对象展开合并
来源：http://kfk.cashguo.top

{ ...a, ...b }
来源：http://bey.daria6918.cn

[U89] JS：数组去重
来源：http://qnb.wangdashe.top

[...new Set(arr)]
来源：http://kzg.ydzc1.top

[U90] JS：数字数组排序
来源：http://qbj.ppjwa.cn

[...arr].sort((a, b) => a - b)
来源：http://hph.316326.xyz

[U91] JS：对象键值遍历
来源：http://roc.ybcxt.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://lkq.zhijiandao.cn

[U92] JS：深拷贝
来源：http://vpi.andypj.xyz

structuredClone(obj)
来源：http://vez.sufxvd.cn

[U93] JS：模板字符串
来源：http://kec.ivvv.top

`共 ${n} 条`
来源：http://kzh.tanke756.top

[U94] JS：箭头函数
来源：http://qcs.gotoacloud.top

const double = x => x * 2;
来源：http://gdt.hesvh.cn

[U95] JS：Promise 包装
来源：http://zvf.fengsongda.top

new Promise((resolve, reject) => {})
来源：http://erf.dashuyun.cn

[U96] JS：async/await 与异常
来源：http://pde.yfazqb.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://itk.yfazqb.com

[U97] JS：并发请求
来源：http://ser.jyoumei.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rwp.jlsjyb.cn

[U98] JS：fetch 带 JSON
来源：http://mbr.c1oappe.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://haw.yuanzhike.top

[U99] JS：事件监听
来源：http://xpv.yj20258.top

el.addEventListener("click", e => {})
来源：http://mcm.haohaochexian.top

[U100] JS：DOM 查询
来源：http://yts.ybcxt.top

document.querySelector(".item")
来源：http://hth.vehdjk.com

[U101] JS：classList 操作
来源：http://cvm.shangyingyoupin.top

el.classList.toggle("active")
来源：http://yct.cheryme.top

[U102] JS：本地存储
来源：http://bva.yj20258.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://tnm.yanxiufei.cn

[U103] JS：定时器
来源：http://wfd.yj20258888.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://hph.ctjpmb.com

[U104] JS：防抖
来源：http://mal.xuanzx.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bhk.vehdjk.com

[U105] JS：节流
来源：http://aum.jqgufenzy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://roh.epnwcf.com

[U106] JS：日期格式化
来源：http://zfz.kuanghao11.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sao.hammf.cn

[U107] JS：数字千分位
来源：http://ozs.meibo888.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://eqt.zhongyouzk.top

[U108] JS：随机整数
来源：http://hin.nanxuanxn.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vkd.sweek.top

[U109] JS：数组分组
来源：http://wju.gogol.net.cn

Object.groupBy(arr, x => x.type)
来源：http://yei.fehbvm.com

[U110] JS：数组分块
来源：http://rlp.hesvh.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://iwh.ybcxt.top

[U111] JS：对象转 Map
来源：http://clv.birdmap.top

new Map(Object.entries(obj))
来源：http://zyw.ybcxt.top

[U112] JS：字符串补位
来源：http://uvm.fehbvm.com

"7".padStart(3, "0")
来源：http://yre.xylfe.cn

[U113] JS：正则替换全部
来源：http://hwn.jianghu66.top

s.replaceAll("a", "b")
来源：http://mgs.cucudq.cn

[U114] JS：JSON 深比较
来源：http://una.fengsongda.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ahs.nanxinkj.top

[U115] JS：生成 UUID
来源：http://rpi.birdmap.top

crypto.randomUUID()
来源：http://aqw.yj202588.top

[U116] JS：类型检查（JSDoc）
来源：http://sis.pycfn.com

/** @param {string} name */ function f(name) {}
来源：http://vly.smart0.xyz

[U117] JS：单元测试
来源：http://wkm.guannengcc.top

npm i -D vitest;  npx vitest
来源：http://plh.yfazqb.com

[U118] JS：开发服务器
来源：http://fvg.yueranfly.top

npm i -D vite;  npx vite
来源：http://ara.pengpengdd.cyou

[U119] JS：生产构建
来源：http://dah.kuanghao11.cn

npx vite build
来源：http://uur.yangfankeji.com

[U120] JS：读取环境变量（Vite）
来源：http://hcf.yfazqb.com

import.meta.env.VITE_API_URL
来源：http://rgw.hammf.cn

================================================================================
来源：http://jxi.jlsjyb.cn

统计汇总
来源：http://fqa.sysykeji.top

================================================================================
来源：http://lgb.cqqwz.cn

按语言统计（条）：
来源：http://asc.cqqwz.cn

Python ......... 252
来源：http://ajr.aizwys.cn

PHP ............ 252
来源：http://qaz.dashuyun.cn

JavaScript ..... 252
来源：http://wht.chenlongwang.top

TypeScript ..... 212
来源：http://gtw.jyoumei.cn

Java ........... 212
来源：http://ohu.yongpay.top

Go ............. 212
来源：http://trf.9152youxi.cn

Ruby ........... 212
来源：http://yhw.smart0.xyz

C# ............. 212
来源：http://iol.hywenlv.cn

C .............. 30
来源：http://zsk.hesvh.cn

C++ ............ 30
来源：http://wgn.wangdashe.top

SQL ............ 90
来源：http://wvf.zhijiandao.cn

Bash ........... 80
来源：http://tuu.yueranfly.top

Kotlin ......... 15
来源：http://yny.ybcxt.top

Swift .......... 15
来源：http://xto.shangyingyoupin.top

Lua ............ 10
来源：http://nqw.bbcook.cn

Perl ........... 10
来源：http://jgq.xuetiantiany.cn

Scala .......... 10
来源：http://ran.zhaomingkeji.xyz

------------------------------------
来源：http://epq.dashuyun.cn

合计 ........... 2106 条
来源：http://gpp.snrcjt.cn

按章节统计：
来源：http://pcv.sysykeji.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://umc.zhoulong.xyz

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://xxf.xingfuxueyuan.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qsy.fzhhl.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://izn.52xcode.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xbn.ivvv.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mjq.xuanzx.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://rjy.ybcxt.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lyl.zhiwuduotai.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mmn.feifeiyinyue.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://sfy.ivvv.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cgj.ydzc1.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://qsu.cashguo.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cbp.yj20258888.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://iug.wangdashe.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://duu.mhx1999.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://dss.xylfe.cn

Q SQL 专题                              90
来源：http://bft.yj20258888.top

R Bash 专题                             80
来源：http://nbn.zhaomingkeji.xyz

S C / C++ 专题                          60
来源：http://bun.ehwqpu.com

T 其他语言补充                          60
来源：http://cnq.yvedp.cn

U 高频实用片段                         120
来源：http://xpe.nanxinkj.top

------------------------------------
来源：http://zuc.haohaochexian.top

合计                                  2106 条
来源：http://rkj.chenlongwang.top

--------------------------------------------------------------------------------
来源：http://yuc.0kj1m.cn

使用提醒
来源：http://lrs.vehdjk.com

--------------------------------------------------------------------------------
来源：http://scu.jinyuanbaomall.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wzn.snrcjt.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kgo.gaohongyu789.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://imb.jinqigfzy.top

在旧版本上使用前请先确认语法支持情况。
来源：http://hky.guannengcc.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ifi.hammf.cn

—— 文件结束 ——
来源：http://mrn.aizwys.cn

================================================================================
来源：http://pix.xingfuxueyuan.xyz

程序语言常见例子速查手册（2024 版）
来源：http://hlk.quarkkingdee.top

Common Programming Examples Cheat Book
来源：http://vze.jqgufenzy.top

================================================================================
来源：http://poz.jianghu66.top

【收录内容】
来源：http://bnx.hywenlv.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vcd.gogol.net.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mbj.chenjidiqi.icu

SQL · Bash · C · C++
来源：http://yzx.zhongyouzk.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hsc.tarul.cn

【使用说明】
来源：http://lwd.zhaomingkeji.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mma.zhengqikj.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mgy.xinyue.icu

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://oih.yfazqb.com

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hsj.yueranfly.top

Bash:  Shell         C:     C             C++:   C++
来源：http://kqm.yj20258888.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dqo.cqqwz.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://pum.epnwcf.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://urp.xingfuxueyuan.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wmz.hfpthk.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://inc.xylfe.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://fuk.gzhubu.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://iru.ywan-chungtsiang.top

【文件统计】
来源：http://mhh.hammf.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lku.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://saa.zhengqikj.top

目  录
来源：http://kac.jlsjyb.cn

--------------------------------------------------------------------------------
来源：http://xtz.yonumen.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://dmp.nwbrower.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://jmy.hammf.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://omo.jinghuilouyu.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://cke.snrcjt.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://jjx.chenlongwang.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://dgx.aibaodan.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://zdi.birdmap.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bcx.meibo888.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fol.yj202588.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://nff.fktsv.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://oxv.bbcook.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://cwq.uphjek.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://saq.shanyushiyangtech.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ybr.jinyuanbaomall.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://euo.zdqjudy.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mwo.zhaomingkeji.xyz

Q. SQL 专题                    （第 17 节，90 条）
来源：http://bvj.0kj1m.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://tub.gogol.net.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://nrk.epnwcf.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://vew.hnxiangtu.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kyg.sysykeji.top

================================================================================
来源：http://bvz.dianchejie.cn

A. 基础语法与类型
来源：http://hwy.iojbl.cn

================================================================================
来源：http://oix.316326.xyz

[A01] Hello World
来源：http://uln.kuanghao11.cn

Py:   print("Hello, World!")
来源：http://nvh.iojbl.cn

PHP:  echo "Hello, World!";
来源：http://fhe.fengsongda.top

JS:   console.log("Hello, World!");
来源：http://rzo.daxiang520.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://pcj.chenzaomai.com

Java: System.out.println("Hello, World!");
来源：http://wbs.shuidangran.top

Go:   fmt.Println("Hello, World!")
来源：http://dtr.fehbvm.com

Ruby: puts "Hello, World!"
来源：http://kbz.jqgufenzy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://idn.tian-w.cn

[A02] 变量声明与赋值
来源：http://fnu.feifeiyinyue.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ncv.yj202588.top

PHP:  $name = "Alex"; $age = 20;
来源：http://rsg.ivvv.top

JS:   let name = "Alex"; const age = 20;
来源：http://erc.jinghuilouyu.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://tco.snrcjt.cn

Java: String name = "Alex"; int age = 20;
来源：http://mnx.jlsjyb.cn

Go:   name := "Alex"; age := 20
来源：http://xmi.chenzaomai.com

Ruby: name = "Alex"; age = 20
来源：http://gnd.yj20258.top

C#:   string name = "Alex"; int age = 20;
来源：http://wqj.chenlongwang.top

[A03] 常量定义
来源：http://gyn.birdmap.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jyw.hcnkem.com

PHP:  const PI = 3.14159;
来源：http://tuw.epnwcf.com

JS:   const PI = 3.14159;
来源：http://gyx.daxiang520.top

TS:   const PI: number = 3.14159;
来源：http://zwt.jianghu66.top

Java: static final double PI = 3.14159;
来源：http://cja.zhaomingkeji.xyz

Go:   const PI = 3.14159
来源：http://pnb.mhx1999.top

Ruby: PI = 3.14159
来源：http://lkv.jinqigfzy.top

C#:   const double PI = 3.14159;
来源：http://hpx.shuidangran.top

[A04] 判断变量类型
来源：http://wgu.hywenlv.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://zuw.aibaodan.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mzx.zhixingplan.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ylu.gaohongyu789.top

TS:   typeof x; x instanceof Date
来源：http://ruz.xinyue.icu

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ddq.ydjk.org.cn

Go:   reflect.TypeOf(x).Name()
来源：http://sze.smart0.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://vdk.fengsongda.top

C#:   x.GetType().Name; x is int
来源：http://mau.sysykeji.top

[A05] 整数除法与取模
来源：http://qif.fengsongda.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://xwn.jinghuilouyu.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://yqa.hfpthk.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://dsl.ppjwa.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://uvz.vqdsnc.cn

Java: 7 / 2; 7 % 2
来源：http://vsa.fehbvm.com

Go:   7 / 2; 7 % 2
来源：http://ptg.yangfankeji.com

Ruby: 7 / 2; 7 % 2
来源：http://jgz.jqgufenzy.top

C#:   7 / 2; 7 % 2
来源：http://mji.xinyue.icu

[A06] 字符串转数字
来源：http://opu.sweek.top

Py:   int("42"); float("3.14")
来源：http://cpx.ppjwa.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://avt.gogol.net.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://yfk.ppjwa.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ngt.shanyushiyangtech.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://tia.yueranfly.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://whv.nwbrower.top

Ruby: "42".to_i; "3.14".to_f
来源：http://yqa.ivvv.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://aot.hammf.cn

[A07] 数字转字符串
来源：http://cbc.svipenyu.cn

Py:   str(42)
来源：http://zhk.ybcxt.top

PHP:  (string) 42; strval(42)
来源：http://ght.birdmap.top

JS:   String(42); (42).toString()
来源：http://sby.52xcode.cn

TS:   String(42)
来源：http://ghu.yueranfly.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://pep.jiagoushi.top

Go:   strconv.Itoa(42)
来源：http://qpi.snrcjt.cn

Ruby: 42.to_s
来源：http://vpg.gotoacloud.top

C#:   42.ToString()
来源：http://mry.zycfv.cn

[A08] 取整与四舍五入
来源：http://erw.tian-w.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://sjp.cdnleiting.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ubo.nanxinkj.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://vlx.birdmap.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://udq.zhaomingkeji.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://vqf.redwolf501.top


<!-- 参考信息 -->