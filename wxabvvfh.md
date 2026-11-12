代发 wailian999

[U71] PHP：抛出异常
来源：http://ylz.fktsv.cn

throw new RuntimeException("失败", 500);
来源：http://kee.jlsjyb.cn

[U72] PHP：写错误日志
来源：http://jlb.c1oappe.top

error_log("失败: " . $e->getMessage());
来源：http://lzw.jinqigufen.top

[U73] PHP：读取 ini 配置
来源：http://iuf.kuanghao11.cn

parse_ini_file("config.ini", true)
来源：http://kah.yj20258888.top

[U74] PHP：读取环境变量
来源：http://kwl.yangfankeji.com

getenv("APP_ENV") ?: "production"
来源：http://dtx.yongpay.top

[U75] PHP：依赖注入
来源：http://hht.yongpay.top

composer require psr/container
来源：http://ogg.snrcjt.cn

[U76] PHP：简单路由
来源：http://qur.bjfxy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vsn.fengsongda.top

[U77] PHP：模板渲染
来源：http://xiu.sysykeji.top

composer require twig/twig
来源：http://kyj.xuanzx.com

[U78] PHP：单元测试
来源：http://ubv.jianghu66.top

composer require --dev phpunit/phpunit
来源：http://mds.cashguo.top

[U79] PHP：静态分析
来源：http://nlq.ppjwa.cn

composer require --dev phpstan/phpstan
来源：http://ngy.jqgfzy.top

[U80] PHP：代码规范修复
来源：http://ojb.wangdashe.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://gqw.yvedp.cn

[U81] JS：初始化项目
来源：http://txf.jinyuanbaomall.cn

npm init -y;  npm i express
来源：http://ifg.ydjk.org.cn

[U82] JS：package.json 脚本
来源：http://pwy.52xcode.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://hub.andypj.xyz

[U83] JS：ES Module 导入导出
来源：http://its.xuanzx.com

export const a = 1;  import { a } from "./m.js";
来源：http://sdu.shanyushiyangkeji.top

[U84] JS：CommonJS 写法
来源：http://ylo.hywenlv.cn

module.exports = { a };  const { a } = require("./m");
来源：http://skm.52xcode.cn

[U85] JS：可选链
来源：http://afy.redwolf501.top

a?.b?.c
来源：http://eoy.ppjwa.cn

[U86] JS：空值合并
来源：http://gke.guowangkeji.top

a ?? b
来源：http://mjk.redwolf501.top

[U87] JS：解构默认值
来源：http://imu.yuxming.cn

const { a = 1, b = 2 } = obj;
来源：http://xff.meibo888.top

[U88] JS：对象展开合并
来源：http://rep.tianlin.xyz

{ ...a, ...b }
来源：http://yny.redwolf501.top

[U89] JS：数组去重
来源：http://yax.fktsv.cn

[...new Set(arr)]
来源：http://mse.hesvh.cn

[U90] JS：数字数组排序
来源：http://yge.xziqi.cn

[...arr].sort((a, b) => a - b)
来源：http://tqf.jyoumei.cn

[U91] JS：对象键值遍历
来源：http://mhi.wangdashe.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mic.nanxinkj.top

[U92] JS：深拷贝
来源：http://dfx.vqdsnc.cn

structuredClone(obj)
来源：http://qav.yuxming.cn

[U93] JS：模板字符串
来源：http://kbh.fktsv.cn

`共 ${n} 条`
来源：http://wfh.wangshuangyany.cn

[U94] JS：箭头函数
来源：http://kpy.gogol.net.cn

const double = x => x * 2;
来源：http://wue.wangshuangyany.cn

[U95] JS：Promise 包装
来源：http://whm.52xcode.cn

new Promise((resolve, reject) => {})
来源：http://viv.hywenlv.cn

[U96] JS：async/await 与异常
来源：http://yip.andypj.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mqr.ydjk.org.cn

[U97] JS：并发请求
来源：http://jxt.jiagoushi.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://tjj.tian-w.cn

[U98] JS：fetch 带 JSON
来源：http://qdb.zhengqikj.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://moy.haohaochexian.top

[U99] JS：事件监听
来源：http://wys.chenjidiqi.icu

el.addEventListener("click", e => {})
来源：http://uza.wangshuangyany.cn

[U100] JS：DOM 查询
来源：http://xea.nanxinkj.top

document.querySelector(".item")
来源：http://gns.hammf.cn

[U101] JS：classList 操作
来源：http://ieu.zhaomingkeji.xyz

el.classList.toggle("active")
来源：http://joj.c1oappe.top

[U102] JS：本地存储
来源：http://hap.yonumen.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://sqq.fengsongda.top

[U103] JS：定时器
来源：http://lvf.sjlbkw.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vfr.jianghu66.top

[U104] JS：防抖
来源：http://unq.fehbvm.com

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ige.yuxming.cn

[U105] JS：节流
来源：http://bbq.guowangkeji.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://nvn.nwbrower.top

[U106] JS：日期格式化
来源：http://blg.fanxiaobao.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://zlz.xingfuxueyuan.xyz

[U107] JS：数字千分位
来源：http://otq.epnwcf.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://vrj.fzhhl.top

[U108] JS：随机整数
来源：http://rps.0kj1m.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://efi.yj202588.top

[U109] JS：数组分组
来源：http://sox.guowangkeji.top

Object.groupBy(arr, x => x.type)
来源：http://bna.xuanzx.com

[U110] JS：数组分块
来源：http://sfh.gzhubu.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://awb.aibaodan.cn

[U111] JS：对象转 Map
来源：http://pin.fzhhl.top

new Map(Object.entries(obj))
来源：http://xtd.haohaochexian.top

[U112] JS：字符串补位
来源：http://eon.zhongyouzk.top

"7".padStart(3, "0")
来源：http://vyg.meibo888.top

[U113] JS：正则替换全部
来源：http://fce.guannengcc.top

s.replaceAll("a", "b")
来源：http://faf.yfazqb.com

[U114] JS：JSON 深比较
来源：http://dxt.tarul.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://kpx.zhongyouzk.top

[U115] JS：生成 UUID
来源：http://vqr.haohaochexian.top

crypto.randomUUID()
来源：http://wdu.jqgfzy.top

[U116] JS：类型检查（JSDoc）
来源：http://cxx.iojbl.cn

/** @param {string} name */ function f(name) {}
来源：http://kfu.wangshuangyany.cn

[U117] JS：单元测试
来源：http://orq.jinqigufen.top

npm i -D vitest;  npx vitest
来源：http://zqb.yj20258888.top

[U118] JS：开发服务器
来源：http://djj.yfazqb.com

npm i -D vite;  npx vite
来源：http://maj.aizwys.cn

[U119] JS：生产构建
来源：http://xii.cheryme.top

npx vite build
来源：http://dbb.feifeiyinyue.top

[U120] JS：读取环境变量（Vite）
来源：http://bio.yangfankeji.com

import.meta.env.VITE_API_URL
来源：http://idd.cdnleiting.top

================================================================================
来源：http://akz.shangyingyoupin.top

统计汇总
来源：http://zuo.yuanzhike.top

================================================================================
来源：http://njw.gzhubu.top

按语言统计（条）：
来源：http://fwn.hcnkem.com

Python ......... 252
来源：http://lmj.aibaodan.cn

PHP ............ 252
来源：http://hku.cheryme.top

JavaScript ..... 252
来源：http://mux.gotoacloud.top

TypeScript ..... 212
来源：http://xvc.hfpthk.cn

Java ........... 212
来源：http://tcr.fktsv.cn

Go ............. 212
来源：http://qsn.0kj1m.cn

Ruby ........... 212
来源：http://wcm.zhijiandao.cn

C# ............. 212
来源：http://iws.havefunace.top

C .............. 30
来源：http://cvr.yongpay.top

C++ ............ 30
来源：http://pid.9152youxi.cn

SQL ............ 90
来源：http://srf.quarkkingdee.top

Bash ........... 80
来源：http://gtl.wangshuangyany.cn

Kotlin ......... 15
来源：http://nmw.zhoulong.xyz

Swift .......... 15
来源：http://cfv.bjfxy.top

Lua ............ 10
来源：http://ewg.sxryk.cn

Perl ........... 10
来源：http://kdd.sxryk.cn

Scala .......... 10
来源：http://ycl.chenlongwang.top

------------------------------------
来源：http://vkw.yongpay.top

合计 ........... 2106 条
来源：http://bqz.haohaochexian.top

按章节统计：
来源：http://ken.wangdashe.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rzm.xuanzx.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dnx.cucudq.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://qww.havefunace.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kza.tianlin.xyz

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://kch.snrcjt.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jea.haohaochexian.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://vrw.wangdashe.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wrd.sxryk.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://hes.fanxiaobao.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://gxk.hywenlv.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://nyc.haohaochexian.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://bdr.ywan-chungtsiang.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://ars.guowangkeji.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://bmv.hammf.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://hil.hnxiangtu.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://xaw.hammf.cn

Q SQL 专题                              90
来源：http://qhz.zhongyouzk.top

R Bash 专题                             80
来源：http://exp.quarkkingdee.top

S C / C++ 专题                          60
来源：http://ism.sxryk.cn

T 其他语言补充                          60
来源：http://yyj.shzxlz.cn

U 高频实用片段                         120
来源：http://mmw.zdqjudy.top

------------------------------------
来源：http://bwy.chenlongwang.top

合计                                  2106 条
来源：http://nde.hywenlv.cn

--------------------------------------------------------------------------------
来源：http://okw.pengpengdd.cyou

使用提醒
来源：http://qkt.hysaishi.cn

--------------------------------------------------------------------------------
来源：http://jhh.daxiang520.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zfm.ydjk.org.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://kvs.iojbl.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://cbn.fktsv.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://hrt.zhaomingkeji.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wai.jianghu66.top

—— 文件结束 ——
来源：http://ezp.gzhubu.top

================================================================================
来源：http://kyy.wangdashe.top

程序语言常见例子速查手册（2024 版）
来源：http://ztn.nanxinkj.top

Common Programming Examples Cheat Book
来源：http://mau.c1oappe.top

================================================================================
来源：http://lkd.dianchejie.cn

【收录内容】
来源：http://myh.c1oappe.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://hxu.gogol.net.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://uwn.316326.xyz

SQL · Bash · C · C++
来源：http://rkw.hywenlv.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://euy.9152youxi.cn

【使用说明】
来源：http://qtu.gogol.net.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://bjm.gaohongyu789.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://prn.pycfn.com

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://inz.aizwys.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://pjp.cqqwz.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://bnr.sweek.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tsp.jyoumei.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://xjv.zhijiandao.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://adm.zhixingplan.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bnj.nanxinkj.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://exz.bjfxy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pmc.ehwqpu.com

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qjo.fzhhl.top

【文件统计】
来源：http://ktj.nwbrower.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://lcx.jyoumei.cn

--------------------------------------------------------------------------------
来源：http://ntq.316326.xyz

目  录
来源：http://fsn.svipenyu.cn

--------------------------------------------------------------------------------
来源：http://tqd.uphjek.com

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wgx.jianghu66.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://uar.fktsv.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zdy.jinqigufen.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zlx.sysykeji.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vnx.ehwqpu.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ylo.52xcode.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://eyq.zhijiandao.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://rws.vehdjk.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wgv.svipenyu.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://dwd.fehbvm.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://cwl.sweek.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hoo.zhaomingkeji.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://cml.yvedp.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mkx.jyoumei.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wbj.haohaochexian.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://tzj.hfpthk.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ogp.jqgfzy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://mjc.kuanghao11.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ucy.ydzc1.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://hcg.ywan-chungtsiang.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mfp.jqgfzy.top

================================================================================
来源：http://kys.aizwys.cn

A. 基础语法与类型
来源：http://ocb.sweek.top

================================================================================
来源：http://uui.xziqi.cn

[A01] Hello World
来源：http://jkt.fehbvm.com

Py:   print("Hello, World!")
来源：http://lto.ywan-chungtsiang.top

PHP:  echo "Hello, World!";
来源：http://dxm.yuxming.cn

JS:   console.log("Hello, World!");
来源：http://cre.pengpengdd.cyou

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://yqr.mhx1999.top

Java: System.out.println("Hello, World!");
来源：http://kbm.nwbrower.top

Go:   fmt.Println("Hello, World!")
来源：http://toh.nanxuanxn.top

Ruby: puts "Hello, World!"
来源：http://bvz.hnqzz.top

C#:   Console.WriteLine("Hello, World!");
来源：http://nkg.cqqwz.cn

[A02] 变量声明与赋值
来源：http://ihf.zhoulong.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://iip.gzhubu.top

PHP:  $name = "Alex"; $age = 20;
来源：http://zhw.andypj.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://jlw.c1oappe.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ruf.jinyuanbaomall.cn

Java: String name = "Alex"; int age = 20;
来源：http://xcf.redwolf501.top

Go:   name := "Alex"; age := 20
来源：http://bvh.yj20258888.top

Ruby: name = "Alex"; age = 20
来源：http://yhj.feifeiyinyue.top

C#:   string name = "Alex"; int age = 20;
来源：http://pbt.yueranfly.top

[A03] 常量定义
来源：http://nix.mhx1999.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://lrs.52xcode.cn

PHP:  const PI = 3.14159;
来源：http://nqo.shangyingyoupin.top

JS:   const PI = 3.14159;
来源：http://zee.havefunace.top

TS:   const PI: number = 3.14159;
来源：http://ahl.gotoacloud.top

Java: static final double PI = 3.14159;
来源：http://zqi.ybcxt.top

Go:   const PI = 3.14159
来源：http://dlg.hysaishi.cn

Ruby: PI = 3.14159
来源：http://ghd.cqqwz.cn

C#:   const double PI = 3.14159;
来源：http://jbs.epnwcf.com

[A04] 判断变量类型
来源：http://ccn.pycfn.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://hwz.shanyushiyangkeji.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://fhb.xziqi.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://kdo.jinqigufen.top

TS:   typeof x; x instanceof Date
来源：http://obm.cashguo.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://enl.hnxiangtu.top

Go:   reflect.TypeOf(x).Name()
来源：http://jlw.hnqzz.top

Ruby: x.class; x.is_a?(Integer)
来源：http://emi.zhixingplan.top

C#:   x.GetType().Name; x is int
来源：http://wex.hammf.cn

[A05] 整数除法与取模
来源：http://kqh.yuxming.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://kiv.vehdjk.com

PHP:  intdiv(7, 2); 7 % 2
来源：http://gty.havefunace.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ewb.smart0.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://znu.jiagoushi.top

Java: 7 / 2; 7 % 2
来源：http://msd.shanyushiyangtech.top

Go:   7 / 2; 7 % 2
来源：http://dys.hnqzz.top

Ruby: 7 / 2; 7 % 2
来源：http://ttv.wangshuangyany.cn

C#:   7 / 2; 7 % 2
来源：http://bpy.yonumen.top

[A06] 字符串转数字
来源：http://dht.smart0.xyz

Py:   int("42"); float("3.14")
来源：http://mqf.316326.xyz

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lzo.ctjpmb.com

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://peu.quarkkingdee.top

TS:   parseInt("42", 10); Number("42")
来源：http://fvm.9152youxi.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rar.zhixingplan.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cdi.sjlbkw.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://rwx.yfazqb.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dwp.ivvv.top

[A07] 数字转字符串
来源：http://lsc.zhiwuduotai.top

Py:   str(42)
来源：http://wtc.yfazqb.com

PHP:  (string) 42; strval(42)
来源：http://hpt.cheryme.top

JS:   String(42); (42).toString()
来源：http://zkw.smart0.xyz

TS:   String(42)
来源：http://hfe.aibaodan.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://hkg.daxiang520.top

Go:   strconv.Itoa(42)
来源：http://hpu.fanxiaobao.xyz

Ruby: 42.to_s
来源：http://zdx.jinqigufen.top

C#:   42.ToString()
来源：http://exy.guannengcc.top

[A08] 取整与四舍五入
来源：http://dln.havefunace.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://eks.fengsongda.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://vuc.jianghu66.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hnp.nwbrower.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://kep.zhongyouzk.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://cut.daria6918.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xat.guowangkeji.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://ihb.redwolf501.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://tie.sweek.top

[A09] 绝对值与最大最小值
来源：http://ejd.gzhubu.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://udi.yongpay.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://rvj.sxryk.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://xik.52xcode.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://zok.fehbvm.com

Java: Math.abs(-5); Math.max(1, 2)
来源：http://yju.vqdsnc.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://cwo.xinyue.icu

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://fut.jinyuanbaomall.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mng.shuidangran.top

[A10] 生成随机数
来源：http://zcr.sysykeji.top

Py:   import random; random.randint(1, 100)
来源：http://zpt.hnxiangtu.top

PHP:  random_int(1, 100);
来源：http://cxa.epnwcf.com

JS:   Math.floor(Math.random() * 100) + 1
来源：http://nge.ctjpmb.com

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mma.shanyushiyangtech.top

Java: new Random().nextInt(100) + 1
来源：http://ads.zdqjudy.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://qca.zhengqikj.top

Ruby: rand(1..100)
来源：http://jjh.hysaishi.cn

C#:   new Random().Next(1, 101)
来源：http://zkw.tanke756.top

[A11] 条件表达式（三元）
来源：http://rgq.vehdjk.com

Py:   "yes" if x > 0 else "no"
来源：http://gxo.ehwqpu.com

PHP:  $x > 0 ? "yes" : "no"
来源：http://ddj.jqgfzy.top


<!-- 参考信息 -->