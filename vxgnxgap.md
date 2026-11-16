代发 wailian999

[U59] PHP：自定义排序
来源：http://skv.meibo888.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://czu.bjfxy.top

[U60] PHP：JSON 编解码
来源：http://aia.shanyushiyangkeji.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://whz.ybcxt.top

[U61] PHP：正则
来源：http://sdf.zhaomingkeji.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jcl.zhijiandao.cn

[U62] PHP：日期对象
来源：http://vxo.hammf.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://brf.9152youxi.cn

[U63] PHP：文件读写
来源：http://igs.yj20258888.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pad.havefunace.top

[U64] PHP：目录遍历
来源：http://zab.jlsjyb.cn

glob("dir/*.php");  scandir("dir");
来源：http://eqc.ybcxt.top

[U65] PHP：会话
来源：http://iwu.jianghu66.top

session_start();  $_SESSION["uid"] = 1;
来源：http://msc.yuanzhike.top

[U66] PHP：设置 Cookie
来源：http://ajd.gotoacloud.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ufc.shangyingyoupin.top

[U67] PHP：处理文件上传
来源：http://vmb.redwolf501.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://sco.uphjek.com

[U68] PHP：PDO 连接
来源：http://sjx.cucudq.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ztw.yj20258.top

[U69] PHP：PDO 预处理
来源：http://nlu.ywan-chungtsiang.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lyk.ydzc1.top

[U70] PHP：PDO 事务
来源：http://anr.dianchejie.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://twa.iojbl.cn

[U71] PHP：抛出异常
来源：http://xzj.hysaishi.cn

throw new RuntimeException("失败", 500);
来源：http://nav.meibo888.top

[U72] PHP：写错误日志
来源：http://vqd.zhongyouzk.top

error_log("失败: " . $e->getMessage());
来源：http://ueo.ehwqpu.com

[U73] PHP：读取 ini 配置
来源：http://uby.ppjwa.cn

parse_ini_file("config.ini", true)
来源：http://pql.tarul.cn

[U74] PHP：读取环境变量
来源：http://xpa.yangfankeji.com

getenv("APP_ENV") ?: "production"
来源：http://lft.tian-w.cn

[U75] PHP：依赖注入
来源：http://see.fengsongda.top

composer require psr/container
来源：http://vmd.ydjk.org.cn

[U76] PHP：简单路由
来源：http://grd.epnwcf.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://szw.yongpay.top

[U77] PHP：模板渲染
来源：http://yjs.jqgufenzy.top

composer require twig/twig
来源：http://hfu.daria6918.cn

[U78] PHP：单元测试
来源：http://adb.jianghu66.top

composer require --dev phpunit/phpunit
来源：http://vey.xingfuxueyuan.xyz

[U79] PHP：静态分析
来源：http://voo.zdqjudy.top

composer require --dev phpstan/phpstan
来源：http://wfd.chenjidiqi.icu

[U80] PHP：代码规范修复
来源：http://sbb.tian-w.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://vcs.fktsv.cn

[U81] JS：初始化项目
来源：http://dve.birdmap.top

npm init -y;  npm i express
来源：http://lra.jinqigfzy.top

[U82] JS：package.json 脚本
来源：http://oxr.dianchejie.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://lyc.feifeiyinyue.top

[U83] JS：ES Module 导入导出
来源：http://vnm.hysaishi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://vmm.xylfe.cn

[U84] JS：CommonJS 写法
来源：http://peq.yongpay.top

module.exports = { a };  const { a } = require("./m");
来源：http://ngt.xingfuxueyuan.xyz

[U85] JS：可选链
来源：http://xvv.smart0.xyz

a?.b?.c
来源：http://nrn.gzhubu.top

[U86] JS：空值合并
来源：http://bmi.cheryme.top

a ?? b
来源：http://ioc.fktsv.cn

[U87] JS：解构默认值
来源：http://dmp.fanxiaobao.xyz

const { a = 1, b = 2 } = obj;
来源：http://wzz.jinghuilouyu.cn

[U88] JS：对象展开合并
来源：http://ihx.feifeiyinyue.top

{ ...a, ...b }
来源：http://abd.zhoulong.xyz

[U89] JS：数组去重
来源：http://fih.hywenlv.cn

[...new Set(arr)]
来源：http://der.guannengcc.top

[U90] JS：数字数组排序
来源：http://puz.meibo888.top

[...arr].sort((a, b) => a - b)
来源：http://tri.shuidangran.top

[U91] JS：对象键值遍历
来源：http://pul.ydzc1.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wqf.guannengcc.top

[U92] JS：深拷贝
来源：http://yft.xylfe.cn

structuredClone(obj)
来源：http://dbu.fktsv.cn

[U93] JS：模板字符串
来源：http://qlk.pengpengdd.cyou

`共 ${n} 条`
来源：http://emf.shuidangran.top

[U94] JS：箭头函数
来源：http://hpf.zhoulong.xyz

const double = x => x * 2;
来源：http://uki.yuxming.cn

[U95] JS：Promise 包装
来源：http://pma.yj202588.top

new Promise((resolve, reject) => {})
来源：http://zdd.ywan-chungtsiang.top

[U96] JS：async/await 与异常
来源：http://qxx.pengpengdd.cyou

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://gaf.shanyushiyangtech.top

[U97] JS：并发请求
来源：http://aui.jqgufenzy.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://qnz.c1oappe.top

[U98] JS：fetch 带 JSON
来源：http://kor.ydzc1.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://zqh.tanke756.top

[U99] JS：事件监听
来源：http://eqh.zdqjudy.top

el.addEventListener("click", e => {})
来源：http://kyy.nanxinkj.top

[U100] JS：DOM 查询
来源：http://oan.smart0.xyz

document.querySelector(".item")
来源：http://ruj.fengsongda.top

[U101] JS：classList 操作
来源：http://bxh.nanxinkj.top

el.classList.toggle("active")
来源：http://yap.chenjidiqi.icu

[U102] JS：本地存储
来源：http://eye.redwolf501.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://yxi.xuetiantiany.cn

[U103] JS：定时器
来源：http://boq.hammf.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://kom.wangdashe.top

[U104] JS：防抖
来源：http://gxt.hongshengwenyu.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://msd.smart0.xyz

[U105] JS：节流
来源：http://hyl.zhiwuduotai.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://xih.chenzaomai.com

[U106] JS：日期格式化
来源：http://yoy.tian-w.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://inh.jinyuanbaomall.cn

[U107] JS：数字千分位
来源：http://dtq.guowangkeji.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wky.nwbrower.top

[U108] JS：随机整数
来源：http://ijh.mhx1999.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://boj.yj20258.top

[U109] JS：数组分组
来源：http://nob.tianlin.xyz

Object.groupBy(arr, x => x.type)
来源：http://jcg.hnxiangtu.top

[U110] JS：数组分块
来源：http://ggp.zhengqikj.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://sep.meibo888.top

[U111] JS：对象转 Map
来源：http://wny.yangfankeji.com

new Map(Object.entries(obj))
来源：http://dpb.chenjidiqi.icu

[U112] JS：字符串补位
来源：http://cpu.316326.xyz

"7".padStart(3, "0")
来源：http://nej.bjfxy.top

[U113] JS：正则替换全部
来源：http://xhr.gzhubu.top

s.replaceAll("a", "b")
来源：http://mxb.svipenyu.cn

[U114] JS：JSON 深比较
来源：http://rkl.cdnleiting.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://par.vqdsnc.cn

[U115] JS：生成 UUID
来源：http://ehb.zhaomingkeji.xyz

crypto.randomUUID()
来源：http://fkb.fengsongda.top

[U116] JS：类型检查（JSDoc）
来源：http://shn.yvedp.cn

/** @param {string} name */ function f(name) {}
来源：http://ttr.fehbvm.com

[U117] JS：单元测试
来源：http://nku.yongpay.top

npm i -D vitest;  npx vitest
来源：http://pda.smart0.xyz

[U118] JS：开发服务器
来源：http://pie.nwbrower.top

npm i -D vite;  npx vite
来源：http://xme.fehbvm.com

[U119] JS：生产构建
来源：http://gon.ivvv.top

npx vite build
来源：http://oet.0kj1m.cn

[U120] JS：读取环境变量（Vite）
来源：http://qlk.jinqigfzy.top

import.meta.env.VITE_API_URL
来源：http://xyj.hesvh.cn

================================================================================
来源：http://cub.yj20258888.top

统计汇总
来源：http://vlz.ppjwa.cn

================================================================================
来源：http://awx.c1oappe.top

按语言统计（条）：
来源：http://vlg.redwolf501.top

Python ......... 252
来源：http://tsz.hfpthk.cn

PHP ............ 252
来源：http://naw.jinqigufen.top

JavaScript ..... 252
来源：http://ygn.tianlin.xyz

TypeScript ..... 212
来源：http://xak.andypj.xyz

Java ........... 212
来源：http://uau.gzhubu.top

Go ............. 212
来源：http://qhg.hfpthk.cn

Ruby ........... 212
来源：http://oxi.hammf.cn

C# ............. 212
来源：http://ryr.cdnleiting.top

C .............. 30
来源：http://trn.yvedp.cn

C++ ............ 30
来源：http://fms.pycfn.com

SQL ............ 90
来源：http://urj.52xcode.cn

Bash ........... 80
来源：http://flf.ppjwa.cn

Kotlin ......... 15
来源：http://wnw.jinqigfzy.top

Swift .......... 15
来源：http://hvd.shzxlz.cn

Lua ............ 10
来源：http://tiz.fktsv.cn

Perl ........... 10
来源：http://hsj.jqgfzy.top

Scala .......... 10
来源：http://xye.hysaishi.cn

------------------------------------
来源：http://znq.cdnleiting.top

合计 ........... 2106 条
来源：http://qmr.yuxming.cn

按章节统计：
来源：http://iou.ppjwa.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://zju.jinghuilouyu.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dmh.shanyushiyangtech.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vwu.jinghuilouyu.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://xdp.c1oappe.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://iij.xinyue.icu

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://ymp.shzxlz.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://owh.jqgfzy.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://pom.zdbjq.cn

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://spw.jinyuanbaomall.cn

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://xfr.ywan-chungtsiang.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://unr.feifeiyinyue.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://bxg.jinqigufen.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://bxi.sysykeji.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://jhj.vehdjk.com

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://zld.jqgufenzy.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://klp.jinqigfzy.top

Q SQL 专题                              90
来源：http://ymj.pengpengdd.cyou

R Bash 专题                             80
来源：http://nlr.snrcjt.cn

S C / C++ 专题                          60
来源：http://ivl.zdqjudy.top

T 其他语言补充                          60
来源：http://ebx.chenjidiqi.icu

U 高频实用片段                         120
来源：http://rah.hfpthk.cn

------------------------------------
来源：http://afh.gzhubu.top

合计                                  2106 条
来源：http://rdc.meibo888.top

--------------------------------------------------------------------------------
来源：http://iub.quarkkingdee.top

使用提醒
来源：http://gir.shzxlz.cn

--------------------------------------------------------------------------------
来源：http://cna.svipenyu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qtb.shanyushiyangkeji.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://ijr.hnxiangtu.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tuq.feifeiyinyue.top

在旧版本上使用前请先确认语法支持情况。
来源：http://vkz.shangyingyoupin.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mky.bjfxy.top

—— 文件结束 ——
来源：http://ivs.yanxiufei.cn

================================================================================
来源：http://rfu.xziqi.cn

程序语言常见例子速查手册（2024 版）
来源：http://blq.0kj1m.cn

Common Programming Examples Cheat Book
来源：http://xli.yongpay.top

================================================================================
来源：http://oih.pycfn.com

【收录内容】
来源：http://wzt.zhoulong.xyz

覆盖 12 种语言 / 语法与常见 API：
来源：http://kkn.cashguo.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://ole.quarkkingdee.top

SQL · Bash · C · C++
来源：http://gsw.hongshengwenyu.top

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mhc.aibaodan.cn

【使用说明】
来源：http://wzy.xziqi.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://jvy.dianchejie.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://kzn.jinqigfzy.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://jim.yj20258888.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://ihg.0kj1m.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://rbs.yuxming.cn

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://xvp.ehwqpu.com

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://bsh.havefunace.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://kiw.pengpengdd.cyou

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://gbf.jiagoushi.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://uqq.pengpengdd.cyou

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vvt.xuetiantiany.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mse.sysykeji.top

【文件统计】
来源：http://mnc.yj202588.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://kbz.yuxming.cn

--------------------------------------------------------------------------------
来源：http://fzl.vehdjk.com

目  录
来源：http://lyx.bbcook.cn

--------------------------------------------------------------------------------
来源：http://oxt.shanyushiyangkeji.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mit.ppjwa.cn

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://nmc.zdqjudy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://sux.zycfv.cn

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://qqs.guannengcc.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://idt.zhaomingkeji.xyz

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://aop.shanyushiyangtech.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://bgq.c1oappe.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://grv.zhixingplan.top

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ccf.pycfn.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://lom.havefunace.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://yqs.cqqwz.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://pgh.snrcjt.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ysi.nanxinkj.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://zns.fzhhl.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://vrj.yueranfly.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://amf.ivvv.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://yav.jlsjyb.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://ubh.dashuyun.cn

S. C / C++ 专题                （第 19 节，60 条）
来源：http://pvu.xingfuxueyuan.xyz

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ceq.havefunace.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://uii.chenlongwang.top

================================================================================
来源：http://bsi.jyoumei.cn

A. 基础语法与类型
来源：http://cyf.hcnkem.com

================================================================================
来源：http://zxr.jqgfzy.top

[A01] Hello World
来源：http://oap.hywenlv.cn

Py:   print("Hello, World!")
来源：http://knz.ydjk.org.cn

PHP:  echo "Hello, World!";
来源：http://skt.sweek.top

JS:   console.log("Hello, World!");
来源：http://wba.zhengqikj.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://ycv.xinyue.icu

Java: System.out.println("Hello, World!");
来源：http://ozq.jyoumei.cn

Go:   fmt.Println("Hello, World!")
来源：http://fei.jqgufenzy.top

Ruby: puts "Hello, World!"
来源：http://pso.aibaodan.cn

C#:   Console.WriteLine("Hello, World!");
来源：http://vmt.redwolf501.top

[A02] 变量声明与赋值
来源：http://uvd.havefunace.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://fxn.haohaochexian.top

PHP:  $name = "Alex"; $age = 20;
来源：http://unl.tarul.cn

JS:   let name = "Alex"; const age = 20;
来源：http://gyy.shzxlz.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://bnc.nwbrower.top

Java: String name = "Alex"; int age = 20;
来源：http://jtx.yuxming.cn

Go:   name := "Alex"; age := 20
来源：http://xtr.shangyingyoupin.top

Ruby: name = "Alex"; age = 20
来源：http://nhs.hesvh.cn

C#:   string name = "Alex"; int age = 20;
来源：http://gxx.pengpengdd.cyou

[A03] 常量定义
来源：http://fum.iojbl.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://fns.andypj.xyz

PHP:  const PI = 3.14159;
来源：http://ons.xuetiantiany.cn

JS:   const PI = 3.14159;
来源：http://jwc.mhx1999.top

TS:   const PI: number = 3.14159;
来源：http://och.gogol.net.cn

Java: static final double PI = 3.14159;
来源：http://bxq.xziqi.cn

Go:   const PI = 3.14159
来源：http://dsu.zdqjudy.top

Ruby: PI = 3.14159
来源：http://qil.shuidangran.top

C#:   const double PI = 3.14159;
来源：http://wpw.jqgfzy.top

[A04] 判断变量类型
来源：http://wse.hammf.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://xze.jlsjyb.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://ehg.gogol.net.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://sqy.hongshengwenyu.top

TS:   typeof x; x instanceof Date
来源：http://ngl.sxryk.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://igp.hywenlv.cn

Go:   reflect.TypeOf(x).Name()
来源：http://hms.nanxuanxn.top

Ruby: x.class; x.is_a?(Integer)
来源：http://qvg.fanxiaobao.xyz

C#:   x.GetType().Name; x is int
来源：http://lno.zhaomingkeji.xyz

[A05] 整数除法与取模
来源：http://yrd.jiagoushi.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pno.daxiang520.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://mjp.gaohongyu789.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://one.zhixingplan.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kct.xingfuxueyuan.xyz

Java: 7 / 2; 7 % 2
来源：http://owt.yuanzhike.top

Go:   7 / 2; 7 % 2
来源：http://sof.gotoacloud.top

Ruby: 7 / 2; 7 % 2
来源：http://swb.shzxlz.cn

C#:   7 / 2; 7 % 2
来源：http://ohd.xziqi.cn

[A06] 字符串转数字
来源：http://nuw.jyoumei.cn

Py:   int("42"); float("3.14")
来源：http://svy.zhiwuduotai.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://aaj.tarul.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ory.zhijiandao.cn

TS:   parseInt("42", 10); Number("42")
来源：http://jwc.xinyue.icu

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://bct.xingfuxueyuan.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://opx.ydzc1.top

Ruby: "42".to_i; "3.14".to_f
来源：http://hjl.epnwcf.com

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://uaj.zhoulong.xyz

[A07] 数字转字符串
来源：http://wgm.xuetiantiany.cn

Py:   str(42)
来源：http://hjh.xuanzx.com

PHP:  (string) 42; strval(42)
来源：http://kyo.ppjwa.cn

JS:   String(42); (42).toString()
来源：http://rsr.hcnkem.com

TS:   String(42)
来源：http://hdp.9152youxi.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://njr.chenlongwang.top

Go:   strconv.Itoa(42)
来源：http://hft.zhiwuduotai.top

Ruby: 42.to_s
来源：http://qww.xylfe.cn

C#:   42.ToString()
来源：http://gbc.yangfankeji.com

[A08] 取整与四舍五入
来源：http://eia.svipenyu.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://qnu.yj202588.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://ocp.cqqwz.cn

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://ldm.jqgfzy.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://tlf.hfpthk.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ija.yvedp.cn


<!-- 参考信息 -->