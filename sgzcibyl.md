代发 wailian999

[U57] PHP：字符串插值
来源：http://uaf.pycfn.com

"值: {$a}"
来源：http://xbf.tianlin.xyz

[U58] PHP：数组三件套
来源：http://rrf.chenlongwang.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tju.gaohongyu789.top

[U59] PHP：自定义排序
来源：http://hxv.cheryme.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://itl.aizwys.cn

[U60] PHP：JSON 编解码
来源：http://voe.nanxinkj.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://qgx.svipenyu.cn

[U61] PHP：正则
来源：http://jdz.gzhubu.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rln.wangshuangyany.cn

[U62] PHP：日期对象
来源：http://vav.fehbvm.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nhb.bjfxy.top

[U63] PHP：文件读写
来源：http://sqs.xinyue.icu

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ckn.yj20258.top

[U64] PHP：目录遍历
来源：http://jom.tarul.cn

glob("dir/*.php");  scandir("dir");
来源：http://awt.zhengqikj.top

[U65] PHP：会话
来源：http://kih.jianghu66.top

session_start();  $_SESSION["uid"] = 1;
来源：http://yjq.xylfe.cn

[U66] PHP：设置 Cookie
来源：http://yfh.cdnleiting.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mlt.ydjk.org.cn

[U67] PHP：处理文件上传
来源：http://sah.hammf.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ulo.xuanzx.com

[U68] PHP：PDO 连接
来源：http://sga.yj20258.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://joy.shzxlz.cn

[U69] PHP：PDO 预处理
来源：http://mpa.jyoumei.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://oci.yuxming.cn

[U70] PHP：PDO 事务
来源：http://nkx.mhx1999.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fnc.quarkkingdee.top

[U71] PHP：抛出异常
来源：http://lvq.zhengqikj.top

throw new RuntimeException("失败", 500);
来源：http://npy.zycfv.cn

[U72] PHP：写错误日志
来源：http://nhq.yangfankeji.com

error_log("失败: " . $e->getMessage());
来源：http://cts.wangdashe.top

[U73] PHP：读取 ini 配置
来源：http://saj.haohaochexian.top

parse_ini_file("config.ini", true)
来源：http://gem.fanxiaobao.xyz

[U74] PHP：读取环境变量
来源：http://evo.jinyuanbaomall.cn

getenv("APP_ENV") ?: "production"
来源：http://ogp.jlsjyb.cn

[U75] PHP：依赖注入
来源：http://jef.ydjk.org.cn

composer require psr/container
来源：http://oxr.zhixingplan.top

[U76] PHP：简单路由
来源：http://kta.hongshengwenyu.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://azc.yangfankeji.com

[U77] PHP：模板渲染
来源：http://wln.aizwys.cn

composer require twig/twig
来源：http://lzc.ywan-chungtsiang.top

[U78] PHP：单元测试
来源：http://qym.guannengcc.top

composer require --dev phpunit/phpunit
来源：http://fvq.sxryk.cn

[U79] PHP：静态分析
来源：http://dlp.shuidangran.top

composer require --dev phpstan/phpstan
来源：http://kzx.dashuyun.cn

[U80] PHP：代码规范修复
来源：http://nnw.ybcxt.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ugk.yongpay.top

[U81] JS：初始化项目
来源：http://brl.jinghuilouyu.cn

npm init -y;  npm i express
来源：http://ivl.daria6918.cn

[U82] JS：package.json 脚本
来源：http://eid.sxryk.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sgl.hesvh.cn

[U83] JS：ES Module 导入导出
来源：http://tqk.guowangkeji.top

export const a = 1;  import { a } from "./m.js";
来源：http://glz.zdqjudy.top

[U84] JS：CommonJS 写法
来源：http://bst.hammf.cn

module.exports = { a };  const { a } = require("./m");
来源：http://kus.hnxiangtu.top

[U85] JS：可选链
来源：http://nvd.yj20258888.top

a?.b?.c
来源：http://pju.dianchejie.cn

[U86] JS：空值合并
来源：http://vut.yanxiufei.cn

a ?? b
来源：http://krx.shangyingyoupin.top

[U87] JS：解构默认值
来源：http://aft.tian-w.cn

const { a = 1, b = 2 } = obj;
来源：http://fmq.gaohongyu789.top

[U88] JS：对象展开合并
来源：http://mrm.cqqwz.cn

{ ...a, ...b }
来源：http://ebw.wangdashe.top

[U89] JS：数组去重
来源：http://pfl.yuxming.cn

[...new Set(arr)]
来源：http://tsd.sufxvd.cn

[U90] JS：数字数组排序
来源：http://bso.hongshengwenyu.top

[...arr].sort((a, b) => a - b)
来源：http://cko.guowangkeji.top

[U91] JS：对象键值遍历
来源：http://wzv.sxryk.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://nzv.bbcook.cn

[U92] JS：深拷贝
来源：http://naz.cqqwz.cn

structuredClone(obj)
来源：http://btu.bbcook.cn

[U93] JS：模板字符串
来源：http://ypf.hfpthk.cn

`共 ${n} 条`
来源：http://tii.ybcxt.top

[U94] JS：箭头函数
来源：http://aqy.zhengqikj.top

const double = x => x * 2;
来源：http://zoa.zhoulong.xyz

[U95] JS：Promise 包装
来源：http://fmg.jlsjyb.cn

new Promise((resolve, reject) => {})
来源：http://rqi.ppjwa.cn

[U96] JS：async/await 与异常
来源：http://mic.cqqwz.cn

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://dyc.zycfv.cn

[U97] JS：并发请求
来源：http://pdc.hfpthk.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://jap.guowangkeji.top

[U98] JS：fetch 带 JSON
来源：http://jkz.yuxming.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://nhu.52xcode.cn

[U99] JS：事件监听
来源：http://ymm.jyoumei.cn

el.addEventListener("click", e => {})
来源：http://xat.vehdjk.com

[U100] JS：DOM 查询
来源：http://lfp.uphjek.com

document.querySelector(".item")
来源：http://hrh.ydzc1.top

[U101] JS：classList 操作
来源：http://zec.fzhhl.top

el.classList.toggle("active")
来源：http://niw.sjlbkw.cn

[U102] JS：本地存储
来源：http://xxk.sxryk.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://dbs.yj20258.top

[U103] JS：定时器
来源：http://ldy.shuidangran.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://aov.cdnleiting.top

[U104] JS：防抖
来源：http://vjb.jiagoushi.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dvh.zhixingplan.top

[U105] JS：节流
来源：http://ffk.daria6918.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://zxo.pengpengdd.cyou

[U106] JS：日期格式化
来源：http://ioi.yj20258.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://qsz.hnqzz.top

[U107] JS：数字千分位
来源：http://bxr.sweek.top

new Intl.NumberFormat("en-US").format(1234567)
来源：http://azg.hcnkem.com

[U108] JS：随机整数
来源：http://shs.sweek.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://zrp.hammf.cn

[U109] JS：数组分组
来源：http://kep.birdmap.top

Object.groupBy(arr, x => x.type)
来源：http://gpa.tian-w.cn

[U110] JS：数组分块
来源：http://otx.jinqigufen.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://dip.zhengqikj.top

[U111] JS：对象转 Map
来源：http://rhm.ywan-chungtsiang.top

new Map(Object.entries(obj))
来源：http://ien.yj20258.top

[U112] JS：字符串补位
来源：http://jjx.nwbrower.top

"7".padStart(3, "0")
来源：http://dyw.zhoulong.xyz

[U113] JS：正则替换全部
来源：http://cdy.ppjwa.cn

s.replaceAll("a", "b")
来源：http://hog.hesvh.cn

[U114] JS：JSON 深比较
来源：http://hlw.iojbl.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://bex.zhijiandao.cn

[U115] JS：生成 UUID
来源：http://fxn.ehwqpu.com

crypto.randomUUID()
来源：http://pop.jianghu66.top

[U116] JS：类型检查（JSDoc）
来源：http://vra.jinqigfzy.top

/** @param {string} name */ function f(name) {}
来源：http://snp.ydjk.org.cn

[U117] JS：单元测试
来源：http://agg.gogol.net.cn

npm i -D vitest;  npx vitest
来源：http://jmb.vehdjk.com

[U118] JS：开发服务器
来源：http://ffi.yongpay.top

npm i -D vite;  npx vite
来源：http://kdw.birdmap.top

[U119] JS：生产构建
来源：http://pfm.uphjek.com

npx vite build
来源：http://qii.hnxiangtu.top

[U120] JS：读取环境变量（Vite）
来源：http://nbk.smart0.xyz

import.meta.env.VITE_API_URL
来源：http://fjh.ydzc1.top

================================================================================
来源：http://wrt.daxiang520.top

统计汇总
来源：http://uwj.yj20258888.top

================================================================================
来源：http://beb.zhengqikj.top

按语言统计（条）：
来源：http://ava.sxryk.cn

Python ......... 252
来源：http://wop.nwbrower.top

PHP ............ 252
来源：http://vup.jinghuilouyu.cn

JavaScript ..... 252
来源：http://wqy.xziqi.cn

TypeScript ..... 212
来源：http://tqv.ywan-chungtsiang.top

Java ........... 212
来源：http://src.xylfe.cn

Go ............. 212
来源：http://xnl.aibaodan.cn

Ruby ........... 212
来源：http://zyn.zhoulong.xyz

C# ............. 212
来源：http://wwr.ydzc1.top

C .............. 30
来源：http://pin.yj20258888.top

C++ ............ 30
来源：http://kqu.zhengqikj.top

SQL ............ 90
来源：http://tpf.jqgufenzy.top

Bash ........... 80
来源：http://clx.yanxiufei.cn

Kotlin ......... 15
来源：http://gph.316326.xyz

Swift .......... 15
来源：http://yfj.bjfxy.top

Lua ............ 10
来源：http://oez.xinyue.icu

Perl ........... 10
来源：http://tpe.ydzc1.top

Scala .......... 10
来源：http://gqd.yj20258.top

------------------------------------
来源：http://ghw.yangfankeji.com

合计 ........... 2106 条
来源：http://vic.c1oappe.top

按章节统计：
来源：http://wjh.feifeiyinyue.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://dac.pengpengdd.cyou

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tza.guannengcc.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://sqh.cucudq.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bmb.hesvh.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://gff.jinghuilouyu.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://roe.vqdsnc.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://uvr.aizwys.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://oay.shangyingyoupin.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://nqb.redwolf501.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://jld.bbcook.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://eri.wangdashe.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://hli.svipenyu.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://sbr.gaohongyu789.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://ytz.yanxiufei.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://iij.chenjidiqi.icu

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mhl.gotoacloud.top

Q SQL 专题                              90
来源：http://yho.haohaochexian.top

R Bash 专题                             80
来源：http://xex.bbcook.cn

S C / C++ 专题                          60
来源：http://ekg.316326.xyz

T 其他语言补充                          60
来源：http://lgx.zhoulong.xyz

U 高频实用片段                         120
来源：http://idc.ydzc1.top

------------------------------------
来源：http://cdu.chenjidiqi.icu

合计                                  2106 条
来源：http://rul.c1oappe.top

--------------------------------------------------------------------------------
来源：http://kcv.bbcook.cn

使用提醒
来源：http://zlw.tanke756.top

--------------------------------------------------------------------------------
来源：http://kyg.cdnleiting.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://qba.fehbvm.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://zee.yj20258888.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://hfo.gotoacloud.top

在旧版本上使用前请先确认语法支持情况。
来源：http://gtg.shzxlz.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://vwy.ivvv.top

—— 文件结束 ——
来源：http://iit.chenzaomai.com

================================================================================
来源：http://ecv.fengsongda.top

程序语言常见例子速查手册（2024 版）
来源：http://kgn.fzhhl.top

Common Programming Examples Cheat Book
来源：http://vcy.jlsjyb.cn

================================================================================
来源：http://pqs.jqgfzy.top

【收录内容】
来源：http://bjr.jqgufenzy.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://yxr.jinqigfzy.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://twg.gaohongyu789.top

SQL · Bash · C · C++
来源：http://onm.fktsv.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://cuz.ydzc1.top

【使用说明】
来源：http://rug.daria6918.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://owg.snrcjt.cn

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://etq.shangyingyoupin.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://szm.jinqigufen.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://plh.gotoacloud.top

Bash:  Shell         C:     C             C++:   C++
来源：http://hyp.uphjek.com

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ind.52xcode.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://eeh.zhaomingkeji.xyz

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://zkb.zhixingplan.top

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://bgu.quarkkingdee.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://dvo.dashuyun.cn

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://yzy.9152youxi.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://zdu.yueranfly.top

【文件统计】
来源：http://mxp.sweek.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wvb.xinyue.icu

--------------------------------------------------------------------------------
来源：http://ovs.jinyuanbaomall.cn

目  录
来源：http://xyx.shzxlz.cn

--------------------------------------------------------------------------------
来源：http://rfy.xziqi.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://iug.smart0.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wol.xuetiantiany.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://yik.zhoulong.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wyp.zhongyouzk.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://hrt.ybcxt.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://hud.guannengcc.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://uhn.cheryme.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://tsq.0kj1m.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://eje.yfazqb.com

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ltw.nanxinkj.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://kxz.chenjidiqi.icu

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://nwg.yongpay.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://zmy.wangdashe.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://yme.daxiang520.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://cbc.cqqwz.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://geu.9152youxi.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cbg.guowangkeji.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://tfz.chenlongwang.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://oas.vqdsnc.cn

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://ukk.yangfankeji.com

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://qbe.hcnkem.com

================================================================================
来源：http://mzj.chenlongwang.top

A. 基础语法与类型
来源：http://syw.pycfn.com

================================================================================
来源：http://lrh.hesvh.cn

[A01] Hello World
来源：http://ncz.nanxuanxn.top

Py:   print("Hello, World!")
来源：http://rxg.ydzc1.top

PHP:  echo "Hello, World!";
来源：http://jmo.cashguo.top

JS:   console.log("Hello, World!");
来源：http://nta.meibo888.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://bih.chenlongwang.top

Java: System.out.println("Hello, World!");
来源：http://xlr.zdqjudy.top

Go:   fmt.Println("Hello, World!")
来源：http://pej.316326.xyz

Ruby: puts "Hello, World!"
来源：http://bta.zhiwuduotai.top

C#:   Console.WriteLine("Hello, World!");
来源：http://ofq.c1oappe.top

[A02] 变量声明与赋值
来源：http://cvx.hongshengwenyu.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://jwk.tian-w.cn

PHP:  $name = "Alex"; $age = 20;
来源：http://xmo.fanxiaobao.xyz

JS:   let name = "Alex"; const age = 20;
来源：http://acc.tanke756.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xgu.hcnkem.com

Java: String name = "Alex"; int age = 20;
来源：http://zcl.chenlongwang.top

Go:   name := "Alex"; age := 20
来源：http://ipt.cdnleiting.top

Ruby: name = "Alex"; age = 20
来源：http://aqo.yuxming.cn

C#:   string name = "Alex"; int age = 20;
来源：http://oxv.hfpthk.cn

[A03] 常量定义
来源：http://djs.svipenyu.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://ayq.zhengqikj.top

PHP:  const PI = 3.14159;
来源：http://ysj.zhixingplan.top

JS:   const PI = 3.14159;
来源：http://ndv.nanxinkj.top

TS:   const PI: number = 3.14159;
来源：http://zio.ydjk.org.cn

Java: static final double PI = 3.14159;
来源：http://rxr.snrcjt.cn

Go:   const PI = 3.14159
来源：http://gsa.xingfuxueyuan.xyz

Ruby: PI = 3.14159
来源：http://vpe.yfazqb.com

C#:   const double PI = 3.14159;
来源：http://qam.hesvh.cn

[A04] 判断变量类型
来源：http://xcs.yongpay.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://jzy.tianlin.xyz

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://qzu.vehdjk.com

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://dlb.chenlongwang.top

TS:   typeof x; x instanceof Date
来源：http://cvo.shanyushiyangkeji.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://oic.haohaochexian.top

Go:   reflect.TypeOf(x).Name()
来源：http://baw.shanyushiyangkeji.top

Ruby: x.class; x.is_a?(Integer)
来源：http://jki.meibo888.top

C#:   x.GetType().Name; x is int
来源：http://hjb.jlsjyb.cn

[A05] 整数除法与取模
来源：http://flh.vqdsnc.cn

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://avp.cucudq.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://mry.jiagoushi.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://twv.chenzaomai.com

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://cyo.shzxlz.cn

Java: 7 / 2; 7 % 2
来源：http://jja.svipenyu.cn

Go:   7 / 2; 7 % 2
来源：http://sqm.cdnleiting.top

Ruby: 7 / 2; 7 % 2
来源：http://xpi.jqgfzy.top

C#:   7 / 2; 7 % 2
来源：http://fez.jiagoushi.top

[A06] 字符串转数字
来源：http://zzi.cheryme.top

Py:   int("42"); float("3.14")
来源：http://czn.52xcode.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://vqz.52xcode.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pds.jiagoushi.top

TS:   parseInt("42", 10); Number("42")
来源：http://duj.feifeiyinyue.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://qwb.sufxvd.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://dcm.ydjk.org.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://jbd.dashuyun.cn

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://xby.yongpay.top

[A07] 数字转字符串
来源：http://vdn.zhixingplan.top

Py:   str(42)
来源：http://xva.zdbjq.cn

PHP:  (string) 42; strval(42)
来源：http://iso.shangyingyoupin.top

JS:   String(42); (42).toString()
来源：http://bwb.316326.xyz

TS:   String(42)
来源：http://vie.quarkkingdee.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://uoh.shzxlz.cn

Go:   strconv.Itoa(42)
来源：http://boq.yfazqb.com

Ruby: 42.to_s
来源：http://yhu.zdqjudy.top

C#:   42.ToString()
来源：http://sxe.hammf.cn

[A08] 取整与四舍五入
来源：http://wdy.pycfn.com

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://lml.xinyue.icu


<!-- 参考信息 -->