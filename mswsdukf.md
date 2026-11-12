代发 wailian999

[U65] PHP：会话
来源：http://dah.nanxinkj.top

session_start();  $_SESSION["uid"] = 1;
来源：http://mqa.bjfxy.top

[U66] PHP：设置 Cookie
来源：http://mpx.pengpengdd.cyou

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mxx.316326.xyz

[U67] PHP：处理文件上传
来源：http://yot.yuxming.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bzw.bbcook.cn

[U68] PHP：PDO 连接
来源：http://xkd.aibaodan.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://biu.xuanzx.com

[U69] PHP：PDO 预处理
来源：http://wje.cheryme.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nps.gogol.net.cn

[U70] PHP：PDO 事务
来源：http://guk.ybcxt.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nyt.cucudq.cn

[U71] PHP：抛出异常
来源：http://ifk.jinghuilouyu.cn

throw new RuntimeException("失败", 500);
来源：http://qkg.ppjwa.cn

[U72] PHP：写错误日志
来源：http://fee.birdmap.top

error_log("失败: " . $e->getMessage());
来源：http://qff.ybcxt.top

[U73] PHP：读取 ini 配置
来源：http://uvs.zycfv.cn

parse_ini_file("config.ini", true)
来源：http://gja.quarkkingdee.top

[U74] PHP：读取环境变量
来源：http://bmy.epnwcf.com

getenv("APP_ENV") ?: "production"
来源：http://zzo.daxiang520.top

[U75] PHP：依赖注入
来源：http://hzf.0kj1m.cn

composer require psr/container
来源：http://jkv.xuanzx.com

[U76] PHP：简单路由
来源：http://okv.sjlbkw.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mwl.ydjk.org.cn

[U77] PHP：模板渲染
来源：http://dzy.jinqigfzy.top

composer require twig/twig
来源：http://niy.zhengqikj.top

[U78] PHP：单元测试
来源：http://wyh.shangyingyoupin.top

composer require --dev phpunit/phpunit
来源：http://rjm.zhaomingkeji.xyz

[U79] PHP：静态分析
来源：http://ict.cashguo.top

composer require --dev phpstan/phpstan
来源：http://ypw.jqgfzy.top

[U80] PHP：代码规范修复
来源：http://vdx.52xcode.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mip.tian-w.cn

[U81] JS：初始化项目
来源：http://vdd.zhoulong.xyz

npm init -y;  npm i express
来源：http://vqx.xingfuxueyuan.xyz

[U82] JS：package.json 脚本
来源：http://dss.sweek.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://scl.hnqzz.top

[U83] JS：ES Module 导入导出
来源：http://amb.yongpay.top

export const a = 1;  import { a } from "./m.js";
来源：http://mvc.xuanzx.com

[U84] JS：CommonJS 写法
来源：http://kct.iojbl.cn

module.exports = { a };  const { a } = require("./m");
来源：http://ybm.jinqigufen.top

[U85] JS：可选链
来源：http://axm.yuxming.cn

a?.b?.c
来源：http://cgz.wangdashe.top

[U86] JS：空值合并
来源：http://mnp.meibo888.top

a ?? b
来源：http://pkh.redwolf501.top

[U87] JS：解构默认值
来源：http://gnc.xingfuxueyuan.xyz

const { a = 1, b = 2 } = obj;
来源：http://pyk.yongpay.top

[U88] JS：对象展开合并
来源：http://znl.bbcook.cn

{ ...a, ...b }
来源：http://nfk.epnwcf.com

[U89] JS：数组去重
来源：http://msr.vqdsnc.cn

[...new Set(arr)]
来源：http://rhp.meibo888.top

[U90] JS：数字数组排序
来源：http://lto.gaohongyu789.top

[...arr].sort((a, b) => a - b)
来源：http://bif.gaohongyu789.top

[U91] JS：对象键值遍历
来源：http://fsr.yfazqb.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://pel.snrcjt.cn

[U92] JS：深拷贝
来源：http://yqa.mhx1999.top

structuredClone(obj)
来源：http://tfy.yfazqb.com

[U93] JS：模板字符串
来源：http://kyg.tian-w.cn

`共 ${n} 条`
来源：http://plv.xylfe.cn

[U94] JS：箭头函数
来源：http://vpf.hnxiangtu.top

const double = x => x * 2;
来源：http://oky.quarkkingdee.top

[U95] JS：Promise 包装
来源：http://bhn.aibaodan.cn

new Promise((resolve, reject) => {})
来源：http://hoy.quarkkingdee.top

[U96] JS：async/await 与异常
来源：http://cvb.andypj.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://kqo.jqgfzy.top

[U97] JS：并发请求
来源：http://myo.sufxvd.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://rqv.snrcjt.cn

[U98] JS：fetch 带 JSON
来源：http://gog.hfpthk.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://vhw.epnwcf.com

[U99] JS：事件监听
来源：http://jof.zhongyouzk.top

el.addEventListener("click", e => {})
来源：http://ydp.kuanghao11.cn

[U100] JS：DOM 查询
来源：http://rpj.jlsjyb.cn

document.querySelector(".item")
来源：http://zhz.snrcjt.cn

[U101] JS：classList 操作
来源：http://vfs.tarul.cn

el.classList.toggle("active")
来源：http://cek.jinghuilouyu.cn

[U102] JS：本地存储
来源：http://cvx.jinqigufen.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ikd.ydjk.org.cn

[U103] JS：定时器
来源：http://fma.jianghu66.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://egc.cucudq.cn

[U104] JS：防抖
来源：http://rkg.fktsv.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jri.zhongyouzk.top

[U105] JS：节流
来源：http://ewe.hysaishi.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://vdz.yuxming.cn

[U106] JS：日期格式化
来源：http://rjr.fanxiaobao.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://pti.yj20258.top

[U107] JS：数字千分位
来源：http://kmk.hongshengwenyu.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://kvs.pengpengdd.cyou

[U108] JS：随机整数
来源：http://pus.quarkkingdee.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://kuj.zdqjudy.top

[U109] JS：数组分组
来源：http://lun.zdqjudy.top

Object.groupBy(arr, x => x.type)
来源：http://qxg.epnwcf.com

[U110] JS：数组分块
来源：http://hwh.uphjek.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://gyh.cashguo.top

[U111] JS：对象转 Map
来源：http://qdc.xingfuxueyuan.xyz

new Map(Object.entries(obj))
来源：http://vqe.tarul.cn

[U112] JS：字符串补位
来源：http://ctk.jlsjyb.cn

"7".padStart(3, "0")
来源：http://xpz.fehbvm.com

[U113] JS：正则替换全部
来源：http://nhc.ywan-chungtsiang.top

s.replaceAll("a", "b")
来源：http://zrh.jinqigfzy.top

[U114] JS：JSON 深比较
来源：http://qli.jiagoushi.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://wyh.pengpengdd.cyou

[U115] JS：生成 UUID
来源：http://xcx.gotoacloud.top

crypto.randomUUID()
来源：http://isn.ybcxt.top

[U116] JS：类型检查（JSDoc）
来源：http://ren.redwolf501.top

/** @param {string} name */ function f(name) {}
来源：http://pnn.yj20258888.top

[U117] JS：单元测试
来源：http://cdk.yj20258888.top

npm i -D vitest;  npx vitest
来源：http://cwb.kuanghao11.cn

[U118] JS：开发服务器
来源：http://kuo.yj20258.top

npm i -D vite;  npx vite
来源：http://tpk.sjlbkw.cn

[U119] JS：生产构建
来源：http://yun.dashuyun.cn

npx vite build
来源：http://fba.sysykeji.top

[U120] JS：读取环境变量（Vite）
来源：http://mhn.cqqwz.cn

import.meta.env.VITE_API_URL
来源：http://sho.sweek.top

================================================================================
来源：http://pen.tarul.cn

统计汇总
来源：http://ozz.vehdjk.com

================================================================================
来源：http://dog.cashguo.top

按语言统计（条）：
来源：http://sxq.tarul.cn

Python ......... 252
来源：http://aru.sufxvd.cn

PHP ............ 252
来源：http://xwg.hfpthk.cn

JavaScript ..... 252
来源：http://mie.sysykeji.top

TypeScript ..... 212
来源：http://xhx.cashguo.top

Java ........... 212
来源：http://fgd.hfpthk.cn

Go ............. 212
来源：http://mwf.yj20258888.top

Ruby ........... 212
来源：http://ywt.daxiang520.top

C# ............. 212
来源：http://ikm.gotoacloud.top

C .............. 30
来源：http://del.guannengcc.top

C++ ............ 30
来源：http://tai.ctjpmb.com

SQL ............ 90
来源：http://qzf.aibaodan.cn

Bash ........... 80
来源：http://foo.aizwys.cn

Kotlin ......... 15
来源：http://rpw.ydjk.org.cn

Swift .......... 15
来源：http://txw.chenlongwang.top

Lua ............ 10
来源：http://tjj.tarul.cn

Perl ........... 10
来源：http://pty.yangfankeji.com

Scala .......... 10
来源：http://awt.shanyushiyangtech.top

------------------------------------
来源：http://nia.zhaomingkeji.xyz

合计 ........... 2106 条
来源：http://hzu.feifeiyinyue.top

按章节统计：
来源：http://tus.sysykeji.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cqi.mhx1999.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://nqd.9152youxi.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://iej.yuanzhike.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://agu.quarkkingdee.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://vco.fzhhl.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mwv.xingfuxueyuan.xyz

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wuo.pycfn.com

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tbl.quarkkingdee.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://xmb.jinqigfzy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ysd.guowangkeji.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cua.yongpay.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sfe.fengsongda.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rch.hysaishi.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kbl.gogol.net.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://saf.cdnleiting.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://eba.guowangkeji.top

Q SQL 专题                              90
来源：http://hvw.pycfn.com

R Bash 专题                             80
来源：http://djb.xingfuxueyuan.xyz

S C / C++ 专题                          60
来源：http://ois.yanxiufei.cn

T 其他语言补充                          60
来源：http://ldo.gzhubu.top

U 高频实用片段                         120
来源：http://aia.yonumen.top

------------------------------------
来源：http://ylx.bjfxy.top

合计                                  2106 条
来源：http://spq.sweek.top

--------------------------------------------------------------------------------
来源：http://eai.jinqigfzy.top

使用提醒
来源：http://gsv.jinqigfzy.top

--------------------------------------------------------------------------------
来源：http://vdc.ehwqpu.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://lkw.gogol.net.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jiv.yj20258.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vcp.nanxinkj.top

在旧版本上使用前请先确认语法支持情况。
来源：http://mjh.sweek.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bbs.zhengqikj.top

—— 文件结束 ——
来源：http://oxx.wangshuangyany.cn

================================================================================
来源：http://kae.snrcjt.cn

程序语言常见例子速查手册（2024 版）
来源：http://tvj.cashguo.top

Common Programming Examples Cheat Book
来源：http://ysv.hfpthk.cn

================================================================================
来源：http://dgl.zycfv.cn

【收录内容】
来源：http://vwz.nwbrower.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://taj.chenzaomai.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ezn.sjlbkw.cn

SQL · Bash · C · C++
来源：http://xzj.kuanghao11.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ump.fktsv.cn

【使用说明】
来源：http://nxi.chenjidiqi.icu

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://xff.cheryme.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rwj.yvedp.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jms.aizwys.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wfr.aibaodan.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://hoe.xylfe.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ciz.xuanzx.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ndy.ctjpmb.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fkm.jinqigfzy.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://dec.sufxvd.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hdt.jlsjyb.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://jbf.ehwqpu.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://dnp.nanxinkj.top

【文件统计】
来源：http://mxp.meibo888.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mzm.wangdashe.top

--------------------------------------------------------------------------------
来源：http://edv.haohaochexian.top

目  录
来源：http://agb.316326.xyz

--------------------------------------------------------------------------------
来源：http://wij.hnxiangtu.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://nin.shuidangran.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ahi.tianlin.xyz

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://ecr.shangyingyoupin.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mdw.shuidangran.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://dzg.feifeiyinyue.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ihm.cdnleiting.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://gwg.jinghuilouyu.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ncx.redwolf501.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://zki.shuidangran.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dmq.yj20258888.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://fjf.tanke756.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mvw.ybcxt.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ekk.hysaishi.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://cjx.yanxiufei.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://eta.hnqzz.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kvn.hfpthk.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wsz.havefunace.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://obu.tian-w.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lli.kuanghao11.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pcy.hnqzz.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wqc.daria6918.cn

================================================================================
来源：http://wzb.hnxiangtu.top

A. 基础语法与类型
来源：http://bza.yongpay.top

================================================================================
来源：http://nwn.yj202588.top

[A01] Hello World
来源：http://ojw.vehdjk.com

Py:   print("Hello, World!")
来源：http://irc.hysaishi.cn

PHP:  echo "Hello, World!";
来源：http://hol.tian-w.cn

JS:   console.log("Hello, World!");
来源：http://nvv.dianchejie.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ulz.jqgfzy.top

Java: System.out.println("Hello, World!");
来源：http://dfo.bbcook.cn

Go:   fmt.Println("Hello, World!")
来源：http://brt.hesvh.cn

Ruby: puts "Hello, World!"
来源：http://qmu.yj20258888.top

C#:   Console.WriteLine("Hello, World!");
来源：http://fpm.jlsjyb.cn

[A02] 变量声明与赋值
来源：http://edo.zhixingplan.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://vhm.bjfxy.top

PHP:  $name = "Alex"; $age = 20;
来源：http://drj.havefunace.top

JS:   let name = "Alex"; const age = 20;
来源：http://fmd.chenjidiqi.icu

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://dfy.gotoacloud.top

Java: String name = "Alex"; int age = 20;
来源：http://bns.havefunace.top

Go:   name := "Alex"; age := 20
来源：http://xre.redwolf501.top

Ruby: name = "Alex"; age = 20
来源：http://udi.cucudq.cn

C#:   string name = "Alex"; int age = 20;
来源：http://yow.yonumen.top

[A03] 常量定义
来源：http://qbn.iojbl.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://acy.jinyuanbaomall.cn

PHP:  const PI = 3.14159;
来源：http://pto.uphjek.com

JS:   const PI = 3.14159;
来源：http://guc.ydzc1.top

TS:   const PI: number = 3.14159;
来源：http://lwi.jyoumei.cn

Java: static final double PI = 3.14159;
来源：http://uuv.yj202588.top

Go:   const PI = 3.14159
来源：http://mpu.shzxlz.cn

Ruby: PI = 3.14159
来源：http://vhy.xingfuxueyuan.xyz

C#:   const double PI = 3.14159;
来源：http://ujv.wangdashe.top

[A04] 判断变量类型
来源：http://phy.gaohongyu789.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://pxo.bbcook.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://gpi.yfazqb.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://rbe.hfpthk.cn

TS:   typeof x; x instanceof Date
来源：http://xew.yj20258.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://oam.jinqigfzy.top

Go:   reflect.TypeOf(x).Name()
来源：http://xnv.chenjidiqi.icu

Ruby: x.class; x.is_a?(Integer)
来源：http://rfc.yj20258.top

C#:   x.GetType().Name; x is int
来源：http://mdw.zdbjq.cn

[A05] 整数除法与取模
来源：http://igg.xziqi.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mnv.wangdashe.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://mfz.gotoacloud.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://tiv.bjfxy.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kpr.haohaochexian.top

Java: 7 / 2; 7 % 2
来源：http://xqm.gogol.net.cn

Go:   7 / 2; 7 % 2
来源：http://qxk.haohaochexian.top

Ruby: 7 / 2; 7 % 2
来源：http://ybk.fengsongda.top

C#:   7 / 2; 7 % 2
来源：http://teu.ppjwa.cn

[A06] 字符串转数字
来源：http://fmq.hnqzz.top

Py:   int("42"); float("3.14")
来源：http://wtm.aizwys.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://sxm.aizwys.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://yki.daria6918.cn

TS:   parseInt("42", 10); Number("42")
来源：http://doh.zhaomingkeji.xyz

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qdn.xziqi.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://ert.shangyingyoupin.top

Ruby: "42".to_i; "3.14".to_f
来源：http://hcc.yueranfly.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qaq.sjlbkw.cn

[A07] 数字转字符串
来源：http://vrx.yongpay.top

Py:   str(42)
来源：http://aya.hesvh.cn

PHP:  (string) 42; strval(42)
来源：http://zfp.zhongyouzk.top

JS:   String(42); (42).toString()
来源：http://tyc.tianlin.xyz

TS:   String(42)
来源：http://dpw.yanxiufei.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vcp.svipenyu.cn

Go:   strconv.Itoa(42)
来源：http://rht.hongshengwenyu.top

Ruby: 42.to_s
来源：http://frn.epnwcf.com

C#:   42.ToString()
来源：http://umy.shuidangran.top

[A08] 取整与四舍五入
来源：http://cex.fehbvm.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://rjh.redwolf501.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kjo.jianghu66.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://gzx.yj202588.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://yqj.fzhhl.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://efl.hysaishi.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tws.bjfxy.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://jie.shanyushiyangtech.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hol.nanxinkj.top

[A09] 绝对值与最大最小值
来源：http://die.fktsv.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://iwi.yangfankeji.com

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://gdi.chenjidiqi.icu

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://tqj.andypj.xyz

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xlc.xziqi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://fpr.hesvh.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://waj.havefunace.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wae.yuanzhike.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://fhl.guowangkeji.top


<!-- 参考信息 -->