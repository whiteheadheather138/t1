代发 wailian999

[U57] PHP：字符串插值
来源：http://vbx.shangyingyoupin.top

"值: {$a}"
来源：http://tlw.feifeiyinyue.top

[U58] PHP：数组三件套
来源：http://lyk.cdnleiting.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://enf.zdbjq.cn

[U59] PHP：自定义排序
来源：http://dez.zhongyouzk.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rzo.hcnkem.com

[U60] PHP：JSON 编解码
来源：http://bhh.tanke756.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vte.chenzaomai.com

[U61] PHP：正则
来源：http://qdm.jinqigufen.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tuf.aibaodan.cn

[U62] PHP：日期对象
来源：http://rur.fehbvm.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://saq.tarul.cn

[U63] PHP：文件读写
来源：http://wxu.shanyushiyangkeji.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pss.zhaomingkeji.xyz

[U64] PHP：目录遍历
来源：http://ngn.cheryme.top

glob("dir/*.php");  scandir("dir");
来源：http://kgo.ydzc1.top

[U65] PHP：会话
来源：http://xbp.hesvh.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://clu.zhoulong.xyz

[U66] PHP：设置 Cookie
来源：http://yue.cashguo.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ufx.jinqigufen.top

[U67] PHP：处理文件上传
来源：http://xyp.xingfuxueyuan.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qyt.tanke756.top

[U68] PHP：PDO 连接
来源：http://opx.hnqzz.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wxn.cashguo.top

[U69] PHP：PDO 预处理
来源：http://rms.daria6918.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://aiw.zhongyouzk.top

[U70] PHP：PDO 事务
来源：http://nqg.aibaodan.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dmu.fzhhl.top

[U71] PHP：抛出异常
来源：http://xla.nanxuanxn.top

throw new RuntimeException("失败", 500);
来源：http://zgz.316326.xyz

[U72] PHP：写错误日志
来源：http://tat.hywenlv.cn

error_log("失败: " . $e->getMessage());
来源：http://eph.sufxvd.cn

[U73] PHP：读取 ini 配置
来源：http://zqc.fktsv.cn

parse_ini_file("config.ini", true)
来源：http://nsh.zdbjq.cn

[U74] PHP：读取环境变量
来源：http://bsn.guowangkeji.top

getenv("APP_ENV") ?: "production"
来源：http://zic.shanyushiyangtech.top

[U75] PHP：依赖注入
来源：http://erv.cqqwz.cn

composer require psr/container
来源：http://mnv.ydzc1.top

[U76] PHP：简单路由
来源：http://xey.tian-w.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://gwl.jinqigfzy.top

[U77] PHP：模板渲染
来源：http://skk.hnqzz.top

composer require twig/twig
来源：http://qut.zhaomingkeji.xyz

[U78] PHP：单元测试
来源：http://mgb.jianghu66.top

composer require --dev phpunit/phpunit
来源：http://mgv.zhaomingkeji.xyz

[U79] PHP：静态分析
来源：http://ujc.tanke756.top

composer require --dev phpstan/phpstan
来源：http://zzq.kuanghao11.cn

[U80] PHP：代码规范修复
来源：http://sjg.sjlbkw.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://kem.zdqjudy.top

[U81] JS：初始化项目
来源：http://ktk.tian-w.cn

npm init -y;  npm i express
来源：http://fsu.52xcode.cn

[U82] JS：package.json 脚本
来源：http://nif.fehbvm.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wfq.yvedp.cn

[U83] JS：ES Module 导入导出
来源：http://svr.ybcxt.top

export const a = 1;  import { a } from "./m.js";
来源：http://dzt.xuetiantiany.cn

[U84] JS：CommonJS 写法
来源：http://fwr.vehdjk.com

module.exports = { a };  const { a } = require("./m");
来源：http://odp.jqgfzy.top

[U85] JS：可选链
来源：http://slb.yueranfly.top

a?.b?.c
来源：http://qeh.pengpengdd.cyou

[U86] JS：空值合并
来源：http://qom.svipenyu.cn

a ?? b
来源：http://ush.yj20258.top

[U87] JS：解构默认值
来源：http://poc.epnwcf.com

const { a = 1, b = 2 } = obj;
来源：http://vpg.cashguo.top

[U88] JS：对象展开合并
来源：http://avo.feifeiyinyue.top

{ ...a, ...b }
来源：http://zuw.hnxiangtu.top

[U89] JS：数组去重
来源：http://oai.iojbl.cn

[...new Set(arr)]
来源：http://kme.daxiang520.top

[U90] JS：数字数组排序
来源：http://eyr.jyoumei.cn

[...arr].sort((a, b) => a - b)
来源：http://ahb.xinyue.icu

[U91] JS：对象键值遍历
来源：http://kxc.bbcook.cn

Object.entries(obj).forEach(([k, v]) => {});
来源：http://zxq.zycfv.cn

[U92] JS：深拷贝
来源：http://dqv.yongpay.top

structuredClone(obj)
来源：http://osx.chenzaomai.com

[U93] JS：模板字符串
来源：http://jnu.zdbjq.cn

`共 ${n} 条`
来源：http://wzu.gotoacloud.top

[U94] JS：箭头函数
来源：http://ylz.feifeiyinyue.top

const double = x => x * 2;
来源：http://odr.havefunace.top

[U95] JS：Promise 包装
来源：http://aop.shangyingyoupin.top

new Promise((resolve, reject) => {})
来源：http://dlt.tian-w.cn

[U96] JS：async/await 与异常
来源：http://hyc.fzhhl.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://uii.yongpay.top

[U97] JS：并发请求
来源：http://qrl.cdnleiting.top

await Promise.all(urls.map(u => fetch(u)))
来源：http://dsh.tanke756.top

[U98] JS：fetch 带 JSON
来源：http://aby.nanxinkj.top

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://jpr.316326.xyz

[U99] JS：事件监听
来源：http://wax.jqgfzy.top

el.addEventListener("click", e => {})
来源：http://poo.jinqigfzy.top

[U100] JS：DOM 查询
来源：http://qzi.daria6918.cn

document.querySelector(".item")
来源：http://vwy.birdmap.top

[U101] JS：classList 操作
来源：http://pse.yanxiufei.cn

el.classList.toggle("active")
来源：http://nob.yangfankeji.com

[U102] JS：本地存储
来源：http://yjt.yuanzhike.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://znb.aizwys.cn

[U103] JS：定时器
来源：http://yrf.xuetiantiany.cn

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://swc.tianlin.xyz

[U104] JS：防抖
来源：http://kcq.hywenlv.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jbr.hongshengwenyu.top

[U105] JS：节流
来源：http://mep.jlsjyb.cn

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://hws.fengsongda.top

[U106] JS：日期格式化
来源：http://psi.ppjwa.cn

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://jal.zdbjq.cn

[U107] JS：数字千分位
来源：http://vju.zhoulong.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://zal.chenzaomai.com

[U108] JS：随机整数
来源：http://wqr.cqqwz.cn

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://ndg.xuetiantiany.cn

[U109] JS：数组分组
来源：http://kuw.zhijiandao.cn

Object.groupBy(arr, x => x.type)
来源：http://ffa.vqdsnc.cn

[U110] JS：数组分块
来源：http://jod.gotoacloud.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://psl.0kj1m.cn

[U111] JS：对象转 Map
来源：http://xuu.redwolf501.top

new Map(Object.entries(obj))
来源：http://rip.jqgfzy.top

[U112] JS：字符串补位
来源：http://igv.hnqzz.top

"7".padStart(3, "0")
来源：http://rrn.feifeiyinyue.top

[U113] JS：正则替换全部
来源：http://bsq.zhiwuduotai.top

s.replaceAll("a", "b")
来源：http://awd.ctjpmb.com

[U114] JS：JSON 深比较
来源：http://omi.tian-w.cn

JSON.stringify(a) === JSON.stringify(b)
来源：http://wez.jinqigufen.top

[U115] JS：生成 UUID
来源：http://czq.fktsv.cn

crypto.randomUUID()
来源：http://nlz.ydzc1.top

[U116] JS：类型检查（JSDoc）
来源：http://gwk.chenlongwang.top

/** @param {string} name */ function f(name) {}
来源：http://gvh.quarkkingdee.top

[U117] JS：单元测试
来源：http://igv.fanxiaobao.xyz

npm i -D vitest;  npx vitest
来源：http://yxd.52xcode.cn

[U118] JS：开发服务器
来源：http://dfw.gogol.net.cn

npm i -D vite;  npx vite
来源：http://rst.havefunace.top

[U119] JS：生产构建
来源：http://eip.jqgfzy.top

npx vite build
来源：http://jbg.yuanzhike.top

[U120] JS：读取环境变量（Vite）
来源：http://sqb.chenzaomai.com

import.meta.env.VITE_API_URL
来源：http://bdm.jyoumei.cn

================================================================================
来源：http://gio.cashguo.top

统计汇总
来源：http://mfu.hnxiangtu.top

================================================================================
来源：http://lvg.dianchejie.cn

按语言统计（条）：
来源：http://xsc.zhoulong.xyz

Python ......... 252
来源：http://kti.9152youxi.cn

PHP ............ 252
来源：http://goe.mhx1999.top

JavaScript ..... 252
来源：http://dng.aibaodan.cn

TypeScript ..... 212
来源：http://gbw.zhiwuduotai.top

Java ........... 212
来源：http://rxc.hesvh.cn

Go ............. 212
来源：http://wrb.yuxming.cn

Ruby ........... 212
来源：http://yeb.aizwys.cn

C# ............. 212
来源：http://nyh.yvedp.cn

C .............. 30
来源：http://pat.zdqjudy.top

C++ ............ 30
来源：http://vqo.jinqigfzy.top

SQL ............ 90
来源：http://ise.shanyushiyangkeji.top

Bash ........... 80
来源：http://zum.zhixingplan.top

Kotlin ......... 15
来源：http://ude.xylfe.cn

Swift .......... 15
来源：http://azu.yangfankeji.com

Lua ............ 10
来源：http://slv.chenlongwang.top

Perl ........... 10
来源：http://zbe.wangshuangyany.cn

Scala .......... 10
来源：http://hgd.birdmap.top

------------------------------------
来源：http://jtq.c1oappe.top

合计 ........... 2106 条
来源：http://mbi.hysaishi.cn

按章节统计：
来源：http://snk.shzxlz.cn

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://jws.daria6918.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://dxd.yj202588.top

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://lmd.jinyuanbaomall.cn

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://leg.dianchejie.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://inx.hongshengwenyu.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://sfa.xziqi.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wsg.cheryme.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://exc.yongpay.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wro.jqgfzy.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://rvh.ctjpmb.com

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://pmg.xuetiantiany.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cir.yuxming.cn

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://kbn.mhx1999.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://qpp.xingfuxueyuan.xyz

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://fdm.zycfv.cn

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mpf.jinghuilouyu.cn

Q SQL 专题                              90
来源：http://cka.pycfn.com

R Bash 专题                             80
来源：http://ffe.ywan-chungtsiang.top

S C / C++ 专题                          60
来源：http://sgb.tanke756.top

T 其他语言补充                          60
来源：http://dbe.cheryme.top

U 高频实用片段                         120
来源：http://tjb.gogol.net.cn

------------------------------------
来源：http://aag.0kj1m.cn

合计                                  2106 条
来源：http://okz.pycfn.com

--------------------------------------------------------------------------------
来源：http://lzg.jqgufenzy.top

使用提醒
来源：http://tea.svipenyu.cn

--------------------------------------------------------------------------------
来源：http://wzt.jianghu66.top

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://yra.dianchejie.cn

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://czi.birdmap.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://vbm.jinqigufen.top

在旧版本上使用前请先确认语法支持情况。
来源：http://mdv.zhaomingkeji.xyz

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mkq.ctjpmb.com

—— 文件结束 ——
来源：http://tis.ywan-chungtsiang.top

================================================================================
来源：http://eop.ydjk.org.cn

程序语言常见例子速查手册（2024 版）
来源：http://hjg.havefunace.top

Common Programming Examples Cheat Book
来源：http://lde.fanxiaobao.xyz

================================================================================
来源：http://ytj.redwolf501.top

【收录内容】
来源：http://nse.vehdjk.com

覆盖 12 种语言 / 语法与常见 API：
来源：http://sfv.sufxvd.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://xyy.zycfv.cn

SQL · Bash · C · C++
来源：http://tiz.hywenlv.cn

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://uxp.zhixingplan.top

【使用说明】
来源：http://jww.cucudq.cn

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://ujf.316326.xyz

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://cca.ywan-chungtsiang.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dng.hesvh.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://uvs.daxiang520.top

Bash:  Shell         C:     C             C++:   C++
来源：http://rtg.feifeiyinyue.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://pif.yuanzhike.top

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://cnj.snrcjt.cn

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wus.fktsv.cn

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://aen.zhoulong.xyz

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://evr.fengsongda.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://ruu.tian-w.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://xoj.ybcxt.top

【文件统计】
来源：http://kxw.ydjk.org.cn

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://cot.vqdsnc.cn

--------------------------------------------------------------------------------
来源：http://edt.chenlongwang.top

目  录
来源：http://jja.hnxiangtu.top

--------------------------------------------------------------------------------
来源：http://yix.tarul.cn

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://jri.316326.xyz

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://kgo.kuanghao11.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://zgt.daxiang520.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://rsk.daria6918.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://kwi.ehwqpu.com

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://lkv.fehbvm.com

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://ccn.haohaochexian.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mjz.shzxlz.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://ymu.cqqwz.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://xjz.ivvv.top

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://xng.shzxlz.cn

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://bwq.uphjek.com

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://owg.havefunace.top

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://hta.daria6918.cn

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://iqs.gogol.net.cn

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://lfg.jinghuilouyu.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://pmc.guowangkeji.top

R. Bash 专题                   （第 18 节，80 条）
来源：http://ydu.tianlin.xyz

S. C / C++ 专题                （第 19 节，60 条）
来源：http://lhr.ybcxt.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://sho.ydjk.org.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://ltu.zhengqikj.top

================================================================================
来源：http://jyc.zhixingplan.top

A. 基础语法与类型
来源：http://zco.yj20258888.top

================================================================================
来源：http://bsx.ppjwa.cn

[A01] Hello World
来源：http://oex.xuetiantiany.cn

Py:   print("Hello, World!")
来源：http://vbj.xingfuxueyuan.xyz

PHP:  echo "Hello, World!";
来源：http://xwm.ivvv.top

JS:   console.log("Hello, World!");
来源：http://szc.vqdsnc.cn

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://uqt.aibaodan.cn

Java: System.out.println("Hello, World!");
来源：http://sxf.meibo888.top

Go:   fmt.Println("Hello, World!")
来源：http://dmz.shanyushiyangkeji.top

Ruby: puts "Hello, World!"
来源：http://hit.hnxiangtu.top

C#:   Console.WriteLine("Hello, World!");
来源：http://bdm.jqgfzy.top

[A02] 变量声明与赋值
来源：http://krm.cucudq.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kqb.xingfuxueyuan.xyz

PHP:  $name = "Alex"; $age = 20;
来源：http://ogp.hongshengwenyu.top

JS:   let name = "Alex"; const age = 20;
来源：http://nsu.jqgufenzy.top

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://ryt.shzxlz.cn

Java: String name = "Alex"; int age = 20;
来源：http://mmq.epnwcf.com

Go:   name := "Alex"; age := 20
来源：http://tua.chenlongwang.top

Ruby: name = "Alex"; age = 20
来源：http://mbo.yj20258888.top

C#:   string name = "Alex"; int age = 20;
来源：http://upx.jiagoushi.top

[A03] 常量定义
来源：http://epb.hongshengwenyu.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://nrg.hongshengwenyu.top

PHP:  const PI = 3.14159;
来源：http://ilc.cqqwz.cn

JS:   const PI = 3.14159;
来源：http://djx.jinqigufen.top

TS:   const PI: number = 3.14159;
来源：http://bkm.zycfv.cn

Java: static final double PI = 3.14159;
来源：http://umf.jlsjyb.cn

Go:   const PI = 3.14159
来源：http://jcl.zhoulong.xyz

Ruby: PI = 3.14159
来源：http://zws.epnwcf.com

C#:   const double PI = 3.14159;
来源：http://klf.gogol.net.cn

[A04] 判断变量类型
来源：http://bmr.hongshengwenyu.top

Py:   type(x).__name__; isinstance(x, int)
来源：http://cof.nanxinkj.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://krp.cqqwz.cn

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://nsr.ywan-chungtsiang.top

TS:   typeof x; x instanceof Date
来源：http://wkk.wangdashe.top

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://zcq.bjfxy.top

Go:   reflect.TypeOf(x).Name()
来源：http://tnm.ppjwa.cn

Ruby: x.class; x.is_a?(Integer)
来源：http://vqs.zhiwuduotai.top

C#:   x.GetType().Name; x is int
来源：http://slu.chenjidiqi.icu

[A05] 整数除法与取模
来源：http://qdh.shangyingyoupin.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pbv.cucudq.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://sec.iojbl.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://cey.jianghu66.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://qbv.jinyuanbaomall.cn

Java: 7 / 2; 7 % 2
来源：http://sbw.jiagoushi.top

Go:   7 / 2; 7 % 2
来源：http://igg.nwbrower.top

Ruby: 7 / 2; 7 % 2
来源：http://nis.zhoulong.xyz

C#:   7 / 2; 7 % 2
来源：http://dea.jianghu66.top

[A06] 字符串转数字
来源：http://dpr.zdbjq.cn

Py:   int("42"); float("3.14")
来源：http://gdj.0kj1m.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://gjt.kuanghao11.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://ssj.52xcode.cn

TS:   parseInt("42", 10); Number("42")
来源：http://ihm.cqqwz.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://dei.yonumen.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wix.zhixingplan.top

Ruby: "42".to_i; "3.14".to_f
来源：http://ted.smart0.xyz

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://dyu.ydzc1.top

[A07] 数字转字符串
来源：http://iua.meibo888.top

Py:   str(42)
来源：http://dmp.0kj1m.cn

PHP:  (string) 42; strval(42)
来源：http://diq.0kj1m.cn

JS:   String(42); (42).toString()
来源：http://xnm.jinyuanbaomall.cn

TS:   String(42)
来源：http://ryg.birdmap.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://idy.sufxvd.cn

Go:   strconv.Itoa(42)
来源：http://bay.yvedp.cn

Ruby: 42.to_s
来源：http://foh.yuanzhike.top

C#:   42.ToString()
来源：http://blw.pengpengdd.cyou

[A08] 取整与四舍五入
来源：http://cbp.zycfv.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://pfh.daria6918.cn


<!-- 参考信息 -->