代发 wailian999

[U59] PHP：自定义排序
来源：http://pnf.nanxinkj.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mba.jinqigfzy.top

[U60] PHP：JSON 编解码
来源：http://dwe.cqqwz.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://swz.cdnleiting.top

[U61] PHP：正则
来源：http://nnt.tanke756.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yzt.daxiang520.top

[U62] PHP：日期对象
来源：http://yaw.feifeiyinyue.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://eha.hesvh.cn

[U63] PHP：文件读写
来源：http://yle.shanyushiyangkeji.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://oel.dashuyun.cn

[U64] PHP：目录遍历
来源：http://wtd.xingfuxueyuan.xyz

glob("dir/*.php");  scandir("dir");
来源：http://pmm.9152youxi.cn

[U65] PHP：会话
来源：http://kqs.jinqigfzy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ziz.yvedp.cn

[U66] PHP：设置 Cookie
来源：http://dbn.xingfuxueyuan.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wxs.fengsongda.top

[U67] PHP：处理文件上传
来源：http://hnx.nanxinkj.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://vaz.hcnkem.com

[U68] PHP：PDO 连接
来源：http://uib.fehbvm.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xig.xziqi.cn

[U69] PHP：PDO 预处理
来源：http://ety.yfazqb.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ntp.sysykeji.top

[U70] PHP：PDO 事务
来源：http://zjv.zhiwuduotai.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ggn.iojbl.cn

[U71] PHP：抛出异常
来源：http://ygy.fehbvm.com

throw new RuntimeException("失败", 500);
来源：http://wnv.zdqjudy.top

[U72] PHP：写错误日志
来源：http://xkp.fzhhl.top

error_log("失败: " . $e->getMessage());
来源：http://kjr.yvedp.cn

[U73] PHP：读取 ini 配置
来源：http://znr.tarul.cn

parse_ini_file("config.ini", true)
来源：http://fzr.tianlin.xyz

[U74] PHP：读取环境变量
来源：http://opk.dianchejie.cn

getenv("APP_ENV") ?: "production"
来源：http://lyq.yanxiufei.cn

[U75] PHP：依赖注入
来源：http://axe.guannengcc.top

composer require psr/container
来源：http://ilm.sxryk.cn

[U76] PHP：简单路由
来源：http://iyf.hfpthk.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://bcm.xinyue.icu

[U77] PHP：模板渲染
来源：http://ncq.c1oappe.top

composer require twig/twig
来源：http://khq.quarkkingdee.top

[U78] PHP：单元测试
来源：http://zpy.jqgufenzy.top

composer require --dev phpunit/phpunit
来源：http://wko.shangyingyoupin.top

[U79] PHP：静态分析
来源：http://jqr.316326.xyz

composer require --dev phpstan/phpstan
来源：http://bme.jqgufenzy.top

[U80] PHP：代码规范修复
来源：http://wei.nwbrower.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://hmd.cashguo.top

[U81] JS：初始化项目
来源：http://bkw.shanyushiyangtech.top

npm init -y;  npm i express
来源：http://ykl.jlsjyb.cn

[U82] JS：package.json 脚本
来源：http://olx.xuanzx.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://qzi.vqdsnc.cn

[U83] JS：ES Module 导入导出
来源：http://jyb.yangfankeji.com

export const a = 1;  import { a } from "./m.js";
来源：http://aup.0kj1m.cn

[U84] JS：CommonJS 写法
来源：http://uop.hysaishi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://jmt.shangyingyoupin.top

[U85] JS：可选链
来源：http://dbi.tianlin.xyz

a?.b?.c
来源：http://cjp.yongpay.top

[U86] JS：空值合并
来源：http://ijj.meibo888.top

a ?? b
来源：http://wgv.hesvh.cn

[U87] JS：解构默认值
来源：http://zye.gzhubu.top

const { a = 1, b = 2 } = obj;
来源：http://kcy.zhengqikj.top

[U88] JS：对象展开合并
来源：http://zjr.shangyingyoupin.top

{ ...a, ...b }
来源：http://ihl.zhaomingkeji.xyz

[U89] JS：数组去重
来源：http://idk.tarul.cn

[...new Set(arr)]
来源：http://obo.hnxiangtu.top

[U90] JS：数字数组排序
来源：http://aec.zhoulong.xyz

[...arr].sort((a, b) => a - b)
来源：http://uue.mhx1999.top

[U91] JS：对象键值遍历
来源：http://lhw.zhoulong.xyz

Object.entries(obj).forEach(([k, v]) => {});
来源：http://bap.jiagoushi.top

[U92] JS：深拷贝
来源：http://uws.andypj.xyz

structuredClone(obj)
来源：http://tpp.guowangkeji.top

[U93] JS：模板字符串
来源：http://hvi.zhengqikj.top

`共 ${n} 条`
来源：http://oqq.feifeiyinyue.top

[U94] JS：箭头函数
来源：http://fem.nanxinkj.top

const double = x => x * 2;
来源：http://xwn.hywenlv.cn

[U95] JS：Promise 包装
来源：http://muw.vehdjk.com

new Promise((resolve, reject) => {})
来源：http://ayb.hesvh.cn

[U96] JS：async/await 与异常
来源：http://xgs.ctjpmb.com

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://xgz.zdbjq.cn

[U97] JS：并发请求
来源：http://umd.fanxiaobao.xyz

await Promise.all(urls.map(u => fetch(u)))
来源：http://kyr.vqdsnc.cn

[U98] JS：fetch 带 JSON
来源：http://bhq.fehbvm.com

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://lyu.epnwcf.com

[U99] JS：事件监听
来源：http://osu.chenlongwang.top

el.addEventListener("click", e => {})
来源：http://suc.birdmap.top

[U100] JS：DOM 查询
来源：http://rut.mhx1999.top

document.querySelector(".item")
来源：http://lzy.quarkkingdee.top

[U101] JS：classList 操作
来源：http://enf.jinqigfzy.top

el.classList.toggle("active")
来源：http://ipc.uphjek.com

[U102] JS：本地存储
来源：http://rsi.fzhhl.top

localStorage.setItem("k", JSON.stringify(v))
来源：http://ncs.yvedp.cn

[U103] JS：定时器
来源：http://aky.xingfuxueyuan.xyz

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://ovh.vqdsnc.cn

[U104] JS：防抖
来源：http://rms.hfpthk.cn

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://twm.zycfv.cn

[U105] JS：节流
来源：http://dgw.jiagoushi.top

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://iis.fehbvm.com

[U106] JS：日期格式化
来源：http://wmr.daxiang520.top

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://rcp.ppjwa.cn

[U107] JS：数字千分位
来源：http://ljg.sufxvd.cn

new Intl.NumberFormat("en-US").format(1234567)
来源：http://dpz.havefunace.top

[U108] JS：随机整数
来源：http://vky.guowangkeji.top

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://pmw.fengsongda.top

[U109] JS：数组分组
来源：http://uln.redwolf501.top

Object.groupBy(arr, x => x.type)
来源：http://hhu.xinyue.icu

[U110] JS：数组分块
来源：http://zfi.sxryk.cn

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://tjt.yj202588.top

[U111] JS：对象转 Map
来源：http://tsr.hongshengwenyu.top

new Map(Object.entries(obj))
来源：http://qah.hnqzz.top

[U112] JS：字符串补位
来源：http://bjn.xinyue.icu

"7".padStart(3, "0")
来源：http://kwt.316326.xyz

[U113] JS：正则替换全部
来源：http://efi.guowangkeji.top

s.replaceAll("a", "b")
来源：http://pxk.pengpengdd.cyou

[U114] JS：JSON 深比较
来源：http://ccq.havefunace.top

JSON.stringify(a) === JSON.stringify(b)
来源：http://nvx.shangyingyoupin.top

[U115] JS：生成 UUID
来源：http://fbh.haohaochexian.top

crypto.randomUUID()
来源：http://gst.jinqigufen.top

[U116] JS：类型检查（JSDoc）
来源：http://yod.iojbl.cn

/** @param {string} name */ function f(name) {}
来源：http://eph.jianghu66.top

[U117] JS：单元测试
来源：http://xgu.daxiang520.top

npm i -D vitest;  npx vitest
来源：http://fsh.andypj.xyz

[U118] JS：开发服务器
来源：http://edg.ydjk.org.cn

npm i -D vite;  npx vite
来源：http://mdq.gaohongyu789.top

[U119] JS：生产构建
来源：http://kzg.tian-w.cn

npx vite build
来源：http://hwp.xinyue.icu

[U120] JS：读取环境变量（Vite）
来源：http://xqk.xziqi.cn

import.meta.env.VITE_API_URL
来源：http://wxt.xuetiantiany.cn

================================================================================
来源：http://lew.52xcode.cn

统计汇总
来源：http://flf.yj20258.top

================================================================================
来源：http://iqv.gaohongyu789.top

按语言统计（条）：
来源：http://ehl.bbcook.cn

Python ......... 252
来源：http://fkl.9152youxi.cn

PHP ............ 252
来源：http://lct.haohaochexian.top

JavaScript ..... 252
来源：http://pkw.snrcjt.cn

TypeScript ..... 212
来源：http://kzv.hnxiangtu.top

Java ........... 212
来源：http://wdc.vehdjk.com

Go ............. 212
来源：http://tbe.ctjpmb.com

Ruby ........... 212
来源：http://ale.quarkkingdee.top

C# ............. 212
来源：http://ezc.shuidangran.top

C .............. 30
来源：http://omt.gzhubu.top

C++ ............ 30
来源：http://kuy.wangshuangyany.cn

SQL ............ 90
来源：http://lgf.hongshengwenyu.top

Bash ........... 80
来源：http://xen.pycfn.com

Kotlin ......... 15
来源：http://lkv.birdmap.top

Swift .......... 15
来源：http://isv.haohaochexian.top

Lua ............ 10
来源：http://uto.zhongyouzk.top

Perl ........... 10
来源：http://ure.gotoacloud.top

Scala .......... 10
来源：http://tjc.c1oappe.top

------------------------------------
来源：http://ilj.snrcjt.cn

合计 ........... 2106 条
来源：http://jxd.kuanghao11.cn

按章节统计：
来源：http://tmn.jqgufenzy.top

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://kow.xuetiantiany.cn

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://tvz.xylfe.cn

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://xqy.yj20258888.top

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://iak.aibaodan.cn

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://uge.hfpthk.cn

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://tvd.jqgufenzy.top

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://ppz.shzxlz.cn

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://byj.guowangkeji.top

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://gzu.fehbvm.com

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://zgu.aibaodan.cn

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://oyu.sweek.top

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://cjb.shanyushiyangtech.top

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://zkh.sjlbkw.cn

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://evp.sufxvd.cn

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://htf.yj20258888.top

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://jtw.gogol.net.cn

Q SQL 专题                              90
来源：http://zes.chenzaomai.com

R Bash 专题                             80
来源：http://kkb.tian-w.cn

S C / C++ 专题                          60
来源：http://xsn.shangyingyoupin.top

T 其他语言补充                          60
来源：http://azu.zhaomingkeji.xyz

U 高频实用片段                         120
来源：http://dke.tianlin.xyz

------------------------------------
来源：http://yas.yj202588.top

合计                                  2106 条
来源：http://uzs.andypj.xyz

--------------------------------------------------------------------------------
来源：http://lzs.daxiang520.top

使用提醒
来源：http://aqn.hfpthk.cn

--------------------------------------------------------------------------------
来源：http://qmw.fehbvm.com

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://nlj.jinqigufen.top

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://syu.c1oappe.top

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://uua.jinghuilouyu.cn

在旧版本上使用前请先确认语法支持情况。
来源：http://zsh.meibo888.top

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://ckq.hnqzz.top

—— 文件结束 ——
来源：http://tzd.svipenyu.cn

================================================================================
来源：http://hzm.kuanghao11.cn

程序语言常见例子速查手册（2024 版）
来源：http://ici.fanxiaobao.xyz

Common Programming Examples Cheat Book
来源：http://onp.daxiang520.top

================================================================================
来源：http://hmz.nanxinkj.top

【收录内容】
来源：http://mxn.guannengcc.top

覆盖 12 种语言 / 语法与常见 API：
来源：http://xmw.aizwys.cn

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://hnb.cucudq.cn

SQL · Bash · C · C++
来源：http://qbc.316326.xyz

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://hti.52xcode.cn

【使用说明】
来源：http://xjt.ywan-chungtsiang.top

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://owi.ywan-chungtsiang.top

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://lld.zhijiandao.cn

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mqm.zhiwuduotai.top

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wsx.fktsv.cn

Bash:  Shell         C:     C             C++:   C++
来源：http://qgi.ywan-chungtsiang.top

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://ous.yvedp.cn

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://rmk.nanxinkj.top

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://gts.uphjek.com

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://ran.chenlongwang.top

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://xjs.birdmap.top

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://nkl.yongpay.top

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://msh.zhoulong.xyz

【文件统计】
来源：http://ldw.sweek.top

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://eug.fzhhl.top

--------------------------------------------------------------------------------
来源：http://glb.cdnleiting.top

目  录
来源：http://jtr.gogol.net.cn

--------------------------------------------------------------------------------
来源：http://pjv.jinqigufen.top

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://poe.shuidangran.top

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://tcc.zdqjudy.top

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://qlw.yj20258.top

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://zmv.fktsv.cn

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://njo.snrcjt.cn

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://eqg.nanxuanxn.top

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://amp.fengsongda.top

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://pyh.pycfn.com

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://jbl.xinyue.icu

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://cav.9152youxi.cn

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://cra.haohaochexian.top

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://hcb.sweek.top

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://nem.fanxiaobao.xyz

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://bww.zhongyouzk.top

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://qqr.yongpay.top

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://vcz.hammf.cn

Q. SQL 专题                    （第 17 节，90 条）
来源：http://cyg.hesvh.cn

R. Bash 专题                   （第 18 节，80 条）
来源：http://xua.bjfxy.top

S. C / C++ 专题                （第 19 节，60 条）
来源：http://tie.sweek.top

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://qsa.aizwys.cn

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://xpe.havefunace.top

================================================================================
来源：http://yie.yongpay.top

A. 基础语法与类型
来源：http://bdl.ehwqpu.com

================================================================================
来源：http://yct.jqgfzy.top

[A01] Hello World
来源：http://ubh.daxiang520.top

Py:   print("Hello, World!")
来源：http://iug.svipenyu.cn

PHP:  echo "Hello, World!";
来源：http://kpx.jinyuanbaomall.cn

JS:   console.log("Hello, World!");
来源：http://qng.daxiang520.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://fif.xuanzx.com

Java: System.out.println("Hello, World!");
来源：http://dvs.gaohongyu789.top

Go:   fmt.Println("Hello, World!")
来源：http://klu.uphjek.com

Ruby: puts "Hello, World!"
来源：http://pwx.epnwcf.com

C#:   Console.WriteLine("Hello, World!");
来源：http://jhe.jinqigfzy.top

[A02] 变量声明与赋值
来源：http://mlo.fzhhl.top

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://kyy.yongpay.top

PHP:  $name = "Alex"; $age = 20;
来源：http://njz.yonumen.top

JS:   let name = "Alex"; const age = 20;
来源：http://yuv.iojbl.cn

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://fbo.feifeiyinyue.top

Java: String name = "Alex"; int age = 20;
来源：http://blv.ppjwa.cn

Go:   name := "Alex"; age := 20
来源：http://gsx.yongpay.top

Ruby: name = "Alex"; age = 20
来源：http://jwh.aizwys.cn

C#:   string name = "Alex"; int age = 20;
来源：http://zna.dashuyun.cn

[A03] 常量定义
来源：http://tui.hfpthk.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://gji.fanxiaobao.xyz

PHP:  const PI = 3.14159;
来源：http://wls.ivvv.top

JS:   const PI = 3.14159;
来源：http://kyd.shzxlz.cn

TS:   const PI: number = 3.14159;
来源：http://kkt.ydzc1.top

Java: static final double PI = 3.14159;
来源：http://wdy.yj20258888.top

Go:   const PI = 3.14159
来源：http://qhh.hfpthk.cn

Ruby: PI = 3.14159
来源：http://vxn.fktsv.cn

C#:   const double PI = 3.14159;
来源：http://faz.xinyue.icu

[A04] 判断变量类型
来源：http://apa.hfpthk.cn

Py:   type(x).__name__; isinstance(x, int)
来源：http://kja.yuxming.cn

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://tyt.hnqzz.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://fxj.hesvh.cn

TS:   typeof x; x instanceof Date
来源：http://fob.hcnkem.com

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wmp.hammf.cn

Go:   reflect.TypeOf(x).Name()
来源：http://uda.xuanzx.com

Ruby: x.class; x.is_a?(Integer)
来源：http://jny.tarul.cn

C#:   x.GetType().Name; x is int
来源：http://pvt.nwbrower.top

[A05] 整数除法与取模
来源：http://mmk.smart0.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://bbh.nanxuanxn.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://ert.cqqwz.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://exr.cucudq.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wvw.tianlin.xyz

Java: 7 / 2; 7 % 2
来源：http://hhv.zhoulong.xyz

Go:   7 / 2; 7 % 2
来源：http://eah.ywan-chungtsiang.top

Ruby: 7 / 2; 7 % 2
来源：http://rik.vqdsnc.cn

C#:   7 / 2; 7 % 2
来源：http://pfp.jyoumei.cn

[A06] 字符串转数字
来源：http://cfe.316326.xyz

Py:   int("42"); float("3.14")
来源：http://vet.iojbl.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://klc.cucudq.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://dwh.guannengcc.top

TS:   parseInt("42", 10); Number("42")
来源：http://nyq.hesvh.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://fsf.316326.xyz

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://zbb.tanke756.top

Ruby: "42".to_i; "3.14".to_f
来源：http://cbe.ivvv.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://tlu.yuxming.cn

[A07] 数字转字符串
来源：http://yfq.bjfxy.top

Py:   str(42)
来源：http://fzl.jinyuanbaomall.cn

PHP:  (string) 42; strval(42)
来源：http://yqq.9152youxi.cn

JS:   String(42); (42).toString()
来源：http://sra.shanyushiyangtech.top

TS:   String(42)
来源：http://qdl.yueranfly.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://kir.jqgufenzy.top

Go:   strconv.Itoa(42)
来源：http://fxo.quarkkingdee.top

Ruby: 42.to_s
来源：http://vsu.pycfn.com

C#:   42.ToString()
来源：http://hev.zhijiandao.cn

[A08] 取整与四舍五入
来源：http://wle.zhiwuduotai.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://kvq.epnwcf.com

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://onm.yj20258.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://jkb.zycfv.cn

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://zmx.hcnkem.com

Java: Math.round(3.567); Math.floor(3.9)
来源：http://oli.316326.xyz


<!-- 参考信息 -->