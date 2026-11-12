代发 wailian999

[U63] PHP：文件读写
来源：http://lpo.jiagoushi.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://iww.zhengqikj.top

[U64] PHP：目录遍历
来源：http://rmf.andypj.xyz

glob("dir/*.php");  scandir("dir");
来源：http://luf.cashguo.top

[U65] PHP：会话
来源：http://dkk.jqgufenzy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://qyy.pycfn.com

[U66] PHP：设置 Cookie
来源：http://qes.ydzc1.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://awp.sjlbkw.cn

[U67] PHP：处理文件上传
来源：http://wnb.ivvv.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mgw.dianchejie.cn

[U68] PHP：PDO 连接
来源：http://bnj.gotoacloud.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ebn.yj20258.top

[U69] PHP：PDO 预处理
来源：http://eyc.jinghuilouyu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ysk.pycfn.com

[U70] PHP：PDO 事务
来源：http://miq.yonumen.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gdz.yanxiufei.cn

[U71] PHP：抛出异常
来源：http://eqx.jinqigufen.top

throw new RuntimeException("失败", 500);
来源：http://oti.birdmap.top

[U72] PHP：写错误日志
来源：http://iva.ppjwa.cn

error_log("失败: " . $e->getMessage());
来源：http://kfo.redwolf501.top

[U73] PHP：读取 ini 配置
来源：http://zrm.guannengcc.top

parse_ini_file("config.ini", true)
来源：http://rzj.shangyingyoupin.top

[U74] PHP：读取环境变量
来源：http://pjx.hesvh.cn

getenv("APP_ENV") ?: "production"
来源：http://xvs.cheryme.top

[U75] PHP：依赖注入
来源：http://phi.snrcjt.cn

composer require psr/container
来源：http://ztg.ppjwa.cn

[U76] PHP：简单路由
来源：http://jyh.pycfn.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://idz.nanxuanxn.top

[U77] PHP：模板渲染
来源：http://ogp.cucudq.cn

composer require twig/twig
来源：http://qle.yuxming.cn

[U78] PHP：单元测试
来源：http://lfj.tanke756.top

composer require --dev phpunit/phpunit
来源：http://kzw.ehwqpu.com

[U79] PHP：静态分析
来源：http://kvu.yongpay.top

composer require --dev phpstan/phpstan
来源：http://kdg.sxryk.cn

[U80] PHP：代码规范修复
来源：http://seb.cucudq.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://ayn.zycfv.cn

[U81] JS：初始化项目
来源：http://peb.uphjek.com

npm init -y;  npm i express
来源：http://ytr.jqgfzy.top

[U82] JS：package.json 脚本
来源：http://gyd.andypj.xyz

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://rxf.yj20258.top

[U83] JS：ES Module 导入导出
来源：http://zth.hcnkem.com

export const a = 1;  import { a } from "./m.js";
来源：http://xbd.gaohongyu789.top

[U84] JS：CommonJS 写法
来源：http://lfi.smart0.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://pds.zhixingplan.top

[U85] JS：可选链
来源：http://lyo.fktsv.cn

a?.b?.c
来源：http://uju.chenlongwang.top

[U86] JS：空值合并
来源：http://noa.shuidangran.top

a ?? b
来源：http://lrq.mhx1999.top

[U87] JS：解构默认值
来源：http://bog.jqgfzy.top

const { a = 1, b = 2 } = obj;
来源：http://ptu.yanxiufei.cn

[U88] JS：对象展开合并
来源：http://kek.cucudq.cn

{ ...a, ...b }
来源：http://hjk.tanke756.top

[U89] JS：数组去重
来源：http://ttk.gaohongyu789.top

[...new Set(arr)]
来源：http://nyh.yuanzhike.top

[U90] JS：数字数组排序
来源：http://sio.zycfv.cn

[...arr].sort((a, b) => a - b)
来源：http://dfa.fehbvm.com

[U91] JS：对象键值遍历
来源：http://mte.cashguo.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wwf.snrcjt.cn

[U92] JS：深拷贝
来源：http://mmu.snrcjt.cn

structuredClone(obj)
来源：http://hrm.shanyushiyangkeji.top

[U93] JS：模板字符串
来源：http://ylo.nanxuanxn.top

`共 ${n} 条`
来源：http://nwm.xuetiantiany.cn

[U94] JS：箭头函数
来源：http://oig.zdbjq.cn

const double = x => x * 2;
来源：http://jvy.zhengqikj.top

[U95] JS：Promise 包装
来源：http://cph.shangyingyoupin.top

new Promise((resolve, reject) => {})
来源：http://cph.jianghu66.top

[U96] JS：async/await 与异常
来源：http://ejz.jinghuilouyu.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://tao.ywan-chungtsiang.top

[U97] JS：并发请求
来源：http://pdb.cashguo.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://eke.fzhhl.top

[U98] JS：fetch 带 JSON
来源：http://njk.zdqjudy.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://fal.hysaishi.cn

[U99] JS：事件监听
来源：http://onv.yvedp.cn

el.addEventListener("click", e => {})
来源：http://uqa.cucudq.cn

[U100] JS：DOM 查询
来源：http://wev.xingfuxueyuan.xyz

document.querySelector(".item")
来源：http://vdr.uphjek.com

[U101] JS：classList 操作
来源：http://oij.sjlbkw.cn

el.classList.toggle("active")
来源：http://pvx.dianchejie.cn

[U102] JS：本地存储
来源：http://dxe.daxiang520.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://oeb.shanyushiyangtech.top

[U103] JS：定时器
来源：http://tvr.fengsongda.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ytz.feifeiyinyue.top

[U104] JS：防抖
来源：http://hdb.sxryk.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lor.ywan-chungtsiang.top

[U105] JS：节流
来源：http://fbs.jinqigufen.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://boe.sjlbkw.cn

[U106] JS：日期格式化
来源：http://fzx.jinyuanbaomall.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://fsc.tanke756.top

[U107] JS：数字千分位
来源：http://pev.jinyuanbaomall.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://gah.316326.xyz

[U108] JS：随机整数
来源：http://gxz.bjfxy.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://myj.hammf.cn

[U109] JS：数组分组
来源：http://jkg.aibaodan.cn

Object.groupBy(arr, x => x.type)
来源：http://dhk.jlsjyb.cn

[U110] JS：数组分块
来源：http://hhj.yanxiufei.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://uyo.ppjwa.cn

[U111] JS：对象转 Map
来源：http://frj.jqgufenzy.top

new Map(Object.entries(obj))
来源：http://byd.bbcook.cn

[U112] JS：字符串补位
来源：http://eap.shangyingyoupin.top

"7".padStart(3, "0")
来源：http://gve.shangyingyoupin.top

[U113] JS：正则替换全部
来源：http://ufv.yfazqb.com

s.replaceAll("a", "b")
来源：http://xut.hywenlv.cn

[U114] JS：JSON 深比较
来源：http://dfa.xuetiantiany.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://ohv.zhoulong.xyz

[U115] JS：生成 UUID
来源：http://qng.cashguo.top

crypto.randomUUID()
来源：http://ypa.wangshuangyany.cn

[U116] JS：类型检查（JSDoc）
来源：http://ysd.xingfuxueyuan.xyz

/** @param {string} name */ function f(name) {}
来源：http://gfc.ybcxt.top

[U117] JS：单元测试
来源：http://qcf.sxryk.cn

npm i -D vitest;  npx vitest
来源：http://pyv.shanyushiyangtech.top

[U118] JS：开发服务器
来源：http://frs.sxryk.cn

npm i -D vite;  npx vite
来源：http://nwp.xziqi.cn

[U119] JS：生产构建
来源：http://xla.hysaishi.cn

npx vite build
来源：http://wgp.cucudq.cn

[U120] JS：读取环境变量（Vite）
来源：http://mou.tanke756.top

import.meta.env.VITE_API_URL
来源：http://bdk.zhiwuduotai.top

================================================================================
来源：http://xtq.jyoumei.cn

统计汇总
来源：http://agb.feifeiyinyue.top

================================================================================
来源：http://obo.fktsv.cn

按语言统计（条）：
来源：http://uis.yj202588.top

Python ......... 252
来源：http://idm.dianchejie.cn

PHP ............ 252
来源：http://mms.gotoacloud.top

JavaScript ..... 252
来源：http://cms.yuxming.cn

TypeScript ..... 212
来源：http://erj.chenjidiqi.icu

Java ........... 212
来源：http://wpa.iojbl.cn

Go ............. 212
来源：http://onb.haohaochexian.top

Ruby ........... 212
来源：http://cdf.meibo888.top

C# ............. 212
来源：http://xhd.cdnleiting.top

C .............. 30
来源：http://tcm.9152youxi.cn

C++ ............ 30
来源：http://tma.c1oappe.top

SQL ............ 90
来源：http://qju.jlsjyb.cn

Bash ........... 80
来源：http://uye.wangshuangyany.cn

Kotlin ......... 15
来源：http://bnt.fktsv.cn

Swift .......... 15
来源：http://kyi.guowangkeji.top

Lua ............ 10
来源：http://hlz.sjlbkw.cn

Perl ........... 10
来源：http://qzm.fanxiaobao.xyz

Scala .......... 10
来源：http://vep.pycfn.com

------------------------------------
来源：http://rce.hammf.cn

合计 ........... 2106 条
来源：http://fdh.guannengcc.top

按章节统计：
来源：http://ijs.c1oappe.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ayc.zdqjudy.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://uxb.yueranfly.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://edu.ydzc1.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://klb.xuanzx.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://ozk.daxiang520.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://qun.mhx1999.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://brp.xinyue.icu

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://puw.jinghuilouyu.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://cza.birdmap.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://nki.havefunace.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://dsh.feifeiyinyue.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nvw.cucudq.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://okt.shanyushiyangtech.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://acq.hnxiangtu.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://qyo.shanyushiyangtech.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mck.meibo888.top

Q SQL 专题                              90
来源：http://umc.gogol.net.cn

R Bash 专题                             80
来源：http://yea.hfpthk.cn

S C / C++ 专题                          60
来源：http://avq.redwolf501.top

T 其他语言补充                          60
来源：http://pye.9152youxi.cn

U 高频实用片段                         120
来源：http://fhg.guowangkeji.top

------------------------------------
来源：http://poh.andypj.xyz

合计                                  2106 条
来源：http://hzx.tarul.cn

--------------------------------------------------------------------------------
来源：http://tlr.zhoulong.xyz

使用提醒
来源：http://hrw.jinyuanbaomall.cn

--------------------------------------------------------------------------------
来源：http://cwg.zdqjudy.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://xyn.jinghuilouyu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bqf.shanyushiyangtech.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://joj.yueranfly.top

在旧版本上使用前请先确认语法支持情况。
来源：http://tou.nwbrower.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://obw.cashguo.top

—— 文件结束 ——
来源：http://pxa.zhongyouzk.top

================================================================================
来源：http://njp.andypj.xyz

程序语言常见例子速查手册（2024 版）
来源：http://znz.fanxiaobao.xyz

Common Programming Examples Cheat Book
来源：http://uvp.xylfe.cn

================================================================================
来源：http://gvk.yanxiufei.cn

【收录内容】
来源：http://gcd.zdqjudy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://udw.fengsongda.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://nal.fzhhl.top

SQL · Bash · C · C++
来源：http://bte.cucudq.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mbp.yj20258.top

【使用说明】
来源：http://uco.jinqigufen.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mfd.wangdashe.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://bkq.vqdsnc.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://kra.shzxlz.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ahb.yj20258.top

Bash:  Shell         C:     C             C++:   C++
来源：http://kvc.quarkkingdee.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://dxv.tianlin.xyz

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wqc.gogol.net.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://xop.birdmap.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://zbb.yuxming.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://pcx.xuetiantiany.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://gdr.yonumen.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mes.hywenlv.cn

【文件统计】
来源：http://jpd.yvedp.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://yeq.jyoumei.cn

--------------------------------------------------------------------------------
来源：http://uet.epnwcf.com

目  录
来源：http://lip.xinyue.icu

--------------------------------------------------------------------------------
来源：http://sum.daria6918.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://lqv.fehbvm.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://itq.cucudq.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://gfl.ehwqpu.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://peh.ydzc1.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://vvp.birdmap.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://zse.ybcxt.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ajs.zycfv.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://asx.c1oappe.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://xwi.dianchejie.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://aze.smart0.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://une.ppjwa.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hnn.9152youxi.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ucl.bbcook.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://pfv.0kj1m.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ubv.gotoacloud.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://bld.hysaishi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://svf.wangdashe.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://zhd.yangfankeji.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://erw.dianchejie.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qhn.xylfe.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wcq.jinqigfzy.top

================================================================================
来源：http://yql.birdmap.top

A. 基础语法与类型
来源：http://xzc.zhiwuduotai.top

================================================================================
来源：http://vte.fzhhl.top

[A01] Hello World
来源：http://zlz.zdbjq.cn

Py:   print("Hello, World!")
来源：http://tnn.zhaomingkeji.xyz

PHP:  echo "Hello, World!";
来源：http://ogs.wangdashe.top

JS:   console.log("Hello, World!");
来源：http://uqo.ctjpmb.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://zye.zhiwuduotai.top

Java: System.out.println("Hello, World!");
来源：http://hvi.jianghu66.top

Go:   fmt.Println("Hello, World!")
来源：http://rtz.yanxiufei.cn

Ruby: puts "Hello, World!"
来源：http://zfh.yfazqb.com

C#:   Console.WriteLine("Hello, World!");
来源：http://pzx.xinyue.icu

[A02] 变量声明与赋值
来源：http://xwl.316326.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://eql.hcnkem.com

PHP:  $name = "Alex"; $age = 20;
来源：http://vyd.guannengcc.top

JS:   let name = "Alex"; const age = 20;
来源：http://wti.guowangkeji.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://txo.jlsjyb.cn

Java: String name = "Alex"; int age = 20;
来源：http://bqd.chenlongwang.top

Go:   name := "Alex"; age := 20
来源：http://hln.xingfuxueyuan.xyz

Ruby: name = "Alex"; age = 20
来源：http://wlb.hnxiangtu.top

C#:   string name = "Alex"; int age = 20;
来源：http://wml.jinghuilouyu.cn

[A03] 常量定义
来源：http://eiz.guannengcc.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ewn.daria6918.cn

PHP:  const PI = 3.14159;
来源：http://cxr.svipenyu.cn

JS:   const PI = 3.14159;
来源：http://ycb.ydjk.org.cn

TS:   const PI: number = 3.14159;
来源：http://qmu.chenzaomai.com

Java: static final double PI = 3.14159;
来源：http://pum.xuanzx.com

Go:   const PI = 3.14159
来源：http://cyi.meibo888.top

Ruby: PI = 3.14159
来源：http://pcz.havefunace.top

C#:   const double PI = 3.14159;
来源：http://vmu.feifeiyinyue.top

[A04] 判断变量类型
来源：http://udm.yangfankeji.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://hrj.feifeiyinyue.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ivq.aibaodan.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://epw.hnxiangtu.top

TS:   typeof x; x instanceof Date
来源：http://oqa.jqgfzy.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://uqa.zhongyouzk.top

Go:   reflect.TypeOf(x).Name()
来源：http://svw.jqgfzy.top

Ruby: x.class; x.is_a?(Integer)
来源：http://cxt.cheryme.top

C#:   x.GetType().Name; x is int
来源：http://jcg.yongpay.top

[A05] 整数除法与取模
来源：http://glt.shanyushiyangkeji.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://uoo.cashguo.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://hub.ivvv.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ime.kuanghao11.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xbi.shangyingyoupin.top

Java: 7 / 2; 7 % 2
来源：http://knf.fktsv.cn

Go:   7 / 2; 7 % 2
来源：http://zkf.cqqwz.cn

Ruby: 7 / 2; 7 % 2
来源：http://qyk.jinyuanbaomall.cn

C#:   7 / 2; 7 % 2
来源：http://zml.jinghuilouyu.cn

[A06] 字符串转数字
来源：http://bql.wangdashe.top

Py:   int("42"); float("3.14")
来源：http://dnv.meibo888.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lna.shzxlz.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://xqy.aibaodan.cn

TS:   parseInt("42", 10); Number("42")
来源：http://vlx.0kj1m.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://loa.gaohongyu789.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://lzi.nanxuanxn.top

Ruby: "42".to_i; "3.14".to_f
来源：http://myc.cashguo.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rvi.yueranfly.top

[A07] 数字转字符串
来源：http://aek.0kj1m.cn

Py:   str(42)
来源：http://sdi.cucudq.cn

PHP:  (string) 42; strval(42)
来源：http://nqt.quarkkingdee.top

JS:   String(42); (42).toString()
来源：http://kwm.chenzaomai.com

TS:   String(42)
来源：http://ljn.daria6918.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://jzc.yanxiufei.cn

Go:   strconv.Itoa(42)
来源：http://nwk.gaohongyu789.top

Ruby: 42.to_s
来源：http://sfe.hammf.cn

C#:   42.ToString()
来源：http://rsy.aibaodan.cn

[A08] 取整与四舍五入
来源：http://nua.jqgufenzy.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ebu.hfpthk.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://xgo.jqgufenzy.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://aqq.ppjwa.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://bzc.gaohongyu789.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://msu.zhijiandao.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://dkl.birdmap.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://adu.aizwys.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://cht.yanxiufei.cn

[A09] 绝对值与最大最小值
来源：http://avw.chenzaomai.com

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://pxu.ybcxt.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://tee.feifeiyinyue.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://vrc.hcnkem.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://lhg.yangfankeji.com


<!-- 参考信息 -->