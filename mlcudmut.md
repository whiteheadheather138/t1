代发 wailian999

[U53] PHP：空合并运算符
来源：http://eyn.jianghu66.top

$v = $a ?? $b ?? "default";
来源：http://hli.52xcode.cn

[U54] PHP：空安全调用
来源：http://kyk.pengpengdd.cyou

$obj?->method()
来源：http://hnc.hysaishi.cn

[U55] PHP：match 表达式
来源：http://miq.zdbjq.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://igf.aizwys.cn

[U56] PHP：命名参数
来源：http://xco.yvedp.cn

f(a: 1, b: 2)
来源：http://hun.wangshuangyany.cn

[U57] PHP：字符串插值
来源：http://lar.0kj1m.cn

"值: {$a}"
来源：http://qdb.tarul.cn

[U58] PHP：数组三件套
来源：http://fei.shanyushiyangtech.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lew.chenjidiqi.icu

[U59] PHP：自定义排序
来源：http://eih.fehbvm.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ijt.yj20258888.top

[U60] PHP：JSON 编解码
来源：http://ofl.xingfuxueyuan.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jyp.ppjwa.cn

[U61] PHP：正则
来源：http://ofu.ppjwa.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kto.wangdashe.top

[U62] PHP：日期对象
来源：http://cnf.yvedp.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xge.hfpthk.cn

[U63] PHP：文件读写
来源：http://ccu.sysykeji.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ngf.cashguo.top

[U64] PHP：目录遍历
来源：http://uvh.sjlbkw.cn

glob("dir/*.php");  scandir("dir");
来源：http://lzf.0kj1m.cn

[U65] PHP：会话
来源：http://ndb.yj20258.top

session_start();  $_SESSION["uid"] = 1;
来源：http://izd.ybcxt.top

[U66] PHP：设置 Cookie
来源：http://kdr.yvedp.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://opo.dashuyun.cn

[U67] PHP：处理文件上传
来源：http://ier.yongpay.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kvu.wangshuangyany.cn

[U68] PHP：PDO 连接
来源：http://gyx.hammf.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ewv.zhongyouzk.top

[U69] PHP：PDO 预处理
来源：http://srd.hysaishi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ark.gzhubu.top

[U70] PHP：PDO 事务
来源：http://mhf.wangshuangyany.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://iff.yj20258888.top

[U71] PHP：抛出异常
来源：http://zxc.zhiwuduotai.top

throw new RuntimeException("失败", 500);
来源：http://ftw.nanxuanxn.top

[U72] PHP：写错误日志
来源：http://qtc.daxiang520.top

error_log("失败: " . $e->getMessage());
来源：http://lec.yvedp.cn

[U73] PHP：读取 ini 配置
来源：http://lqj.shangyingyoupin.top

parse_ini_file("config.ini", true)
来源：http://dme.xziqi.cn

[U74] PHP：读取环境变量
来源：http://ggi.zhaomingkeji.xyz

getenv("APP_ENV") ?: "production"
来源：http://sud.havefunace.top

[U75] PHP：依赖注入
来源：http://jew.wangdashe.top

composer require psr/container
来源：http://rro.epnwcf.com

[U76] PHP：简单路由
来源：http://ajh.zhoulong.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hkw.dashuyun.cn

[U77] PHP：模板渲染
来源：http://ltq.jiagoushi.top

composer require twig/twig
来源：http://plt.cashguo.top

[U78] PHP：单元测试
来源：http://rxz.quarkkingdee.top

composer require --dev phpunit/phpunit
来源：http://kxg.hesvh.cn

[U79] PHP：静态分析
来源：http://zea.gzhubu.top

composer require --dev phpstan/phpstan
来源：http://znz.chenjidiqi.icu

[U80] PHP：代码规范修复
来源：http://rre.tanke756.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://glg.andypj.xyz

[U81] JS：初始化项目
来源：http://dff.sysykeji.top

npm init -y;  npm i express
来源：http://udy.hcnkem.com

[U82] JS：package.json 脚本
来源：http://clm.zdqjudy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://crv.epnwcf.com

[U83] JS：ES Module 导入导出
来源：http://xct.guannengcc.top

export const a = 1;  import { a } from "./m.js";
来源：http://tzj.daria6918.cn

[U84] JS：CommonJS 写法
来源：http://rcw.9152youxi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://pgv.jinqigfzy.top

[U85] JS：可选链
来源：http://jgt.jyoumei.cn

a?.b?.c
来源：http://qah.ctjpmb.com

[U86] JS：空值合并
来源：http://pno.fanxiaobao.xyz

a ?? b
来源：http://wwy.zhijiandao.cn

[U87] JS：解构默认值
来源：http://rgy.yuxming.cn

const { a = 1, b = 2 } = obj;
来源：http://xas.ybcxt.top

[U88] JS：对象展开合并
来源：http://hzm.yueranfly.top

{ ...a, ...b }
来源：http://ppb.bbcook.cn

[U89] JS：数组去重
来源：http://arw.yj202588.top

[...new Set(arr)]
来源：http://hjt.gzhubu.top

[U90] JS：数字数组排序
来源：http://eyj.ydjk.org.cn

[...arr].sort((a, b) => a - b)
来源：http://rnm.tarul.cn

[U91] JS：对象键值遍历
来源：http://pnj.0kj1m.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ezd.jiagoushi.top

[U92] JS：深拷贝
来源：http://dqq.zhiwuduotai.top

structuredClone(obj)
来源：http://xiv.bbcook.cn

[U93] JS：模板字符串
来源：http://pyu.gzhubu.top

`共 ${n} 条`
来源：http://qxz.guowangkeji.top

[U94] JS：箭头函数
来源：http://air.yonumen.top

const double = x => x * 2;
来源：http://mqs.svipenyu.cn

[U95] JS：Promise 包装
来源：http://uxv.havefunace.top

new Promise((resolve, reject) => {})
来源：http://lii.fzhhl.top

[U96] JS：async/await 与异常
来源：http://amb.snrcjt.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gpk.zdbjq.cn

[U97] JS：并发请求
来源：http://spv.fehbvm.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://qxx.zdbjq.cn

[U98] JS：fetch 带 JSON
来源：http://iyt.fehbvm.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://dcy.quarkkingdee.top

[U99] JS：事件监听
来源：http://fxw.fehbvm.com

el.addEventListener("click", e => {})
来源：http://pur.yvedp.cn

[U100] JS：DOM 查询
来源：http://amm.fengsongda.top

document.querySelector(".item")
来源：http://ggh.pengpengdd.cyou

[U101] JS：classList 操作
来源：http://syx.chenjidiqi.icu

el.classList.toggle("active")
来源：http://vlx.jinqigfzy.top

[U102] JS：本地存储
来源：http://dzt.vqdsnc.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://ujt.zdqjudy.top

[U103] JS：定时器
来源：http://lun.guowangkeji.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://tdg.ydjk.org.cn

[U104] JS：防抖
来源：http://ffz.ybcxt.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wmu.zdqjudy.top

[U105] JS：节流
来源：http://qrm.yueranfly.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ulg.hongshengwenyu.top

[U106] JS：日期格式化
来源：http://ezl.yj20258888.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mco.meibo888.top

[U107] JS：数字千分位
来源：http://tnf.sxryk.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://snd.yongpay.top

[U108] JS：随机整数
来源：http://nrk.ywan-chungtsiang.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vqi.jinghuilouyu.cn

[U109] JS：数组分组
来源：http://vih.haohaochexian.top

Object.groupBy(arr, x => x.type)
来源：http://tnk.xziqi.cn

[U110] JS：数组分块
来源：http://zyh.uphjek.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://onf.cashguo.top

[U111] JS：对象转 Map
来源：http://wxw.ehwqpu.com

new Map(Object.entries(obj))
来源：http://vou.hywenlv.cn

[U112] JS：字符串补位
来源：http://htd.tianlin.xyz

"7".padStart(3, "0")
来源：http://iau.cqqwz.cn

[U113] JS：正则替换全部
来源：http://pov.xinyue.icu

s.replaceAll("a", "b")
来源：http://ast.shanyushiyangtech.top

[U114] JS：JSON 深比较
来源：http://yby.shanyushiyangtech.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://mle.yj202588.top

[U115] JS：生成 UUID
来源：http://sfj.smart0.xyz

crypto.randomUUID()
来源：http://rkg.zhijiandao.cn

[U116] JS：类型检查（JSDoc）
来源：http://fck.zhongyouzk.top

/** @param {string} name */ function f(name) {}
来源：http://lzh.yj20258.top

[U117] JS：单元测试
来源：http://rhj.tarul.cn

npm i -D vitest;  npx vitest
来源：http://xnl.meibo888.top

[U118] JS：开发服务器
来源：http://rha.bjfxy.top

npm i -D vite;  npx vite
来源：http://vth.mhx1999.top

[U119] JS：生产构建
来源：http://sma.birdmap.top

npx vite build
来源：http://moi.hammf.cn

[U120] JS：读取环境变量（Vite）
来源：http://ebv.zhoulong.xyz

import.meta.env.VITE_API_URL
来源：http://mwl.52xcode.cn

================================================================================
来源：http://mmi.wangdashe.top

统计汇总
来源：http://trg.hesvh.cn

================================================================================
来源：http://tkr.svipenyu.cn

按语言统计（条）：
来源：http://gkt.ivvv.top

Python ......... 252
来源：http://pth.zdbjq.cn

PHP ............ 252
来源：http://ebw.dianchejie.cn

JavaScript ..... 252
来源：http://itc.ydzc1.top

TypeScript ..... 212
来源：http://fkk.smart0.xyz

Java ........... 212
来源：http://cpz.xuanzx.com

Go ............. 212
来源：http://pvt.vehdjk.com

Ruby ........... 212
来源：http://hsu.sufxvd.cn

C# ............. 212
来源：http://kmm.feifeiyinyue.top

C .............. 30
来源：http://exq.jinqigfzy.top

C++ ............ 30
来源：http://lqs.xuanzx.com

SQL ............ 90
来源：http://hxo.ivvv.top

Bash ........... 80
来源：http://sdz.shzxlz.cn

Kotlin ......... 15
来源：http://org.bjfxy.top

Swift .......... 15
来源：http://pol.aibaodan.cn

Lua ............ 10
来源：http://csv.xziqi.cn

Perl ........... 10
来源：http://kfs.pengpengdd.cyou

Scala .......... 10
来源：http://qnw.yonumen.top

------------------------------------
来源：http://hnw.ybcxt.top

合计 ........... 2106 条
来源：http://xty.xingfuxueyuan.xyz

按章节统计：
来源：http://qda.quarkkingdee.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jnd.xuetiantiany.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://hxn.xuetiantiany.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://bkx.bjfxy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://alr.chenlongwang.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gpv.vqdsnc.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wba.hammf.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ihv.yanxiufei.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://aid.vqdsnc.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://ubm.zhongyouzk.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://ykc.jqgfzy.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://jai.cheryme.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://nvb.sjlbkw.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mzb.yangfankeji.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zot.feifeiyinyue.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://jwj.hywenlv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://lly.fanxiaobao.xyz

Q SQL 专题                              90
来源：http://yqw.jqgufenzy.top

R Bash 专题                             80
来源：http://rvx.mhx1999.top

S C / C++ 专题                          60
来源：http://xcd.yj20258888.top

T 其他语言补充                          60
来源：http://kaa.hywenlv.cn

U 高频实用片段                         120
来源：http://ccs.aizwys.cn

------------------------------------
来源：http://nqx.havefunace.top

合计                                  2106 条
来源：http://rfv.yueranfly.top

--------------------------------------------------------------------------------
来源：http://jyx.zycfv.cn

使用提醒
来源：http://hzc.tarul.cn

--------------------------------------------------------------------------------
来源：http://lji.jinqigufen.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hry.daxiang520.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://xbj.bbcook.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://met.fehbvm.com

在旧版本上使用前请先确认语法支持情况。
来源：http://bre.ctjpmb.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://qxq.shangyingyoupin.top

—— 文件结束 ——
来源：http://mtw.feifeiyinyue.top

================================================================================
来源：http://kub.ybcxt.top

程序语言常见例子速查手册（2024 版）
来源：http://spv.shangyingyoupin.top

Common Programming Examples Cheat Book
来源：http://ntl.ctjpmb.com

================================================================================
来源：http://xas.jiagoushi.top

【收录内容】
来源：http://xrp.zhijiandao.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://jgl.xuanzx.com

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://vrg.hongshengwenyu.top

SQL · Bash · C · C++
来源：http://jus.jlsjyb.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://but.hammf.cn

【使用说明】
来源：http://qvi.zhaomingkeji.xyz

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://gqo.cashguo.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://qhh.nwbrower.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://hra.tianlin.xyz

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://dxi.sjlbkw.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://jzo.sufxvd.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mtl.xuetiantiany.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://amy.pengpengdd.cyou

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://tuc.dashuyun.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://nry.jiagoushi.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kkm.hnqzz.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://bae.zhijiandao.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://tvj.zhongyouzk.top

【文件统计】
来源：http://bvx.birdmap.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xad.redwolf501.top

--------------------------------------------------------------------------------
来源：http://njt.hesvh.cn

目  录
来源：http://rrh.fktsv.cn

--------------------------------------------------------------------------------
来源：http://zws.vqdsnc.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://fys.zhaomingkeji.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://zep.chenzaomai.com

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://xmx.meibo888.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://ype.jqgufenzy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://bvq.yfazqb.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ipb.ydjk.org.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rez.0kj1m.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://yjb.fktsv.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://cvw.chenjidiqi.icu

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fjo.ybcxt.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://vmf.gzhubu.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wav.dashuyun.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://jbn.gotoacloud.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://ypd.yangfankeji.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ajn.jinyuanbaomall.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://cpm.quarkkingdee.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nwb.tianlin.xyz

R. Bash 专题                   （第 18 节，80 条）
来源：http://zrz.52xcode.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://oix.sysykeji.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://zbo.iojbl.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xyh.dianchejie.cn

================================================================================
来源：http://mxc.guannengcc.top

A. 基础语法与类型
来源：http://wvh.zdbjq.cn

================================================================================
来源：http://hkh.zhaomingkeji.xyz

[A01] Hello World
来源：http://ptj.shanyushiyangtech.top

Py:   print("Hello, World!")
来源：http://oeo.fanxiaobao.xyz

PHP:  echo "Hello, World!";
来源：http://tcr.tarul.cn

JS:   console.log("Hello, World!");
来源：http://vti.xuanzx.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://svw.snrcjt.cn

Java: System.out.println("Hello, World!");
来源：http://mrb.jinqigufen.top

Go:   fmt.Println("Hello, World!")
来源：http://urh.hesvh.cn

Ruby: puts "Hello, World!"
来源：http://ivv.fehbvm.com

C#:   Console.WriteLine("Hello, World!");
来源：http://hsz.yfazqb.com

[A02] 变量声明与赋值
来源：http://bkb.haohaochexian.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://pfk.quarkkingdee.top

PHP:  $name = "Alex"; $age = 20;
来源：http://pzo.wangshuangyany.cn

JS:   let name = "Alex"; const age = 20;
来源：http://qhe.zycfv.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://hnt.pycfn.com

Java: String name = "Alex"; int age = 20;
来源：http://sym.dianchejie.cn

Go:   name := "Alex"; age := 20
来源：http://uju.guannengcc.top

Ruby: name = "Alex"; age = 20
来源：http://yfh.ehwqpu.com

C#:   string name = "Alex"; int age = 20;
来源：http://bbd.gzhubu.top

[A03] 常量定义
来源：http://eps.jinyuanbaomall.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://grl.jqgufenzy.top

PHP:  const PI = 3.14159;
来源：http://kpx.nanxinkj.top

JS:   const PI = 3.14159;
来源：http://eza.yongpay.top

TS:   const PI: number = 3.14159;
来源：http://zmj.yj202588.top

Java: static final double PI = 3.14159;
来源：http://wpf.xuanzx.com

Go:   const PI = 3.14159
来源：http://gfk.ydjk.org.cn

Ruby: PI = 3.14159
来源：http://viv.jinghuilouyu.cn

C#:   const double PI = 3.14159;
来源：http://usb.xuanzx.com

[A04] 判断变量类型
来源：http://gyy.haohaochexian.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://xjb.wangshuangyany.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jap.daxiang520.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://for.bjfxy.top

TS:   typeof x; x instanceof Date
来源：http://wdb.cdnleiting.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://nue.hcnkem.com

Go:   reflect.TypeOf(x).Name()
来源：http://gne.cashguo.top

Ruby: x.class; x.is_a?(Integer)
来源：http://nbm.jinyuanbaomall.cn

C#:   x.GetType().Name; x is int
来源：http://sjh.ctjpmb.com

[A05] 整数除法与取模
来源：http://fht.gotoacloud.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mbl.chenjidiqi.icu

PHP:  intdiv(7, 2); 7 % 2
来源：http://vek.9152youxi.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://aip.daxiang520.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://xrc.dianchejie.cn

Java: 7 / 2; 7 % 2
来源：http://xum.316326.xyz

Go:   7 / 2; 7 % 2
来源：http://dyu.9152youxi.cn

Ruby: 7 / 2; 7 % 2
来源：http://cry.xuanzx.com

C#:   7 / 2; 7 % 2
来源：http://ccd.zdbjq.cn

[A06] 字符串转数字
来源：http://fcw.jlsjyb.cn

Py:   int("42"); float("3.14")
来源：http://nga.zhixingplan.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://xsc.havefunace.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://tul.jqgfzy.top

TS:   parseInt("42", 10); Number("42")
来源：http://zzb.gotoacloud.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://apk.jqgfzy.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://aht.jlsjyb.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://eon.ydjk.org.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://fnz.sjlbkw.cn

[A07] 数字转字符串
来源：http://tub.gaohongyu789.top

Py:   str(42)
来源：http://dks.jqgufenzy.top

PHP:  (string) 42; strval(42)
来源：http://pnl.fzhhl.top


<!-- 参考信息 -->