代发 wailian999

[U67] PHP：处理文件上传
来源：http://ljm.jinyuanbaomall.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tzu.bbcook.cn

[U68] PHP：PDO 连接
来源：http://kem.shuidangran.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://opj.gogol.net.cn

[U69] PHP：PDO 预处理
来源：http://xiq.sxryk.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://qqs.nanxuanxn.top

[U70] PHP：PDO 事务
来源：http://lgr.hammf.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tfq.zhengqikj.top

[U71] PHP：抛出异常
来源：http://opi.yonumen.top

throw new RuntimeException("失败", 500);
来源：http://bte.zycfv.cn

[U72] PHP：写错误日志
来源：http://uhu.ehwqpu.com

error_log("失败: " . $e->getMessage());
来源：http://qzd.jyoumei.cn

[U73] PHP：读取 ini 配置
来源：http://guk.ctjpmb.com

parse_ini_file("config.ini", true)
来源：http://nyu.fanxiaobao.xyz

[U74] PHP：读取环境变量
来源：http://ezq.svipenyu.cn

getenv("APP_ENV") ?: "production"
来源：http://tqb.haohaochexian.top

[U75] PHP：依赖注入
来源：http://kyj.epnwcf.com

composer require psr/container
来源：http://fda.haohaochexian.top

[U76] PHP：简单路由
来源：http://zpm.quarkkingdee.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wuf.zhaomingkeji.xyz

[U77] PHP：模板渲染
来源：http://xkf.yj202588.top

composer require twig/twig
来源：http://ajd.jinqigfzy.top

[U78] PHP：单元测试
来源：http://gbv.zycfv.cn

composer require --dev phpunit/phpunit
来源：http://ytn.hammf.cn

[U79] PHP：静态分析
来源：http://bbg.zhijiandao.cn

composer require --dev phpstan/phpstan
来源：http://cjb.52xcode.cn

[U80] PHP：代码规范修复
来源：http://gdj.zhengqikj.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://rhk.yuanzhike.top

[U81] JS：初始化项目
来源：http://wnb.hnxiangtu.top

npm init -y;  npm i express
来源：http://oda.zhiwuduotai.top

[U82] JS：package.json 脚本
来源：http://xqz.hnxiangtu.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uxb.zhixingplan.top

[U83] JS：ES Module 导入导出
来源：http://jdz.smart0.xyz

export const a = 1;  import { a } from "./m.js";
来源：http://pqx.birdmap.top

[U84] JS：CommonJS 写法
来源：http://eyy.xuanzx.com

module.exports = { a };  const { a } = require("./m");
来源：http://lna.yanxiufei.cn

[U85] JS：可选链
来源：http://gba.chenlongwang.top

a?.b?.c
来源：http://fmr.ppjwa.cn

[U86] JS：空值合并
来源：http://bsq.guowangkeji.top

a ?? b
来源：http://bug.ybcxt.top

[U87] JS：解构默认值
来源：http://pmq.zhengqikj.top

const { a = 1, b = 2 } = obj;
来源：http://qdm.ybcxt.top

[U88] JS：对象展开合并
来源：http://rrw.jiagoushi.top

{ ...a, ...b }
来源：http://bhp.pycfn.com

[U89] JS：数组去重
来源：http://vgb.feifeiyinyue.top

[...new Set(arr)]
来源：http://shm.havefunace.top

[U90] JS：数字数组排序
来源：http://dql.cucudq.cn

[...arr].sort((a, b) => a - b)
来源：http://laj.c1oappe.top

[U91] JS：对象键值遍历
来源：http://bsh.yfazqb.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bpj.yanxiufei.cn

[U92] JS：深拷贝
来源：http://riq.vehdjk.com

structuredClone(obj)
来源：http://fyc.zycfv.cn

[U93] JS：模板字符串
来源：http://msy.52xcode.cn

`共 ${n} 条`
来源：http://ayp.sjlbkw.cn

[U94] JS：箭头函数
来源：http://dvt.ehwqpu.com

const double = x => x * 2;
来源：http://tie.chenlongwang.top

[U95] JS：Promise 包装
来源：http://hxg.c1oappe.top

new Promise((resolve, reject) => {})
来源：http://kvy.xuanzx.com

[U96] JS：async/await 与异常
来源：http://dbt.redwolf501.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://znh.fzhhl.top

[U97] JS：并发请求
来源：http://ahs.wangshuangyany.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://qxv.cdnleiting.top

[U98] JS：fetch 带 JSON
来源：http://dmt.shanyushiyangkeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ouy.andypj.xyz

[U99] JS：事件监听
来源：http://mff.zycfv.cn

el.addEventListener("click", e => {})
来源：http://awt.0kj1m.cn

[U100] JS：DOM 查询
来源：http://vas.pycfn.com

document.querySelector(".item")
来源：http://wmr.sweek.top

[U101] JS：classList 操作
来源：http://rwa.shanyushiyangtech.top

el.classList.toggle("active")
来源：http://xtg.mhx1999.top

[U102] JS：本地存储
来源：http://vll.sweek.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ptv.jinghuilouyu.cn

[U103] JS：定时器
来源：http://ryt.guowangkeji.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://zdo.bjfxy.top

[U104] JS：防抖
来源：http://dcy.aizwys.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fti.gzhubu.top

[U105] JS：节流
来源：http://agy.gaohongyu789.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fdb.9152youxi.cn

[U106] JS：日期格式化
来源：http://wfl.ywan-chungtsiang.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://lxi.0kj1m.cn

[U107] JS：数字千分位
来源：http://fcw.ehwqpu.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cgu.shanyushiyangkeji.top

[U108] JS：随机整数
来源：http://wdv.vehdjk.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mrg.jianghu66.top

[U109] JS：数组分组
来源：http://prx.ydjk.org.cn

Object.groupBy(arr, x => x.type)
来源：http://nqu.zhoulong.xyz

[U110] JS：数组分块
来源：http://hwi.birdmap.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://fqg.ehwqpu.com

[U111] JS：对象转 Map
来源：http://pqm.pycfn.com

new Map(Object.entries(obj))
来源：http://wpp.yj202588.top

[U112] JS：字符串补位
来源：http://uhu.ppjwa.cn

"7".padStart(3, "0")
来源：http://npy.52xcode.cn

[U113] JS：正则替换全部
来源：http://onj.pycfn.com

s.replaceAll("a", "b")
来源：http://pju.shanyushiyangtech.top

[U114] JS：JSON 深比较
来源：http://kur.yonumen.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://fgg.zhiwuduotai.top

[U115] JS：生成 UUID
来源：http://rpx.zhoulong.xyz

crypto.randomUUID()
来源：http://bra.zhaomingkeji.xyz

[U116] JS：类型检查（JSDoc）
来源：http://elz.wangshuangyany.cn

/** @param {string} name */ function f(name) {}
来源：http://yhp.ywan-chungtsiang.top

[U117] JS：单元测试
来源：http://ijv.birdmap.top

npm i -D vitest;  npx vitest
来源：http://krd.zhijiandao.cn

[U118] JS：开发服务器
来源：http://vdb.sjlbkw.cn

npm i -D vite;  npx vite
来源：http://aku.ydzc1.top

[U119] JS：生产构建
来源：http://wdh.hesvh.cn

npx vite build
来源：http://ssd.feifeiyinyue.top

[U120] JS：读取环境变量（Vite）
来源：http://ful.yonumen.top

import.meta.env.VITE_API_URL
来源：http://gjk.cashguo.top

================================================================================
来源：http://ios.hfpthk.cn

统计汇总
来源：http://wss.pengpengdd.cyou

================================================================================
来源：http://fse.ydzc1.top

按语言统计（条）：
来源：http://mrq.gotoacloud.top

Python ......... 252
来源：http://dow.aibaodan.cn

PHP ............ 252
来源：http://nlp.aizwys.cn

JavaScript ..... 252
来源：http://efg.mhx1999.top

TypeScript ..... 212
来源：http://kfk.daxiang520.top

Java ........... 212
来源：http://oql.vqdsnc.cn

Go ............. 212
来源：http://qog.chenjidiqi.icu

Ruby ........... 212
来源：http://zvj.xingfuxueyuan.xyz

C# ............. 212
来源：http://oft.shanyushiyangkeji.top

C .............. 30
来源：http://wfc.zdbjq.cn

C++ ............ 30
来源：http://yke.jiagoushi.top

SQL ............ 90
来源：http://eos.ehwqpu.com

Bash ........... 80
来源：http://kaq.chenlongwang.top

Kotlin ......... 15
来源：http://xyi.andypj.xyz

Swift .......... 15
来源：http://eug.sysykeji.top

Lua ............ 10
来源：http://eip.xuanzx.com

Perl ........... 10
来源：http://ire.haohaochexian.top

Scala .......... 10
来源：http://fzt.aizwys.cn

------------------------------------
来源：http://abp.ywan-chungtsiang.top

合计 ........... 2106 条
来源：http://con.gzhubu.top

按章节统计：
来源：http://gpa.feifeiyinyue.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rbh.zhixingplan.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qvx.yuanzhike.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lwe.feifeiyinyue.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://azi.tian-w.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kcu.svipenyu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://pxb.xuanzx.com

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://dzf.pengpengdd.cyou

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://gkm.bbcook.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hiu.zhongyouzk.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rqq.c1oappe.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://iqh.bbcook.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://efs.sufxvd.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ird.shangyingyoupin.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://kpl.ppjwa.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://joa.nwbrower.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://sim.mhx1999.top

Q SQL 专题                              90
来源：http://txi.hysaishi.cn

R Bash 专题                             80
来源：http://kve.9152youxi.cn

S C / C++ 专题                          60
来源：http://ham.jinyuanbaomall.cn

T 其他语言补充                          60
来源：http://gss.daria6918.cn

U 高频实用片段                         120
来源：http://atg.0kj1m.cn

------------------------------------
来源：http://zvz.cdnleiting.top

合计                                  2106 条
来源：http://bdp.ydjk.org.cn

--------------------------------------------------------------------------------
来源：http://hqj.gzhubu.top

使用提醒
来源：http://adx.wangshuangyany.cn

--------------------------------------------------------------------------------
来源：http://jlt.jianghu66.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://pmj.tian-w.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://gca.zhengqikj.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://xra.hcnkem.com

在旧版本上使用前请先确认语法支持情况。
来源：http://pie.xuetiantiany.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://lul.ivvv.top

—— 文件结束 ——
来源：http://hqi.52xcode.cn

================================================================================
来源：http://flv.hysaishi.cn

程序语言常见例子速查手册（2024 版）
来源：http://gpx.sjlbkw.cn

Common Programming Examples Cheat Book
来源：http://mpd.shanyushiyangtech.top

================================================================================
来源：http://cns.daxiang520.top

【收录内容】
来源：http://yjd.bbcook.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://xug.shzxlz.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ezs.nwbrower.top

SQL · Bash · C · C++
来源：http://edj.bjfxy.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jxk.zhongyouzk.top

【使用说明】
来源：http://yjp.zdqjudy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://anb.vehdjk.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://gro.tarul.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vbc.ydjk.org.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://pty.daxiang520.top

Bash:  Shell         C:     C             C++:   C++
来源：http://zth.yvedp.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://scb.havefunace.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://tbm.chenzaomai.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://uan.cdnleiting.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hou.ydzc1.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wbb.jyoumei.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://dou.jlsjyb.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://sqb.xuetiantiany.cn

【文件统计】
来源：http://qtm.jlsjyb.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rpu.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://ksy.feifeiyinyue.top

目  录
来源：http://hrq.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://alv.jyoumei.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jju.wangshuangyany.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wxe.sufxvd.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://usx.yfazqb.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ygr.yanxiufei.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://uyr.shanyushiyangkeji.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lug.tianlin.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://exe.guannengcc.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://ijw.redwolf501.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tjy.yj202588.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://deu.tarul.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://emn.pycfn.com

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hja.xziqi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mng.gogol.net.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pks.meibo888.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jqq.sxryk.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bng.fzhhl.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://dnx.jlsjyb.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://wty.yangfankeji.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wyr.0kj1m.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://rdo.cheryme.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qxb.yj20258888.top

================================================================================
来源：http://qea.xuanzx.com

A. 基础语法与类型
来源：http://rvq.shuidangran.top

================================================================================
来源：http://sqq.hysaishi.cn

[A01] Hello World
来源：http://qrm.chenlongwang.top

Py:   print("Hello, World!")
来源：http://ggx.jinghuilouyu.cn

PHP:  echo "Hello, World!";
来源：http://zqp.xuetiantiany.cn

JS:   console.log("Hello, World!");
来源：http://feg.hywenlv.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://tsz.svipenyu.cn

Java: System.out.println("Hello, World!");
来源：http://jsa.cashguo.top

Go:   fmt.Println("Hello, World!")
来源：http://uoi.vehdjk.com

Ruby: puts "Hello, World!"
来源：http://sge.hywenlv.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://jzf.vqdsnc.cn

[A02] 变量声明与赋值
来源：http://rso.bjfxy.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://lqy.wangshuangyany.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://aqz.havefunace.top

JS:   let name = "Alex"; const age = 20;
来源：http://ytx.ydzc1.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wrl.shanyushiyangtech.top

Java: String name = "Alex"; int age = 20;
来源：http://ipa.yonumen.top

Go:   name := "Alex"; age := 20
来源：http://skj.hesvh.cn

Ruby: name = "Alex"; age = 20
来源：http://bvh.yj20258888.top

C#:   string name = "Alex"; int age = 20;
来源：http://myg.gogol.net.cn

[A03] 常量定义
来源：http://cig.chenjidiqi.icu

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://jaw.yueranfly.top

PHP:  const PI = 3.14159;
来源：http://bid.shzxlz.cn

JS:   const PI = 3.14159;
来源：http://bmq.hywenlv.cn

TS:   const PI: number = 3.14159;
来源：http://tii.pengpengdd.cyou

Java: static final double PI = 3.14159;
来源：http://fic.vqdsnc.cn

Go:   const PI = 3.14159
来源：http://vrj.jqgfzy.top

Ruby: PI = 3.14159
来源：http://pbf.hnxiangtu.top

C#:   const double PI = 3.14159;
来源：http://ccc.hongshengwenyu.top

[A04] 判断变量类型
来源：http://zsl.yongpay.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://yml.hysaishi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://raw.wangshuangyany.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://sxm.vehdjk.com

TS:   typeof x; x instanceof Date
来源：http://dac.pengpengdd.cyou

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://rce.dashuyun.cn

Go:   reflect.TypeOf(x).Name()
来源：http://pim.hcnkem.com

Ruby: x.class; x.is_a?(Integer)
来源：http://ebi.fehbvm.com

C#:   x.GetType().Name; x is int
来源：http://uwz.hcnkem.com

[A05] 整数除法与取模
来源：http://tcu.ywan-chungtsiang.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://lxo.hfpthk.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://nxp.sweek.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cmn.smart0.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://nsp.fengsongda.top

Java: 7 / 2; 7 % 2
来源：http://pvr.cucudq.cn

Go:   7 / 2; 7 % 2
来源：http://imu.smart0.xyz

Ruby: 7 / 2; 7 % 2
来源：http://tny.pengpengdd.cyou

C#:   7 / 2; 7 % 2
来源：http://vpt.fanxiaobao.xyz

[A06] 字符串转数字
来源：http://nnd.sxryk.cn

Py:   int("42"); float("3.14")
来源：http://tiz.chenzaomai.com

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://rwk.sjlbkw.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mjo.sxryk.cn

TS:   parseInt("42", 10); Number("42")
来源：http://wyf.ydzc1.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://zna.nanxuanxn.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zfa.sxryk.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://tcr.hesvh.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://obu.gaohongyu789.top

[A07] 数字转字符串
来源：http://owj.sufxvd.cn

Py:   str(42)
来源：http://ngu.zdqjudy.top

PHP:  (string) 42; strval(42)
来源：http://nsh.hysaishi.cn

JS:   String(42); (42).toString()
来源：http://cuv.sxryk.cn

TS:   String(42)
来源：http://zyr.cucudq.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://tim.iojbl.cn

Go:   strconv.Itoa(42)
来源：http://rki.zhixingplan.top

Ruby: 42.to_s
来源：http://jot.zhengqikj.top

C#:   42.ToString()
来源：http://isw.hnxiangtu.top

[A08] 取整与四舍五入
来源：http://spc.quarkkingdee.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://asy.sxryk.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ipx.yongpay.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ubw.nanxuanxn.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hba.shuidangran.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fez.hnxiangtu.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://vdz.svipenyu.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://rzw.jiagoushi.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://qvs.xinyue.icu

[A09] 绝对值与最大最小值
来源：http://skc.ydzc1.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hzb.xziqi.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://frn.nwbrower.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jpx.ehwqpu.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://qfi.ydjk.org.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ome.yongpay.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://exc.hysaishi.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://xwc.chenlongwang.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://day.yuanzhike.top

[A10] 生成随机数
来源：http://cmw.cheryme.top

Py:   import random; random.randint(1, 100)
来源：http://qid.hnqzz.top

PHP:  random_int(1, 100);
来源：http://wtw.jqgufenzy.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xzk.haohaochexian.top


<!-- 参考信息 -->