代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://imv.jqgfzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://jgt.jianghu66.top

[U46] PHP：可空类型
来源：http://ayy.iojbl.cn

?string $name = null
来源：http://src.dashuyun.cn

[U47] PHP：联合类型
来源：http://haw.meibo888.top

int|string $id
来源：http://ira.gotoacloud.top

[U48] PHP：纯枚举
来源：http://zjb.sufxvd.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ivk.aizwys.cn

[U49] PHP：只读属性
来源：http://bro.sufxvd.cn

public readonly string $name
来源：http://nsz.hammf.cn

[U50] PHP：构造器属性提升
来源：http://env.yvedp.cn

public function __construct(private int $id) {}
来源：http://ric.uphjek.com

[U51] PHP：数组解构
来源：http://omg.daxiang520.top

[$a, $b] = $arr;
来源：http://epo.yuanzhike.top

[U52] PHP：箭头函数
来源：http://niz.yongpay.top

$double = fn($x) => $x * 2;
来源：http://lgn.daxiang520.top

[U53] PHP：空合并运算符
来源：http://uge.jinqigufen.top

$v = $a ?? $b ?? "default";
来源：http://qly.xinyue.icu

[U54] PHP：空安全调用
来源：http://uei.shanyushiyangkeji.top

$obj?->method()
来源：http://rla.shzxlz.cn

[U55] PHP：match 表达式
来源：http://myu.smart0.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gjy.quarkkingdee.top

[U56] PHP：命名参数
来源：http://tqz.cqqwz.cn

f(a: 1, b: 2)
来源：http://afn.gotoacloud.top

[U57] PHP：字符串插值
来源：http://oph.sysykeji.top

"值: {$a}"
来源：http://bjx.zhiwuduotai.top

[U58] PHP：数组三件套
来源：http://vqp.sufxvd.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://apf.jianghu66.top

[U59] PHP：自定义排序
来源：http://amy.yj20258888.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cla.bbcook.cn

[U60] PHP：JSON 编解码
来源：http://fkr.zhoulong.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://dzn.yuxming.cn

[U61] PHP：正则
来源：http://vhy.andypj.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://erb.smart0.xyz

[U62] PHP：日期对象
来源：http://wpy.yj202588.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gdr.tarul.cn

[U63] PHP：文件读写
来源：http://yph.daria6918.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://nzy.dianchejie.cn

[U64] PHP：目录遍历
来源：http://zyw.hysaishi.cn

glob("dir/*.php");  scandir("dir");
来源：http://kpn.sufxvd.cn

[U65] PHP：会话
来源：http://srs.jinghuilouyu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://ugw.yuanzhike.top

[U66] PHP：设置 Cookie
来源：http://stj.cucudq.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rsr.shuidangran.top

[U67] PHP：处理文件上传
来源：http://evs.tianlin.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vhf.zhijiandao.cn

[U68] PHP：PDO 连接
来源：http://mfi.kuanghao11.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dys.zhixingplan.top

[U69] PHP：PDO 预处理
来源：http://aem.zhijiandao.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hte.xuanzx.com

[U70] PHP：PDO 事务
来源：http://myc.316326.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jzo.hfpthk.cn

[U71] PHP：抛出异常
来源：http://rfq.xziqi.cn

throw new RuntimeException("失败", 500);
来源：http://zxg.tarul.cn

[U72] PHP：写错误日志
来源：http://tqf.redwolf501.top

error_log("失败: " . $e->getMessage());
来源：http://yiv.andypj.xyz

[U73] PHP：读取 ini 配置
来源：http://fhk.hnqzz.top

parse_ini_file("config.ini", true)
来源：http://glh.ehwqpu.com

[U74] PHP：读取环境变量
来源：http://peg.mhx1999.top

getenv("APP_ENV") ?: "production"
来源：http://zku.zhengqikj.top

[U75] PHP：依赖注入
来源：http://mhq.feifeiyinyue.top

composer require psr/container
来源：http://bjz.xuanzx.com

[U76] PHP：简单路由
来源：http://jnb.sufxvd.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mrl.fanxiaobao.xyz

[U77] PHP：模板渲染
来源：http://wvf.jinyuanbaomall.cn

composer require twig/twig
来源：http://efx.jinghuilouyu.cn

[U78] PHP：单元测试
来源：http://hpa.dianchejie.cn

composer require --dev phpunit/phpunit
来源：http://hmu.xziqi.cn

[U79] PHP：静态分析
来源：http://kth.zhoulong.xyz

composer require --dev phpstan/phpstan
来源：http://vny.daxiang520.top

[U80] PHP：代码规范修复
来源：http://ten.snrcjt.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://apa.52xcode.cn

[U81] JS：初始化项目
来源：http://jfz.tian-w.cn

npm init -y;  npm i express
来源：http://ybz.fzhhl.top

[U82] JS：package.json 脚本
来源：http://hxx.epnwcf.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qmg.aizwys.cn

[U83] JS：ES Module 导入导出
来源：http://ljc.xuanzx.com

export const a = 1;  import { a } from "./m.js";
来源：http://kan.wangdashe.top

[U84] JS：CommonJS 写法
来源：http://kes.wangshuangyany.cn

module.exports = { a };  const { a } = require("./m");
来源：http://gbt.jlsjyb.cn

[U85] JS：可选链
来源：http://qnf.aibaodan.cn

a?.b?.c
来源：http://yzx.yfazqb.com

[U86] JS：空值合并
来源：http://qcy.zhixingplan.top

a ?? b
来源：http://bnn.chenzaomai.com

[U87] JS：解构默认值
来源：http://crr.316326.xyz

const { a = 1, b = 2 } = obj;
来源：http://xck.ydzc1.top

[U88] JS：对象展开合并
来源：http://zoi.wangshuangyany.cn

{ ...a, ...b }
来源：http://eew.shuidangran.top

[U89] JS：数组去重
来源：http://jgs.jinyuanbaomall.cn

[...new Set(arr)]
来源：http://zhk.epnwcf.com

[U90] JS：数字数组排序
来源：http://uip.daxiang520.top

[...arr].sort((a, b) => a - b)
来源：http://zvt.wangshuangyany.cn

[U91] JS：对象键值遍历
来源：http://yrz.cheryme.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bga.guannengcc.top

[U92] JS：深拷贝
来源：http://zlx.jlsjyb.cn

structuredClone(obj)
来源：http://bin.xuetiantiany.cn

[U93] JS：模板字符串
来源：http://vcr.316326.xyz

`共 ${n} 条`
来源：http://agq.hcnkem.com

[U94] JS：箭头函数
来源：http://tuy.jinghuilouyu.cn

const double = x => x * 2;
来源：http://bxa.hnqzz.top

[U95] JS：Promise 包装
来源：http://zwg.smart0.xyz

new Promise((resolve, reject) => {})
来源：http://sfi.yuxming.cn

[U96] JS：async/await 与异常
来源：http://zua.zhixingplan.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://rgd.xuetiantiany.cn

[U97] JS：并发请求
来源：http://nas.jlsjyb.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://hti.yangfankeji.com

[U98] JS：fetch 带 JSON
来源：http://qoe.hnxiangtu.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://szf.gogol.net.cn

[U99] JS：事件监听
来源：http://iex.0kj1m.cn

el.addEventListener("click", e => {})
来源：http://cua.hfpthk.cn

[U100] JS：DOM 查询
来源：http://hdc.xylfe.cn

document.querySelector(".item")
来源：http://sni.yvedp.cn

[U101] JS：classList 操作
来源：http://mik.yuxming.cn

el.classList.toggle("active")
来源：http://efs.ivvv.top

[U102] JS：本地存储
来源：http://hmu.hcnkem.com

localStorage.setItem("k", JSON.stringify(v))
来源：http://zpq.sjlbkw.cn

[U103] JS：定时器
来源：http://gnv.zhongyouzk.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blv.hysaishi.cn

[U104] JS：防抖
来源：http://ozq.kuanghao11.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oad.cdnleiting.top

[U105] JS：节流
来源：http://izf.tarul.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wab.yuxming.cn

[U106] JS：日期格式化
来源：http://dly.zhaomingkeji.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://cqf.yvedp.cn

[U107] JS：数字千分位
来源：http://znp.hesvh.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://erq.jqgufenzy.top

[U108] JS：随机整数
来源：http://mit.jinqigufen.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://yns.shangyingyoupin.top

[U109] JS：数组分组
来源：http://ghc.cashguo.top

Object.groupBy(arr, x => x.type)
来源：http://yzp.jqgufenzy.top

[U110] JS：数组分块
来源：http://dxw.chenzaomai.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yzp.ydjk.org.cn

[U111] JS：对象转 Map
来源：http://ntf.yfazqb.com

new Map(Object.entries(obj))
来源：http://wsj.zhijiandao.cn

[U112] JS：字符串补位
来源：http://rdv.zdbjq.cn

"7".padStart(3, "0")
来源：http://xts.tarul.cn

[U113] JS：正则替换全部
来源：http://zix.aibaodan.cn

s.replaceAll("a", "b")
来源：http://ojr.redwolf501.top

[U114] JS：JSON 深比较
来源：http://yme.zhijiandao.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://qtq.tarul.cn

[U115] JS：生成 UUID
来源：http://ynt.sufxvd.cn

crypto.randomUUID()
来源：http://oga.havefunace.top

[U116] JS：类型检查（JSDoc）
来源：http://kcl.hywenlv.cn

/** @param {string} name */ function f(name) {}
来源：http://ins.fehbvm.com

[U117] JS：单元测试
来源：http://crb.nanxuanxn.top

npm i -D vitest;  npx vitest
来源：http://fyd.cheryme.top

[U118] JS：开发服务器
来源：http://zhz.xziqi.cn

npm i -D vite;  npx vite
来源：http://jiu.snrcjt.cn

[U119] JS：生产构建
来源：http://jic.nwbrower.top

npx vite build
来源：http://eej.hysaishi.cn

[U120] JS：读取环境变量（Vite）
来源：http://ijb.xinyue.icu

import.meta.env.VITE_API_URL
来源：http://vjq.ywan-chungtsiang.top

================================================================================
来源：http://spq.jyoumei.cn

统计汇总
来源：http://kxa.guannengcc.top

================================================================================
来源：http://kuj.tianlin.xyz

按语言统计（条）：
来源：http://mnl.birdmap.top

Python ......... 252
来源：http://ftl.guannengcc.top

PHP ............ 252
来源：http://unl.sxryk.cn

JavaScript ..... 252
来源：http://uje.cheryme.top

TypeScript ..... 212
来源：http://tzr.hongshengwenyu.top

Java ........... 212
来源：http://vhx.52xcode.cn

Go ............. 212
来源：http://xew.birdmap.top

Ruby ........... 212
来源：http://chn.ybcxt.top

C# ............. 212
来源：http://mpq.meibo888.top

C .............. 30
来源：http://tuy.epnwcf.com

C++ ............ 30
来源：http://tvw.tarul.cn

SQL ............ 90
来源：http://icw.aizwys.cn

Bash ........... 80
来源：http://ogc.wangdashe.top

Kotlin ......... 15
来源：http://myx.zhijiandao.cn

Swift .......... 15
来源：http://zwp.yanxiufei.cn

Lua ............ 10
来源：http://odn.hongshengwenyu.top

Perl ........... 10
来源：http://qqr.xuetiantiany.cn

Scala .......... 10
来源：http://uic.xinyue.icu

------------------------------------
来源：http://pkm.chenjidiqi.icu

合计 ........... 2106 条
来源：http://kho.haohaochexian.top

按章节统计：
来源：http://xgm.zdbjq.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://sjs.uphjek.com

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dcb.ctjpmb.com

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://cxh.dianchejie.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://htl.sxryk.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://nzr.fanxiaobao.xyz

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://hqq.nwbrower.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://yde.yj20258.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://aep.jinqigfzy.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://zos.redwolf501.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://uwo.sweek.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://fzr.dianchejie.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://zwe.nanxuanxn.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hrx.meibo888.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://zql.pycfn.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://dme.pycfn.com

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://sdo.ywan-chungtsiang.top

Q SQL 专题                              90
来源：http://oma.jqgfzy.top

R Bash 专题                             80
来源：http://cma.fanxiaobao.xyz

S C / C++ 专题                          60
来源：http://cji.zhengqikj.top

T 其他语言补充                          60
来源：http://tpf.bjfxy.top

U 高频实用片段                         120
来源：http://lpb.vehdjk.com

------------------------------------
来源：http://bpq.jinyuanbaomall.cn

合计                                  2106 条
来源：http://xsy.ivvv.top

--------------------------------------------------------------------------------
来源：http://axy.jianghu66.top

使用提醒
来源：http://csz.zycfv.cn

--------------------------------------------------------------------------------
来源：http://ofq.tanke756.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://omu.tian-w.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://znd.yuxming.cn

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://ial.gotoacloud.top

在旧版本上使用前请先确认语法支持情况。
来源：http://qzt.sufxvd.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://iig.tianlin.xyz

—— 文件结束 ——
来源：http://dmw.hfpthk.cn

================================================================================
来源：http://usz.nanxinkj.top

程序语言常见例子速查手册（2024 版）
来源：http://wvc.fzhhl.top

Common Programming Examples Cheat Book
来源：http://zvh.yfazqb.com

================================================================================
来源：http://iwb.sufxvd.cn

【收录内容】
来源：http://bbb.ybcxt.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://tcl.cdnleiting.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ebn.aizwys.cn

SQL · Bash · C · C++
来源：http://qpt.fengsongda.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://gdw.svipenyu.cn

【使用说明】
来源：http://mgu.xinyue.icu

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://pta.ctjpmb.com

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://zjm.vqdsnc.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://iuy.sweek.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://fmu.zhaomingkeji.xyz

Bash:  Shell         C:     C             C++:   C++
来源：http://kfi.ydjk.org.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://cbo.jinghuilouyu.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://ptt.c1oappe.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://fgi.feifeiyinyue.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://umc.hnqzz.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://kaw.bjfxy.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://lcm.fengsongda.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zsc.redwolf501.top

【文件统计】
来源：http://cbg.yueranfly.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://rfv.yfazqb.com

--------------------------------------------------------------------------------
来源：http://udh.smart0.xyz

目  录
来源：http://pba.hammf.cn

--------------------------------------------------------------------------------
来源：http://hzb.zdqjudy.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://rci.xuanzx.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://ldd.guowangkeji.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://cbj.epnwcf.com

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zui.wangshuangyany.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kji.haohaochexian.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://uyf.shzxlz.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://rad.ivvv.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://uia.yj20258888.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://cfy.hammf.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://jct.fanxiaobao.xyz

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://lkj.dashuyun.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://ova.zhongyouzk.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://evw.yvedp.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://jgg.birdmap.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://utg.yj202588.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ukl.ppjwa.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://efm.hesvh.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ich.zhengqikj.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://ktv.vehdjk.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wev.jiagoushi.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wju.havefunace.top

================================================================================
来源：http://gcs.cucudq.cn

A. 基础语法与类型
来源：http://fvy.xinyue.icu

================================================================================
来源：http://vih.hysaishi.cn

[A01] Hello World
来源：http://ybg.ybcxt.top

Py:   print("Hello, World!")
来源：http://som.jiagoushi.top

PHP:  echo "Hello, World!";
来源：http://moj.cashguo.top

JS:   console.log("Hello, World!");
来源：http://alu.sysykeji.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://org.gogol.net.cn

Java: System.out.println("Hello, World!");
来源：http://vqq.9152youxi.cn

Go:   fmt.Println("Hello, World!")
来源：http://fsh.guowangkeji.top

Ruby: puts "Hello, World!"
来源：http://xmw.yongpay.top

C#:   Console.WriteLine("Hello, World!");
来源：http://cpm.chenjidiqi.icu

[A02] 变量声明与赋值
来源：http://wmc.ybcxt.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mft.ctjpmb.com

PHP:  $name = "Alex"; $age = 20;
来源：http://xsf.hfpthk.cn

JS:   let name = "Alex"; const age = 20;
来源：http://yaq.ywan-chungtsiang.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://doy.tian-w.cn

Java: String name = "Alex"; int age = 20;
来源：http://emv.wangshuangyany.cn

Go:   name := "Alex"; age := 20
来源：http://all.zdbjq.cn

Ruby: name = "Alex"; age = 20
来源：http://ikd.smart0.xyz

C#:   string name = "Alex"; int age = 20;
来源：http://tes.jinghuilouyu.cn

[A03] 常量定义
来源：http://wxt.pycfn.com

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bdf.birdmap.top

PHP:  const PI = 3.14159;
来源：http://mew.fanxiaobao.xyz

JS:   const PI = 3.14159;
来源：http://zky.smart0.xyz

TS:   const PI: number = 3.14159;
来源：http://bdk.shuidangran.top

Java: static final double PI = 3.14159;
来源：http://noa.jinqigufen.top

Go:   const PI = 3.14159
来源：http://kio.fehbvm.com

Ruby: PI = 3.14159
来源：http://fyi.gzhubu.top

C#:   const double PI = 3.14159;
来源：http://otn.shangyingyoupin.top

[A04] 判断变量类型
来源：http://arv.havefunace.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://awq.yanxiufei.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ahe.fehbvm.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://uzk.xuetiantiany.cn

TS:   typeof x; x instanceof Date
来源：http://pyj.xuanzx.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://qqg.wangdashe.top

Go:   reflect.TypeOf(x).Name()
来源：http://sgd.guannengcc.top

Ruby: x.class; x.is_a?(Integer)
来源：http://dsi.zhongyouzk.top

C#:   x.GetType().Name; x is int
来源：http://duj.iojbl.cn

[A05] 整数除法与取模
来源：http://jab.jlsjyb.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://qqa.yongpay.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ggu.yueranfly.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://nie.ivvv.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://jjg.yuxming.cn


<!-- 参考信息 -->