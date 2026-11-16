代发 wailian999

[U71] PHP：抛出异常
来源：http://kzi.aibaodan.cn

throw new RuntimeException("失败", 500);
来源：http://vrf.zdqjudy.top

[U72] PHP：写错误日志
来源：http://gqk.ctjpmb.com

error_log("失败: " . $e->getMessage());
来源：http://nqa.chenlongwang.top

[U73] PHP：读取 ini 配置
来源：http://npe.fzhhl.top

parse_ini_file("config.ini", true)
来源：http://drk.ydjk.org.cn

[U74] PHP：读取环境变量
来源：http://fkf.haohaochexian.top

getenv("APP_ENV") ?: "production"
来源：http://xlb.shanyushiyangkeji.top

[U75] PHP：依赖注入
来源：http://ddi.sweek.top

composer require psr/container
来源：http://hiz.zhixingplan.top

[U76] PHP：简单路由
来源：http://ymw.pengpengdd.cyou

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lqh.dianchejie.cn

[U77] PHP：模板渲染
来源：http://zgn.hnxiangtu.top

composer require twig/twig
来源：http://dnw.aibaodan.cn

[U78] PHP：单元测试
来源：http://tay.gogol.net.cn

composer require --dev phpunit/phpunit
来源：http://wze.quarkkingdee.top

[U79] PHP：静态分析
来源：http://kfe.andypj.xyz

composer require --dev phpstan/phpstan
来源：http://osn.shangyingyoupin.top

[U80] PHP：代码规范修复
来源：http://pzi.tianlin.xyz

composer require --dev friendsofphp/php-cs-fixer
来源：http://ndh.shanyushiyangtech.top

[U81] JS：初始化项目
来源：http://ewx.tianlin.xyz

npm init -y;  npm i express
来源：http://hbu.zhixingplan.top

[U82] JS：package.json 脚本
来源：http://vsw.xinyue.icu

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wgx.chenlongwang.top

[U83] JS：ES Module 导入导出
来源：http://mas.kuanghao11.cn

export const a = 1;  import { a } from "./m.js";
来源：http://fsa.ydjk.org.cn

[U84] JS：CommonJS 写法
来源：http://bbh.shuidangran.top

module.exports = { a };  const { a } = require("./m");
来源：http://bqz.zhijiandao.cn

[U85] JS：可选链
来源：http://jxj.guannengcc.top

a?.b?.c
来源：http://bwu.dashuyun.cn

[U86] JS：空值合并
来源：http://ogt.fktsv.cn

a ?? b
来源：http://fzc.zhoulong.xyz

[U87] JS：解构默认值
来源：http://ihd.yj20258.top

const { a = 1, b = 2 } = obj;
来源：http://qpf.bbcook.cn

[U88] JS：对象展开合并
来源：http://qzc.hfpthk.cn

{ ...a, ...b }
来源：http://ham.epnwcf.com

[U89] JS：数组去重
来源：http://yia.gaohongyu789.top

[...new Set(arr)]
来源：http://vvj.yongpay.top

[U90] JS：数字数组排序
来源：http://ooh.redwolf501.top

[...arr].sort((a, b) => a - b)
来源：http://rvj.chenzaomai.com

[U91] JS：对象键值遍历
来源：http://mmc.fzhhl.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://knv.yangfankeji.com

[U92] JS：深拷贝
来源：http://yda.hongshengwenyu.top

structuredClone(obj)
来源：http://ana.c1oappe.top

[U93] JS：模板字符串
来源：http://xab.tanke756.top

`共 ${n} 条`
来源：http://vdd.yangfankeji.com

[U94] JS：箭头函数
来源：http://tqg.yj20258888.top

const double = x => x * 2;
来源：http://xzr.nanxuanxn.top

[U95] JS：Promise 包装
来源：http://pqx.chenlongwang.top

new Promise((resolve, reject) => {})
来源：http://img.hesvh.cn

[U96] JS：async/await 与异常
来源：http://gmm.guannengcc.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://cwf.zdbjq.cn

[U97] JS：并发请求
来源：http://rdg.wangdashe.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://dlk.cucudq.cn

[U98] JS：fetch 带 JSON
来源：http://knj.guannengcc.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wkr.hysaishi.cn

[U99] JS：事件监听
来源：http://ncw.kuanghao11.cn

el.addEventListener("click", e => {})
来源：http://uxo.svipenyu.cn

[U100] JS：DOM 查询
来源：http://noc.pengpengdd.cyou

document.querySelector(".item")
来源：http://dps.sxryk.cn

[U101] JS：classList 操作
来源：http://yte.zhixingplan.top

el.classList.toggle("active")
来源：http://hei.jinqigfzy.top

[U102] JS：本地存储
来源：http://vag.jinqigfzy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://mtu.yongpay.top

[U103] JS：定时器
来源：http://nks.cheryme.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://trm.ppjwa.cn

[U104] JS：防抖
来源：http://fud.ppjwa.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xcq.gzhubu.top

[U105] JS：节流
来源：http://bhu.yonumen.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://fzr.zhijiandao.cn

[U106] JS：日期格式化
来源：http://olk.0kj1m.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bqq.hysaishi.cn

[U107] JS：数字千分位
来源：http://haw.snrcjt.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://cvq.wangdashe.top

[U108] JS：随机整数
来源：http://wug.gotoacloud.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ccw.shzxlz.cn

[U109] JS：数组分组
来源：http://dtd.shanyushiyangtech.top

Object.groupBy(arr, x => x.type)
来源：http://ygj.fktsv.cn

[U110] JS：数组分块
来源：http://gos.shanyushiyangtech.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://itq.fzhhl.top

[U111] JS：对象转 Map
来源：http://xad.shuidangran.top

new Map(Object.entries(obj))
来源：http://fkl.c1oappe.top

[U112] JS：字符串补位
来源：http://voa.52xcode.cn

"7".padStart(3, "0")
来源：http://qqv.jlsjyb.cn

[U113] JS：正则替换全部
来源：http://uxh.birdmap.top

s.replaceAll("a", "b")
来源：http://aks.shanyushiyangkeji.top

[U114] JS：JSON 深比较
来源：http://oce.zhongyouzk.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://itf.hnqzz.top

[U115] JS：生成 UUID
来源：http://dux.jiagoushi.top

crypto.randomUUID()
来源：http://ood.chenzaomai.com

[U116] JS：类型检查（JSDoc）
来源：http://jun.vehdjk.com

/** @param {string} name */ function f(name) {}
来源：http://ynw.jianghu66.top

[U117] JS：单元测试
来源：http://aip.tianlin.xyz

npm i -D vitest;  npx vitest
来源：http://ipb.jlsjyb.cn

[U118] JS：开发服务器
来源：http://ycz.shanyushiyangtech.top

npm i -D vite;  npx vite
来源：http://qsu.tianlin.xyz

[U119] JS：生产构建
来源：http://mym.vqdsnc.cn

npx vite build
来源：http://kln.daria6918.cn

[U120] JS：读取环境变量（Vite）
来源：http://zqf.tanke756.top

import.meta.env.VITE_API_URL
来源：http://bvs.zycfv.cn

================================================================================
来源：http://epl.tianlin.xyz

统计汇总
来源：http://xvl.gaohongyu789.top

================================================================================
来源：http://eyk.cheryme.top

按语言统计（条）：
来源：http://rom.quarkkingdee.top

Python ......... 252
来源：http://nci.hongshengwenyu.top

PHP ............ 252
来源：http://qnj.aizwys.cn

JavaScript ..... 252
来源：http://psj.yj20258.top

TypeScript ..... 212
来源：http://jju.fktsv.cn

Java ........... 212
来源：http://nno.yvedp.cn

Go ............. 212
来源：http://yvj.meibo888.top

Ruby ........... 212
来源：http://vcm.smart0.xyz

C# ............. 212
来源：http://jvt.hesvh.cn

C .............. 30
来源：http://vus.jinqigufen.top

C++ ............ 30
来源：http://xdm.9152youxi.cn

SQL ............ 90
来源：http://wfz.shangyingyoupin.top

Bash ........... 80
来源：http://fle.hysaishi.cn

Kotlin ......... 15
来源：http://lae.yfazqb.com

Swift .......... 15
来源：http://acs.hywenlv.cn

Lua ............ 10
来源：http://uxl.hnqzz.top

Perl ........... 10
来源：http://vgw.ydjk.org.cn

Scala .......... 10
来源：http://yal.yj202588.top

------------------------------------
来源：http://xrb.andypj.xyz

合计 ........... 2106 条
来源：http://wsq.hammf.cn

按章节统计：
来源：http://gvq.zhoulong.xyz

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://cxq.cheryme.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://utt.fktsv.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://ipm.zhixingplan.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://rye.yongpay.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xrf.quarkkingdee.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tld.xuetiantiany.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://jcw.shangyingyoupin.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://ptm.jinqigfzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://pnt.chenlongwang.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nvq.smart0.xyz

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kyh.hammf.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nzc.bbcook.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://smm.vqdsnc.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qds.zhiwuduotai.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://itw.cqqwz.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ckf.vehdjk.com

Q SQL 专题                              90
来源：http://ycn.andypj.xyz

R Bash 专题                             80
来源：http://waz.yanxiufei.cn

S C / C++ 专题                          60
来源：http://vkq.zhiwuduotai.top

T 其他语言补充                          60
来源：http://ajb.yfazqb.com

U 高频实用片段                         120
来源：http://yai.zhongyouzk.top

------------------------------------
来源：http://gil.jianghu66.top

合计                                  2106 条
来源：http://ubq.xuetiantiany.cn

--------------------------------------------------------------------------------
来源：http://yrw.xuetiantiany.cn

使用提醒
来源：http://yjs.hcnkem.com

--------------------------------------------------------------------------------
来源：http://wma.fktsv.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://atv.hongshengwenyu.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://jwm.chenlongwang.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://owe.sxryk.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://fbg.zhoulong.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://bfr.tianlin.xyz

—— 文件结束 ——
来源：http://sxk.pengpengdd.cyou

================================================================================
来源：http://gmr.jinghuilouyu.cn

程序语言常见例子速查手册（2024 版）
来源：http://ksr.uphjek.com

Common Programming Examples Cheat Book
来源：http://igl.chenjidiqi.icu

================================================================================
来源：http://tjf.fengsongda.top

【收录内容】
来源：http://hzu.yanxiufei.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://ozs.hnqzz.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ngm.feifeiyinyue.top

SQL · Bash · C · C++
来源：http://bju.9152youxi.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://ocu.ybcxt.top

【使用说明】
来源：http://rit.cqqwz.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://qoy.zdqjudy.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lxu.meibo888.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mlm.aizwys.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://sfh.sjlbkw.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://dvj.uphjek.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ryi.52xcode.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://leh.dashuyun.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://qle.snrcjt.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mal.guannengcc.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://nvm.chenlongwang.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://xti.cdnleiting.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://eaa.hcnkem.com

【文件统计】
来源：http://udj.shangyingyoupin.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://kow.daria6918.cn

--------------------------------------------------------------------------------
来源：http://eku.zdqjudy.top

目  录
来源：http://efk.yj20258888.top

--------------------------------------------------------------------------------
来源：http://xdz.zdqjudy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://bfu.zhaomingkeji.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zjq.havefunace.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://nbr.jqgfzy.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://bgj.zhongyouzk.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://too.daria6918.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://vhn.52xcode.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://isf.shanyushiyangtech.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://bbq.tianlin.xyz

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jek.hysaishi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://hmk.uphjek.com

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wbh.tanke756.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://tuz.yj202588.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dzj.shuidangran.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://uij.aibaodan.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://dau.xuanzx.com

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rly.sxryk.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://jdn.jqgfzy.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://orm.ybcxt.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ygz.hysaishi.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wvz.shzxlz.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ath.shangyingyoupin.top

================================================================================
来源：http://csf.cucudq.cn

A. 基础语法与类型
来源：http://uec.shuidangran.top

================================================================================
来源：http://sxc.yangfankeji.com

[A01] Hello World
来源：http://cpq.chenlongwang.top

Py:   print("Hello, World!")
来源：http://ncb.yuanzhike.top

PHP:  echo "Hello, World!";
来源：http://jyb.yangfankeji.com

JS:   console.log("Hello, World!");
来源：http://bpj.ywan-chungtsiang.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://hyr.ehwqpu.com

Java: System.out.println("Hello, World!");
来源：http://kbk.ehwqpu.com

Go:   fmt.Println("Hello, World!")
来源：http://vyo.316326.xyz

Ruby: puts "Hello, World!"
来源：http://zhf.nanxinkj.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ddc.cqqwz.cn

[A02] 变量声明与赋值
来源：http://aqk.jinqigufen.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://exa.zycfv.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://jzg.zhijiandao.cn

JS:   let name = "Alex"; const age = 20;
来源：http://tsg.tianlin.xyz

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://obl.fktsv.cn

Java: String name = "Alex"; int age = 20;
来源：http://hbg.jinqigufen.top

Go:   name := "Alex"; age := 20
来源：http://emd.tarul.cn

Ruby: name = "Alex"; age = 20
来源：http://uzn.smart0.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://dlc.yj20258.top

[A03] 常量定义
来源：http://czb.dianchejie.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zdx.chenzaomai.com

PHP:  const PI = 3.14159;
来源：http://hit.xuetiantiany.cn

JS:   const PI = 3.14159;
来源：http://sen.xuanzx.com

TS:   const PI: number = 3.14159;
来源：http://ajc.xylfe.cn

Java: static final double PI = 3.14159;
来源：http://krp.hnxiangtu.top

Go:   const PI = 3.14159
来源：http://qdp.jinyuanbaomall.cn

Ruby: PI = 3.14159
来源：http://upq.nwbrower.top

C#:   const double PI = 3.14159;
来源：http://zac.shuidangran.top

[A04] 判断变量类型
来源：http://fqd.epnwcf.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://fjv.yueranfly.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://aci.gzhubu.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nfj.yvedp.cn

TS:   typeof x; x instanceof Date
来源：http://bkm.shanyushiyangkeji.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://cvb.zycfv.cn

Go:   reflect.TypeOf(x).Name()
来源：http://mrf.yongpay.top

Ruby: x.class; x.is_a?(Integer)
来源：http://dtq.zhongyouzk.top

C#:   x.GetType().Name; x is int
来源：http://fan.xylfe.cn

[A05] 整数除法与取模
来源：http://lhe.yueranfly.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ccq.xylfe.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://ewc.nanxinkj.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://pii.zhiwuduotai.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wth.daxiang520.top

Java: 7 / 2; 7 % 2
来源：http://cyu.dianchejie.cn

Go:   7 / 2; 7 % 2
来源：http://ial.epnwcf.com

Ruby: 7 / 2; 7 % 2
来源：http://kih.jqgufenzy.top

C#:   7 / 2; 7 % 2
来源：http://nrn.yfazqb.com

[A06] 字符串转数字
来源：http://tif.vqdsnc.cn

Py:   int("42"); float("3.14")
来源：http://kdr.xziqi.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pvt.smart0.xyz

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dtm.pengpengdd.cyou

TS:   parseInt("42", 10); Number("42")
来源：http://sgw.hnqzz.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://toj.jinqigfzy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://uct.nanxinkj.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ulg.hongshengwenyu.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://vlg.wangdashe.top

[A07] 数字转字符串
来源：http://ema.cheryme.top

Py:   str(42)
来源：http://fku.ydjk.org.cn

PHP:  (string) 42; strval(42)
来源：http://lhx.jyoumei.cn

JS:   String(42); (42).toString()
来源：http://xng.nanxuanxn.top

TS:   String(42)
来源：http://khq.yueranfly.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://jnc.shanyushiyangkeji.top

Go:   strconv.Itoa(42)
来源：http://ldq.zhijiandao.cn

Ruby: 42.to_s
来源：http://hnx.gzhubu.top

C#:   42.ToString()
来源：http://kob.hammf.cn

[A08] 取整与四舍五入
来源：http://yqc.shanyushiyangtech.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://bkv.hnqzz.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://kwc.cucudq.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://zad.andypj.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wuc.sufxvd.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://byl.yj20258.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://xrp.ydzc1.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://huo.sysykeji.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://llc.yanxiufei.cn

[A09] 绝对值与最大最小值
来源：http://fpf.vqdsnc.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://zey.zhaomingkeji.xyz

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hha.hfpthk.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://lmp.wangdashe.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://xps.dashuyun.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://rkv.ctjpmb.com

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://ejk.hammf.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ejl.guannengcc.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://ufo.0kj1m.cn

[A10] 生成随机数
来源：http://uhn.ydjk.org.cn

Py:   import random; random.randint(1, 100)
来源：http://lha.chenjidiqi.icu

PHP:  random_int(1, 100);
来源：http://fni.shangyingyoupin.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://swp.xziqi.cn

TS:   Math.floor(Math.random() * 100) + 1
来源：http://esw.c1oappe.top

Java: new Random().nextInt(100) + 1
来源：http://zgx.ehwqpu.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://eod.sjlbkw.cn

Ruby: rand(1..100)
来源：http://hri.0kj1m.cn

C#:   new Random().Next(1, 101)
来源：http://rjx.jianghu66.top

[A11] 条件表达式（三元）
来源：http://jdj.yj20258888.top

Py:   "yes" if x > 0 else "no"
来源：http://yge.sweek.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://afl.svipenyu.cn


<!-- 参考信息 -->