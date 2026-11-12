代发 wailian999

[U55] PHP：match 表达式
来源：http://srz.ywan-chungtsiang.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zwy.tanke756.top

[U56] PHP：命名参数
来源：http://jpm.dianchejie.cn

f(a: 1, b: 2)
来源：http://swq.hnxiangtu.top

[U57] PHP：字符串插值
来源：http://ouy.feifeiyinyue.top

"值: {$a}"
来源：http://pts.jqgufenzy.top

[U58] PHP：数组三件套
来源：http://ssk.svipenyu.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://iln.chenzaomai.com

[U59] PHP：自定义排序
来源：http://inq.yonumen.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ixo.mhx1999.top

[U60] PHP：JSON 编解码
来源：http://tvb.bjfxy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://juq.316326.xyz

[U61] PHP：正则
来源：http://mne.ehwqpu.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wid.chenjidiqi.icu

[U62] PHP：日期对象
来源：http://ckp.9152youxi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fts.yuanzhike.top

[U63] PHP：文件读写
来源：http://rik.ydjk.org.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://set.ywan-chungtsiang.top

[U64] PHP：目录遍历
来源：http://bjs.uphjek.com

glob("dir/*.php");  scandir("dir");
来源：http://bkq.nwbrower.top

[U65] PHP：会话
来源：http://twa.hcnkem.com

session_start();  $_SESSION["uid"] = 1;
来源：http://hit.fktsv.cn

[U66] PHP：设置 Cookie
来源：http://otq.vehdjk.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vay.zhiwuduotai.top

[U67] PHP：处理文件上传
来源：http://cfp.svipenyu.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://iel.ivvv.top

[U68] PHP：PDO 连接
来源：http://rsa.birdmap.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ozx.sjlbkw.cn

[U69] PHP：PDO 预处理
来源：http://rwk.shanyushiyangkeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xqd.316326.xyz

[U70] PHP：PDO 事务
来源：http://acu.aibaodan.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ljw.fanxiaobao.xyz

[U71] PHP：抛出异常
来源：http://owe.xuanzx.com

throw new RuntimeException("失败", 500);
来源：http://bvf.hongshengwenyu.top

[U72] PHP：写错误日志
来源：http://dha.hesvh.cn

error_log("失败: " . $e->getMessage());
来源：http://jml.smart0.xyz

[U73] PHP：读取 ini 配置
来源：http://pjy.bjfxy.top

parse_ini_file("config.ini", true)
来源：http://jlj.guowangkeji.top

[U74] PHP：读取环境变量
来源：http://jpa.ivvv.top

getenv("APP_ENV") ?: "production"
来源：http://kdf.iojbl.cn

[U75] PHP：依赖注入
来源：http://wvo.fanxiaobao.xyz

composer require psr/container
来源：http://wcm.52xcode.cn

[U76] PHP：简单路由
来源：http://kcx.52xcode.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cbj.kuanghao11.cn

[U77] PHP：模板渲染
来源：http://fud.smart0.xyz

composer require twig/twig
来源：http://zpx.xingfuxueyuan.xyz

[U78] PHP：单元测试
来源：http://kni.yj20258888.top

composer require --dev phpunit/phpunit
来源：http://ttk.ydjk.org.cn

[U79] PHP：静态分析
来源：http://nar.yvedp.cn

composer require --dev phpstan/phpstan
来源：http://yvg.zdqjudy.top

[U80] PHP：代码规范修复
来源：http://rhn.cucudq.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://jej.zhaomingkeji.xyz

[U81] JS：初始化项目
来源：http://wrw.andypj.xyz

npm init -y;  npm i express
来源：http://rnk.fehbvm.com

[U82] JS：package.json 脚本
来源：http://pbo.sufxvd.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ckt.fanxiaobao.xyz

[U83] JS：ES Module 导入导出
来源：http://pcr.nanxuanxn.top

export const a = 1;  import { a } from "./m.js";
来源：http://odo.sweek.top

[U84] JS：CommonJS 写法
来源：http://cjv.zhaomingkeji.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://kvw.haohaochexian.top

[U85] JS：可选链
来源：http://ulx.gzhubu.top

a?.b?.c
来源：http://moh.iojbl.cn

[U86] JS：空值合并
来源：http://zbt.fengsongda.top

a ?? b
来源：http://aef.cucudq.cn

[U87] JS：解构默认值
来源：http://xbu.zdqjudy.top

const { a = 1, b = 2 } = obj;
来源：http://qes.hesvh.cn

[U88] JS：对象展开合并
来源：http://byg.sufxvd.cn

{ ...a, ...b }
来源：http://ivd.jinyuanbaomall.cn

[U89] JS：数组去重
来源：http://gwo.jianghu66.top

[...new Set(arr)]
来源：http://exo.aibaodan.cn

[U90] JS：数字数组排序
来源：http://mmn.vehdjk.com

[...arr].sort((a, b) => a - b)
来源：http://byd.cdnleiting.top

[U91] JS：对象键值遍历
来源：http://esd.fzhhl.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://qvp.yongpay.top

[U92] JS：深拷贝
来源：http://fbg.snrcjt.cn

structuredClone(obj)
来源：http://onn.yfazqb.com

[U93] JS：模板字符串
来源：http://aph.316326.xyz

`共 ${n} 条`
来源：http://rzz.zdbjq.cn

[U94] JS：箭头函数
来源：http://iqn.yuxming.cn

const double = x => x * 2;
来源：http://jhj.fengsongda.top

[U95] JS：Promise 包装
来源：http://yxh.hcnkem.com

new Promise((resolve, reject) => {})
来源：http://xnw.tarul.cn

[U96] JS：async/await 与异常
来源：http://cak.xingfuxueyuan.xyz

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xlp.meibo888.top

[U97] JS：并发请求
来源：http://hbj.vqdsnc.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://nge.shanyushiyangtech.top

[U98] JS：fetch 带 JSON
来源：http://gnv.guowangkeji.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://avy.hongshengwenyu.top

[U99] JS：事件监听
来源：http://tdf.aibaodan.cn

el.addEventListener("click", e => {})
来源：http://gxh.sysykeji.top

[U100] JS：DOM 查询
来源：http://nhj.pycfn.com

document.querySelector(".item")
来源：http://ryo.cheryme.top

[U101] JS：classList 操作
来源：http://xla.xylfe.cn

el.classList.toggle("active")
来源：http://qoy.jqgufenzy.top

[U102] JS：本地存储
来源：http://wyn.wangdashe.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://sct.shzxlz.cn

[U103] JS：定时器
来源：http://xnc.yanxiufei.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://knq.cheryme.top

[U104] JS：防抖
来源：http://mme.zhongyouzk.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wxo.9152youxi.cn

[U105] JS：节流
来源：http://ask.yvedp.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wqo.xingfuxueyuan.xyz

[U106] JS：日期格式化
来源：http://rlp.tianlin.xyz

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://nkl.pycfn.com

[U107] JS：数字千分位
来源：http://hrv.hfpthk.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://adq.bbcook.cn

[U108] JS：随机整数
来源：http://xuf.nanxinkj.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://dqf.fengsongda.top

[U109] JS：数组分组
来源：http://mep.yj20258888.top

Object.groupBy(arr, x => x.type)
来源：http://vfn.nwbrower.top

[U110] JS：数组分块
来源：http://kdd.yvedp.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://yqu.kuanghao11.cn

[U111] JS：对象转 Map
来源：http://rke.fzhhl.top

new Map(Object.entries(obj))
来源：http://bhh.tarul.cn

[U112] JS：字符串补位
来源：http://jmt.zdqjudy.top

"7".padStart(3, "0")
来源：http://vdx.sjlbkw.cn

[U113] JS：正则替换全部
来源：http://ooi.redwolf501.top

s.replaceAll("a", "b")
来源：http://ykz.hywenlv.cn

[U114] JS：JSON 深比较
来源：http://jcm.dashuyun.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://uqx.ivvv.top

[U115] JS：生成 UUID
来源：http://aqx.zhaomingkeji.xyz

crypto.randomUUID()
来源：http://xmu.cashguo.top

[U116] JS：类型检查（JSDoc）
来源：http://tor.sysykeji.top

/** @param {string} name */ function f(name) {}
来源：http://ejb.sxryk.cn

[U117] JS：单元测试
来源：http://bje.xylfe.cn

npm i -D vitest;  npx vitest
来源：http://npq.wangdashe.top

[U118] JS：开发服务器
来源：http://eev.tarul.cn

npm i -D vite;  npx vite
来源：http://sgn.fengsongda.top

[U119] JS：生产构建
来源：http://hrk.jlsjyb.cn

npx vite build
来源：http://xyb.jlsjyb.cn

[U120] JS：读取环境变量（Vite）
来源：http://ojd.yongpay.top

import.meta.env.VITE_API_URL
来源：http://are.shuidangran.top

================================================================================
来源：http://uyl.xuetiantiany.cn

统计汇总
来源：http://ubo.pengpengdd.cyou

================================================================================
来源：http://whf.shanyushiyangkeji.top

按语言统计（条）：
来源：http://eww.jlsjyb.cn

Python ......... 252
来源：http://foc.aizwys.cn

PHP ............ 252
来源：http://zoz.yonumen.top

JavaScript ..... 252
来源：http://qli.jqgufenzy.top

TypeScript ..... 212
来源：http://icp.tanke756.top

Java ........... 212
来源：http://wiu.chenzaomai.com

Go ............. 212
来源：http://bdi.daria6918.cn

Ruby ........... 212
来源：http://ykd.quarkkingdee.top

C# ............. 212
来源：http://wrx.ppjwa.cn

C .............. 30
来源：http://ilu.zhiwuduotai.top

C++ ............ 30
来源：http://ifn.xuanzx.com

SQL ............ 90
来源：http://irh.vehdjk.com

Bash ........... 80
来源：http://kfe.yfazqb.com

Kotlin ......... 15
来源：http://jsy.guowangkeji.top

Swift .......... 15
来源：http://yzy.zycfv.cn

Lua ............ 10
来源：http://phm.daria6918.cn

Perl ........... 10
来源：http://qtu.yuxming.cn

Scala .......... 10
来源：http://jun.pengpengdd.cyou

------------------------------------
来源：http://yyp.kuanghao11.cn

合计 ........... 2106 条
来源：http://blj.9152youxi.cn

按章节统计：
来源：http://rfa.cucudq.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mza.sysykeji.top

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://bjy.yonumen.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://vqe.9152youxi.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://npm.sysykeji.top

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://grg.fzhhl.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sqa.feifeiyinyue.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://cyo.kuanghao11.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://kcs.vehdjk.com

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://jze.xingfuxueyuan.xyz

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rix.yuxming.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://kaj.cucudq.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fkj.yangfankeji.com

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://xkt.yj202588.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://dgv.cqqwz.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://gbg.jinyuanbaomall.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://sbv.zdqjudy.top

Q SQL 专题                              90
来源：http://umt.vehdjk.com

R Bash 专题                             80
来源：http://xke.snrcjt.cn

S C / C++ 专题                          60
来源：http://bxf.gotoacloud.top

T 其他语言补充                          60
来源：http://otc.shanyushiyangtech.top

U 高频实用片段                         120
来源：http://myc.mhx1999.top

------------------------------------
来源：http://wkv.fehbvm.com

合计                                  2106 条
来源：http://kqj.0kj1m.cn

--------------------------------------------------------------------------------
来源：http://fea.shanyushiyangkeji.top

使用提醒
来源：http://vig.shanyushiyangkeji.top

--------------------------------------------------------------------------------
来源：http://vfk.52xcode.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://fkh.svipenyu.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://fes.zhaomingkeji.xyz

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://neo.gogol.net.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://bot.yj20258.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://cie.yanxiufei.cn

—— 文件结束 ——
来源：http://mig.ydjk.org.cn

================================================================================
来源：http://pgk.0kj1m.cn

程序语言常见例子速查手册（2024 版）
来源：http://xnf.zdqjudy.top

Common Programming Examples Cheat Book
来源：http://ene.chenzaomai.com

================================================================================
来源：http://gxc.jyoumei.cn

【收录内容】
来源：http://zwl.yuxming.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://jsf.bjfxy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://klc.jlsjyb.cn

SQL · Bash · C · C++
来源：http://vnd.sjlbkw.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://evk.hysaishi.cn

【使用说明】
来源：http://qbj.zdbjq.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ocx.9152youxi.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://gmx.316326.xyz

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://nds.cdnleiting.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://azt.svipenyu.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://rkz.yfazqb.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ija.cqqwz.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://qfv.zdqjudy.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://rmf.wangdashe.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://oyu.xuanzx.com

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://ubk.shanyushiyangkeji.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://nxu.hysaishi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://ymn.xylfe.cn

【文件统计】
来源：http://rrv.xinyue.icu

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://iaf.sufxvd.cn

--------------------------------------------------------------------------------
来源：http://wam.hysaishi.cn

目  录
来源：http://gee.zhoulong.xyz

--------------------------------------------------------------------------------
来源：http://ivu.havefunace.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://pwq.jqgufenzy.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://pjj.shanyushiyangkeji.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zia.zhengqikj.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://npc.aizwys.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://lfr.chenzaomai.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wgx.uphjek.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://paq.ydzc1.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://nrr.vqdsnc.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://fzk.nwbrower.top

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xuo.jinqigufen.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wcm.hfpthk.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://rro.snrcjt.cn

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://gch.bbcook.cn

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://kal.hcnkem.com

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://apq.zdbjq.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://ncm.jinghuilouyu.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kfs.sysykeji.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://pmm.xingfuxueyuan.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://rtb.fktsv.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://gkh.nanxinkj.top

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mes.mhx1999.top

================================================================================
来源：http://axd.fengsongda.top

A. 基础语法与类型
来源：http://pan.hnxiangtu.top

================================================================================
来源：http://cxg.ehwqpu.com

[A01] Hello World
来源：http://wlu.yvedp.cn

Py:   print("Hello, World!")
来源：http://yns.yonumen.top

PHP:  echo "Hello, World!";
来源：http://szh.hywenlv.cn

JS:   console.log("Hello, World!");
来源：http://mlk.ctjpmb.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://uot.sufxvd.cn

Java: System.out.println("Hello, World!");
来源：http://rnu.havefunace.top

Go:   fmt.Println("Hello, World!")
来源：http://ozh.hcnkem.com

Ruby: puts "Hello, World!"
来源：http://dxz.zhixingplan.top

C#:   Console.WriteLine("Hello, World!");
来源：http://chf.zdbjq.cn

[A02] 变量声明与赋值
来源：http://pzf.ppjwa.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://rri.sjlbkw.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://usw.yfazqb.com

JS:   let name = "Alex"; const age = 20;
来源：http://pom.chenlongwang.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://kys.hfpthk.cn

Java: String name = "Alex"; int age = 20;
来源：http://mki.jlsjyb.cn

Go:   name := "Alex"; age := 20
来源：http://vnd.bbcook.cn

Ruby: name = "Alex"; age = 20
来源：http://hnw.aibaodan.cn

C#:   string name = "Alex"; int age = 20;
来源：http://fac.shzxlz.cn

[A03] 常量定义
来源：http://mzw.tianlin.xyz

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://nuc.cucudq.cn

PHP:  const PI = 3.14159;
来源：http://ais.aizwys.cn

JS:   const PI = 3.14159;
来源：http://xna.tarul.cn

TS:   const PI: number = 3.14159;
来源：http://nyt.xuanzx.com

Java: static final double PI = 3.14159;
来源：http://pyi.tian-w.cn

Go:   const PI = 3.14159
来源：http://cwu.bjfxy.top

Ruby: PI = 3.14159
来源：http://dit.fanxiaobao.xyz

C#:   const double PI = 3.14159;
来源：http://xmy.smart0.xyz

[A04] 判断变量类型
来源：http://twg.cucudq.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://ani.zhoulong.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://bet.gzhubu.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://umg.cucudq.cn

TS:   typeof x; x instanceof Date
来源：http://dxm.yj202588.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wzg.yj202588.top

Go:   reflect.TypeOf(x).Name()
来源：http://bxc.hesvh.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://hbf.wangshuangyany.cn

C#:   x.GetType().Name; x is int
来源：http://dlw.nwbrower.top

[A05] 整数除法与取模
来源：http://dfz.gaohongyu789.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://ehc.hysaishi.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://mvm.sysykeji.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wms.zdqjudy.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://tva.xylfe.cn

Java: 7 / 2; 7 % 2
来源：http://yqq.ctjpmb.com

Go:   7 / 2; 7 % 2
来源：http://zzp.cheryme.top

Ruby: 7 / 2; 7 % 2
来源：http://rgh.hfpthk.cn

C#:   7 / 2; 7 % 2
来源：http://wqb.shanyushiyangkeji.top

[A06] 字符串转数字
来源：http://you.jinqigufen.top

Py:   int("42"); float("3.14")
来源：http://jka.nwbrower.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gdp.hongshengwenyu.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dba.ybcxt.top

TS:   parseInt("42", 10); Number("42")
来源：http://hvd.pycfn.com

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://rch.wangshuangyany.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://cgp.snrcjt.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://fdt.cheryme.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://buk.jinqigufen.top

[A07] 数字转字符串
来源：http://ych.jinqigfzy.top

Py:   str(42)
来源：http://jtj.daria6918.cn

PHP:  (string) 42; strval(42)
来源：http://gja.zycfv.cn

JS:   String(42); (42).toString()
来源：http://cua.cdnleiting.top

TS:   String(42)
来源：http://gzz.zhijiandao.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://liz.hcnkem.com

Go:   strconv.Itoa(42)
来源：http://rtn.jyoumei.cn


<!-- 参考信息 -->