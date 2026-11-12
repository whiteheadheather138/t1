代发 wailian999

[U77] PHP：模板渲染
来源：http://aiu.xziqi.cn

composer require twig/twig
来源：http://fpw.zhijiandao.cn

[U78] PHP：单元测试
来源：http://qrw.jyoumei.cn

composer require --dev phpunit/phpunit
来源：http://tdy.shangyingyoupin.top

[U79] PHP：静态分析
来源：http://akz.0kj1m.cn

composer require --dev phpstan/phpstan
来源：http://pwg.jinghuilouyu.cn

[U80] PHP：代码规范修复
来源：http://gbw.aibaodan.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mim.hongshengwenyu.top

[U81] JS：初始化项目
来源：http://sdu.yj202588.top

npm init -y;  npm i express
来源：http://qje.guowangkeji.top

[U82] JS：package.json 脚本
来源：http://out.fengsongda.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jbj.nanxinkj.top

[U83] JS：ES Module 导入导出
来源：http://emy.zhongyouzk.top

export const a = 1;  import { a } from "./m.js";
来源：http://csq.svipenyu.cn

[U84] JS：CommonJS 写法
来源：http://ruq.ctjpmb.com

module.exports = { a };  const { a } = require("./m");
来源：http://ehz.yj20258888.top

[U85] JS：可选链
来源：http://ggz.fengsongda.top

a?.b?.c
来源：http://few.nwbrower.top

[U86] JS：空值合并
来源：http://drh.hnqzz.top

a ?? b
来源：http://tyh.yueranfly.top

[U87] JS：解构默认值
来源：http://qur.0kj1m.cn

const { a = 1, b = 2 } = obj;
来源：http://ldg.yangfankeji.com

[U88] JS：对象展开合并
来源：http://pxs.cdnleiting.top

{ ...a, ...b }
来源：http://isd.zhiwuduotai.top

[U89] JS：数组去重
来源：http://ooq.zhixingplan.top

[...new Set(arr)]
来源：http://gxd.hysaishi.cn

[U90] JS：数字数组排序
来源：http://xar.jinqigfzy.top

[...arr].sort((a, b) => a - b)
来源：http://nsb.shangyingyoupin.top

[U91] JS：对象键值遍历
来源：http://cay.shzxlz.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ifx.hfpthk.cn

[U92] JS：深拷贝
来源：http://llp.pengpengdd.cyou

structuredClone(obj)
来源：http://mvm.fehbvm.com

[U93] JS：模板字符串
来源：http://uwn.hywenlv.cn

`共 ${n} 条`
来源：http://gle.yonumen.top

[U94] JS：箭头函数
来源：http://zcs.daria6918.cn

const double = x => x * 2;
来源：http://eip.xuetiantiany.cn

[U95] JS：Promise 包装
来源：http://yfi.ywan-chungtsiang.top

new Promise((resolve, reject) => {})
来源：http://ycj.svipenyu.cn

[U96] JS：async/await 与异常
来源：http://qqj.yangfankeji.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://asn.jinghuilouyu.cn

[U97] JS：并发请求
来源：http://lpb.chenzaomai.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://ito.zhoulong.xyz

[U98] JS：fetch 带 JSON
来源：http://wir.mhx1999.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://awq.cashguo.top

[U99] JS：事件监听
来源：http://djm.shzxlz.cn

el.addEventListener("click", e => {})
来源：http://ajp.uphjek.com

[U100] JS：DOM 查询
来源：http://aqw.shuidangran.top

document.querySelector(".item")
来源：http://ani.daxiang520.top

[U101] JS：classList 操作
来源：http://phv.zhijiandao.cn

el.classList.toggle("active")
来源：http://ebi.zycfv.cn

[U102] JS：本地存储
来源：http://xvo.cashguo.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://aor.aizwys.cn

[U103] JS：定时器
来源：http://rfz.cheryme.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://qfd.wangshuangyany.cn

[U104] JS：防抖
来源：http://hjw.zhixingplan.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oxr.yueranfly.top

[U105] JS：节流
来源：http://lxb.zdqjudy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xto.hongshengwenyu.top

[U106] JS：日期格式化
来源：http://wve.316326.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://ien.fzhhl.top

[U107] JS：数字千分位
来源：http://pgq.redwolf501.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zlx.gaohongyu789.top

[U108] JS：随机整数
来源：http://ier.yuxming.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://cvw.pycfn.com

[U109] JS：数组分组
来源：http://knq.sysykeji.top

Object.groupBy(arr, x => x.type)
来源：http://wbn.shangyingyoupin.top

[U110] JS：数组分块
来源：http://czt.zdbjq.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://vkv.smart0.xyz

[U111] JS：对象转 Map
来源：http://pap.hnqzz.top

new Map(Object.entries(obj))
来源：http://ykk.tianlin.xyz

[U112] JS：字符串补位
来源：http://yqs.ydzc1.top

"7".padStart(3, "0")
来源：http://scs.haohaochexian.top

[U113] JS：正则替换全部
来源：http://mdn.xuanzx.com

s.replaceAll("a", "b")
来源：http://hxu.zhoulong.xyz

[U114] JS：JSON 深比较
来源：http://yjx.cucudq.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://znq.dianchejie.cn

[U115] JS：生成 UUID
来源：http://fwv.zycfv.cn

crypto.randomUUID()
来源：http://kwm.guowangkeji.top

[U116] JS：类型检查（JSDoc）
来源：http://nja.yueranfly.top

/** @param {string} name */ function f(name) {}
来源：http://gxu.smart0.xyz

[U117] JS：单元测试
来源：http://ejn.aizwys.cn

npm i -D vitest;  npx vitest
来源：http://drj.guowangkeji.top

[U118] JS：开发服务器
来源：http://lsa.hnqzz.top

npm i -D vite;  npx vite
来源：http://gkw.xziqi.cn

[U119] JS：生产构建
来源：http://xkm.aibaodan.cn

npx vite build
来源：http://olz.cheryme.top

[U120] JS：读取环境变量（Vite）
来源：http://emz.pengpengdd.cyou

import.meta.env.VITE_API_URL
来源：http://zrn.sweek.top

================================================================================
来源：http://ofv.hfpthk.cn

统计汇总
来源：http://ruh.fanxiaobao.xyz

================================================================================
来源：http://koe.nwbrower.top

按语言统计（条）：
来源：http://xcu.ybcxt.top

Python ......... 252
来源：http://cls.andypj.xyz

PHP ............ 252
来源：http://zfv.feifeiyinyue.top

JavaScript ..... 252
来源：http://chy.bbcook.cn

TypeScript ..... 212
来源：http://yoo.dianchejie.cn

Java ........... 212
来源：http://ofh.ivvv.top

Go ............. 212
来源：http://xwk.vehdjk.com

Ruby ........... 212
来源：http://jcg.yuanzhike.top

C# ............. 212
来源：http://wgs.shangyingyoupin.top

C .............. 30
来源：http://mut.ywan-chungtsiang.top

C++ ............ 30
来源：http://tpf.meibo888.top

SQL ............ 90
来源：http://ysc.jyoumei.cn

Bash ........... 80
来源：http://ida.hesvh.cn

Kotlin ......... 15
来源：http://sle.zhixingplan.top

Swift .......... 15
来源：http://mls.zhongyouzk.top

Lua ............ 10
来源：http://ouz.xuanzx.com

Perl ........... 10
来源：http://uik.shzxlz.cn

Scala .......... 10
来源：http://wkr.gaohongyu789.top

------------------------------------
来源：http://zru.chenzaomai.com

合计 ........... 2106 条
来源：http://owd.cqqwz.cn

按章节统计：
来源：http://org.zhiwuduotai.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://rqh.bjfxy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mqk.jyoumei.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://uau.yj20258.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://gbx.tarul.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://lft.sjlbkw.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tgr.hfpthk.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wsa.hammf.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://xih.xingfuxueyuan.xyz

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ybi.316326.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://yxu.jlsjyb.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://xhk.yuxming.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://lxs.birdmap.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://cxz.zhengqikj.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wus.xingfuxueyuan.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://nzx.zhongyouzk.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mrb.yueranfly.top

Q SQL 专题                              90
来源：http://gdg.zhijiandao.cn

R Bash 专题                             80
来源：http://kjq.vehdjk.com

S C / C++ 专题                          60
来源：http://mzk.xinyue.icu

T 其他语言补充                          60
来源：http://gdh.xingfuxueyuan.xyz

U 高频实用片段                         120
来源：http://ksa.hysaishi.cn

------------------------------------
来源：http://opx.hysaishi.cn

合计                                  2106 条
来源：http://xae.zhaomingkeji.xyz

--------------------------------------------------------------------------------
来源：http://ayn.andypj.xyz

使用提醒
来源：http://vhq.hcnkem.com

--------------------------------------------------------------------------------
来源：http://lks.gzhubu.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://glu.daria6918.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://djw.yanxiufei.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://uae.fehbvm.com

在旧版本上使用前请先确认语法支持情况。
来源：http://qys.iojbl.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://hrc.fzhhl.top

—— 文件结束 ——
来源：http://uuv.shuidangran.top

================================================================================
来源：http://fec.epnwcf.com

程序语言常见例子速查手册（2024 版）
来源：http://ldf.jqgufenzy.top

Common Programming Examples Cheat Book
来源：http://xtj.fktsv.cn

================================================================================
来源：http://mxw.fehbvm.com

【收录内容】
来源：http://kus.chenjidiqi.icu

覆盖 12 种语言 / 语法与常见 API：
来源：http://gpj.jqgufenzy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://phq.jinqigufen.top

SQL · Bash · C · C++
来源：http://wxu.quarkkingdee.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://udc.ydjk.org.cn

【使用说明】
来源：http://yid.tianlin.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://nwj.vehdjk.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://rtj.jqgufenzy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://pcd.bbcook.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://hlz.xylfe.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://wub.guowangkeji.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://yhl.jinyuanbaomall.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bwk.nanxuanxn.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://nzs.yonumen.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://hup.pycfn.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vwu.hnqzz.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://oqj.zhongyouzk.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zvh.tanke756.top

【文件统计】
来源：http://njq.zdqjudy.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://jko.nanxuanxn.top

--------------------------------------------------------------------------------
来源：http://tpy.sjlbkw.cn

目  录
来源：http://uaw.redwolf501.top

--------------------------------------------------------------------------------
来源：http://uvi.cheryme.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://ims.sjlbkw.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://eyi.cheryme.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://kqb.pycfn.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xuy.xziqi.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nzm.tian-w.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://eix.sjlbkw.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://jul.jinqigfzy.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://das.jqgufenzy.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://slx.pengpengdd.cyou

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://bjk.9152youxi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://igh.shanyushiyangkeji.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://tks.sufxvd.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ydt.cdnleiting.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ajk.birdmap.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://pvb.zhengqikj.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://sgs.yj20258888.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kzi.cashguo.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://cjy.yangfankeji.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://nmj.ywan-chungtsiang.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://stu.epnwcf.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://kby.chenjidiqi.icu

================================================================================
来源：http://jal.sjlbkw.cn

A. 基础语法与类型
来源：http://fsc.yj20258888.top

================================================================================
来源：http://oer.gogol.net.cn

[A01] Hello World
来源：http://rpf.zhoulong.xyz

Py:   print("Hello, World!")
来源：http://uzu.shzxlz.cn

PHP:  echo "Hello, World!";
来源：http://spt.zhoulong.xyz

JS:   console.log("Hello, World!");
来源：http://nxy.316326.xyz

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://cfi.ehwqpu.com

Java: System.out.println("Hello, World!");
来源：http://xtz.zhaomingkeji.xyz

Go:   fmt.Println("Hello, World!")
来源：http://ybm.yongpay.top

Ruby: puts "Hello, World!"
来源：http://qcp.xingfuxueyuan.xyz

C#:   Console.WriteLine("Hello, World!");
来源：http://mmj.yueranfly.top

[A02] 变量声明与赋值
来源：http://cgt.dashuyun.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://sjl.havefunace.top

PHP:  $name = "Alex"; $age = 20;
来源：http://wxu.zhiwuduotai.top

JS:   let name = "Alex"; const age = 20;
来源：http://hcn.wangshuangyany.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://qsl.jyoumei.cn

Java: String name = "Alex"; int age = 20;
来源：http://onv.bbcook.cn

Go:   name := "Alex"; age := 20
来源：http://nle.yueranfly.top

Ruby: name = "Alex"; age = 20
来源：http://grg.yangfankeji.com

C#:   string name = "Alex"; int age = 20;
来源：http://ely.tian-w.cn

[A03] 常量定义
来源：http://shk.sufxvd.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mww.hammf.cn

PHP:  const PI = 3.14159;
来源：http://lee.hnxiangtu.top

JS:   const PI = 3.14159;
来源：http://vgh.quarkkingdee.top

TS:   const PI: number = 3.14159;
来源：http://lhu.zhoulong.xyz

Java: static final double PI = 3.14159;
来源：http://njv.hongshengwenyu.top

Go:   const PI = 3.14159
来源：http://imy.yuxming.cn

Ruby: PI = 3.14159
来源：http://ggy.ydzc1.top

C#:   const double PI = 3.14159;
来源：http://uxz.zhaomingkeji.xyz

[A04] 判断变量类型
来源：http://gqs.zhaomingkeji.xyz

Py:   type(x).__name__; isinstance(x, int)
来源：http://scy.pengpengdd.cyou

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://oxw.316326.xyz

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://kps.cucudq.cn

TS:   typeof x; x instanceof Date
来源：http://ocg.fzhhl.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://nid.ppjwa.cn

Go:   reflect.TypeOf(x).Name()
来源：http://wzf.jinqigufen.top

Ruby: x.class; x.is_a?(Integer)
来源：http://hxd.gotoacloud.top

C#:   x.GetType().Name; x is int
来源：http://dng.gotoacloud.top

[A05] 整数除法与取模
来源：http://lgy.xingfuxueyuan.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ado.fzhhl.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://gmq.cdnleiting.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://djy.snrcjt.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://pkw.hnqzz.top

Java: 7 / 2; 7 % 2
来源：http://iso.ctjpmb.com

Go:   7 / 2; 7 % 2
来源：http://fow.wangdashe.top

Ruby: 7 / 2; 7 % 2
来源：http://hbp.hammf.cn

C#:   7 / 2; 7 % 2
来源：http://gof.chenjidiqi.icu

[A06] 字符串转数字
来源：http://znh.zhoulong.xyz

Py:   int("42"); float("3.14")
来源：http://qdg.cheryme.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://ihb.meibo888.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tpp.havefunace.top

TS:   parseInt("42", 10); Number("42")
来源：http://xbq.nanxinkj.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://arb.hnqzz.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://sqc.ydzc1.top

Ruby: "42".to_i; "3.14".to_f
来源：http://cnf.yanxiufei.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://uhw.xingfuxueyuan.xyz

[A07] 数字转字符串
来源：http://ybs.gaohongyu789.top

Py:   str(42)
来源：http://ydi.zdqjudy.top

PHP:  (string) 42; strval(42)
来源：http://elt.sufxvd.cn

JS:   String(42); (42).toString()
来源：http://sjc.xinyue.icu

TS:   String(42)
来源：http://opp.xingfuxueyuan.xyz

Java: String.valueOf(42); Integer.toString(42)
来源：http://wzh.shanyushiyangtech.top

Go:   strconv.Itoa(42)
来源：http://jdn.xuetiantiany.cn

Ruby: 42.to_s
来源：http://qqe.jianghu66.top

C#:   42.ToString()
来源：http://cgx.xylfe.cn

[A08] 取整与四舍五入
来源：http://kfh.yfazqb.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://klw.316326.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xem.yfazqb.com

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xwa.hcnkem.com

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://tjm.cheryme.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://fgx.fzhhl.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ydn.redwolf501.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://flk.zhongyouzk.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://bpn.pycfn.com

[A09] 绝对值与最大最小值
来源：http://yho.hnqzz.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://ltz.guowangkeji.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://ugx.aizwys.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://jcs.cucudq.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://sms.ybcxt.top

Java: Math.abs(-5); Math.max(1, 2)
来源：http://uwo.yj202588.top

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://fjl.kuanghao11.cn

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://ibg.bbcook.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://irz.xinyue.icu

[A10] 生成随机数
来源：http://ulh.jlsjyb.cn

Py:   import random; random.randint(1, 100)
来源：http://sqe.fehbvm.com

PHP:  random_int(1, 100);
来源：http://lhn.yueranfly.top

JS:   Math.floor(Math.random() * 100) + 1
来源：http://vhb.daxiang520.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://aza.bjfxy.top

Java: new Random().nextInt(100) + 1
来源：http://swj.cucudq.cn

Go:   rand.Intn(100) + 1               // math/rand
来源：http://equ.sjlbkw.cn

Ruby: rand(1..100)
来源：http://mxq.sxryk.cn

C#:   new Random().Next(1, 101)
来源：http://ovu.hammf.cn

[A11] 条件表达式（三元）
来源：http://hms.chenlongwang.top

Py:   "yes" if x > 0 else "no"
来源：http://tvq.pengpengdd.cyou

PHP:  $x > 0 ? "yes" : "no"
来源：http://ipf.yfazqb.com

JS:   x > 0 ? "yes" : "no"
来源：http://ozv.316326.xyz

TS:   x > 0 ? "yes" : "no"
来源：http://qgp.xuetiantiany.cn

Java: x > 0 ? "yes" : "no"
来源：http://wpy.redwolf501.top

Go:   // 无三元运算符，需用 if 语句
来源：http://mpx.haohaochexian.top

Ruby: x > 0 ? "yes" : "no"
来源：http://ucu.quarkkingdee.top

C#:   x > 0 ? "yes" : "no"
来源：http://zug.wangshuangyany.cn

[A12] 字符串插值 / 格式化
来源：http://ent.chenjidiqi.icu

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ruv.gaohongyu789.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://abg.meibo888.top

JS:   `Hello, ${name}!`
来源：http://ydx.jqgufenzy.top

TS:   `Hello, ${name}!`
来源：http://xzu.yangfankeji.com

Java: "Hello, %s!".formatted(name)
来源：http://usn.fzhhl.top


<!-- 参考信息 -->