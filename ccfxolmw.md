代发 wailian999

[U47] PHP：联合类型
来源：http://low.zycfv.cn

int|string $id
来源：http://ijt.nanxuanxn.top

[U48] PHP：纯枚举
来源：http://bly.zycfv.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://sqx.shzxlz.cn

[U49] PHP：只读属性
来源：http://lik.pycfn.com

public readonly string $name
来源：http://cqr.nwbrower.top

[U50] PHP：构造器属性提升
来源：http://lxh.wangshuangyany.cn

public function __construct(private int $id) {}
来源：http://snk.sxryk.cn

[U51] PHP：数组解构
来源：http://kfh.shanyushiyangkeji.top

[$a, $b] = $arr;
来源：http://zrs.hysaishi.cn

[U52] PHP：箭头函数
来源：http://eyr.wangshuangyany.cn

$double = fn($x) => $x * 2;
来源：http://fwt.hongshengwenyu.top

[U53] PHP：空合并运算符
来源：http://qnt.nanxinkj.top

$v = $a ?? $b ?? "default";
来源：http://zyh.chenjidiqi.icu

[U54] PHP：空安全调用
来源：http://ehg.tanke756.top

$obj?->method()
来源：http://lft.cashguo.top

[U55] PHP：match 表达式
来源：http://pjs.dianchejie.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rif.yfazqb.com

[U56] PHP：命名参数
来源：http://azm.tarul.cn

f(a: 1, b: 2)
来源：http://emc.zhengqikj.top

[U57] PHP：字符串插值
来源：http://ytf.c1oappe.top

"值: {$a}"
来源：http://kst.vqdsnc.cn

[U58] PHP：数组三件套
来源：http://lyi.ivvv.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ugx.aibaodan.cn

[U59] PHP：自定义排序
来源：http://rco.jinqigufen.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nzc.yj202588.top

[U60] PHP：JSON 编解码
来源：http://qlm.cashguo.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tdq.guannengcc.top

[U61] PHP：正则
来源：http://anz.hysaishi.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://xkm.chenjidiqi.icu

[U62] PHP：日期对象
来源：http://iad.feifeiyinyue.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zwa.zhaomingkeji.xyz

[U63] PHP：文件读写
来源：http://xij.nanxuanxn.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://prn.shangyingyoupin.top

[U64] PHP：目录遍历
来源：http://eha.yuanzhike.top

glob("dir/*.php");  scandir("dir");
来源：http://dnz.cashguo.top

[U65] PHP：会话
来源：http://szk.cashguo.top

session_start();  $_SESSION["uid"] = 1;
来源：http://syh.daria6918.cn

[U66] PHP：设置 Cookie
来源：http://whe.zhixingplan.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yij.hnqzz.top

[U67] PHP：处理文件上传
来源：http://anh.ywan-chungtsiang.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://isl.hesvh.cn

[U68] PHP：PDO 连接
来源：http://bdl.zhixingplan.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xwg.tianlin.xyz

[U69] PHP：PDO 预处理
来源：http://dxn.shuidangran.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xru.hcnkem.com

[U70] PHP：PDO 事务
来源：http://fsy.sufxvd.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://khd.sufxvd.cn

[U71] PHP：抛出异常
来源：http://kak.pengpengdd.cyou

throw new RuntimeException("失败", 500);
来源：http://mzb.fanxiaobao.xyz

[U72] PHP：写错误日志
来源：http://vlg.guannengcc.top

error_log("失败: " . $e->getMessage());
来源：http://ibx.sxryk.cn

[U73] PHP：读取 ini 配置
来源：http://tih.andypj.xyz

parse_ini_file("config.ini", true)
来源：http://gxz.birdmap.top

[U74] PHP：读取环境变量
来源：http://hpa.hnqzz.top

getenv("APP_ENV") ?: "production"
来源：http://zck.hcnkem.com

[U75] PHP：依赖注入
来源：http://dpi.ppjwa.cn

composer require psr/container
来源：http://adt.jqgufenzy.top

[U76] PHP：简单路由
来源：http://vxd.jiagoushi.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://xmj.9152youxi.cn

[U77] PHP：模板渲染
来源：http://zdl.chenjidiqi.icu

composer require twig/twig
来源：http://ypa.xinyue.icu

[U78] PHP：单元测试
来源：http://loj.aizwys.cn

composer require --dev phpunit/phpunit
来源：http://kym.yj20258888.top

[U79] PHP：静态分析
来源：http://rmi.zhongyouzk.top

composer require --dev phpstan/phpstan
来源：http://gzi.tianlin.xyz

[U80] PHP：代码规范修复
来源：http://srn.meibo888.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://dpa.zhongyouzk.top

[U81] JS：初始化项目
来源：http://ijx.yanxiufei.cn

npm init -y;  npm i express
来源：http://aqd.vehdjk.com

[U82] JS：package.json 脚本
来源：http://gfr.guowangkeji.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fel.zhoulong.xyz

[U83] JS：ES Module 导入导出
来源：http://uqy.yuxming.cn

export const a = 1;  import { a } from "./m.js";
来源：http://hoc.birdmap.top

[U84] JS：CommonJS 写法
来源：http://hwm.shuidangran.top

module.exports = { a };  const { a } = require("./m");
来源：http://caw.pengpengdd.cyou

[U85] JS：可选链
来源：http://hju.zycfv.cn

a?.b?.c
来源：http://xfp.cashguo.top

[U86] JS：空值合并
来源：http://wss.zdbjq.cn

a ?? b
来源：http://ayq.cucudq.cn

[U87] JS：解构默认值
来源：http://fgj.zhixingplan.top

const { a = 1, b = 2 } = obj;
来源：http://cmd.xylfe.cn

[U88] JS：对象展开合并
来源：http://eij.yj202588.top

{ ...a, ...b }
来源：http://yad.chenjidiqi.icu

[U89] JS：数组去重
来源：http://wwf.jianghu66.top

[...new Set(arr)]
来源：http://pms.zhaomingkeji.xyz

[U90] JS：数字数组排序
来源：http://kvy.nanxuanxn.top

[...arr].sort((a, b) => a - b)
来源：http://iov.birdmap.top

[U91] JS：对象键值遍历
来源：http://cdx.aizwys.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wnm.chenjidiqi.icu

[U92] JS：深拷贝
来源：http://rvq.dianchejie.cn

structuredClone(obj)
来源：http://mwf.zhaomingkeji.xyz

[U93] JS：模板字符串
来源：http://gbo.hysaishi.cn

`共 ${n} 条`
来源：http://uut.hesvh.cn

[U94] JS：箭头函数
来源：http://bte.fanxiaobao.xyz

const double = x => x * 2;
来源：http://bes.gotoacloud.top

[U95] JS：Promise 包装
来源：http://ogl.jqgfzy.top

new Promise((resolve, reject) => {})
来源：http://dmg.havefunace.top

[U96] JS：async/await 与异常
来源：http://ooa.shanyushiyangtech.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://yca.yj202588.top

[U97] JS：并发请求
来源：http://tvn.daxiang520.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://bws.feifeiyinyue.top

[U98] JS：fetch 带 JSON
来源：http://cpp.hnxiangtu.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://iwh.hammf.cn

[U99] JS：事件监听
来源：http://jow.aizwys.cn

el.addEventListener("click", e => {})
来源：http://aht.smart0.xyz

[U100] JS：DOM 查询
来源：http://zfx.hcnkem.com

document.querySelector(".item")
来源：http://iob.cheryme.top

[U101] JS：classList 操作
来源：http://zwz.nwbrower.top

el.classList.toggle("active")
来源：http://imi.cdnleiting.top

[U102] JS：本地存储
来源：http://hte.ydjk.org.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://cey.cucudq.cn

[U103] JS：定时器
来源：http://rev.hysaishi.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://eny.kuanghao11.cn

[U104] JS：防抖
来源：http://hma.aibaodan.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dmy.yj20258.top

[U105] JS：节流
来源：http://fwz.yanxiufei.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ieq.jlsjyb.cn

[U106] JS：日期格式化
来源：http://kam.smart0.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://sfw.zhaomingkeji.xyz

[U107] JS：数字千分位
来源：http://gnu.vehdjk.com

new Intl.NumberFormat("en-US").format(1234567)
来源：http://nph.ydzc1.top

[U108] JS：随机整数
来源：http://emo.mhx1999.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://glj.zdbjq.cn

[U109] JS：数组分组
来源：http://aec.nanxinkj.top

Object.groupBy(arr, x => x.type)
来源：http://kmj.ctjpmb.com

[U110] JS：数组分块
来源：http://har.pycfn.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tjm.jqgfzy.top

[U111] JS：对象转 Map
来源：http://xkf.chenjidiqi.icu

new Map(Object.entries(obj))
来源：http://haa.yvedp.cn

[U112] JS：字符串补位
来源：http://xpe.zycfv.cn

"7".padStart(3, "0")
来源：http://fmk.mhx1999.top

[U113] JS：正则替换全部
来源：http://yqd.chenjidiqi.icu

s.replaceAll("a", "b")
来源：http://ewo.hfpthk.cn

[U114] JS：JSON 深比较
来源：http://gcj.sjlbkw.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://sxc.yuxming.cn

[U115] JS：生成 UUID
来源：http://iui.yj20258888.top

crypto.randomUUID()
来源：http://qpk.zdqjudy.top

[U116] JS：类型检查（JSDoc）
来源：http://obl.epnwcf.com

/** @param {string} name */ function f(name) {}
来源：http://lbj.kuanghao11.cn

[U117] JS：单元测试
来源：http://ujh.hysaishi.cn

npm i -D vitest;  npx vitest
来源：http://hao.shuidangran.top

[U118] JS：开发服务器
来源：http://mxu.cqqwz.cn

npm i -D vite;  npx vite
来源：http://ymm.ybcxt.top

[U119] JS：生产构建
来源：http://fiu.daxiang520.top

npx vite build
来源：http://zqt.uphjek.com

[U120] JS：读取环境变量（Vite）
来源：http://yzp.hcnkem.com

import.meta.env.VITE_API_URL
来源：http://daw.fzhhl.top

================================================================================
来源：http://ocx.cqqwz.cn

统计汇总
来源：http://cjz.yfazqb.com

================================================================================
来源：http://xxz.sufxvd.cn

按语言统计（条）：
来源：http://rvc.zdbjq.cn

Python ......... 252
来源：http://auy.wangshuangyany.cn

PHP ............ 252
来源：http://rkd.sweek.top

JavaScript ..... 252
来源：http://emp.nwbrower.top

TypeScript ..... 212
来源：http://vdn.hnxiangtu.top

Java ........... 212
来源：http://ajc.tanke756.top

Go ............. 212
来源：http://drl.cheryme.top

Ruby ........... 212
来源：http://iul.cucudq.cn

C# ............. 212
来源：http://vpe.52xcode.cn

C .............. 30
来源：http://wvb.ydjk.org.cn

C++ ............ 30
来源：http://yey.yvedp.cn

SQL ............ 90
来源：http://fgr.ivvv.top

Bash ........... 80
来源：http://lkk.shanyushiyangtech.top

Kotlin ......... 15
来源：http://jco.mhx1999.top

Swift .......... 15
来源：http://chm.yj202588.top

Lua ............ 10
来源：http://lou.cdnleiting.top

Perl ........... 10
来源：http://qhz.chenzaomai.com

Scala .......... 10
来源：http://cec.sysykeji.top

------------------------------------
来源：http://dlz.sufxvd.cn

合计 ........... 2106 条
来源：http://usc.hnxiangtu.top

按章节统计：
来源：http://ckb.haohaochexian.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://ffi.chenzaomai.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://vyn.xingfuxueyuan.xyz

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://anw.cqqwz.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://weo.snrcjt.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://anb.yueranfly.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ffw.daria6918.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://twj.cdnleiting.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mae.tarul.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zwa.zdbjq.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://vjv.c1oappe.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://lji.cdnleiting.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://flf.hywenlv.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://rfr.ehwqpu.com

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://epc.sufxvd.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://znz.smart0.xyz

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://tpn.xuanzx.com

Q SQL 专题                              90
来源：http://hrh.hcnkem.com

R Bash 专题                             80
来源：http://xhn.fzhhl.top

S C / C++ 专题                          60
来源：http://yfd.ybcxt.top

T 其他语言补充                          60
来源：http://sxo.shanyushiyangkeji.top

U 高频实用片段                         120
来源：http://mgr.zdbjq.cn

------------------------------------
来源：http://bwj.jinyuanbaomall.cn

合计                                  2106 条
来源：http://trp.svipenyu.cn

--------------------------------------------------------------------------------
来源：http://rcl.yanxiufei.cn

使用提醒
来源：http://stj.zhixingplan.top

--------------------------------------------------------------------------------
来源：http://qqs.tarul.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zkb.bjfxy.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://shz.gotoacloud.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ptq.wangshuangyany.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://kdq.nanxuanxn.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://abj.quarkkingdee.top

—— 文件结束 ——
来源：http://egd.cqqwz.cn

================================================================================
来源：http://qkb.xziqi.cn

程序语言常见例子速查手册（2024 版）
来源：http://zyi.fanxiaobao.xyz

Common Programming Examples Cheat Book
来源：http://hpb.shuidangran.top

================================================================================
来源：http://ram.tian-w.cn

【收录内容】
来源：http://uhn.aibaodan.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://szh.fengsongda.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://uog.shanyushiyangtech.top

SQL · Bash · C · C++
来源：http://qeh.yongpay.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mfa.kuanghao11.cn

【使用说明】
来源：http://gxs.xinyue.icu

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://cez.xinyue.icu

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://glt.meibo888.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://vko.jiagoushi.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://juq.tianlin.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://cov.yj20258.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wsf.fengsongda.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://fqs.ehwqpu.com

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://vot.shzxlz.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://fzz.nanxinkj.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://vgq.jyoumei.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://pus.ywan-chungtsiang.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ymv.sweek.top

【文件统计】
来源：http://twv.cucudq.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://xtr.xingfuxueyuan.xyz

--------------------------------------------------------------------------------
来源：http://bjd.cdnleiting.top

目  录
来源：http://keb.hywenlv.cn

--------------------------------------------------------------------------------
来源：http://lhd.cqqwz.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kyq.redwolf501.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://uhz.yj202588.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://bnx.yueranfly.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://nlw.jinqigfzy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://ukt.yanxiufei.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://glh.dashuyun.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ovz.aibaodan.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://duy.vehdjk.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://vyg.gogol.net.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://fpp.daxiang520.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://cjd.yueranfly.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rkm.zhaomingkeji.xyz

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ktq.svipenyu.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wfo.shangyingyoupin.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://jxy.zhiwuduotai.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://rmv.shanyushiyangkeji.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://rsu.sxryk.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://yov.ctjpmb.com

S. C / C++ 专题                （第 19 节，60 条）
来源：http://alu.ppjwa.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://pev.jinqigfzy.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xne.smart0.xyz

================================================================================
来源：http://bsi.zhengqikj.top

A. 基础语法与类型
来源：http://tym.52xcode.cn

================================================================================
来源：http://kgs.smart0.xyz

[A01] Hello World
来源：http://ifd.zhaomingkeji.xyz

Py:   print("Hello, World!")
来源：http://haj.shanyushiyangtech.top

PHP:  echo "Hello, World!";
来源：http://bcu.cashguo.top

JS:   console.log("Hello, World!");
来源：http://dsq.redwolf501.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mbf.vehdjk.com

Java: System.out.println("Hello, World!");
来源：http://ssn.316326.xyz

Go:   fmt.Println("Hello, World!")
来源：http://edx.pycfn.com

Ruby: puts "Hello, World!"
来源：http://gmq.iojbl.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://jkv.shanyushiyangkeji.top

[A02] 变量声明与赋值
来源：http://chj.pengpengdd.cyou

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://ijn.gogol.net.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://ctn.daxiang520.top

JS:   let name = "Alex"; const age = 20;
来源：http://rhw.nwbrower.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://zmr.pycfn.com

Java: String name = "Alex"; int age = 20;
来源：http://kej.hesvh.cn

Go:   name := "Alex"; age := 20
来源：http://oel.hysaishi.cn

Ruby: name = "Alex"; age = 20
来源：http://dir.hywenlv.cn

C#:   string name = "Alex"; int age = 20;
来源：http://jaq.guannengcc.top

[A03] 常量定义
来源：http://trs.jinqigfzy.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bmr.svipenyu.cn

PHP:  const PI = 3.14159;
来源：http://mzo.pycfn.com

JS:   const PI = 3.14159;
来源：http://wyx.fanxiaobao.xyz

TS:   const PI: number = 3.14159;
来源：http://zcy.tian-w.cn

Java: static final double PI = 3.14159;
来源：http://xie.jqgufenzy.top

Go:   const PI = 3.14159
来源：http://zkd.yj202588.top

Ruby: PI = 3.14159
来源：http://ikl.ppjwa.cn

C#:   const double PI = 3.14159;
来源：http://gqc.tarul.cn

[A04] 判断变量类型
来源：http://hzg.yonumen.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://zzg.9152youxi.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qpi.hcnkem.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://tbx.aizwys.cn

TS:   typeof x; x instanceof Date
来源：http://afy.guowangkeji.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://dxt.nanxinkj.top

Go:   reflect.TypeOf(x).Name()
来源：http://xsc.ydzc1.top

Ruby: x.class; x.is_a?(Integer)
来源：http://zfs.hysaishi.cn

C#:   x.GetType().Name; x is int
来源：http://qhg.ivvv.top

[A05] 整数除法与取模
来源：http://rzd.gogol.net.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://hcl.fanxiaobao.xyz

PHP:  intdiv(7, 2); 7 % 2
来源：http://hsk.ehwqpu.com

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://yst.yueranfly.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://rwz.sysykeji.top

Java: 7 / 2; 7 % 2
来源：http://tfn.quarkkingdee.top

Go:   7 / 2; 7 % 2
来源：http://sdy.shangyingyoupin.top

Ruby: 7 / 2; 7 % 2
来源：http://eff.sysykeji.top

C#:   7 / 2; 7 % 2
来源：http://qsq.0kj1m.cn


<!-- 参考信息 -->