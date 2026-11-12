代发 wailian999

[U71] PHP：抛出异常
来源：http://gmd.ybcxt.top

throw new RuntimeException("失败", 500);
来源：http://gmk.jqgufenzy.top

[U72] PHP：写错误日志
来源：http://nvz.zhijiandao.cn

error_log("失败: " . $e->getMessage());
来源：http://bhu.gotoacloud.top

[U73] PHP：读取 ini 配置
来源：http://epj.gotoacloud.top

parse_ini_file("config.ini", true)
来源：http://szq.nwbrower.top

[U74] PHP：读取环境变量
来源：http://gez.havefunace.top

getenv("APP_ENV") ?: "production"
来源：http://noa.nanxuanxn.top

[U75] PHP：依赖注入
来源：http://wbi.ehwqpu.com

composer require psr/container
来源：http://oyr.bjfxy.top

[U76] PHP：简单路由
来源：http://zmi.yueranfly.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gar.sysykeji.top

[U77] PHP：模板渲染
来源：http://dvk.yj20258.top

composer require twig/twig
来源：http://hnf.sjlbkw.cn

[U78] PHP：单元测试
来源：http://zlt.meibo888.top

composer require --dev phpunit/phpunit
来源：http://vtv.jianghu66.top

[U79] PHP：静态分析
来源：http://awp.haohaochexian.top

composer require --dev phpstan/phpstan
来源：http://tvr.hysaishi.cn

[U80] PHP：代码规范修复
来源：http://hws.zhengqikj.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://mqd.bjfxy.top

[U81] JS：初始化项目
来源：http://cmc.gotoacloud.top

npm init -y;  npm i express
来源：http://atj.aizwys.cn

[U82] JS：package.json 脚本
来源：http://jyx.zhoulong.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vfc.chenjidiqi.icu

[U83] JS：ES Module 导入导出
来源：http://nlw.vehdjk.com

export const a = 1;  import { a } from "./m.js";
来源：http://xms.zhiwuduotai.top

[U84] JS：CommonJS 写法
来源：http://taj.snrcjt.cn

module.exports = { a };  const { a } = require("./m");
来源：http://tya.ydjk.org.cn

[U85] JS：可选链
来源：http://uih.yj202588.top

a?.b?.c
来源：http://pzk.vqdsnc.cn

[U86] JS：空值合并
来源：http://fmz.jinqigfzy.top

a ?? b
来源：http://shq.jinyuanbaomall.cn

[U87] JS：解构默认值
来源：http://xau.svipenyu.cn

const { a = 1, b = 2 } = obj;
来源：http://wvg.tian-w.cn

[U88] JS：对象展开合并
来源：http://ifk.zhijiandao.cn

{ ...a, ...b }
来源：http://ywf.chenzaomai.com

[U89] JS：数组去重
来源：http://fva.kuanghao11.cn

[...new Set(arr)]
来源：http://bqt.ppjwa.cn

[U90] JS：数字数组排序
来源：http://nko.shanyushiyangtech.top

[...arr].sort((a, b) => a - b)
来源：http://afo.yonumen.top

[U91] JS：对象键值遍历
来源：http://jrv.jianghu66.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bgs.yongpay.top

[U92] JS：深拷贝
来源：http://vyf.sufxvd.cn

structuredClone(obj)
来源：http://qvx.fzhhl.top

[U93] JS：模板字符串
来源：http://dfs.sxryk.cn

`共 ${n} 条`
来源：http://miy.jinghuilouyu.cn

[U94] JS：箭头函数
来源：http://prp.shuidangran.top

const double = x => x * 2;
来源：http://bbs.hcnkem.com

[U95] JS：Promise 包装
来源：http://rpa.fzhhl.top

new Promise((resolve, reject) => {})
来源：http://pxj.ppjwa.cn

[U96] JS：async/await 与异常
来源：http://blk.zhongyouzk.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://hfs.zhoulong.xyz

[U97] JS：并发请求
来源：http://nfv.ybcxt.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://ezx.zdbjq.cn

[U98] JS：fetch 带 JSON
来源：http://ddw.hysaishi.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://cbe.jiagoushi.top

[U99] JS：事件监听
来源：http://vdj.gzhubu.top

el.addEventListener("click", e => {})
来源：http://uzh.yanxiufei.cn

[U100] JS：DOM 查询
来源：http://hgm.ivvv.top

document.querySelector(".item")
来源：http://zop.ybcxt.top

[U101] JS：classList 操作
来源：http://jxl.ivvv.top

el.classList.toggle("active")
来源：http://yqk.sjlbkw.cn

[U102] JS：本地存储
来源：http://eik.fktsv.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://fmb.gotoacloud.top

[U103] JS：定时器
来源：http://qhr.chenjidiqi.icu

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mss.yvedp.cn

[U104] JS：防抖
来源：http://iie.shuidangran.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iby.sweek.top

[U105] JS：节流
来源：http://nmg.sjlbkw.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://cst.fzhhl.top

[U106] JS：日期格式化
来源：http://ekw.redwolf501.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ijf.jqgufenzy.top

[U107] JS：数字千分位
来源：http://meq.andypj.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://apf.pycfn.com

[U108] JS：随机整数
来源：http://ckf.shanyushiyangtech.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://uqf.feifeiyinyue.top

[U109] JS：数组分组
来源：http://jdy.yuanzhike.top

Object.groupBy(arr, x => x.type)
来源：http://jam.fehbvm.com

[U110] JS：数组分块
来源：http://ccc.52xcode.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://ogu.hongshengwenyu.top

[U111] JS：对象转 Map
来源：http://yvj.sufxvd.cn

new Map(Object.entries(obj))
来源：http://mts.sysykeji.top

[U112] JS：字符串补位
来源：http://nfg.jyoumei.cn

"7".padStart(3, "0")
来源：http://rpi.ybcxt.top

[U113] JS：正则替换全部
来源：http://rtl.tian-w.cn

s.replaceAll("a", "b")
来源：http://wez.yuanzhike.top

[U114] JS：JSON 深比较
来源：http://jwg.sysykeji.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://ieo.yuxming.cn

[U115] JS：生成 UUID
来源：http://ajg.zhongyouzk.top

crypto.randomUUID()
来源：http://kif.snrcjt.cn

[U116] JS：类型检查（JSDoc）
来源：http://mwk.chenjidiqi.icu

/** @param {string} name */ function f(name) {}
来源：http://iid.gzhubu.top

[U117] JS：单元测试
来源：http://dzg.ybcxt.top

npm i -D vitest;  npx vitest
来源：http://szq.bbcook.cn

[U118] JS：开发服务器
来源：http://yfc.zycfv.cn

npm i -D vite;  npx vite
来源：http://ycp.zhoulong.xyz

[U119] JS：生产构建
来源：http://qvx.yanxiufei.cn

npx vite build
来源：http://ctz.pengpengdd.cyou

[U120] JS：读取环境变量（Vite）
来源：http://kzk.fzhhl.top

import.meta.env.VITE_API_URL
来源：http://cir.jianghu66.top

================================================================================
来源：http://moh.c1oappe.top

统计汇总
来源：http://ucg.wangshuangyany.cn

================================================================================
来源：http://ouq.yuxming.cn

按语言统计（条）：
来源：http://qgq.mhx1999.top

Python ......... 252
来源：http://yyw.jianghu66.top

PHP ............ 252
来源：http://ogv.gotoacloud.top

JavaScript ..... 252
来源：http://lzc.jlsjyb.cn

TypeScript ..... 212
来源：http://wyc.jinghuilouyu.cn

Java ........... 212
来源：http://ios.52xcode.cn

Go ............. 212
来源：http://rtp.jinyuanbaomall.cn

Ruby ........... 212
来源：http://sod.jqgfzy.top

C# ............. 212
来源：http://mgj.yj20258.top

C .............. 30
来源：http://plz.shangyingyoupin.top

C++ ............ 30
来源：http://vbx.shanyushiyangtech.top

SQL ............ 90
来源：http://txf.nanxinkj.top

Bash ........... 80
来源：http://tvh.chenjidiqi.icu

Kotlin ......... 15
来源：http://tkm.ybcxt.top

Swift .......... 15
来源：http://cww.zhoulong.xyz

Lua ............ 10
来源：http://qfi.epnwcf.com

Perl ........... 10
来源：http://dzc.meibo888.top

Scala .......... 10
来源：http://jsd.yonumen.top

------------------------------------
来源：http://wtw.wangdashe.top

合计 ........... 2106 条
来源：http://hzs.jyoumei.cn

按章节统计：
来源：http://ntj.sysykeji.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://juc.shangyingyoupin.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://qyk.zhoulong.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://idd.cqqwz.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://uzl.yongpay.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wwq.nwbrower.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://evx.jinyuanbaomall.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://yec.bbcook.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://tah.sysykeji.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ehr.shanyushiyangtech.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mrp.9152youxi.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://cqt.cucudq.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://kcl.sxryk.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hji.yj202588.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://waq.guowangkeji.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://ctr.ybcxt.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tmu.gaohongyu789.top

Q SQL 专题                              90
来源：http://cfr.ywan-chungtsiang.top

R Bash 专题                             80
来源：http://ikj.ywan-chungtsiang.top

S C / C++ 专题                          60
来源：http://csa.hcnkem.com

T 其他语言补充                          60
来源：http://lzt.zhijiandao.cn

U 高频实用片段                         120
来源：http://kui.hnxiangtu.top

------------------------------------
来源：http://rsi.chenlongwang.top

合计                                  2106 条
来源：http://oyj.hysaishi.cn

--------------------------------------------------------------------------------
来源：http://nvk.wangshuangyany.cn

使用提醒
来源：http://qhh.svipenyu.cn

--------------------------------------------------------------------------------
来源：http://are.sjlbkw.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://tin.hcnkem.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jkd.nanxinkj.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://qvz.fengsongda.top

在旧版本上使用前请先确认语法支持情况。
来源：http://xon.hywenlv.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://zya.havefunace.top

—— 文件结束 ——
来源：http://ltl.gotoacloud.top

================================================================================
来源：http://jay.guowangkeji.top

程序语言常见例子速查手册（2024 版）
来源：http://mce.fengsongda.top

Common Programming Examples Cheat Book
来源：http://jax.jqgfzy.top

================================================================================
来源：http://agn.feifeiyinyue.top

【收录内容】
来源：http://lei.zhaomingkeji.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://xyl.yongpay.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://gof.aizwys.cn

SQL · Bash · C · C++
来源：http://icm.quarkkingdee.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://smd.sufxvd.cn

【使用说明】
来源：http://adu.mhx1999.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://llx.ydjk.org.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://gzh.shangyingyoupin.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://bis.quarkkingdee.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://rzt.yongpay.top

Bash:  Shell         C:     C             C++:   C++
来源：http://veu.quarkkingdee.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://hcp.ydjk.org.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wee.yj20258888.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gtq.jqgufenzy.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://cxi.pengpengdd.cyou

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://yjd.xuanzx.com

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://cbq.52xcode.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://jxt.tanke756.top

【文件统计】
来源：http://zxi.hnxiangtu.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://qpn.guannengcc.top

--------------------------------------------------------------------------------
来源：http://jvv.yuanzhike.top

目  录
来源：http://wcd.zhongyouzk.top

--------------------------------------------------------------------------------
来源：http://esu.aizwys.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ima.pengpengdd.cyou

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://rso.9152youxi.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://tcc.uphjek.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bjq.epnwcf.com

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hat.pengpengdd.cyou

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://kdh.fktsv.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://fri.zhaomingkeji.xyz

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://eiv.birdmap.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://qch.jqgufenzy.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cit.sxryk.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://kfy.shzxlz.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://gaz.iojbl.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cpa.gaohongyu789.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://msp.shanyushiyangtech.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://stq.havefunace.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kgr.ydzc1.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://zuv.cheryme.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://lur.yvedp.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rmp.aibaodan.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wkx.316326.xyz

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ytp.birdmap.top

================================================================================
来源：http://brq.sxryk.cn

A. 基础语法与类型
来源：http://yns.fzhhl.top

================================================================================
来源：http://tur.feifeiyinyue.top

[A01] Hello World
来源：http://omg.xuanzx.com

Py:   print("Hello, World!")
来源：http://ymu.daxiang520.top

PHP:  echo "Hello, World!";
来源：http://lxe.ybcxt.top

JS:   console.log("Hello, World!");
来源：http://lik.jinqigfzy.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hgi.iojbl.cn

Java: System.out.println("Hello, World!");
来源：http://srp.cqqwz.cn

Go:   fmt.Println("Hello, World!")
来源：http://ljh.redwolf501.top

Ruby: puts "Hello, World!"
来源：http://nik.wangshuangyany.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://dvc.hysaishi.cn

[A02] 变量声明与赋值
来源：http://whm.jiagoushi.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://uni.tian-w.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://xnz.tianlin.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://gho.havefunace.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://luu.yj20258888.top

Java: String name = "Alex"; int age = 20;
来源：http://nuz.zdqjudy.top

Go:   name := "Alex"; age := 20
来源：http://iju.cdnleiting.top

Ruby: name = "Alex"; age = 20
来源：http://rly.cheryme.top

C#:   string name = "Alex"; int age = 20;
来源：http://dur.quarkkingdee.top

[A03] 常量定义
来源：http://rmo.0kj1m.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://afu.dianchejie.cn

PHP:  const PI = 3.14159;
来源：http://uou.yuanzhike.top

JS:   const PI = 3.14159;
来源：http://wyn.jinyuanbaomall.cn

TS:   const PI: number = 3.14159;
来源：http://mva.daxiang520.top

Java: static final double PI = 3.14159;
来源：http://uoe.ydzc1.top

Go:   const PI = 3.14159
来源：http://prc.feifeiyinyue.top

Ruby: PI = 3.14159
来源：http://gnz.sjlbkw.cn

C#:   const double PI = 3.14159;
来源：http://fdj.yj20258888.top

[A04] 判断变量类型
来源：http://xcy.cucudq.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://yzn.xziqi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ctc.yvedp.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://etm.andypj.xyz

TS:   typeof x; x instanceof Date
来源：http://qeg.yangfankeji.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://xvp.hnxiangtu.top

Go:   reflect.TypeOf(x).Name()
来源：http://mxa.chenzaomai.com

Ruby: x.class; x.is_a?(Integer)
来源：http://eos.9152youxi.cn

C#:   x.GetType().Name; x is int
来源：http://zfh.vqdsnc.cn

[A05] 整数除法与取模
来源：http://evs.ybcxt.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://akn.yanxiufei.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://raq.chenzaomai.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://imu.hnxiangtu.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://twt.tanke756.top

Java: 7 / 2; 7 % 2
来源：http://ghy.0kj1m.cn

Go:   7 / 2; 7 % 2
来源：http://jyy.zhoulong.xyz

Ruby: 7 / 2; 7 % 2
来源：http://kho.pycfn.com

C#:   7 / 2; 7 % 2
来源：http://zta.52xcode.cn

[A06] 字符串转数字
来源：http://pqq.fktsv.cn

Py:   int("42"); float("3.14")
来源：http://ulo.xingfuxueyuan.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kxd.yj20258.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mkt.svipenyu.cn

TS:   parseInt("42", 10); Number("42")
来源：http://lvy.daxiang520.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://oer.hongshengwenyu.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://smh.316326.xyz

Ruby: "42".to_i; "3.14".to_f
来源：http://huw.sxryk.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fff.hysaishi.cn

[A07] 数字转字符串
来源：http://vim.xuanzx.com

Py:   str(42)
来源：http://fne.hywenlv.cn

PHP:  (string) 42; strval(42)
来源：http://jjj.gzhubu.top

JS:   String(42); (42).toString()
来源：http://pky.chenlongwang.top

TS:   String(42)
来源：http://aij.ppjwa.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://hlw.gogol.net.cn

Go:   strconv.Itoa(42)
来源：http://zeu.tanke756.top

Ruby: 42.to_s
来源：http://tea.zhijiandao.cn

C#:   42.ToString()
来源：http://riq.yj20258888.top

[A08] 取整与四舍五入
来源：http://lcv.dashuyun.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ikv.zhiwuduotai.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://yzt.fengsongda.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://czq.pycfn.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://sjp.hnqzz.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://lfl.ehwqpu.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://uxt.chenjidiqi.icu

Ruby: 3.567.round(2); 3.9.floor
来源：http://zff.zhongyouzk.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://ivu.ctjpmb.com

[A09] 绝对值与最大最小值
来源：http://eov.zhaomingkeji.xyz

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://xzd.guannengcc.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://yjm.xingfuxueyuan.xyz

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vlk.cheryme.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://nbc.hnxiangtu.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://ivz.tarul.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.dianchejie.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://umw.nwbrower.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://emp.chenlongwang.top

[A10] 生成随机数
来源：http://ebh.vehdjk.com

Py:   import random; random.randint(1, 100)
来源：http://end.xylfe.cn

PHP:  random_int(1, 100);
来源：http://hbt.yuxming.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://xqr.jlsjyb.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://txe.gaohongyu789.top

Java: new Random().nextInt(100) + 1
来源：http://fju.shuidangran.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://gxu.yj202588.top

Ruby: rand(1..100)
来源：http://wir.fktsv.cn

C#:   new Random().Next(1, 101)
来源：http://qtt.shangyingyoupin.top

[A11] 条件表达式（三元）
来源：http://tsj.zhengqikj.top

Py:   "yes" if x > 0 else "no"
来源：http://zel.dianchejie.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://idl.fktsv.cn


<!-- 参考信息 -->