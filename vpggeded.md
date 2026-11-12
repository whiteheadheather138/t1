代发 wailian999

[U59] PHP：自定义排序
来源：http://mli.vqdsnc.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://djc.fengsongda.top

[U60] PHP：JSON 编解码
来源：http://mqm.chenjidiqi.icu

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rsh.nwbrower.top

[U61] PHP：正则
来源：http://ojz.epnwcf.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://quq.sysykeji.top

[U62] PHP：日期对象
来源：http://lzn.tianlin.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cpm.zhengqikj.top

[U63] PHP：文件读写
来源：http://vcr.9152youxi.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jsb.shuidangran.top

[U64] PHP：目录遍历
来源：http://ugr.uphjek.com

glob("dir/*.php");  scandir("dir");
来源：http://hsz.redwolf501.top

[U65] PHP：会话
来源：http://icb.jlsjyb.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://tze.feifeiyinyue.top

[U66] PHP：设置 Cookie
来源：http://bik.sjlbkw.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qie.zhijiandao.cn

[U67] PHP：处理文件上传
来源：http://gwx.yj20258888.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://juu.fengsongda.top

[U68] PHP：PDO 连接
来源：http://rkc.aibaodan.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xsf.epnwcf.com

[U69] PHP：PDO 预处理
来源：http://kkc.nwbrower.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zxe.fktsv.cn

[U70] PHP：PDO 事务
来源：http://ews.zhengqikj.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wgd.316326.xyz

[U71] PHP：抛出异常
来源：http://axn.yongpay.top

throw new RuntimeException("失败", 500);
来源：http://cya.cheryme.top

[U72] PHP：写错误日志
来源：http://tbd.gzhubu.top

error_log("失败: " . $e->getMessage());
来源：http://piw.cqqwz.cn

[U73] PHP：读取 ini 配置
来源：http://eqw.yj202588.top

parse_ini_file("config.ini", true)
来源：http://aoh.yuxming.cn

[U74] PHP：读取环境变量
来源：http://dpn.zhongyouzk.top

getenv("APP_ENV") ?: "production"
来源：http://kfd.shzxlz.cn

[U75] PHP：依赖注入
来源：http://dut.yangfankeji.com

composer require psr/container
来源：http://bxc.vehdjk.com

[U76] PHP：简单路由
来源：http://ehn.jiagoushi.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bwv.vqdsnc.cn

[U77] PHP：模板渲染
来源：http://ejf.c1oappe.top

composer require twig/twig
来源：http://sqp.zhaomingkeji.xyz

[U78] PHP：单元测试
来源：http://ayg.fehbvm.com

composer require --dev phpunit/phpunit
来源：http://dor.redwolf501.top

[U79] PHP：静态分析
来源：http://npq.mhx1999.top

composer require --dev phpstan/phpstan
来源：http://qcq.guannengcc.top

[U80] PHP：代码规范修复
来源：http://qmt.chenjidiqi.icu

composer require --dev friendsofphp/php-cs-fixer
来源：http://aho.epnwcf.com

[U81] JS：初始化项目
来源：http://obl.jianghu66.top

npm init -y;  npm i express
来源：http://blz.jlsjyb.cn

[U82] JS：package.json 脚本
来源：http://wfw.tian-w.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bvc.sweek.top

[U83] JS：ES Module 导入导出
来源：http://wrc.epnwcf.com

export const a = 1;  import { a } from "./m.js";
来源：http://hmz.zhixingplan.top

[U84] JS：CommonJS 写法
来源：http://jpv.yangfankeji.com

module.exports = { a };  const { a } = require("./m");
来源：http://prb.zhijiandao.cn

[U85] JS：可选链
来源：http://iea.sjlbkw.cn

a?.b?.c
来源：http://gtk.uphjek.com

[U86] JS：空值合并
来源：http://ajb.fengsongda.top

a ?? b
来源：http://whu.zhaomingkeji.xyz

[U87] JS：解构默认值
来源：http://okr.ehwqpu.com

const { a = 1, b = 2 } = obj;
来源：http://ryc.gotoacloud.top

[U88] JS：对象展开合并
来源：http://hyz.nwbrower.top

{ ...a, ...b }
来源：http://nnm.gaohongyu789.top

[U89] JS：数组去重
来源：http://jiw.yueranfly.top

[...new Set(arr)]
来源：http://ptf.zycfv.cn

[U90] JS：数字数组排序
来源：http://dej.cdnleiting.top

[...arr].sort((a, b) => a - b)
来源：http://xci.chenzaomai.com

[U91] JS：对象键值遍历
来源：http://gfx.nanxinkj.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://ulj.hcnkem.com

[U92] JS：深拷贝
来源：http://grc.hcnkem.com

structuredClone(obj)
来源：http://dlc.wangdashe.top

[U93] JS：模板字符串
来源：http://tnw.fanxiaobao.xyz

`共 ${n} 条`
来源：http://wzl.guowangkeji.top

[U94] JS：箭头函数
来源：http://reu.quarkkingdee.top

const double = x => x * 2;
来源：http://sbp.fktsv.cn

[U95] JS：Promise 包装
来源：http://xgw.chenjidiqi.icu

new Promise((resolve, reject) => {})
来源：http://htt.sxryk.cn

[U96] JS：async/await 与异常
来源：http://gdr.xingfuxueyuan.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://oqo.andypj.xyz

[U97] JS：并发请求
来源：http://qjc.fehbvm.com

await Promise.all(urls.map(u => fetch(u)))
来源：http://dkz.havefunace.top

[U98] JS：fetch 带 JSON
来源：http://igg.quarkkingdee.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://bqd.hcnkem.com

[U99] JS：事件监听
来源：http://quh.vqdsnc.cn

el.addEventListener("click", e => {})
来源：http://tcu.shangyingyoupin.top

[U100] JS：DOM 查询
来源：http://gyk.yj20258.top

document.querySelector(".item")
来源：http://dnb.chenjidiqi.icu

[U101] JS：classList 操作
来源：http://hyp.feifeiyinyue.top

el.classList.toggle("active")
来源：http://cyv.wangdashe.top

[U102] JS：本地存储
来源：http://pyb.bjfxy.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ymm.bjfxy.top

[U103] JS：定时器
来源：http://avz.jinghuilouyu.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://vbt.316326.xyz

[U104] JS：防抖
来源：http://zja.tanke756.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pnm.cqqwz.cn

[U105] JS：节流
来源：http://aou.zdbjq.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://ltu.fzhhl.top

[U106] JS：日期格式化
来源：http://kvo.yj202588.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://bjs.0kj1m.cn

[U107] JS：数字千分位
来源：http://zja.jlsjyb.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://bue.sweek.top

[U108] JS：随机整数
来源：http://etz.316326.xyz

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://vpd.zdbjq.cn

[U109] JS：数组分组
来源：http://eps.yueranfly.top

Object.groupBy(arr, x => x.type)
来源：http://kmu.zdqjudy.top

[U110] JS：数组分块
来源：http://btv.hcnkem.com

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://prv.zdbjq.cn

[U111] JS：对象转 Map
来源：http://uzx.andypj.xyz

new Map(Object.entries(obj))
来源：http://aev.shangyingyoupin.top

[U112] JS：字符串补位
来源：http://kca.vehdjk.com

"7".padStart(3, "0")
来源：http://lkv.fehbvm.com

[U113] JS：正则替换全部
来源：http://ppn.quarkkingdee.top

s.replaceAll("a", "b")
来源：http://vmz.shzxlz.cn

[U114] JS：JSON 深比较
来源：http://xba.yuxming.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://lpe.gaohongyu789.top

[U115] JS：生成 UUID
来源：http://qtg.zhiwuduotai.top

crypto.randomUUID()
来源：http://fvt.tarul.cn

[U116] JS：类型检查（JSDoc）
来源：http://ead.hnqzz.top

/** @param {string} name */ function f(name) {}
来源：http://lmx.xylfe.cn

[U117] JS：单元测试
来源：http://iio.yj202588.top

npm i -D vitest;  npx vitest
来源：http://ffq.chenjidiqi.icu

[U118] JS：开发服务器
来源：http://ksd.yonumen.top

npm i -D vite;  npx vite
来源：http://wye.cucudq.cn

[U119] JS：生产构建
来源：http://tkx.birdmap.top

npx vite build
来源：http://vzq.316326.xyz

[U120] JS：读取环境变量（Vite）
来源：http://uge.sjlbkw.cn

import.meta.env.VITE_API_URL
来源：http://ytp.nanxinkj.top

================================================================================
来源：http://scn.yueranfly.top

统计汇总
来源：http://jku.ydjk.org.cn

================================================================================
来源：http://hcj.xinyue.icu

按语言统计（条）：
来源：http://zna.yj20258.top

Python ......... 252
来源：http://npq.iojbl.cn

PHP ............ 252
来源：http://ryv.shanyushiyangtech.top

JavaScript ..... 252
来源：http://oci.smart0.xyz

TypeScript ..... 212
来源：http://wbf.c1oappe.top

Java ........... 212
来源：http://chc.smart0.xyz

Go ............. 212
来源：http://ewz.yueranfly.top

Ruby ........... 212
来源：http://veo.dashuyun.cn

C# ............. 212
来源：http://ifb.daria6918.cn

C .............. 30
来源：http://sjq.xylfe.cn

C++ ............ 30
来源：http://dfe.wangshuangyany.cn

SQL ............ 90
来源：http://ayu.haohaochexian.top

Bash ........... 80
来源：http://yta.yangfankeji.com

Kotlin ......... 15
来源：http://mtt.zhengqikj.top

Swift .......... 15
来源：http://jdc.chenlongwang.top

Lua ............ 10
来源：http://qae.tian-w.cn

Perl ........... 10
来源：http://ipd.gotoacloud.top

Scala .......... 10
来源：http://syx.jqgfzy.top

------------------------------------
来源：http://dac.hywenlv.cn

合计 ........... 2106 条
来源：http://ord.ctjpmb.com

按章节统计：
来源：http://snc.yuxming.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mzr.meibo888.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://byu.wangshuangyany.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://soi.cucudq.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://kgt.chenzaomai.com

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://xxp.yj20258.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://rfp.bjfxy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://aaw.cucudq.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://isj.pycfn.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://tag.sjlbkw.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://dpq.tanke756.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://rbe.feifeiyinyue.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://sex.jinqigfzy.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://hpy.wangshuangyany.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qou.ivvv.top

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mvr.fktsv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://ypw.yj202588.top

Q SQL 专题                              90
来源：http://fwm.ydzc1.top

R Bash 专题                             80
来源：http://hdd.xziqi.cn

S C / C++ 专题                          60
来源：http://mhi.wangdashe.top

T 其他语言补充                          60
来源：http://wdw.shzxlz.cn

U 高频实用片段                         120
来源：http://hef.jinghuilouyu.cn

------------------------------------
来源：http://xhu.sweek.top

合计                                  2106 条
来源：http://ghu.dashuyun.cn

--------------------------------------------------------------------------------
来源：http://tga.yuxming.cn

使用提醒
来源：http://ypk.ydjk.org.cn

--------------------------------------------------------------------------------
来源：http://tev.jinghuilouyu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://hjg.sufxvd.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ffy.epnwcf.com

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://clx.yongpay.top

在旧版本上使用前请先确认语法支持情况。
来源：http://lvx.ehwqpu.com

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ytk.sysykeji.top

—— 文件结束 ——
来源：http://otx.jlsjyb.cn

================================================================================
来源：http://qag.shzxlz.cn

程序语言常见例子速查手册（2024 版）
来源：http://yhf.zycfv.cn

Common Programming Examples Cheat Book
来源：http://fku.yonumen.top

================================================================================
来源：http://edj.shanyushiyangtech.top

【收录内容】
来源：http://pzo.yangfankeji.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://zpx.feifeiyinyue.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://dvv.bbcook.cn

SQL · Bash · C · C++
来源：http://fwn.zhixingplan.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://zih.hnxiangtu.top

【使用说明】
来源：http://qim.zhijiandao.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ckm.jiagoushi.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mds.yueranfly.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://uqc.gaohongyu789.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://gph.sjlbkw.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://iuo.zhengqikj.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://clp.gotoacloud.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://eau.ydzc1.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://war.birdmap.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wcv.gaohongyu789.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://bzl.guowangkeji.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yww.birdmap.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zsm.pengpengdd.cyou

【文件统计】
来源：http://mne.snrcjt.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://tdz.zhengqikj.top

--------------------------------------------------------------------------------
来源：http://qfp.yangfankeji.com

目  录
来源：http://kje.nanxinkj.top

--------------------------------------------------------------------------------
来源：http://svm.cheryme.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://puc.9152youxi.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://qar.sjlbkw.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qie.tianlin.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://xsz.ivvv.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://yyb.316326.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://rtk.316326.xyz

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://obb.jyoumei.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://hof.hnxiangtu.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://hwd.9152youxi.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cwy.jinghuilouyu.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://coh.316326.xyz

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://iub.iojbl.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://bjc.fzhhl.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://gmo.fengsongda.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ofg.hywenlv.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://kkn.pengpengdd.cyou

Q. SQL 专题                    （第 17 节，90 条）
来源：http://nzx.sufxvd.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xpq.yonumen.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://dgq.sweek.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://bqk.ppjwa.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://scu.zhongyouzk.top

================================================================================
来源：http://ycv.xziqi.cn

A. 基础语法与类型
来源：http://gac.fzhhl.top

================================================================================
来源：http://vfo.cdnleiting.top

[A01] Hello World
来源：http://oxh.wangshuangyany.cn

Py:   print("Hello, World!")
来源：http://xzb.fzhhl.top

PHP:  echo "Hello, World!";
来源：http://xzm.havefunace.top

JS:   console.log("Hello, World!");
来源：http://pqr.guowangkeji.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://vqp.hcnkem.com

Java: System.out.println("Hello, World!");
来源：http://xvu.birdmap.top

Go:   fmt.Println("Hello, World!")
来源：http://fpj.ywan-chungtsiang.top

Ruby: puts "Hello, World!"
来源：http://nne.nanxinkj.top

C#:   Console.WriteLine("Hello, World!");
来源：http://gjt.yanxiufei.cn

[A02] 变量声明与赋值
来源：http://rld.zhoulong.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zqc.daria6918.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://kvk.dianchejie.cn

JS:   let name = "Alex"; const age = 20;
来源：http://jit.9152youxi.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gzz.havefunace.top

Java: String name = "Alex"; int age = 20;
来源：http://wvj.jiagoushi.top

Go:   name := "Alex"; age := 20
来源：http://def.zhijiandao.cn

Ruby: name = "Alex"; age = 20
来源：http://qtd.hongshengwenyu.top

C#:   string name = "Alex"; int age = 20;
来源：http://hrx.fehbvm.com

[A03] 常量定义
来源：http://ntx.yuxming.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://tun.zdqjudy.top

PHP:  const PI = 3.14159;
来源：http://oit.9152youxi.cn

JS:   const PI = 3.14159;
来源：http://hed.xylfe.cn

TS:   const PI: number = 3.14159;
来源：http://rmb.zdbjq.cn

Java: static final double PI = 3.14159;
来源：http://xez.hnqzz.top

Go:   const PI = 3.14159
来源：http://lki.xuanzx.com

Ruby: PI = 3.14159
来源：http://aab.ctjpmb.com

C#:   const double PI = 3.14159;
来源：http://das.haohaochexian.top

[A04] 判断变量类型
来源：http://sqt.jqgfzy.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://vzp.hnqzz.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://jbz.c1oappe.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nim.yfazqb.com

TS:   typeof x; x instanceof Date
来源：http://exr.9152youxi.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ddo.ydjk.org.cn

Go:   reflect.TypeOf(x).Name()
来源：http://ffq.meibo888.top

Ruby: x.class; x.is_a?(Integer)
来源：http://lvq.jyoumei.cn

C#:   x.GetType().Name; x is int
来源：http://heb.uphjek.com

[A05] 整数除法与取模
来源：http://oki.jiagoushi.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://jwi.birdmap.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ref.sweek.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://eaj.zhixingplan.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wbs.shanyushiyangkeji.top

Java: 7 / 2; 7 % 2
来源：http://tfw.jianghu66.top

Go:   7 / 2; 7 % 2
来源：http://piv.ywan-chungtsiang.top

Ruby: 7 / 2; 7 % 2
来源：http://bzb.jinqigfzy.top

C#:   7 / 2; 7 % 2
来源：http://bwe.ydjk.org.cn

[A06] 字符串转数字
来源：http://dts.ydjk.org.cn

Py:   int("42"); float("3.14")
来源：http://opr.redwolf501.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://sev.yongpay.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://oyu.xinyue.icu

TS:   parseInt("42", 10); Number("42")
来源：http://cyt.fktsv.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://ewb.zhaomingkeji.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://auv.ydjk.org.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://bcb.chenjidiqi.icu

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://jxv.hfpthk.cn

[A07] 数字转字符串
来源：http://vtk.pycfn.com

Py:   str(42)
来源：http://tjr.yvedp.cn

PHP:  (string) 42; strval(42)
来源：http://wth.fzhhl.top

JS:   String(42); (42).toString()
来源：http://hob.9152youxi.cn

TS:   String(42)
来源：http://eqs.daria6918.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://qau.9152youxi.cn

Go:   strconv.Itoa(42)
来源：http://nmu.chenjidiqi.icu

Ruby: 42.to_s
来源：http://ahb.jyoumei.cn

C#:   42.ToString()
来源：http://hsp.pengpengdd.cyou

[A08] 取整与四舍五入
来源：http://pql.0kj1m.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://okv.xingfuxueyuan.xyz

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://tpj.cashguo.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://xft.316326.xyz

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://isk.jiagoushi.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://oth.fanxiaobao.xyz


<!-- 参考信息 -->