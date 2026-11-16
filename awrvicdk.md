代发 wailian999

[U57] PHP：字符串插值
来源：http://psb.xinyue.icu

"值: {$a}"
来源：http://jjk.zhoulong.xyz

[U58] PHP：数组三件套
来源：http://oij.quarkkingdee.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://oqd.gzhubu.top

[U59] PHP：自定义排序
来源：http://jjm.fanxiaobao.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://anb.epnwcf.com

[U60] PHP：JSON 编解码
来源：http://nwg.yj20258.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xcm.andypj.xyz

[U61] PHP：正则
来源：http://rzq.vehdjk.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://shi.wangdashe.top

[U62] PHP：日期对象
来源：http://uxv.cucudq.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://amu.daria6918.cn

[U63] PHP：文件读写
来源：http://ysj.shanyushiyangkeji.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mml.jyoumei.cn

[U64] PHP：目录遍历
来源：http://hsu.shanyushiyangtech.top

glob("dir/*.php");  scandir("dir");
来源：http://nzw.sufxvd.cn

[U65] PHP：会话
来源：http://mmh.ehwqpu.com

session_start();  $_SESSION["uid"] = 1;
来源：http://hup.dianchejie.cn

[U66] PHP：设置 Cookie
来源：http://mii.shangyingyoupin.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://asb.yj202588.top

[U67] PHP：处理文件上传
来源：http://xbs.fengsongda.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://nsf.havefunace.top

[U68] PHP：PDO 连接
来源：http://nqj.gaohongyu789.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://izd.fanxiaobao.xyz

[U69] PHP：PDO 预处理
来源：http://aah.sweek.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xuh.gogol.net.cn

[U70] PHP：PDO 事务
来源：http://ref.sxryk.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nph.zdbjq.cn

[U71] PHP：抛出异常
来源：http://cas.fktsv.cn

throw new RuntimeException("失败", 500);
来源：http://hyo.yongpay.top

[U72] PHP：写错误日志
来源：http://vqz.9152youxi.cn

error_log("失败: " . $e->getMessage());
来源：http://elf.shangyingyoupin.top

[U73] PHP：读取 ini 配置
来源：http://qky.epnwcf.com

parse_ini_file("config.ini", true)
来源：http://nvb.fktsv.cn

[U74] PHP：读取环境变量
来源：http://gar.shangyingyoupin.top

getenv("APP_ENV") ?: "production"
来源：http://epl.xziqi.cn

[U75] PHP：依赖注入
来源：http://ewh.hesvh.cn

composer require psr/container
来源：http://crt.sjlbkw.cn

[U76] PHP：简单路由
来源：http://jyo.guowangkeji.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ikj.sweek.top

[U77] PHP：模板渲染
来源：http://vrh.gotoacloud.top

composer require twig/twig
来源：http://yge.shuidangran.top

[U78] PHP：单元测试
来源：http://lxy.hywenlv.cn

composer require --dev phpunit/phpunit
来源：http://aoz.tianlin.xyz

[U79] PHP：静态分析
来源：http://dpq.zhiwuduotai.top

composer require --dev phpstan/phpstan
来源：http://gce.chenjidiqi.icu

[U80] PHP：代码规范修复
来源：http://mbr.ydzc1.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://rgo.yangfankeji.com

[U81] JS：初始化项目
来源：http://pco.52xcode.cn

npm init -y;  npm i express
来源：http://khf.xinyue.icu

[U82] JS：package.json 脚本
来源：http://gpr.shuidangran.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://fmh.tarul.cn

[U83] JS：ES Module 导入导出
来源：http://qkf.gogol.net.cn

export const a = 1;  import { a } from "./m.js";
来源：http://iqw.meibo888.top

[U84] JS：CommonJS 写法
来源：http://poy.0kj1m.cn

module.exports = { a };  const { a } = require("./m");
来源：http://iac.yj20258888.top

[U85] JS：可选链
来源：http://jct.quarkkingdee.top

a?.b?.c
来源：http://zpq.52xcode.cn

[U86] JS：空值合并
来源：http://xfu.jinqigfzy.top

a ?? b
来源：http://lrp.gaohongyu789.top

[U87] JS：解构默认值
来源：http://wyx.zhengqikj.top

const { a = 1, b = 2 } = obj;
来源：http://lqr.vqdsnc.cn

[U88] JS：对象展开合并
来源：http://rwm.c1oappe.top

{ ...a, ...b }
来源：http://kcj.sjlbkw.cn

[U89] JS：数组去重
来源：http://lfe.zhixingplan.top

[...new Set(arr)]
来源：http://ivj.bjfxy.top

[U90] JS：数字数组排序
来源：http://qut.gogol.net.cn

[...arr].sort((a, b) => a - b)
来源：http://ztq.hongshengwenyu.top

[U91] JS：对象键值遍历
来源：http://wxp.hnqzz.top

Object.entries(obj).forEach(([k, v]) => {});
来源：http://vhg.tian-w.cn

[U92] JS：深拷贝
来源：http://wjo.shanyushiyangtech.top

structuredClone(obj)
来源：http://zuy.zhoulong.xyz

[U93] JS：模板字符串
来源：http://tub.andypj.xyz

`共 ${n} 条`
来源：http://hcv.yj20258.top

[U94] JS：箭头函数
来源：http://vyn.aibaodan.cn

const double = x => x * 2;
来源：http://gbr.hywenlv.cn

[U95] JS：Promise 包装
来源：http://zdg.52xcode.cn

new Promise((resolve, reject) => {})
来源：http://hon.zhaomingkeji.xyz

[U96] JS：async/await 与异常
来源：http://bbj.yueranfly.top

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://nng.yanxiufei.cn

[U97] JS：并发请求
来源：http://bzd.daria6918.cn

await Promise.all(urls.map(u => fetch(u)))
来源：http://aaz.xinyue.icu

[U98] JS：fetch 带 JSON
来源：http://eyk.daria6918.cn

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mwq.hongshengwenyu.top

[U99] JS：事件监听
来源：http://dib.fanxiaobao.xyz

el.addEventListener("click", e => {})
来源：http://yqk.cdnleiting.top

[U100] JS：DOM 查询
来源：http://new.jiagoushi.top

document.querySelector(".item")
来源：http://pnj.jinqigufen.top

[U101] JS：classList 操作
来源：http://zxl.shuidangran.top

el.classList.toggle("active")
来源：http://gcp.jyoumei.cn

[U102] JS：本地存储
来源：http://inb.jlsjyb.cn

localStorage.setItem("k", JSON.stringify(v))
来源：http://zou.daxiang520.top

[U103] JS：定时器
来源：http://pki.quarkkingdee.top

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://jiy.yanxiufei.cn

[U104] JS：防抖
来源：http://njz.nanxuanxn.top

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://paj.yfazqb.com

[U105] JS：节流
来源：http://qux.bjfxy.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://way.hongshengwenyu.top

[U106] JS：日期格式化
来源：http://ogy.nwbrower.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://enw.smart0.xyz

[U107] JS：数字千分位
来源：http://pvv.zhaomingkeji.xyz

new Intl.NumberFormat("en-US").format(1234567)
来源：http://elj.daxiang520.top

[U108] JS：随机整数
来源：http://alt.quarkkingdee.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://bok.cheryme.top

[U109] JS：数组分组
来源：http://geq.wangdashe.top

Object.groupBy(arr, x => x.type)
来源：http://sqf.fengsongda.top

[U110] JS：数组分块
来源：http://dyw.wangdashe.top

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://rmg.sjlbkw.cn

[U111] JS：对象转 Map
来源：http://zxf.kuanghao11.cn

new Map(Object.entries(obj))
来源：http://zev.bjfxy.top

[U112] JS：字符串补位
来源：http://rlb.ywan-chungtsiang.top

"7".padStart(3, "0")
来源：http://lkx.pycfn.com

[U113] JS：正则替换全部
来源：http://yre.shzxlz.cn

s.replaceAll("a", "b")
来源：http://hsu.cucudq.cn

[U114] JS：JSON 深比较
来源：http://tyw.tanke756.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://lbo.daria6918.cn

[U115] JS：生成 UUID
来源：http://ulg.hnqzz.top

crypto.randomUUID()
来源：http://fbh.jyoumei.cn

[U116] JS：类型检查（JSDoc）
来源：http://fgc.9152youxi.cn

/** @param {string} name */ function f(name) {}
来源：http://dzb.jyoumei.cn

[U117] JS：单元测试
来源：http://gux.vqdsnc.cn

npm i -D vitest;  npx vitest
来源：http://amg.hfpthk.cn

[U118] JS：开发服务器
来源：http://yzv.zhengqikj.top

npm i -D vite;  npx vite
来源：http://jhb.9152youxi.cn

[U119] JS：生产构建
来源：http://nqd.redwolf501.top

npx vite build
来源：http://zfb.cucudq.cn

[U120] JS：读取环境变量（Vite）
来源：http://itn.nwbrower.top

import.meta.env.VITE_API_URL
来源：http://uwp.hammf.cn

================================================================================
来源：http://qos.pycfn.com

统计汇总
来源：http://hmn.yj202588.top

================================================================================
来源：http://mxl.dashuyun.cn

按语言统计（条）：
来源：http://tbp.mhx1999.top

Python ......... 252
来源：http://qgk.yuanzhike.top

PHP ............ 252
来源：http://aza.redwolf501.top

JavaScript ..... 252
来源：http://ixm.zhijiandao.cn

TypeScript ..... 212
来源：http://nrp.chenzaomai.com

Java ........... 212
来源：http://zyk.52xcode.cn

Go ............. 212
来源：http://ajy.ydzc1.top

Ruby ........... 212
来源：http://soz.zhengqikj.top

C# ............. 212
来源：http://kun.hesvh.cn

C .............. 30
来源：http://lam.kuanghao11.cn

C++ ............ 30
来源：http://tiw.0kj1m.cn

SQL ............ 90
来源：http://kgi.birdmap.top

Bash ........... 80
来源：http://vjb.cucudq.cn

Kotlin ......... 15
来源：http://alv.shanyushiyangtech.top

Swift .......... 15
来源：http://dnl.jiagoushi.top

Lua ............ 10
来源：http://yfj.cdnleiting.top

Perl ........... 10
来源：http://vrv.jyoumei.cn

Scala .......... 10
来源：http://qao.bbcook.cn

------------------------------------
来源：http://aan.uphjek.com

合计 ........... 2106 条
来源：http://lno.cucudq.cn

按章节统计：
来源：http://sld.nwbrower.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kpa.sjlbkw.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://gus.chenjidiqi.icu

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://rwy.zdqjudy.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://bar.gogol.net.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://zyj.hnqzz.top

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://jgw.52xcode.cn

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://kre.gotoacloud.top

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mka.nanxinkj.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://rlr.nanxuanxn.top

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://tic.zhiwuduotai.top

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://maq.tian-w.cn

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://fyz.shanyushiyangkeji.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mok.shanyushiyangkeji.top

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://hjz.cqqwz.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://uec.yj20258.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://rfg.yuanzhike.top

Q SQL 专题                              90
来源：http://sdb.yangfankeji.com

R Bash 专题                             80
来源：http://jok.zhengqikj.top

S C / C++ 专题                          60
来源：http://bsk.nanxuanxn.top

T 其他语言补充                          60
来源：http://vhy.xziqi.cn

U 高频实用片段                         120
来源：http://gda.aizwys.cn

------------------------------------
来源：http://pvu.fanxiaobao.xyz

合计                                  2106 条
来源：http://csf.yuxming.cn

--------------------------------------------------------------------------------
来源：http://uhg.ydzc1.top

使用提醒
来源：http://gkh.redwolf501.top

--------------------------------------------------------------------------------
来源：http://rsv.jinghuilouyu.cn

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://zuy.yfazqb.com

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://oor.zhengqikj.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://tro.sufxvd.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://ksn.cucudq.cn

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://euz.jinghuilouyu.cn

—— 文件结束 ——
来源：http://qdg.nwbrower.top

================================================================================
来源：http://tuj.jinghuilouyu.cn

程序语言常见例子速查手册（2024 版）
来源：http://yzz.sufxvd.cn

Common Programming Examples Cheat Book
来源：http://oxu.fengsongda.top

================================================================================
来源：http://phk.jinqigufen.top

【收录内容】
来源：http://grv.ppjwa.cn

覆盖 12 种语言 / 语法与常见 API：
来源：http://tkv.zhongyouzk.top

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://yna.hcnkem.com

SQL · Bash · C · C++
来源：http://ssp.xuanzx.com

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://jwj.zdqjudy.top

【使用说明】
来源：http://qne.bjfxy.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://lqu.zhengqikj.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://efu.haohaochexian.top

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://dsb.bbcook.cn

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://tgu.ybcxt.top

Bash:  Shell         C:     C             C++:   C++
来源：http://fwb.tianlin.xyz

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://irh.iojbl.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://vgb.fzhhl.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://yuu.yangfankeji.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wyf.gzhubu.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://hre.hnqzz.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://vza.zdbjq.cn

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wrh.fktsv.cn

【文件统计】
来源：http://uwl.shanyushiyangkeji.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://ddr.xuetiantiany.cn

--------------------------------------------------------------------------------
来源：http://guj.shanyushiyangkeji.top

目  录
来源：http://xti.xylfe.cn

--------------------------------------------------------------------------------
来源：http://upg.nanxinkj.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://kxi.fehbvm.com

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://smk.gogol.net.cn

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mgu.zhaomingkeji.xyz

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://css.jqgufenzy.top

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://nbj.tanke756.top

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://ysw.iojbl.cn

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://nak.0kj1m.cn

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pfb.hysaishi.cn

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://aoh.zdbjq.cn

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://ztq.fktsv.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mzh.nanxuanxn.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wck.meibo888.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://ctz.zhaomingkeji.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://oig.xingfuxueyuan.xyz

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://ujp.cashguo.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://szw.shuidangran.top

Q. SQL 专题                    （第 17 节，90 条）
来源：http://kqy.xuetiantiany.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://voh.gotoacloud.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://sic.epnwcf.com

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://fia.yuxming.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://bxm.havefunace.top

================================================================================
来源：http://wvi.yangfankeji.com

A. 基础语法与类型
来源：http://axt.jlsjyb.cn

================================================================================
来源：http://jlq.ydzc1.top

[A01] Hello World
来源：http://ltr.zhoulong.xyz

Py:   print("Hello, World!")
来源：http://xkz.yj20258.top

PHP:  echo "Hello, World!";
来源：http://ztj.tianlin.xyz

JS:   console.log("Hello, World!");
来源：http://ykw.epnwcf.com

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wnc.yongpay.top

Java: System.out.println("Hello, World!");
来源：http://lyg.chenlongwang.top

Go:   fmt.Println("Hello, World!")
来源：http://nkr.xingfuxueyuan.xyz

Ruby: puts "Hello, World!"
来源：http://jjz.fzhhl.top

C#:   Console.WriteLine("Hello, World!");
来源：http://kye.zhixingplan.top

[A02] 变量声明与赋值
来源：http://clp.ppjwa.cn

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://zbe.ctjpmb.com

PHP:  $name = "Alex"; $age = 20;
来源：http://rqm.dashuyun.cn

JS:   let name = "Alex"; const age = 20;
来源：http://lkx.kuanghao11.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://xdo.havefunace.top

Java: String name = "Alex"; int age = 20;
来源：http://hto.c1oappe.top

Go:   name := "Alex"; age := 20
来源：http://uac.epnwcf.com

Ruby: name = "Alex"; age = 20
来源：http://uco.yj20258888.top

C#:   string name = "Alex"; int age = 20;
来源：http://xfo.zycfv.cn

[A03] 常量定义
来源：http://gra.yuanzhike.top

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://zqk.cheryme.top

PHP:  const PI = 3.14159;
来源：http://hrd.gotoacloud.top

JS:   const PI = 3.14159;
来源：http://pia.quarkkingdee.top

TS:   const PI: number = 3.14159;
来源：http://wxu.haohaochexian.top

Java: static final double PI = 3.14159;
来源：http://ota.xziqi.cn

Go:   const PI = 3.14159
来源：http://axa.ywan-chungtsiang.top

Ruby: PI = 3.14159
来源：http://dsm.zhengqikj.top

C#:   const double PI = 3.14159;
来源：http://kyz.zhongyouzk.top

[A04] 判断变量类型
来源：http://rre.yangfankeji.com

Py:   type(x).__name__; isinstance(x, int)
来源：http://ifd.dashuyun.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://smz.gzhubu.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wuv.cucudq.cn

TS:   typeof x; x instanceof Date
来源：http://biy.52xcode.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://ton.sysykeji.top

Go:   reflect.TypeOf(x).Name()
来源：http://nha.fengsongda.top

Ruby: x.class; x.is_a?(Integer)
来源：http://nlo.feifeiyinyue.top

C#:   x.GetType().Name; x is int
来源：http://wbh.hysaishi.cn

[A05] 整数除法与取模
来源：http://red.jinqigfzy.top

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://fnd.sjlbkw.cn

PHP:  intdiv(7, 2); 7 % 2
来源：http://hjv.hnxiangtu.top

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://jqg.fanxiaobao.xyz

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://kxz.cheryme.top

Java: 7 / 2; 7 % 2
来源：http://jcs.tanke756.top

Go:   7 / 2; 7 % 2
来源：http://ubp.ybcxt.top

Ruby: 7 / 2; 7 % 2
来源：http://yru.zhaomingkeji.xyz

C#:   7 / 2; 7 % 2
来源：http://pgt.meibo888.top

[A06] 字符串转数字
来源：http://kuc.dianchejie.cn

Py:   int("42"); float("3.14")
来源：http://wjw.shangyingyoupin.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://pev.bjfxy.top

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://pdl.hnxiangtu.top

TS:   parseInt("42", 10); Number("42")
来源：http://ilp.cheryme.top

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://yke.dashuyun.cn

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://idq.ydjk.org.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://wsc.hnxiangtu.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://qun.jinghuilouyu.cn

[A07] 数字转字符串
来源：http://tjs.ybcxt.top

Py:   str(42)
来源：http://jrp.fktsv.cn

PHP:  (string) 42; strval(42)
来源：http://hmx.316326.xyz

JS:   String(42); (42).toString()
来源：http://oup.hysaishi.cn

TS:   String(42)
来源：http://iqv.yj20258888.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://gld.shangyingyoupin.top

Go:   strconv.Itoa(42)
来源：http://cqr.yvedp.cn

Ruby: 42.to_s
来源：http://zyk.0kj1m.cn

C#:   42.ToString()
来源：http://gih.ybcxt.top

[A08] 取整与四舍五入
来源：http://tzq.fanxiaobao.xyz

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://dwr.hnxiangtu.top


<!-- 参考信息 -->