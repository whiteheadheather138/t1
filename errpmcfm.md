代发 wailian999

[U63] PHP：文件读写
来源：http://ezh.feifeiyinyue.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ium.birdmap.top

[U64] PHP：目录遍历
来源：http://kkc.vehdjk.com

glob("dir/*.php");  scandir("dir");
来源：http://nme.0kj1m.cn

[U65] PHP：会话
来源：http://rcc.nwbrower.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ibi.pycfn.com

[U66] PHP：设置 Cookie
来源：http://kkl.hongshengwenyu.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://oyi.chenlongwang.top

[U67] PHP：处理文件上传
来源：http://tzj.bbcook.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jfz.xziqi.cn

[U68] PHP：PDO 连接
来源：http://fkx.fehbvm.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rlp.zhiwuduotai.top

[U69] PHP：PDO 预处理
来源：http://asr.cashguo.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://uui.ybcxt.top

[U70] PHP：PDO 事务
来源：http://rvg.iojbl.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://kcw.9152youxi.cn

[U71] PHP：抛出异常
来源：http://hea.ivvv.top

throw new RuntimeException("失败", 500);
来源：http://oib.quarkkingdee.top

[U72] PHP：写错误日志
来源：http://pla.uphjek.com

error_log("失败: " . $e->getMessage());
来源：http://uqy.sufxvd.cn

[U73] PHP：读取 ini 配置
来源：http://bxo.bbcook.cn

parse_ini_file("config.ini", true)
来源：http://hkb.fengsongda.top

[U74] PHP：读取环境变量
来源：http://isl.fzhhl.top

getenv("APP_ENV") ?: "production"
来源：http://ssi.yangfankeji.com

[U75] PHP：依赖注入
来源：http://ijf.jqgfzy.top

composer require psr/container
来源：http://cao.sweek.top

[U76] PHP：简单路由
来源：http://syj.redwolf501.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xnw.shzxlz.cn

[U77] PHP：模板渲染
来源：http://doy.nwbrower.top

composer require twig/twig
来源：http://tyh.xuetiantiany.cn

[U78] PHP：单元测试
来源：http://cjf.sweek.top

composer require --dev phpunit/phpunit
来源：http://pdo.vqdsnc.cn

[U79] PHP：静态分析
来源：http://eyr.ydjk.org.cn

composer require --dev phpstan/phpstan
来源：http://gtj.xuetiantiany.cn

[U80] PHP：代码规范修复
来源：http://fwa.cqqwz.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://slr.dashuyun.cn

[U81] JS：初始化项目
来源：http://mrs.yj202588.top

npm init -y;  npm i express
来源：http://rgp.wangdashe.top

[U82] JS：package.json 脚本
来源：http://ghd.cdnleiting.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://vdi.0kj1m.cn

[U83] JS：ES Module 导入导出
来源：http://dca.bjfxy.top

export const a = 1;  import { a } from "./m.js";
来源：http://epa.gaohongyu789.top

[U84] JS：CommonJS 写法
来源：http://dwe.aizwys.cn

module.exports = { a };  const { a } = require("./m");
来源：http://wny.jyoumei.cn

[U85] JS：可选链
来源：http://awv.sysykeji.top

a?.b?.c
来源：http://gtr.jinyuanbaomall.cn

[U86] JS：空值合并
来源：http://irh.tianlin.xyz

a ?? b
来源：http://ohq.xingfuxueyuan.xyz

[U87] JS：解构默认值
来源：http://din.zdqjudy.top

const { a = 1, b = 2 } = obj;
来源：http://trr.316326.xyz

[U88] JS：对象展开合并
来源：http://ufo.52xcode.cn

{ ...a, ...b }
来源：http://jxh.yuxming.cn

[U89] JS：数组去重
来源：http://bdw.ydjk.org.cn

[...new Set(arr)]
来源：http://okd.yanxiufei.cn

[U90] JS：数字数组排序
来源：http://wyf.wangdashe.top

[...arr].sort((a, b) => a - b)
来源：http://udi.c1oappe.top

[U91] JS：对象键值遍历
来源：http://brf.chenzaomai.com

Object.entries(obj).forEach(([k, v]) => {});
来源：http://msl.nanxinkj.top

[U92] JS：深拷贝
来源：http://tqf.shangyingyoupin.top

structuredClone(obj)
来源：http://boq.hnqzz.top

[U93] JS：模板字符串
来源：http://atf.zhongyouzk.top

`共 ${n} 条`
来源：http://etc.yj20258.top

[U94] JS：箭头函数
来源：http://lxk.kuanghao11.cn

const double = x => x * 2;
来源：http://umk.yonumen.top

[U95] JS：Promise 包装
来源：http://itf.shzxlz.cn

new Promise((resolve, reject) => {})
来源：http://blw.52xcode.cn

[U96] JS：async/await 与异常
来源：http://fdl.xinyue.icu

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://qmi.vehdjk.com

[U97] JS：并发请求
来源：http://jpa.wangshuangyany.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://tmw.dashuyun.cn

[U98] JS：fetch 带 JSON
来源：http://qjo.ybcxt.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://ngf.zhongyouzk.top

[U99] JS：事件监听
来源：http://vyn.yongpay.top

el.addEventListener("click", e => {})
来源：http://blb.yonumen.top

[U100] JS：DOM 查询
来源：http://kyj.hfpthk.cn

document.querySelector(".item")
来源：http://soo.andypj.xyz

[U101] JS：classList 操作
来源：http://pdm.birdmap.top

el.classList.toggle("active")
来源：http://jiu.daria6918.cn

[U102] JS：本地存储
来源：http://cmh.jlsjyb.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ycx.shanyushiyangtech.top

[U103] JS：定时器
来源：http://nyc.zhongyouzk.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://dfp.havefunace.top

[U104] JS：防抖
来源：http://ujq.feifeiyinyue.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zsh.snrcjt.cn

[U105] JS：节流
来源：http://dmj.zdbjq.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://pgf.guowangkeji.top

[U106] JS：日期格式化
来源：http://dsm.xziqi.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cpk.zdbjq.cn

[U107] JS：数字千分位
来源：http://xxl.jiagoushi.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://yru.meibo888.top

[U108] JS：随机整数
来源：http://cpc.ctjpmb.com

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bxe.hammf.cn

[U109] JS：数组分组
来源：http://nlc.cucudq.cn

Object.groupBy(arr, x => x.type)
来源：http://ufw.hnqzz.top

[U110] JS：数组分块
来源：http://gyc.chenjidiqi.icu

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://smr.sufxvd.cn

[U111] JS：对象转 Map
来源：http://hca.zhongyouzk.top

new Map(Object.entries(obj))
来源：http://gls.shangyingyoupin.top

[U112] JS：字符串补位
来源：http://mcs.ydzc1.top

"7".padStart(3, "0")
来源：http://zxg.jinqigufen.top

[U113] JS：正则替换全部
来源：http://uig.52xcode.cn

s.replaceAll("a", "b")
来源：http://xil.yj20258888.top

[U114] JS：JSON 深比较
来源：http://bpg.yj20258.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://bob.zhoulong.xyz

[U115] JS：生成 UUID
来源：http://cvm.xingfuxueyuan.xyz

crypto.randomUUID()
来源：http://vwd.xziqi.cn

[U116] JS：类型检查（JSDoc）
来源：http://wgd.sxryk.cn

/** @param {string} name */ function f(name) {}
来源：http://axv.zhaomingkeji.xyz

[U117] JS：单元测试
来源：http://aky.ydjk.org.cn

npm i -D vitest;  npx vitest
来源：http://mio.bjfxy.top

[U118] JS：开发服务器
来源：http://kvd.xingfuxueyuan.xyz

npm i -D vite;  npx vite
来源：http://kud.birdmap.top

[U119] JS：生产构建
来源：http://jxk.fktsv.cn

npx vite build
来源：http://otq.nwbrower.top

[U120] JS：读取环境变量（Vite）
来源：http://zdd.jinyuanbaomall.cn

import.meta.env.VITE_API_URL
来源：http://ibp.jyoumei.cn

================================================================================
来源：http://vgo.ehwqpu.com

统计汇总
来源：http://gro.shangyingyoupin.top

================================================================================
来源：http://jaf.ehwqpu.com

按语言统计（条）：
来源：http://khf.fktsv.cn

Python ......... 252
来源：http://nfq.jinghuilouyu.cn

PHP ............ 252
来源：http://vzj.hesvh.cn

JavaScript ..... 252
来源：http://ajp.guowangkeji.top

TypeScript ..... 212
来源：http://bbq.vehdjk.com

Java ........... 212
来源：http://bsu.gaohongyu789.top

Go ............. 212
来源：http://bgj.fanxiaobao.xyz

Ruby ........... 212
来源：http://pbs.zycfv.cn

C# ............. 212
来源：http://gdl.jinqigfzy.top

C .............. 30
来源：http://jpc.meibo888.top

C++ ............ 30
来源：http://sxh.chenjidiqi.icu

SQL ............ 90
来源：http://mno.dashuyun.cn

Bash ........... 80
来源：http://mlz.jianghu66.top

Kotlin ......... 15
来源：http://nuh.tianlin.xyz

Swift .......... 15
来源：http://xng.hcnkem.com

Lua ............ 10
来源：http://lhd.hammf.cn

Perl ........... 10
来源：http://trj.pengpengdd.cyou

Scala .......... 10
来源：http://tjh.chenzaomai.com

------------------------------------
来源：http://ajw.zhengqikj.top

合计 ........... 2106 条
来源：http://vlg.xingfuxueyuan.xyz

按章节统计：
来源：http://zrs.52xcode.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://vkq.ybcxt.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://imt.havefunace.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://aug.jinqigfzy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://pwk.chenjidiqi.icu

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://duv.tanke756.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hqu.hysaishi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://bkx.tarul.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://lsi.aizwys.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ljq.zhaomingkeji.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zts.redwolf501.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://adj.yongpay.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://dhj.redwolf501.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sob.fanxiaobao.xyz

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://amc.hysaishi.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://sne.zycfv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ebb.gogol.net.cn

Q SQL 专题                              90
来源：http://cnv.zdqjudy.top

R Bash 专题                             80
来源：http://kyf.ehwqpu.com

S C / C++ 专题                          60
来源：http://xwt.cdnleiting.top

T 其他语言补充                          60
来源：http://hum.xziqi.cn

U 高频实用片段                         120
来源：http://njl.feifeiyinyue.top

------------------------------------
来源：http://vnl.cucudq.cn

合计                                  2106 条
来源：http://ehs.guannengcc.top

--------------------------------------------------------------------------------
来源：http://mzp.hammf.cn

使用提醒
来源：http://hnz.hnxiangtu.top

--------------------------------------------------------------------------------
来源：http://urf.fanxiaobao.xyz

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zxr.svipenyu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://bbi.jiagoushi.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://kif.nwbrower.top

在旧版本上使用前请先确认语法支持情况。
来源：http://snl.jlsjyb.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ext.xingfuxueyuan.xyz

—— 文件结束 ——
来源：http://oyw.yueranfly.top

================================================================================
来源：http://vzt.dashuyun.cn

程序语言常见例子速查手册（2024 版）
来源：http://txe.shanyushiyangkeji.top

Common Programming Examples Cheat Book
来源：http://avc.fengsongda.top

================================================================================
来源：http://lqg.tian-w.cn

【收录内容】
来源：http://yps.cucudq.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://vmu.yonumen.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mam.yvedp.cn

SQL · Bash · C · C++
来源：http://vqy.vehdjk.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://xhf.tarul.cn

【使用说明】
来源：http://cra.jinyuanbaomall.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ipt.birdmap.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://yra.smart0.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hwb.andypj.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://qwh.aizwys.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://hls.nanxuanxn.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://tvv.jiagoushi.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://nkb.hesvh.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://why.smart0.xyz

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://sag.tarul.cn

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://obh.jyoumei.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bei.andypj.xyz

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://qrr.gogol.net.cn

【文件统计】
来源：http://fha.nanxuanxn.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wqs.zhijiandao.cn

--------------------------------------------------------------------------------
来源：http://ekl.cashguo.top

目  录
来源：http://qhn.andypj.xyz

--------------------------------------------------------------------------------
来源：http://kjl.jianghu66.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://tpm.jqgufenzy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://xfe.yonumen.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://chd.hongshengwenyu.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://yoy.sxryk.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://uuv.sweek.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ouj.tanke756.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://dng.gzhubu.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://lbs.52xcode.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://tuy.cashguo.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://gsb.chenjidiqi.icu

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://tgo.shuidangran.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://nww.jiagoushi.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://dko.gotoacloud.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://xpf.meibo888.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://yrn.chenjidiqi.icu

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://syj.xuetiantiany.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://ezt.gogol.net.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://zsu.chenzaomai.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://twf.xinyue.icu

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mej.0kj1m.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://tea.hnqzz.top

================================================================================
来源：http://yyn.fktsv.cn

A. 基础语法与类型
来源：http://cqg.hcnkem.com

================================================================================
来源：http://jpy.hesvh.cn

[A01] Hello World
来源：http://grv.hnqzz.top

Py:   print("Hello, World!")
来源：http://lxy.jianghu66.top

PHP:  echo "Hello, World!";
来源：http://czh.shangyingyoupin.top

JS:   console.log("Hello, World!");
来源：http://qob.cucudq.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://xvj.yj202588.top

Java: System.out.println("Hello, World!");
来源：http://zcz.wangshuangyany.cn

Go:   fmt.Println("Hello, World!")
来源：http://ysd.nwbrower.top

Ruby: puts "Hello, World!"
来源：http://vcp.yfazqb.com

C#:   Console.WriteLine("Hello, World!");
来源：http://hff.gaohongyu789.top

[A02] 变量声明与赋值
来源：http://dvu.havefunace.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://pyp.hnxiangtu.top

PHP:  $name = "Alex"; $age = 20;
来源：http://suo.zhoulong.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://uic.hnxiangtu.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ksn.sweek.top

Java: String name = "Alex"; int age = 20;
来源：http://dgt.shanyushiyangkeji.top

Go:   name := "Alex"; age := 20
来源：http://xcc.ehwqpu.com

Ruby: name = "Alex"; age = 20
来源：http://fjo.dashuyun.cn

C#:   string name = "Alex"; int age = 20;
来源：http://hqy.jinyuanbaomall.cn

[A03] 常量定义
来源：http://syy.tarul.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bpz.havefunace.top

PHP:  const PI = 3.14159;
来源：http://crf.zdbjq.cn

JS:   const PI = 3.14159;
来源：http://lcf.yj20258.top

TS:   const PI: number = 3.14159;
来源：http://qru.jqgfzy.top

Java: static final double PI = 3.14159;
来源：http://tla.hnxiangtu.top

Go:   const PI = 3.14159
来源：http://euf.nanxinkj.top

Ruby: PI = 3.14159
来源：http://qnv.hesvh.cn

C#:   const double PI = 3.14159;
来源：http://lun.mhx1999.top

[A04] 判断变量类型
来源：http://zxa.chenlongwang.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://glt.dianchejie.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://yfw.epnwcf.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://ldj.dashuyun.cn

TS:   typeof x; x instanceof Date
来源：http://tpa.sysykeji.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://tvs.dashuyun.cn

Go:   reflect.TypeOf(x).Name()
来源：http://grf.fktsv.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://ont.chenzaomai.com

C#:   x.GetType().Name; x is int
来源：http://sao.52xcode.cn

[A05] 整数除法与取模
来源：http://gin.ctjpmb.com

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pea.yj20258888.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://yiv.cqqwz.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://ngn.fehbvm.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://zgi.jlsjyb.cn

Java: 7 / 2; 7 % 2
来源：http://kxp.hcnkem.com

Go:   7 / 2; 7 % 2
来源：http://qfn.hnxiangtu.top

Ruby: 7 / 2; 7 % 2
来源：http://ojw.yj20258.top

C#:   7 / 2; 7 % 2
来源：http://fbp.shuidangran.top

[A06] 字符串转数字
来源：http://hiw.vehdjk.com

Py:   int("42"); float("3.14")
来源：http://oic.sweek.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blg.yanxiufei.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ifh.tianlin.xyz

TS:   parseInt("42", 10); Number("42")
来源：http://eml.iojbl.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://exv.vqdsnc.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://nnl.shuidangran.top

Ruby: "42".to_i; "3.14".to_f
来源：http://lkd.jyoumei.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://cgo.jinghuilouyu.cn

[A07] 数字转字符串
来源：http://abb.aibaodan.cn

Py:   str(42)
来源：http://hlw.yj202588.top

PHP:  (string) 42; strval(42)
来源：http://uha.jinqigufen.top

JS:   String(42); (42).toString()
来源：http://tkx.nwbrower.top

TS:   String(42)
来源：http://ndx.dashuyun.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://jus.zdbjq.cn

Go:   strconv.Itoa(42)
来源：http://gie.xuanzx.com

Ruby: 42.to_s
来源：http://hpz.ywan-chungtsiang.top

C#:   42.ToString()
来源：http://usn.fktsv.cn

[A08] 取整与四舍五入
来源：http://rap.0kj1m.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://sud.pycfn.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://aft.nanxinkj.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mdq.fengsongda.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://eoy.andypj.xyz

Java: Math.round(3.567); Math.floor(3.9)
来源：http://iub.vehdjk.com

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://ihn.zhoulong.xyz

Ruby: 3.567.round(2); 3.9.floor
来源：http://rxi.nwbrower.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://gog.jqgufenzy.top

[A09] 绝对值与最大最小值
来源：http://djp.52xcode.cn

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://uyp.jinqigufen.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://jts.mhx1999.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://fnp.iojbl.cn

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://jlj.mhx1999.top


<!-- 参考信息 -->