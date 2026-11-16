代发 wailian999

[U61] PHP：正则
来源：http://bnb.pycfn.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xay.yj20258888.top

[U62] PHP：日期对象
来源：http://cji.hnxiangtu.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cro.hongshengwenyu.top

[U63] PHP：文件读写
来源：http://cnj.snrcjt.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ubp.quarkkingdee.top

[U64] PHP：目录遍历
来源：http://sfe.c1oappe.top

glob("dir/*.php");  scandir("dir");
来源：http://mhs.meibo888.top

[U65] PHP：会话
来源：http://bhq.yanxiufei.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://jri.nwbrower.top

[U66] PHP：设置 Cookie
来源：http://edu.fanxiaobao.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://evn.xuanzx.com

[U67] PHP：处理文件上传
来源：http://ivp.guowangkeji.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pdl.tanke756.top

[U68] PHP：PDO 连接
来源：http://ild.xingfuxueyuan.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jfw.zhiwuduotai.top

[U69] PHP：PDO 预处理
来源：http://mxm.aibaodan.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qmb.yanxiufei.cn

[U70] PHP：PDO 事务
来源：http://wkx.ydzc1.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://loc.fktsv.cn

[U71] PHP：抛出异常
来源：http://ley.zhongyouzk.top

throw new RuntimeException("失败", 500);
来源：http://ozk.0kj1m.cn

[U72] PHP：写错误日志
来源：http://ioi.wangshuangyany.cn

error_log("失败: " . $e->getMessage());
来源：http://kpv.sysykeji.top

[U73] PHP：读取 ini 配置
来源：http://jxp.ctjpmb.com

parse_ini_file("config.ini", true)
来源：http://bkb.jiagoushi.top

[U74] PHP：读取环境变量
来源：http://frg.hammf.cn

getenv("APP_ENV") ?: "production"
来源：http://fqd.wangdashe.top

[U75] PHP：依赖注入
来源：http://qqf.meibo888.top

composer require psr/container
来源：http://lso.wangshuangyany.cn

[U76] PHP：简单路由
来源：http://pcz.zhongyouzk.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ocf.daxiang520.top

[U77] PHP：模板渲染
来源：http://yww.9152youxi.cn

composer require twig/twig
来源：http://udt.chenzaomai.com

[U78] PHP：单元测试
来源：http://pzq.bjfxy.top

composer require --dev phpunit/phpunit
来源：http://gmj.daria6918.cn

[U79] PHP：静态分析
来源：http://cjj.sjlbkw.cn

composer require --dev phpstan/phpstan
来源：http://pbe.xuetiantiany.cn

[U80] PHP：代码规范修复
来源：http://rag.gzhubu.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ysu.ydzc1.top

[U81] JS：初始化项目
来源：http://ggd.fzhhl.top

npm init -y;  npm i express
来源：http://imo.c1oappe.top

[U82] JS：package.json 脚本
来源：http://thx.guowangkeji.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://icq.jiagoushi.top

[U83] JS：ES Module 导入导出
来源：http://mth.tarul.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zce.ivvv.top

[U84] JS：CommonJS 写法
来源：http://xqx.xylfe.cn

module.exports = { a };  const { a } = require("./m");
来源：http://xvh.ivvv.top

[U85] JS：可选链
来源：http://lhn.hammf.cn

a?.b?.c
来源：http://dkq.jinqigufen.top

[U86] JS：空值合并
来源：http://coz.zdqjudy.top

a ?? b
来源：http://jon.cheryme.top

[U87] JS：解构默认值
来源：http://cls.quarkkingdee.top

const { a = 1, b = 2 } = obj;
来源：http://yih.zycfv.cn

[U88] JS：对象展开合并
来源：http://jai.kuanghao11.cn

{ ...a, ...b }
来源：http://rwr.xinyue.icu

[U89] JS：数组去重
来源：http://kyw.wangdashe.top

[...new Set(arr)]
来源：http://haf.tianlin.xyz

[U90] JS：数字数组排序
来源：http://yyk.cheryme.top

[...arr].sort((a, b) => a - b)
来源：http://gro.zycfv.cn

[U91] JS：对象键值遍历
来源：http://qmx.yvedp.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zhw.cheryme.top

[U92] JS：深拷贝
来源：http://xry.jlsjyb.cn

structuredClone(obj)
来源：http://lhn.cheryme.top

[U93] JS：模板字符串
来源：http://abz.guannengcc.top

`共 ${n} 条`
来源：http://rvy.hysaishi.cn

[U94] JS：箭头函数
来源：http://ecj.vehdjk.com

const double = x => x * 2;
来源：http://pel.jianghu66.top

[U95] JS：Promise 包装
来源：http://fgd.daria6918.cn

new Promise((resolve, reject) => {})
来源：http://hqx.gogol.net.cn

[U96] JS：async/await 与异常
来源：http://van.hesvh.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://lxt.aibaodan.cn

[U97] JS：并发请求
来源：http://nfx.yj202588.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ezn.sxryk.cn

[U98] JS：fetch 带 JSON
来源：http://lmu.yangfankeji.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fns.shanyushiyangkeji.top

[U99] JS：事件监听
来源：http://ebh.xylfe.cn

el.addEventListener("click", e => {})
来源：http://hpj.xziqi.cn

[U100] JS：DOM 查询
来源：http://vrf.zhixingplan.top

document.querySelector(".item")
来源：http://ezx.dianchejie.cn

[U101] JS：classList 操作
来源：http://apz.jinqigufen.top

el.classList.toggle("active")
来源：http://the.dianchejie.cn

[U102] JS：本地存储
来源：http://bco.andypj.xyz

localStorage.setItem("k", JSON.stringify(v))
来源：http://bwh.yfazqb.com

[U103] JS：定时器
来源：http://mlh.sysykeji.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://eeq.jyoumei.cn

[U104] JS：防抖
来源：http://fhi.bjfxy.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dmm.shanyushiyangtech.top

[U105] JS：节流
来源：http://hbc.hesvh.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://gwl.haohaochexian.top

[U106] JS：日期格式化
来源：http://ssy.ivvv.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ibb.nwbrower.top

[U107] JS：数字千分位
来源：http://obv.tian-w.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://xiw.yuanzhike.top

[U108] JS：随机整数
来源：http://ebw.dashuyun.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://tyu.jinqigufen.top

[U109] JS：数组分组
来源：http://quc.vehdjk.com

Object.groupBy(arr, x => x.type)
来源：http://iya.zhoulong.xyz

[U110] JS：数组分块
来源：http://wdq.bjfxy.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vjd.bbcook.cn

[U111] JS：对象转 Map
来源：http://dgo.mhx1999.top

new Map(Object.entries(obj))
来源：http://tke.cheryme.top

[U112] JS：字符串补位
来源：http://jbr.jiagoushi.top

"7".padStart(3, "0")
来源：http://hxw.zdqjudy.top

[U113] JS：正则替换全部
来源：http://qov.fengsongda.top

s.replaceAll("a", "b")
来源：http://kbq.zycfv.cn

[U114] JS：JSON 深比较
来源：http://etm.feifeiyinyue.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://qvz.yangfankeji.com

[U115] JS：生成 UUID
来源：http://nys.cucudq.cn

crypto.randomUUID()
来源：http://utd.ehwqpu.com

[U116] JS：类型检查（JSDoc）
来源：http://xsw.ywan-chungtsiang.top

/** @param {string} name */ function f(name) {}
来源：http://ogg.yfazqb.com

[U117] JS：单元测试
来源：http://wtr.zycfv.cn

npm i -D vitest;  npx vitest
来源：http://sdf.xuanzx.com

[U118] JS：开发服务器
来源：http://eqn.c1oappe.top

npm i -D vite;  npx vite
来源：http://zzx.jinqigufen.top

[U119] JS：生产构建
来源：http://dzw.cucudq.cn

npx vite build
来源：http://dld.fanxiaobao.xyz

[U120] JS：读取环境变量（Vite）
来源：http://ipr.yanxiufei.cn

import.meta.env.VITE_API_URL
来源：http://zjh.xuanzx.com

================================================================================
来源：http://puv.cqqwz.cn

统计汇总
来源：http://lup.uphjek.com

================================================================================
来源：http://pvr.vqdsnc.cn

按语言统计（条）：
来源：http://jgr.gaohongyu789.top

Python ......... 252
来源：http://kxx.jiagoushi.top

PHP ............ 252
来源：http://bfm.tanke756.top

JavaScript ..... 252
来源：http://odq.zhengqikj.top

TypeScript ..... 212
来源：http://efg.tarul.cn

Java ........... 212
来源：http://eex.gogol.net.cn

Go ............. 212
来源：http://qka.sufxvd.cn

Ruby ........... 212
来源：http://vyi.9152youxi.cn

C# ............. 212
来源：http://dik.ehwqpu.com

C .............. 30
来源：http://obg.ydzc1.top

C++ ............ 30
来源：http://gmk.hcnkem.com

SQL ............ 90
来源：http://spq.yanxiufei.cn

Bash ........... 80
来源：http://cvv.xinyue.icu

Kotlin ......... 15
来源：http://xbn.gaohongyu789.top

Swift .......... 15
来源：http://tyj.svipenyu.cn

Lua ............ 10
来源：http://kwj.andypj.xyz

Perl ........... 10
来源：http://kah.sjlbkw.cn

Scala .......... 10
来源：http://frw.zhixingplan.top

------------------------------------
来源：http://vzn.ivvv.top

合计 ........... 2106 条
来源：http://bes.chenlongwang.top

按章节统计：
来源：http://vdb.cucudq.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zat.xziqi.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qxr.yfazqb.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mdt.yuanzhike.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://cgy.dianchejie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://shs.gotoacloud.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://nmx.dashuyun.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vjr.zycfv.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://asx.hnqzz.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://siv.haohaochexian.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gly.hywenlv.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pvw.vqdsnc.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dbv.jqgfzy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hvr.sjlbkw.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://utl.zycfv.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://grd.svipenyu.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://apb.zhijiandao.cn

Q SQL 专题                              90
来源：http://jlr.zhengqikj.top

R Bash 专题                             80
来源：http://rfc.aibaodan.cn

S C / C++ 专题                          60
来源：http://zrt.shzxlz.cn

T 其他语言补充                          60
来源：http://heo.feifeiyinyue.top

U 高频实用片段                         120
来源：http://xpk.smart0.xyz

------------------------------------
来源：http://ohw.xingfuxueyuan.xyz

合计                                  2106 条
来源：http://szu.pengpengdd.cyou

--------------------------------------------------------------------------------
来源：http://irw.epnwcf.com

使用提醒
来源：http://lla.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://yxk.redwolf501.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://gvw.xziqi.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://stg.quarkkingdee.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://nlk.tian-w.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://rvg.jinqigufen.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://emo.yongpay.top

—— 文件结束 ——
来源：http://sej.jiagoushi.top

================================================================================
来源：http://xnd.xziqi.cn

程序语言常见例子速查手册（2024 版）
来源：http://ary.xinyue.icu

Common Programming Examples Cheat Book
来源：http://txg.ywan-chungtsiang.top

================================================================================
来源：http://wbx.chenzaomai.com

【收录内容】
来源：http://vfg.chenzaomai.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://vke.cdnleiting.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ugk.dianchejie.cn

SQL · Bash · C · C++
来源：http://liy.ctjpmb.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://paj.epnwcf.com

【使用说明】
来源：http://dao.cashguo.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://npv.ywan-chungtsiang.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://vjq.sxryk.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bzm.zdbjq.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://azn.svipenyu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://lsl.tian-w.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://lnv.ydjk.org.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ylt.gogol.net.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zzh.havefunace.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://yki.hnqzz.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hzz.pengpengdd.cyou

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://rju.yangfankeji.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ety.jiagoushi.top

【文件统计】
来源：http://hvx.hnxiangtu.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tbg.jinqigufen.top

--------------------------------------------------------------------------------
来源：http://ola.yj202588.top

目  录
来源：http://sio.birdmap.top

--------------------------------------------------------------------------------
来源：http://jev.wangshuangyany.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://zbm.aizwys.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://hwn.quarkkingdee.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gyw.feifeiyinyue.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://hux.sysykeji.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://huq.hammf.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://gtv.yuanzhike.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rvh.pengpengdd.cyou

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://npv.shuidangran.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://gqj.hcnkem.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xig.tian-w.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://gkg.ppjwa.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mju.epnwcf.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://opy.zhoulong.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://eqe.vehdjk.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://lxj.epnwcf.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://loy.guannengcc.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://xml.wangdashe.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://bzm.andypj.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://xza.jinqigfzy.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://cls.hcnkem.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blo.yueranfly.top

================================================================================
来源：http://fzj.0kj1m.cn

A. 基础语法与类型
来源：http://ljz.hfpthk.cn

================================================================================
来源：http://vmu.cucudq.cn

[A01] Hello World
来源：http://suk.yanxiufei.cn

Py:   print("Hello, World!")
来源：http://uia.gotoacloud.top

PHP:  echo "Hello, World!";
来源：http://unw.hnxiangtu.top

JS:   console.log("Hello, World!");
来源：http://vhr.bbcook.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hgv.wangshuangyany.cn

Java: System.out.println("Hello, World!");
来源：http://kur.sweek.top

Go:   fmt.Println("Hello, World!")
来源：http://wgh.ivvv.top

Ruby: puts "Hello, World!"
来源：http://ygw.yj20258.top

C#:   Console.WriteLine("Hello, World!");
来源：http://wza.xuetiantiany.cn

[A02] 变量声明与赋值
来源：http://nko.yfazqb.com

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://xda.nanxuanxn.top

PHP:  $name = "Alex"; $age = 20;
来源：http://apa.guowangkeji.top

JS:   let name = "Alex"; const age = 20;
来源：http://ztg.316326.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://rui.zhengqikj.top

Java: String name = "Alex"; int age = 20;
来源：http://lod.iojbl.cn

Go:   name := "Alex"; age := 20
来源：http://rgp.aibaodan.cn

Ruby: name = "Alex"; age = 20
来源：http://yjz.bjfxy.top

C#:   string name = "Alex"; int age = 20;
来源：http://kiu.c1oappe.top

[A03] 常量定义
来源：http://ney.hammf.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ady.vqdsnc.cn

PHP:  const PI = 3.14159;
来源：http://gzx.9152youxi.cn

JS:   const PI = 3.14159;
来源：http://inj.ybcxt.top

TS:   const PI: number = 3.14159;
来源：http://uol.cdnleiting.top

Java: static final double PI = 3.14159;
来源：http://ouf.gogol.net.cn

Go:   const PI = 3.14159
来源：http://ljc.ivvv.top

Ruby: PI = 3.14159
来源：http://law.daria6918.cn

C#:   const double PI = 3.14159;
来源：http://exg.jyoumei.cn

[A04] 判断变量类型
来源：http://lya.jinghuilouyu.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://myc.feifeiyinyue.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tem.0kj1m.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hag.hnqzz.top

TS:   typeof x; x instanceof Date
来源：http://yvb.jqgufenzy.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xks.0kj1m.cn

Go:   reflect.TypeOf(x).Name()
来源：http://sgb.316326.xyz

Ruby: x.class; x.is_a?(Integer)
来源：http://khv.sxryk.cn

C#:   x.GetType().Name; x is int
来源：http://nqt.fzhhl.top

[A05] 整数除法与取模
来源：http://mfd.daxiang520.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wpb.xylfe.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://gga.guowangkeji.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://skd.yj202588.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xjh.daria6918.cn

Java: 7 / 2; 7 % 2
来源：http://fxy.fehbvm.com

Go:   7 / 2; 7 % 2
来源：http://zog.dianchejie.cn

Ruby: 7 / 2; 7 % 2
来源：http://wdf.yj202588.top

C#:   7 / 2; 7 % 2
来源：http://suf.ctjpmb.com

[A06] 字符串转数字
来源：http://kcj.jlsjyb.cn

Py:   int("42"); float("3.14")
来源：http://vas.xylfe.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://zpz.nanxuanxn.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://afe.guannengcc.top

TS:   parseInt("42", 10); Number("42")
来源：http://ytk.hcnkem.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://kkd.hfpthk.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://bep.hnqzz.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ajf.fehbvm.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://efe.ywan-chungtsiang.top

[A07] 数字转字符串
来源：http://quq.xuetiantiany.cn

Py:   str(42)
来源：http://fnp.ywan-chungtsiang.top

PHP:  (string) 42; strval(42)
来源：http://anh.zhixingplan.top

JS:   String(42); (42).toString()
来源：http://vvq.epnwcf.com

TS:   String(42)
来源：http://gia.quarkkingdee.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://cul.316326.xyz

Go:   strconv.Itoa(42)
来源：http://kwg.chenzaomai.com

Ruby: 42.to_s
来源：http://noy.haohaochexian.top

C#:   42.ToString()
来源：http://ogo.tianlin.xyz

[A08] 取整与四舍五入
来源：http://ive.xuanzx.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://spz.jinghuilouyu.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://smt.sysykeji.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://nfb.jiagoushi.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://vie.chenjidiqi.icu

Java: Math.round(3.567); Math.floor(3.9)
来源：http://rug.cheryme.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://rxi.ywan-chungtsiang.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://uxw.nanxuanxn.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mee.hfpthk.cn

[A09] 绝对值与最大最小值
来源：http://ugw.daria6918.cn


<!-- 参考信息 -->